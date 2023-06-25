# Comparing `tmp/chargemaster_parsers-0.0.2.tar.gz` & `tmp/chargemaster_parsers-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chargemaster_parsers-0.0.2.tar", last modified: Sun Jun 11 05:51:09 2023, max compression
+gzip compressed data, was "chargemaster_parsers-0.0.3.tar", last modified: Sun Jun 25 19:47:45 2023, max compression
```

## Comparing `chargemaster_parsers-0.0.2.tar` & `chargemaster_parsers-0.0.3.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 05:51:09.183607 chargemaster_parsers-0.0.2/
--rw-rw-rw-   0        0        0     1090 2023-05-28 05:22:14.000000 chargemaster_parsers-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2833 2023-06-11 05:51:09.183103 chargemaster_parsers-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2353 2023-06-11 05:45:35.000000 chargemaster_parsers-0.0.2/README.md
--rw-rw-rw-   0        0        0      603 2023-06-11 05:32:35.000000 chargemaster_parsers-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-11 05:51:09.183607 chargemaster_parsers-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-11 05:51:09.164602 chargemaster_parsers-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-11 05:51:09.167604 chargemaster_parsers-0.0.2/src/chargemaster_parsers/
--rw-rw-rw-   0        0        0       39 2023-06-08 05:45:26.000000 chargemaster_parsers-0.0.2/src/chargemaster_parsers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:51:09.177109 chargemaster_parsers-0.0.2/src/chargemaster_parsers/parsers/
--rw-rw-rw-   0        0        0      401 2023-06-11 04:46:06.000000 chargemaster_parsers-0.0.2/src/chargemaster_parsers/parsers/__init__.py
--rw-rw-rw-   0        0        0     3627 2023-06-11 04:50:47.000000 chargemaster_parsers-0.0.2/src/chargemaster_parsers/parsers/cedars_sinai.py
--rw-rw-rw-   0        0        0     4512 2023-06-11 04:49:06.000000 chargemaster_parsers-0.0.2/src/chargemaster_parsers/parsers/kaiser.py
--rw-rw-rw-   0        0        0     3121 2023-06-11 04:57:40.000000 chargemaster_parsers-0.0.2/src/chargemaster_parsers/parsers/parsers.py
--rw-rw-rw-   0        0        0      810 2023-06-11 04:48:59.000000 chargemaster_parsers-0.0.2/src/chargemaster_parsers/parsers/rady.py
--rw-rw-rw-   0        0        0     7149 2023-06-11 04:48:54.000000 chargemaster_parsers-0.0.2/src/chargemaster_parsers/parsers/scripps.py
--rw-rw-rw-   0        0        0    19082 2023-06-11 04:45:30.000000 chargemaster_parsers-0.0.2/src/chargemaster_parsers/parsers/sharp.py
--rw-rw-rw-   0        0        0     7571 2023-06-11 04:48:36.000000 chargemaster_parsers-0.0.2/src/chargemaster_parsers/parsers/ucsd.py
-drwxrwxrwx   0        0        0        0 2023-06-11 05:51:09.171602 chargemaster_parsers-0.0.2/src/chargemaster_parsers.egg-info/
--rw-rw-rw-   0        0        0     2833 2023-06-11 05:51:09.000000 chargemaster_parsers-0.0.2/src/chargemaster_parsers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      806 2023-06-11 05:51:09.000000 chargemaster_parsers-0.0.2/src/chargemaster_parsers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 05:51:09.000000 chargemaster_parsers-0.0.2/src/chargemaster_parsers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-11 05:51:09.000000 chargemaster_parsers-0.0.2/src/chargemaster_parsers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-11 05:51:09.000000 chargemaster_parsers-0.0.2/src/chargemaster_parsers.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-11 05:51:09.182101 chargemaster_parsers-0.0.2/tests/
--rw-rw-rw-   0        0        0     3638 2023-06-11 04:56:03.000000 chargemaster_parsers-0.0.2/tests/test_cedars_sinai.py
--rw-rw-rw-   0        0        0     3547 2023-06-11 04:55:34.000000 chargemaster_parsers-0.0.2/tests/test_kaiser.py
--rw-rw-rw-   0        0        0     2420 2023-06-08 06:21:40.000000 chargemaster_parsers-0.0.2/tests/test_parser.py
--rw-rw-rw-   0        0        0     1700 2023-06-11 04:55:08.000000 chargemaster_parsers-0.0.2/tests/test_rady.py
--rw-rw-rw-   0        0        0     6525 2023-06-11 04:52:05.000000 chargemaster_parsers-0.0.2/tests/test_scripps.py
--rw-rw-rw-   0        0        0     2094 2023-06-11 04:54:22.000000 chargemaster_parsers-0.0.2/tests/test_sharp.py
--rw-rw-rw-   0        0        0    11705 2023-06-11 04:54:33.000000 chargemaster_parsers-0.0.2/tests/test_ucsd.py
+drwxrwxrwx   0        0        0        0 2023-06-25 19:47:45.567427 chargemaster_parsers-0.0.3/
+-rw-rw-rw-   0        0        0     1090 2023-05-28 05:22:14.000000 chargemaster_parsers-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     6837 2023-06-25 19:47:45.566926 chargemaster_parsers-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6343 2023-06-23 06:01:09.000000 chargemaster_parsers-0.0.3/README.md
+-rw-rw-rw-   0        0        0      630 2023-06-25 19:46:31.000000 chargemaster_parsers-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-25 19:47:45.567427 chargemaster_parsers-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-25 19:47:45.542926 chargemaster_parsers-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-25 19:47:45.546926 chargemaster_parsers-0.0.3/src/chargemaster_parsers/
+-rw-rw-rw-   0        0        0       39 2023-06-08 05:45:26.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 19:47:45.558426 chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/
+-rw-rw-rw-   0        0        0      493 2023-06-25 19:46:37.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/__init__.py
+-rw-rw-rw-   0        0        0     3627 2023-06-11 04:50:47.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/cedars_sinai.py
+-rw-rw-rw-   0        0        0     4512 2023-06-11 04:49:06.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/kaiser.py
+-rw-rw-rw-   0        0        0     3121 2023-06-11 04:57:40.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/parsers.py
+-rw-rw-rw-   0        0        0      810 2023-06-11 04:48:59.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/rady.py
+-rw-rw-rw-   0        0        0     7727 2023-06-23 06:11:45.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/scripps.py
+-rw-rw-rw-   0        0        0    19082 2023-06-11 04:45:30.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/sharp.py
+-rw-rw-rw-   0        0        0    12028 2023-06-25 05:34:46.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/stanford.py
+-rw-rw-rw-   0        0        0     2641 2023-06-25 19:46:37.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/uci.py
+-rw-rw-rw-   0        0        0     8004 2023-06-19 06:39:14.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/ucsd.py
+drwxrwxrwx   0        0        0        0 2023-06-25 19:47:45.550927 chargemaster_parsers-0.0.3/src/chargemaster_parsers.egg-info/
+-rw-rw-rw-   0        0        0     6837 2023-06-25 19:47:45.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      932 2023-06-25 19:47:45.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 19:47:45.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-25 19:47:45.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-25 19:47:45.000000 chargemaster_parsers-0.0.3/src/chargemaster_parsers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 19:47:45.565927 chargemaster_parsers-0.0.3/tests/
+-rw-rw-rw-   0        0        0     3638 2023-06-11 04:56:03.000000 chargemaster_parsers-0.0.3/tests/test_cedars_sinai.py
+-rw-rw-rw-   0        0        0     3547 2023-06-11 04:55:34.000000 chargemaster_parsers-0.0.3/tests/test_kaiser.py
+-rw-rw-rw-   0        0        0     2420 2023-06-08 06:21:40.000000 chargemaster_parsers-0.0.3/tests/test_parser.py
+-rw-rw-rw-   0        0        0     1700 2023-06-11 04:55:08.000000 chargemaster_parsers-0.0.3/tests/test_rady.py
+-rw-rw-rw-   0        0        0     6802 2023-06-23 06:16:44.000000 chargemaster_parsers-0.0.3/tests/test_scripps.py
+-rw-rw-rw-   0        0        0     2094 2023-06-11 04:54:22.000000 chargemaster_parsers-0.0.3/tests/test_sharp.py
+-rw-rw-rw-   0        0        0     4185 2023-06-25 05:38:02.000000 chargemaster_parsers-0.0.3/tests/test_stanford.py
+-rw-rw-rw-   0        0        0     3804 2023-06-25 19:46:37.000000 chargemaster_parsers-0.0.3/tests/test_uci.py
+-rw-rw-rw-   0        0        0    22776 2023-06-23 06:17:01.000000 chargemaster_parsers-0.0.3/tests/test_ucsd.py
```

### Comparing `chargemaster_parsers-0.0.2/LICENSE` & `chargemaster_parsers-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chargemaster_parsers-0.0.2/pyproject.toml` & `chargemaster_parsers-0.0.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chargemaster_parsers"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
-  { name="Jaocb Schaer" },
+  { name="Jacob Schaer" },
+  { name="Yvonne Kaire" }
 ]
 description = "A library for parsing machine readable healthcare chargemasters"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `chargemaster_parsers-0.0.2/src/chargemaster_parsers/parsers/cedars_sinai.py` & `chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/cedars_sinai.py`

 * *Files identical despite different names*

