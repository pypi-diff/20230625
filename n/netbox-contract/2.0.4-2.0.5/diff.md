# Comparing `tmp/netbox-contract-2.0.4.tar.gz` & `tmp/netbox-contract-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-contract-2.0.4.tar", last modified: Sun Jun 18 16:14:40 2023, max compression
+gzip compressed data, was "netbox-contract-2.0.5.tar", last modified: Sun Jun 25 10:08:53 2023, max compression
```

## Comparing `netbox-contract-2.0.4.tar` & `netbox-contract-2.0.5.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-18 16:14:40.482623 netbox-contract-2.0.4/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1056 2023-01-03 17:10:18.000000 netbox-contract-2.0.4/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-03-12 14:44:04.000000 netbox-contract-2.0.4/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3733 2023-06-18 16:14:40.478623 netbox-contract-2.0.4/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3194 2023-06-18 16:08:41.000000 netbox-contract-2.0.4/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)      774 2023-06-18 16:12:50.000000 netbox-contract-2.0.4/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-06-18 16:14:40.482623 netbox-contract-2.0.4/setup.cfg
--rw-rw-r--   0 vscode    (1000) vscode    (1000)       52 2023-01-03 18:27:10.000000 netbox-contract-2.0.4/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-18 16:14:40.454622 netbox-contract-2.0.4/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-18 16:14:40.462622 netbox-contract-2.0.4/src/netbox_contract/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      469 2023-06-18 16:13:17.000000 netbox-contract-2.0.4/src/netbox_contract/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-18 16:14:40.470622 netbox-contract-2.0.4/src/netbox_contract/api/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/api/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4090 2023-06-18 15:21:49.000000 netbox-contract-2.0.4/src/netbox_contract/api/serializers.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      387 2023-06-01 20:59:57.000000 netbox-contract-2.0.4/src/netbox_contract/api/urls.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      983 2023-06-18 15:21:49.000000 netbox-contract-2.0.4/src/netbox_contract/api/views.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1444 2023-06-18 15:21:49.000000 netbox-contract-2.0.4/src/netbox_contract/filtersets.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     7013 2023-06-18 16:08:41.000000 netbox-contract-2.0.4/src/netbox_contract/forms.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-18 16:14:40.474623 netbox-contract-2.0.4/src/netbox_contract/migrations/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4598 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0001_initial.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      764 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1579 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      601 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      584 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      563 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0006_alter_contract_circuit.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      403 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0007_invoice_date.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      386 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0008_invoice_comments.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      428 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0009_contract_external_reference.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      494 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0010_invoice_contracts.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0011_auto_20230122_2112.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      339 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0012_remove_invoice_contract.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      549 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      422 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0014_contract_end_date.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2104 2023-06-01 20:59:57.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0015_contractassignement.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      630 2023-06-18 15:21:49.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0016_contract_parent.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      416 2023-06-18 16:08:41.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/0017_alter_contract_accounting_dimensions.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/migrations/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5692 2023-06-18 16:08:41.000000 netbox-contract-2.0.4/src/netbox_contract/models.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2240 2023-06-18 13:35:02.000000 netbox-contract-2.0.4/src/netbox_contract/navigation.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/search.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3785 2023-06-18 15:21:49.000000 netbox-contract-2.0.4/src/netbox_contract/tables.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2027 2023-06-01 20:59:57.000000 netbox-contract-2.0.4/src/netbox_contract/template_content.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-18 16:14:40.474623 netbox-contract-2.0.4/src/netbox_contract/templates/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      917 2023-06-18 13:30:49.000000 netbox-contract-2.0.4/src/netbox_contract/templates/contract_assignements_bottom.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)      362 2023-06-18 13:30:49.000000 netbox-contract-2.0.4/src/netbox_contract/templates/contract_list_bottom.html
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-18 16:14:40.478623 netbox-contract-2.0.4/src/netbox_contract/templates/netbox_contract/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4598 2023-06-18 15:21:49.000000 netbox-contract-2.0.4/src/netbox_contract/templates/netbox_contract/contract.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)      810 2023-06-01 20:59:57.000000 netbox-contract-2.0.4/src/netbox_contract/templates/netbox_contract/contract_assignement.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2284 2023-03-12 17:52:54.000000 netbox-contract-2.0.4/src/netbox_contract/templates/netbox_contract/invoice.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1128 2023-03-12 14:46:55.000000 netbox-contract-2.0.4/src/netbox_contract/templates/netbox_contract/serviceprovider.html
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3871 2023-06-18 13:35:02.000000 netbox-contract-2.0.4/src/netbox_contract/urls.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8622 2023-06-18 13:35:02.000000 netbox-contract-2.0.4/src/netbox_contract/views.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-18 16:14:40.466622 netbox-contract-2.0.4/src/netbox_contract.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3733 2023-06-18 16:14:40.000000 netbox-contract-2.0.4/src/netbox_contract.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2276 2023-06-18 16:14:40.000000 netbox-contract-2.0.4/src/netbox_contract.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-18 16:14:40.000000 netbox-contract-2.0.4/src/netbox_contract.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-02-19 10:47:00.000000 netbox-contract-2.0.4/src/netbox_contract.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-06-18 16:14:40.000000 netbox-contract-2.0.4/src/netbox_contract.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-06-18 16:14:40.000000 netbox-contract-2.0.4/src/netbox_contract.egg-info/top_level.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-25 10:08:53.026430 netbox-contract-2.0.5/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1056 2023-01-03 17:10:18.000000 netbox-contract-2.0.5/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       87 2023-03-12 14:44:04.000000 netbox-contract-2.0.5/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4155 2023-06-25 10:08:53.022430 netbox-contract-2.0.5/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3616 2023-06-25 10:06:22.000000 netbox-contract-2.0.5/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      774 2023-06-25 10:08:29.000000 netbox-contract-2.0.5/pyproject.toml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-06-25 10:08:53.026430 netbox-contract-2.0.5/setup.cfg
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)       52 2023-01-03 18:27:10.000000 netbox-contract-2.0.5/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-25 10:08:52.910428 netbox-contract-2.0.5/src/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-25 10:08:52.954429 netbox-contract-2.0.5/src/netbox_contract/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      469 2023-06-25 10:08:36.000000 netbox-contract-2.0.5/src/netbox_contract/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-25 10:08:52.962429 netbox-contract-2.0.5/src/netbox_contract/api/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-12 14:46:55.000000 netbox-contract-2.0.5/src/netbox_contract/api/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4090 2023-06-18 15:21:49.000000 netbox-contract-2.0.5/src/netbox_contract/api/serializers.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      387 2023-06-01 20:59:57.000000 netbox-contract-2.0.5/src/netbox_contract/api/urls.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      983 2023-06-18 15:21:49.000000 netbox-contract-2.0.5/src/netbox_contract/api/views.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1444 2023-06-18 15:21:49.000000 netbox-contract-2.0.5/src/netbox_contract/filtersets.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     7178 2023-06-25 09:21:12.000000 netbox-contract-2.0.5/src/netbox_contract/forms.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-25 10:08:53.010430 netbox-contract-2.0.5/src/netbox_contract/migrations/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4598 2023-03-12 14:46:55.000000 netbox-contract-2.0.5/src/netbox_contract/migrations/0001_initial.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      764 2023-03-12 14:46:55.000000 netbox-contract-2.0.5/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1579 2023-03-12 14:46:55.000000 netbox-contract-2.0.5/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      601 2023-03-12 14:46:55.000000 netbox-contract-2.0.5/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      584 2023-03-12 14:46:55.000000 netbox-contract-2.0.5/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      563 2023-03-12 14:46:55.000000 netbox-contract-2.0.5/src/netbox_contract/migrations/0006_alter_contract_circuit.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      403 2023-03-12 14:46:55.000000 netbox-contract-2.0.5/src/netbox_contract/migrations/0007_invoice_date.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      386 2023-03-12 14:46:55.000000 netbox-contract-2.0.5/src/netbox_contract/migrations/0008_invoice_comments.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      428 2023-03-12 14:46:55.000000 netbox-contract-2.0.5/src/netbox_contract/migrations/0009_contract_external_reference.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      494 2023-03-12 14:46:55.000000 netbox-contract-2.0.5/src/netbox_contract/migrations/0010_invoice_contracts.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-03-12 14:46:55.000000 netbox-contract-2.0.5/src/netbox_contract/migrations/0011_auto_20230122_2112.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      339 2023-03-12 14:46:55.000000 netbox-contract-2.0.5/src/netbox_contract/migrations/0012_remove_invoice_contract.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      549 2023-03-12 14:46:55.000000 netbox-contract-2.0.5/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      422 2023-03-12 14:46:55.000000 netbox-contract-2.0.5/src/netbox_contract/migrations/0014_contract_end_date.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2104 2023-06-01 20:59:57.000000 netbox-contract-2.0.5/src/netbox_contract/migrations/0015_contractassignement.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      630 2023-06-18 15:21:49.000000 netbox-contract-2.0.5/src/netbox_contract/migrations/0016_contract_parent.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      416 2023-06-18 16:08:41.000000 netbox-contract-2.0.5/src/netbox_contract/migrations/0017_alter_contract_accounting_dimensions.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-03-12 14:46:55.000000 netbox-contract-2.0.5/src/netbox_contract/migrations/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5692 2023-06-18 16:08:41.000000 netbox-contract-2.0.5/src/netbox_contract/models.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2240 2023-06-18 13:35:02.000000 netbox-contract-2.0.5/src/netbox_contract/navigation.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-03-12 14:46:55.000000 netbox-contract-2.0.5/src/netbox_contract/search.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4137 2023-06-25 10:05:08.000000 netbox-contract-2.0.5/src/netbox_contract/tables.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2027 2023-06-01 20:59:57.000000 netbox-contract-2.0.5/src/netbox_contract/template_content.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-25 10:08:53.014430 netbox-contract-2.0.5/src/netbox_contract/templates/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2566 2023-06-25 09:18:53.000000 netbox-contract-2.0.5/src/netbox_contract/templates/contact_assignements_bottom.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      917 2023-06-18 13:30:49.000000 netbox-contract-2.0.5/src/netbox_contract/templates/contract_assignements_bottom.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      362 2023-06-18 13:30:49.000000 netbox-contract-2.0.5/src/netbox_contract/templates/contract_list_bottom.html
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-25 10:08:53.022430 netbox-contract-2.0.5/src/netbox_contract/templates/netbox_contract/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4598 2023-06-18 15:21:49.000000 netbox-contract-2.0.5/src/netbox_contract/templates/netbox_contract/contract.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      810 2023-06-01 20:59:57.000000 netbox-contract-2.0.5/src/netbox_contract/templates/netbox_contract/contract_assignement.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2284 2023-03-12 17:52:54.000000 netbox-contract-2.0.5/src/netbox_contract/templates/netbox_contract/invoice.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1136 2023-06-25 09:18:53.000000 netbox-contract-2.0.5/src/netbox_contract/templates/netbox_contract/serviceprovider.html
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3871 2023-06-21 19:25:05.000000 netbox-contract-2.0.5/src/netbox_contract/urls.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8640 2023-06-25 10:05:08.000000 netbox-contract-2.0.5/src/netbox_contract/views.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-25 10:08:52.958429 netbox-contract-2.0.5/src/netbox_contract.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4155 2023-06-25 10:08:52.000000 netbox-contract-2.0.5/src/netbox_contract.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2339 2023-06-25 10:08:52.000000 netbox-contract-2.0.5/src/netbox_contract.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-25 10:08:52.000000 netbox-contract-2.0.5/src/netbox_contract.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-21 12:00:44.000000 netbox-contract-2.0.5/src/netbox_contract.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-06-25 10:08:52.000000 netbox-contract-2.0.5/src/netbox_contract.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-06-25 10:08:52.000000 netbox-contract-2.0.5/src/netbox_contract.egg-info/top_level.txt
```

### Comparing `netbox-contract-2.0.4/LICENSE` & `netbox-contract-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.4/PKG-INFO` & `netbox-contract-2.0.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: netbox-contract
-Version: 2.0.4
-Summary: Contract management plugin for Netbox
-Author-email: Marc Lebreuil <marc@famillelebreuil.net>
-Project-URL: Homepage, https://github.com/mlebreuil/netbox-contract
-Project-URL: Bug Tracker, https://github.com/mlebreuil/netbox-contract/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Contract pluggin
 ## Overview
 The pluggin adds contracts and invoices model to Netbox.  
 It allows to register contract with objects.  
 Add invoices to contracts.  
 
 ## Installation