### Comparing `chargemaster_parsers-0.0.2/src/chargemaster_parsers/parsers/kaiser.py` & `chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/kaiser.py`

 * *Files identical despite different names*

### Comparing `chargemaster_parsers-0.0.2/src/chargemaster_parsers/parsers/parsers.py` & `chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/parsers.py`

 * *Files identical despite different names*

### Comparing `chargemaster_parsers-0.0.2/src/chargemaster_parsers/parsers/rady.py` & `chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/rady.py`

 * *Files identical despite different names*

### Comparing `chargemaster_parsers-0.0.2/src/chargemaster_parsers/parsers/scripps.py` & `chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/scripps.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,26 +36,28 @@
                 procedure_identifier = None
                 procedure_description = None
                 ndc_code = None
                 nubc_revenue_code = None
                 cpt_code = None
                 hcpcs_code = None
                 ms_drg_code = None
-                max_reimbursement = None
-                min_reimbursement = None
                 expected_reimbursement = None
                 in_patient = None
                 payer = None
                 plan = None
                 gross_charge = None
 
                 gross_charges_outpatient = None
                 gross_charges_inpatient = None
                 expected_inpatient_reimbursement = None
                 expected_outpatient_reimbursement = None
+                min_inpatient_reimbursement = None
+                max_inpatient_reimbursement = None
+                min_outpatient_reimbursement = None
+                max_outpatient_reimbursement = None
 
                 location = row["LOCATION"].strip()
                 procedure_identifier = row["PROCEDURE CODE"]
 
                 if procedure_identifier.startswith('MS'):
                     ms_drg_code = procedure_identifier[2:]
                 procedure_description = row["PROCEDURE DESCRIPTION"]
@@ -84,28 +86,45 @@
                     pass
 
                 try:
                     expected_outpatient_reimbursement = float(row["OP_EXPECTED_REIMBURSMENT"])
                 except ValueError:
                     pass
 
+                try:
+                    min_inpatient_reimbursement = float(row["IP_MIN"])
+                except ValueError:
+                    pass
+
+                try:
+                    max_inpatient_reimbursement = float(row["IP_MAX"])
+                except ValueError:
+                    pass
+
+                try:
+                    min_outpatient_reimbursement = float(row["OP_MIN"])
+                except ValueError:
+                    pass
+
+                try:
+                    max_outpatient_reimbursement = float(row["OP_MAX"])
+                except ValueError:
+                    pass
+
                 # Every line references cash but make sure to only yield it once
                 if procedure_identifier not in cash_procedures_yielded and cash is not None:
                     yield ChargeMasterEntry(
                             location = location,
                             procedure_identifier = procedure_identifier,
                             procedure_description = procedure_description,
                             ndc_code = ndc_code,
                             nubc_revenue_code = nubc_revenue_code,
                             cpt_code = cpt_code,
                             hcpcs_code = hcpcs_code,
                             ms_drg_code = ms_drg_code,
-                            max_reimbursement = max_reimbursement,
-                            min_reimbursement = min_reimbursement,
-                            expected_reimbursement = expected_inpatient_reimbursement,
                             in_patient = True,
                             payer = "Cash",
                             gross_charge = cash,
                         )
                     cash_procedures_yielded.add(procedure_identifier)
 
                 for plan in plan.split(','):