@@ -102,7 +88,14 @@
 
 * Add bulk update capability for contract assignement
 * [#63](https://github.com/mlebreuil/netbox-contract/issues/63) Correct an API issue on the invoice object.
 * [#64](https://github.com/mlebreuil/netbox-contract/issues/64) Add hierarchy to contract; New parent field created.
 * [#65](https://github.com/mlebreuil/netbox-contract/issues/65) Add end date to contact import form.
 * Removed the possibility of add or modify circuits to contracts. The field becomes read only and will be removed in next major release.
 * Make accounting dimensions optional.
+
+#### version 2.0.5
+
+* [#75](https://github.com/mlebreuil/netbox-contract/issues/74) Fix contract assignement for service providers.
+* [#73](https://github.com/mlebreuil/netbox-contract/issues/73) Add comment field to contract import form
+* [#72](https://github.com/mlebreuil/netbox-contract/issues/72) Add fields to the contract assignement bottom tables
+* Remove the 'add' actions from the contract assignment list view
```

### Comparing `netbox-contract-2.0.4/README.md` & `netbox-contract-2.0.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: netbox-contract
+Version: 2.0.5
+Summary: Contract management plugin for Netbox
+Author-email: Marc Lebreuil <marc@famillelebreuil.net>
+Project-URL: Homepage, https://github.com/mlebreuil/netbox-contract
+Project-URL: Bug Tracker, https://github.com/mlebreuil/netbox-contract/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Contract pluggin
 ## Overview
 The pluggin adds contracts and invoices model to Netbox.  
 It allows to register contract with objects.  
 Add invoices to contracts.  
 
 ## Installation
@@ -88,7 +102,14 @@
 
 * Add bulk update capability for contract assignement
 * [#63](https://github.com/mlebreuil/netbox-contract/issues/63) Correct an API issue on the invoice object.
 * [#64](https://github.com/mlebreuil/netbox-contract/issues/64) Add hierarchy to contract; New parent field created.
 * [#65](https://github.com/mlebreuil/netbox-contract/issues/65) Add end date to contact import form.
 * Removed the possibility of add or modify circuits to contracts. The field becomes read only and will be removed in next major release.
 * Make accounting dimensions optional.
+
+#### version 2.0.5
+
+* [#75](https://github.com/mlebreuil/netbox-contract/issues/74) Fix contract assignement for service providers.
+* [#73](https://github.com/mlebreuil/netbox-contract/issues/73) Add comment field to contract import form
+* [#72](https://github.com/mlebreuil/netbox-contract/issues/72) Add fields to the contract assignement bottom tables
+* Remove the 'add' actions from the contract assignment list view
```

### Comparing `netbox-contract-2.0.4/pyproject.toml` & `netbox-contract-2.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "netbox-contract"
-version = "2.0.4"
+version = "2.0.5"
 authors = [
   { name="Marc Lebreuil", email="marc@famillelebreuil.net" },
 ]
 description = "Contract management plugin for Netbox"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

### Comparing `netbox-contract-2.0.4/src/netbox_contract/api/serializers.py` & `netbox-contract-2.0.5/src/netbox_contract/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.4/src/netbox_contract/api/views.py` & `netbox-contract-2.0.5/src/netbox_contract/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.4/src/netbox_contract/filtersets.py` & `netbox-contract-2.0.5/src/netbox_contract/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.4/src/netbox_contract/forms.py` & `netbox-contract-2.0.5/src/netbox_contract/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from django import forms
 from django.contrib.contenttypes.models import ContentType
 import django_filters
 from netbox.forms import NetBoxModelForm, NetBoxModelFilterSetForm, NetBoxModelBulkEditForm, NetBoxModelImportForm
-from utilities.forms.fields import CommentField, DynamicModelChoiceField, DynamicModelMultipleChoiceField, MultipleChoiceField, CSVModelChoiceField, SlugField, CSVContentTypeField
+from utilities.forms.fields import CommentField, CSVChoiceField, DynamicModelChoiceField, DynamicModelMultipleChoiceField, MultipleChoiceField, CSVModelChoiceField, SlugField, CSVContentTypeField
 from utilities.forms.widgets import DatePicker
 from extras.filters import TagFilter
 from circuits.models import Circuit
 from tenancy.models import Tenant
 from .models import Contract, Invoice, ServiceProvider, StatusChoices, ContractAssignement
 
 class ContractForm(NetBoxModelForm):
@@ -94,27 +94,31 @@
     )
     tenant = CSVModelChoiceField(
         queryset=Tenant.objects.all(),
         to_field_name='name',
         help_text='Tenant name',
         required=False
     )
+    status = CSVChoiceField(
+        choices=StatusChoices,
+        help_text='Contract status'
+    )
     parent = CSVModelChoiceField(
         queryset=Contract.objects.all(),
         to_field_name='name',
         help_text='Contract name',
         required=False
     )
 
     class Meta:
         model = Contract
         fields = [
-            'name', 'external_partie', 'internal_partie','tenant', 'status',
+            'name', 'external_partie', 'internal_partie', 'external_reference','tenant', 'status',
             'start_date', 'end_date','initial_term', 'renewal_term', 'mrc', 'nrc',
-            'invoice_frequency', 'parent'
+            'invoice_frequency', 'documents', 'comments', 'parent'
         ]
 
 class ContractBulkEditForm(NetBoxModelBulkEditForm):
     name = forms.CharField(
         max_length=100,
         required=True
     )
```

### Comparing `netbox-contract-2.0.4/src/netbox_contract/migrations/0001_initial.py` & `netbox-contract-2.0.5/src/netbox_contract/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.4/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py` & `netbox-contract-2.0.5/src/netbox_contract/migrations/0002_alter_contract_circuit_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.4/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py` & `netbox-contract-2.0.5/src/netbox_contract/migrations/0003_alter_contract_custom_field_data_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.4/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py` & `netbox-contract-2.0.5/src/netbox_contract/migrations/0004_contract_currency_invoice_currency.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.4/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py` & `netbox-contract-2.0.5/src/netbox_contract/migrations/0005_contract_accounting_dimensions_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.4/src/netbox_contract/migrations/0006_alter_contract_circuit.py` & `netbox-contract-2.0.5/src/netbox_contract/migrations/0006_alter_contract_circuit.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.4/src/netbox_contract/migrations/0011_auto_20230122_2112.py` & `netbox-contract-2.0.5/src/netbox_contract/migrations/0011_auto_20230122_2112.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.4/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py` & `netbox-contract-2.0.5/src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.4/src/netbox_contract/migrations/0015_contractassignement.py` & `netbox-contract-2.0.5/src/netbox_contract/migrations/0015_contractassignement.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.4/src/netbox_contract/migrations/0016_contract_parent.py` & `netbox-contract-2.0.5/src/netbox_contract/migrations/0016_contract_parent.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.4/src/netbox_contract/models.py` & `netbox-contract-2.0.5/src/netbox_contract/models.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.4/src/netbox_contract/navigation.py` & `netbox-contract-2.0.5/src/netbox_contract/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.4/src/netbox_contract/search.py` & `netbox-contract-2.0.5/src/netbox_contract/search.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.4/src/netbox_contract/tables.py` & `netbox-contract-2.0.5/src/netbox_contract/tables.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,33 +30,39 @@
     )
     actions = columns.ActionsColumn(
         actions=('edit', 'delete')
     )
 
     class Meta(NetBoxTable.Meta):
         model = ContractAssignement
-        fields = ('pk','contract','contract__external_partie','contract__status', 'actions')
-        default_columns = ('pk', 'contract','contract__external_partie','contract__status')
+        fields = ('pk','contract','contract__external_partie','contract__status','contract__start_date',
+                  'contract__end_date','contract__mrc','contract__nrc', 'actions')
+        default_columns = ('pk', 'contract','contract__external_partie','contract__status','contract__start_date',
+                  'contract__end_date','contract__mrc','contract__nrc',)
 
 class ContractAssignementContractTable(NetBoxTable):
     content_type = columns.ContentTypeColumn(
         verbose_name='Object Type'
     )
     content_object = tables.Column(
         linkify=True,
+        verbose_name='Object',
         orderable=False
     )
+    content_object__status = tables.Column(
+        verbose_name='Status'
+    )
     actions = columns.ActionsColumn(
         actions=('edit', 'delete')
     )
 
     class Meta(NetBoxTable.Meta):
         model = ContractAssignement
-        fields = ('pk', 'content_type', 'content_object','actions')
-        default_columns = ('pk', 'content_type', 'content_object')
+        fields = ('pk', 'content_type', 'content_object','content_object__status','actions')
+        default_columns = ('pk', 'content_type', 'content_object','content_object__status')
 
 class ContractListTable(NetBoxTable):
 
     name = tables.Column(
         linkify=True
     )
     external_partie = tables.Column(
```

### Comparing `netbox-contract-2.0.4/src/netbox_contract/template_content.py` & `netbox-contract-2.0.5/src/netbox_contract/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.4/src/netbox_contract/templates/contract_assignements_bottom.html` & `netbox-contract-2.0.5/src/netbox_contract/templates/contract_assignements_bottom.html`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.4/src/netbox_contract/templates/netbox_contract/contract.html` & `netbox-contract-2.0.5/src/netbox_contract/templates/netbox_contract/contract.html`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.4/src/netbox_contract/templates/netbox_contract/contract_assignement.html` & `netbox-contract-2.0.5/src/netbox_contract/templates/netbox_contract/contract_assignement.html`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.4/src/netbox_contract/templates/netbox_contract/invoice.html` & `netbox-contract-2.0.5/src/netbox_contract/templates/netbox_contract/invoice.html`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.4/src/netbox_contract/templates/netbox_contract/serviceprovider.html` & `netbox-contract-2.0.5/src/netbox_contract/templates/netbox_contract/serviceprovider.html`

 * *Files 3% similar despite different names*

```diff
@@ -27,11 +27,11 @@
             </tr>
           </table>
         </div>
       </div>
       {% include 'inc/panels/custom_fields.html' %}
       {% include 'inc/panels/comments.html' %}
       {% include 'inc/panels/tags.html' %}
-      {% include 'inc/panels/contacts.html' %}
+      {% include 'contact_assignements_bottom.html' %}
     </div>
   </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {% extends 'generic/object.html' %} {% block content %}
 ** Service Provider **
 Name       {{ object.name }}
 slug       {{ object.slug }}
 portal_url {% if object.portal_url %} {{_object.portal_url_}} {% else %} {
            { ''|placeholder }} {% endif %}
 {% include 'inc/panels/custom_fields.html' %} {% include 'inc/panels/
-comments.html' %} {% include 'inc/panels/tags.html' %} {% include 'inc/panels/
-contacts.html' %}
+comments.html' %} {% include 'inc/panels/tags.html' %} {% include
+'contact_assignements_bottom.html' %}
 {% endblock content %}
```

### Comparing `netbox-contract-2.0.4/src/netbox_contract/urls.py` & `netbox-contract-2.0.5/src/netbox_contract/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-contract-2.0.4/src/netbox_contract/views.py` & `netbox-contract-2.0.5/src/netbox_contract/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,66 +1,70 @@
 from datetime import timedelta, date
 from dateutil.relativedelta import relativedelta
 from django.core.exceptions import ObjectDoesNotExist
 from django.contrib.contenttypes.models import ContentType
 from django.shortcuts import render, get_object_or_404
 from netbox.views import generic
+from tenancy.views import ObjectContactsView
 from netbox.views.generic.utils import get_prerequisite_model
 from utilities.utils import count_related, normalize_querydict
 from utilities.forms import restrict_form_fields
+from utilities.views import ViewTab, register_model_view
 from circuits.models import Circuit
-from . import forms, models, tables, filtersets
+from .models import ServiceProvider, ContractAssignement, Contract, Invoice
+from . import forms, tables, filtersets
 
 # ServiceProvider views
 
 class ServiceProviderView(generic.ObjectView):
-    queryset = models.ServiceProvider.objects.all()
+    queryset = ServiceProvider.objects.all()
 
 class ServiceProviderListView(generic.ObjectListView):
-    queryset = models.ServiceProvider.objects.all()
+    queryset = ServiceProvider.objects.all()
     table = tables.ServiceProviderListTable
     filterset = filtersets.ServiceProviderFilterSet
     filterset_form = forms.ServiceProviderFilterSetForm
 
 class ServiceProviderEditView(generic.ObjectEditView):
-    queryset = models.ServiceProvider.objects.all()
+    queryset = ServiceProvider.objects.all()
     form = forms.ServiceProviderForm
 
 class ServiceProviderDeleteView(generic.ObjectDeleteView):
-    queryset = models.ServiceProvider.objects.all()
+    queryset = ServiceProvider.objects.all()
 
 class ServiceProviderBulkImportView(generic.BulkImportView):
-    queryset = models.ServiceProvider.objects.all()
+    queryset = ServiceProvider.objects.all()
     model_form = forms.ServiceProviderCSVForm
     table = tables.ServiceProviderListTable
 
 class ServiceProviderBulkEditView(generic.BulkEditView):
-    queryset = models.ServiceProvider.objects.annotate()
+    queryset = ServiceProvider.objects.annotate()
     filterset = filtersets.ServiceProviderFilterSet
     table = tables.ServiceProviderListTable
     form = forms.ServiceProviderBulkEditForm
 
 class ServiceProviderBulkDeleteView(generic.BulkDeleteView):
-    queryset = models.ServiceProvider.objects.annotate()
+    queryset = ServiceProvider.objects.annotate()
     filterset = filtersets.ServiceProviderFilterSet
     table = tables.ServiceProviderListTable
 
 # Contract assignement view
 
 class ContractAssignementView(generic.ObjectView):
-    queryset = models.ContractAssignement.objects.all()
+    queryset = ContractAssignement.objects.all()
 
 class ContractAssignementListView(generic.ObjectListView):
-    queryset = models.ContractAssignement.objects.all()
+    queryset = ContractAssignement.objects.all()
     table = tables.ContractAssignementListTable
     filterset = filtersets.ContractAssignementFilterSet
     filterset_form = forms.ContractAssignementFilterSetForm
+    actions = ['import', 'export', ]
 
 class ContractAssignementEditView(generic.ObjectEditView):
-    queryset = models.ContractAssignement.objects.all()
+    queryset = ContractAssignement.objects.all()
     form = forms.ContractAssignementForm
 
     def alter_object(self, instance, request, args, kwargs):
         if not instance.pk and kwargs:
             # Assign the object based on URL kwargs
             content_type = get_object_or_404(ContentType, pk=request.GET.get('content_type'))
             instance.object = get_object_or_404(content_type.model_class(), pk=request.GET.get('object_id'))
@@ -69,25 +73,25 @@
     def get_extra_addanother_params(self, request):
         return {
             'content_type': request.GET.get('content_type'),
             'object_id': request.GET.get('object_id'),
         }
 
 class ContractAssignementDeleteView(generic.ObjectDeleteView):
-    queryset = models.ContractAssignement.objects.all()
+    queryset = ContractAssignement.objects.all()
 
 class ContractAssignementBulkImportView(generic.BulkImportView):
-    queryset = models.ContractAssignement.objects.all()
+    queryset = ContractAssignement.objects.all()
     model_form = forms.ContractAssignementImportForm
     table = tables.ContractAssignementListTable
 
 # Contract views
 
 class ContractView(generic.ObjectView):
-    queryset = models.Contract.objects.all()
+    queryset = Contract.objects.all()
 
     def get_extra_context(self, request, instance):
         invoices_table = tables.InvoiceListTable(instance.invoices.all())
         invoices_table.configure(request)
         circuit_table = tables.ContractCircuitListTable(instance.circuit.all())
         circuit_table.configure(request)
         assignements_table = tables.ContractAssignementContractTable(instance.assignments.all())
@@ -96,67 +100,67 @@
         return {
             'invoices_table': invoices_table,
             'circuit_table': circuit_table,
             'assignements_table': assignements_table,
         }
 
 class ContractListView(generic.ObjectListView):
-    queryset = models.Contract.objects.all()
+    queryset = Contract.objects.all()
     table = tables.ContractListTable
     filterset = filtersets.ContractFilterSet
     filterset_form = forms.ContractFilterSetForm
 
 class ContractEditView(generic.ObjectEditView):
-    queryset = models.Contract.objects.all()
+    queryset = Contract.objects.all()
     form = forms.ContractForm
 
 class ContractDeleteView(generic.ObjectDeleteView):
-    queryset = models.Contract.objects.all()
+    queryset = Contract.objects.all()
 
 class ContractBulkImportView(generic.BulkImportView):
-    queryset = models.Contract.objects.all()
+    queryset = Contract.objects.all()
     model_form = forms.ContractCSVForm
     table = tables.ContractListTable
 
 class ContractBulkEditView(generic.BulkEditView):
-    queryset = models.Contract.objects.annotate(
+    queryset = Contract.objects.annotate(
         count_circuits=count_related(Circuit, 'contracts')
     )
     filterset = filtersets.ContractFilterSet
     table = tables.ContractListTable
     form = forms.ContractBulkEditForm
 
 class ContractBulkDeleteView(generic.BulkDeleteView):
-    queryset = models.Contract.objects.annotate(
+    queryset = Contract.objects.annotate(
         count_circuits=count_related(Circuit, 'contracts')
     )
     filterset = filtersets.ContractFilterSet
     table = tables.ContractListTable
 
 # Invoice views
 
 class InvoiceView(generic.ObjectView):
-    queryset = models.Invoice.objects.all()
+    queryset = Invoice.objects.all()
 
     def get_extra_context(self, request, instance):
         contracts_table = tables.ContractListTable(instance.contracts.all())
         contracts_table.configure(request)
 
         return {
             'contracts_table': contracts_table,
         }
 
 class InvoiceListView(generic.ObjectListView):
-    queryset = models.Invoice.objects.all()
+    queryset = Invoice.objects.all()
     table = tables.InvoiceListTable
     filterset = filtersets.InvoiceFilterSet
     filterset_form = forms.InvoiceFilterSetForm
 
 class InvoiceEditView(generic.ObjectEditView):
-    queryset = models.Invoice.objects.all()
+    queryset = Invoice.objects.all()
     form = forms.InvoiceForm
 
     def get(self, request, *args, **kwargs):
         """
         GET request handler
             Overrides the ObjectEditView function to include form initialization
             with data from the parent contract object
@@ -167,15 +171,15 @@
         obj = self.get_object(**kwargs)
         obj = self.alter_object(obj, request, args, kwargs)
         model = self.queryset.model
 
         initial_data = normalize_querydict(request.GET)
         initial_data['date'] = date.today()
         if 'contracts' in initial_data.keys():
-            contract = models.Contract.objects.get(pk=initial_data['contracts'])
+            contract = Contract.objects.get(pk=initial_data['contracts'])
 
             try:
                 last_invoice = contract.invoices.latest('period_end')
                 new_period_start = last_invoice.period_end + timedelta(days=1)
             except ObjectDoesNotExist:
                 if contract.start_date :
                     new_period_start = contract.start_date
@@ -202,24 +206,24 @@
             'form': form,
             'return_url': self.get_return_url(request, obj),
             'prerequisite_model': get_prerequisite_model(self.queryset),
             **self.get_extra_context(request, obj),
         })
 
 class InvoiceDeleteView(generic.ObjectDeleteView):
-    queryset = models.Invoice.objects.all()
+    queryset = Invoice.objects.all()
 
 class InvoiceBulkImportView(generic.BulkImportView):
-    queryset = models.Invoice.objects.all()
+    queryset = Invoice.objects.all()
     model_form = forms.InvoiceCSVForm
     table = tables.InvoiceListTable
 
 class InvoiceBulkEditView(generic.BulkEditView):
-    queryset = models.Invoice.objects.all()
+    queryset = Invoice.objects.all()
     filterset = filtersets.InvoiceFilterSet
     table = tables.InvoiceListTable
     form = forms.InvoiceBulkEditForm
 
 class InvoiceBulkDeleteView(generic.BulkDeleteView):
-    queryset = models.Invoice.objects.all()
+    queryset = Invoice.objects.all()
     filterset = filtersets.InvoiceFilterSet
     table = tables.InvoiceListTable
```

### Comparing `netbox-contract-2.0.4/src/netbox_contract.egg-info/PKG-INFO` & `netbox-contract-2.0.5/src/netbox_contract.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-contract
-Version: 2.0.4
+Version: 2.0.5
 Summary: Contract management plugin for Netbox
 Author-email: Marc Lebreuil <marc@famillelebreuil.net>
 Project-URL: Homepage, https://github.com/mlebreuil/netbox-contract
 Project-URL: Bug Tracker, https://github.com/mlebreuil/netbox-contract/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -102,7 +102,14 @@
 
 * Add bulk update capability for contract assignement
 * [#63](https://github.com/mlebreuil/netbox-contract/issues/63) Correct an API issue on the invoice object.
 * [#64](https://github.com/mlebreuil/netbox-contract/issues/64) Add hierarchy to contract; New parent field created.
 * [#65](https://github.com/mlebreuil/netbox-contract/issues/65) Add end date to contact import form.
 * Removed the possibility of add or modify circuits to contracts. The field becomes read only and will be removed in next major release.
 * Make accounting dimensions optional.
+
+#### version 2.0.5
+
+* [#75](https://github.com/mlebreuil/netbox-contract/issues/74) Fix contract assignement for service providers.
+* [#73](https://github.com/mlebreuil/netbox-contract/issues/73) Add comment field to contract import form
+* [#72](https://github.com/mlebreuil/netbox-contract/issues/72) Add fields to the contract assignement bottom tables
+* Remove the 'add' actions from the contract assignment list view
```

### Comparing `netbox-contract-2.0.4/src/netbox_contract.egg-info/SOURCES.txt` & `netbox-contract-2.0.5/src/netbox_contract.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,13 +37,14 @@
 src/netbox_contract/migrations/0012_remove_invoice_contract.py
 src/netbox_contract/migrations/0013_contract_documents_invoice_documents.py
 src/netbox_contract/migrations/0014_contract_end_date.py
 src/netbox_contract/migrations/0015_contractassignement.py
 src/netbox_contract/migrations/0016_contract_parent.py
 src/netbox_contract/migrations/0017_alter_contract_accounting_dimensions.py
 src/netbox_contract/migrations/__init__.py
+src/netbox_contract/templates/contact_assignements_bottom.html
 src/netbox_contract/templates/contract_assignements_bottom.html
 src/netbox_contract/templates/contract_list_bottom.html
 src/netbox_contract/templates/netbox_contract/contract.html
 src/netbox_contract/templates/netbox_contract/contract_assignement.html
 src/netbox_contract/templates/netbox_contract/invoice.html
 src/netbox_contract/templates/netbox_contract/serviceprovider.html
```