@@ -115,16 +134,16 @@
                             procedure_identifier = procedure_identifier,
                             procedure_description = procedure_description,
                             ndc_code = ndc_code,
                             nubc_revenue_code = nubc_revenue_code,
                             cpt_code = cpt_code,
                             hcpcs_code = hcpcs_code,
                             ms_drg_code = ms_drg_code,
-                            max_reimbursement = max_reimbursement,
-                            min_reimbursement = min_reimbursement,
+                            max_reimbursement = max_inpatient_reimbursement,
+                            min_reimbursement = min_inpatient_reimbursement,
                             expected_reimbursement = expected_inpatient_reimbursement,
                             in_patient = True,
                             payer = payer,
                             plan = plan.strip(),
                             gross_charge = gross_charges_inpatient,
                         )
                     if gross_charges_outpatient:
@@ -133,15 +152,15 @@
                             procedure_identifier = procedure_identifier,
                             procedure_description = procedure_description,
                             ndc_code = ndc_code,
                             nubc_revenue_code = nubc_revenue_code,
                             cpt_code = cpt_code,
                             hcpcs_code = hcpcs_code,
                             ms_drg_code = ms_drg_code,
-                            max_reimbursement = max_reimbursement,
-                            min_reimbursement = min_reimbursement,
+                            max_reimbursement = max_outpatient_reimbursement,
+                            min_reimbursement = min_outpatient_reimbursement,
                             expected_reimbursement = expected_outpatient_reimbursement,
                             in_patient = False,
                             payer = payer,
                             plan = plan.strip(),
                             gross_charge = gross_charges_outpatient,
                         )
```

### Comparing `chargemaster_parsers-0.0.2/src/chargemaster_parsers/parsers/sharp.py` & `chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/sharp.py`

 * *Files identical despite different names*

### Comparing `chargemaster_parsers-0.0.2/src/chargemaster_parsers/parsers/ucsd.py` & `chargemaster_parsers-0.0.3/src/chargemaster_parsers/parsers/ucsd.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 
 from .parsers import ChargeMasterEntry, ChargeMasterParser
 
 NDC_REGEX = r"^(\d{4}-\d{4}-\d{2}|\d{5}-(?:\d{3}-\d{2}|\d{4}-\d{1,2}))"
 NUBC_REV_CODE_REGEX = r'(^[0-9]{4})\s*-\s*'
 CODE_MATCHERS = (
-    ("CPT", r'^CPT.+?([0-9]+)$'),
+    ("CPT", r'^CPT.+?([0-9]{4}[0-9A-Z])$'),
     ("HCPCS", r'^HCPCS\s+(.+)$'),
     ("DRG", r"^MS-DRG\s+V[0-9]+\s+\(FY [0-9]+\)\s+(.+?)$")
 )
 
 class UCSDChargeMasterParser(ChargeMasterParser):
     INSTITUTION_NAME = "UCSD"
     ARTIFACT_URL = "http://hsfiles.ucsd.edu/patientBilling/UC-San-Diego-Standard-Charges-956006144.json"
@@ -22,15 +22,15 @@
         # codecs decode error functions end up leaving behind the quote, and registering a new one would lack sufficient
         # context to find the weird sequences
         decoded = artifacts[self.ARTIFACT_URL].read().decode('utf-8', errors='replace').replace('�"�', "").replace('"Where "Variable" exists,', '"Where \'Variable\' exists,')
         for row in json.loads(decoded):
             # Deal with non-ascii stuff and whitespace
             filtered_row = {}
             for key, value in row.items():
-                filtered_key = key.encode('ascii', errors='ignore').decode().strip()
+                filtered_key = key.encode('ascii', errors='ignore').decode().replace("_", " ").strip().upper()
                 filtered_value = None
                 if value:
                     filtered_value = value.encode('ascii', errors='ignore').decode().strip()
                 filtered_row[filtered_key] = filtered_value
 
             location = None
             procedure_identifier = None
@@ -49,24 +49,29 @@
             gross_charge = None
             
             quantity = None
             in_patient_price = None
 
             try:
                 # This can be "Variable" - which we'll treat as None
-                min_reimbursement = float(filtered_row.pop('REIMB_MIN'))
+                min_reimbursement = float(filtered_row.pop('REIMB MIN'))
             except (KeyError, ValueError, TypeError):
                 pass
 
             try:
                 # This can be "Variable" - which we'll treat as None
-                max_reimbursement = float(filtered_row.pop('REIMB_MAX'))
+                max_reimbursement = float(filtered_row.pop('REIMB MAX'))
             except (KeyError, ValueError, TypeError):
                 pass
 
+            if min_reimbursement and max_reimbursement:
+                # Handle case where they're swapped for.. who knows what reason
+                min_reimbursement, max_reimbursement = sorted((min_reimbursement, max_reimbursement))
+
+
             try:
                 # This should only occur when "Code Type" == "ERX"
                 ndc = filtered_row.pop('NDC')
                 ndc_match = re.match(NDC_REGEX, ndc)
                 if ndc_match:
                     ndc_code = ndc_match.groups()[0]
                 else:
@@ -81,65 +86,67 @@
                 # This field isn't very useful - sometimes a float, sometimes a string like "1 pill"
                 quantity = filtered_row.pop('QUANTITY')
             except KeyError:
                 pass
 
             # This is usually "Variable", sometimes "OP_PRICE" almost useless espeicallys since we have min/max and insurance rates
             try:
-                in_patient_price = float(filtered_row.pop("IP_PRICE"))
+                in_patient_price = float(filtered_row.pop("IP PRICE"))
             except (KeyError, ValueError, TypeError):
                 pass
 
             try:
-                code = filtered_row.pop("Code")
-                for candidate_code_type, code_matcher in CODE_MATCHERS:
-                    match = re.match(code_matcher, code)
-                    if match:
-                        if candidate_code_type == "CPT":
-                            cpt_code = match.groups()[0]
-                        elif candidate_code_type == "HCPCS":
-                            hcpcs_code = match.groups()[0]
-                        elif candidate_code_type == "DRG":
-                            ms_drg_code = match.groups()[0]
-                        break
+                code = filtered_row.pop("CODE")
+                if code is not None:
+                    for candidate_code_type, code_matcher in CODE_MATCHERS:
+                        match = re.match(code_matcher, code)
+                        if match:
+                            if candidate_code_type == "CPT":
+                                cpt_code = match.groups()[0]
+                            elif candidate_code_type == "HCPCS":
+                                hcpcs_code = match.groups()[0]
+                            elif candidate_code_type == "DRG":
+                                ms_drg_code = match.groups()[0]
+                            break
             except KeyError:
                 pass
 
             try:
                 procedure_identifier = filtered_row.pop("PROCEDURE")
             except (KeyError, ValueError):
                 pass
 
             # If we didn't already figure out the NUBC code, try to find in the Rev Code field
             try:
-                rev_code = filtered_row.pop("Rev Code")
-                matched = False
-                if nubc_revenue_code is None:
-                    nubc_revenue_code_match = re.match(NUBC_REV_CODE_REGEX, rev_code)
-                    if nubc_revenue_code_match:
-                        nubc_revenue_code = nubc_revenue_code_match.groups()[0]
-                        matched = True
-                if not matched:
-                    procedure_description = rev_code
+                rev_code = filtered_row.pop("REV CODE")
+                if rev_code is not None:
+                    matched = False
+                    if nubc_revenue_code is None:
+                        nubc_revenue_code_match = re.match(NUBC_REV_CODE_REGEX, rev_code)
+                        if nubc_revenue_code_match:
+                            nubc_revenue_code = nubc_revenue_code_match.groups()[0]
+                            matched = True
+                    if not matched:
+                        procedure_description = rev_code
             except KeyError:
                 pass
 
 
             # Ignore this field - it's
             # ERX for NDC
             # SUP for Supplies will have an NUBC Rev Code
             # .. etc
             try:
-                filtered_row.pop("Code Type")
+                filtered_row.pop("CODE TYPE")
             except KeyError:
                 pass
 
             # Almost always garbage - what does an integer here even mean?!
             try:
-                description = filtered_row.pop("PROCEDURE_DESCRIPTION")
+                description = filtered_row.pop("PROCEDURE DESCRIPTION")
                 if description != "1" and procedure_description is None:
                     procedure_description = description
 
             except KeyError:
                 pass
```

### Comparing `chargemaster_parsers-0.0.2/src/chargemaster_parsers.egg-info/SOURCES.txt` & `chargemaster_parsers-0.0.3/src/chargemaster_parsers.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,19 @@
 src/chargemaster_parsers/parsers/__init__.py
 src/chargemaster_parsers/parsers/cedars_sinai.py
 src/chargemaster_parsers/parsers/kaiser.py
 src/chargemaster_parsers/parsers/parsers.py
 src/chargemaster_parsers/parsers/rady.py
 src/chargemaster_parsers/parsers/scripps.py
 src/chargemaster_parsers/parsers/sharp.py
+src/chargemaster_parsers/parsers/stanford.py
+src/chargemaster_parsers/parsers/uci.py
 src/chargemaster_parsers/parsers/ucsd.py
 tests/test_cedars_sinai.py
 tests/test_kaiser.py
 tests/test_parser.py
 tests/test_rady.py
 tests/test_scripps.py
 tests/test_sharp.py
+tests/test_stanford.py
+tests/test_uci.py
 tests/test_ucsd.py
```

### Comparing `chargemaster_parsers-0.0.2/tests/test_cedars_sinai.py` & `chargemaster_parsers-0.0.3/tests/test_cedars_sinai.py`

 * *Files identical despite different names*

### Comparing `chargemaster_parsers-0.0.2/tests/test_kaiser.py` & `chargemaster_parsers-0.0.3/tests/test_kaiser.py`

 * *Files identical despite different names*

### Comparing `chargemaster_parsers-0.0.2/tests/test_parser.py` & `chargemaster_parsers-0.0.3/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `chargemaster_parsers-0.0.2/tests/test_rady.py` & `chargemaster_parsers-0.0.3/tests/test_rady.py`

 * *Files identical despite different names*

### Comparing `chargemaster_parsers-0.0.2/tests/test_scripps.py` & `chargemaster_parsers-0.0.3/tests/test_scripps.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,26 +38,27 @@
             location = 'Scripps Green Hospital',
             procedure_description = "HC High Cost Appl Skin Substitute T/a/L Up to 100 Sq Cm, 1st 25 Sq Cm or Less",
             in_patient = False,
             payer = 'AETNA MEDI-CAL',
             plan = 'AETNA MEDI-CAL BETTER HEALTH OF CA',
             gross_charge = 10626.0,
             expected_reimbursement = 0.0,
+            max_reimbursement = 10626.00,
+            min_reimbursement = 1381.38
+
         ),
     ]
 
     actual_result = list(parser.parse_artifacts({
         ScrippsChargeMasterParser.SCRIPPS_GREEN_HOSPITAL_ARTIFACT_URL : io.BytesIO(rows.encode('utf-8')),
         ScrippsChargeMasterParser.SCRIPPS_MEMORIAL_HOSPITAL_ENCINITAS_ARTIFACT_URL: io.BytesIO(),
         ScrippsChargeMasterParser.SCRIPPS_MEMORIAL_HOSPITAL_LA_JOLLA_ARTIFACT_URL: io.BytesIO(),
         ScrippsChargeMasterParser.SCRIPPS_MERCY_HOSPITAL_SAN_DIEGO_ARTIFACT_URL: io.BytesIO(),
         ScrippsChargeMasterParser.SCRIPPS_MERCY_HOSPITAL_CHULA_VISTA_ARTIFACT_URL: io.BytesIO(),
     }))
-    #import pprint
-    #pprint.pprint(actual_result)
     assert sorted(expected_result) == sorted(actual_result)
 
 
 def test_ms_drg(parser):
     rows = "\n".join(
         ["LOCATION|PROCEDURE CODE|PROCEDURE DESCRIPTION|PAYER|PLAN|GROSS CHARGES IP|IP_EXPECTED_REIMBURSMENT|GROSS CHARGES OP|OP_EXPECTED_REIMBURSMENT|IP_MIN|IP_MAX|OP_MIN|OP_MAX|CASH/SELF PAY",
          "Scripps Green Hospital|MS940|O.R. Procedures With Diagnoses Of Other Contact With Health Services With Cc|AETNA MEDI-CAL [213]|AETNA MEDI-CAL BETTER HEALTH OF CA [21301], AETNA MEDI-CAL HMO - COMM CARE IPA [21302], AETNA MEDI-CAL HMO - PROSPECT MED GRP [21303]|105058.34||||9000.00|101685.89|||52529.17",
@@ -70,36 +71,42 @@
             procedure_identifier = 'MS940',
             location = 'Scripps Green Hospital',
             procedure_description = "O.R. Procedures With Diagnoses Of Other Contact With Health Services With Cc",
             ms_drg_code = '940',
             in_patient = True,
             payer = 'AETNA MEDI-CAL',
             plan = 'AETNA MEDI-CAL BETTER HEALTH OF CA',
-            gross_charge = 105058.34
+            gross_charge = 105058.34,
+            max_reimbursement=101685.89,
+            min_reimbursement=9000.0,
         ),
         ChargeMasterEntry(
             procedure_identifier = 'MS940',
             location = 'Scripps Green Hospital',
             procedure_description = "O.R. Procedures With Diagnoses Of Other Contact With Health Services With Cc",
             ms_drg_code = '940',
             in_patient = True,
             payer = 'AETNA MEDI-CAL',
             plan = 'AETNA MEDI-CAL HMO - HEALTH EXCEL IPA',
-            gross_charge = 105058.34
+            gross_charge = 105058.34,
+            max_reimbursement=101685.89,
+            min_reimbursement=9000.0,
         ),
         ChargeMasterEntry(
             procedure_identifier = 'MS940',
             location = 'Scripps Green Hospital',
             procedure_description = "O.R. Procedures With Diagnoses Of Other Contact With Health Services With Cc",
             ms_drg_code = '940',
             in_patient = True,
             payer = 'AETNA MEDICARE ADVANTAGE',
             plan = 'AETNA MCR ADV HMO - HEALTH EXCEL IPA',
             expected_reimbursement = 18463.8,
-            gross_charge = 105058.34
+            gross_charge = 105058.34,
+            max_reimbursement=101685.89,
+            min_reimbursement=9000.0,
         ),
         ChargeMasterEntry(
             procedure_identifier = 'MS940',
             location = 'Scripps Green Hospital',
             procedure_description = "O.R. Procedures With Diagnoses Of Other Contact With Health Services With Cc",
             ms_drg_code = '940',
             in_patient = True,
```

### Comparing `chargemaster_parsers-0.0.2/tests/test_sharp.py` & `chargemaster_parsers-0.0.3/tests/test_sharp.py`

 * *Files identical despite different names*

