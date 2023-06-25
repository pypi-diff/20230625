# Comparing `tmp/pynad-2.2.0.tar.gz` & `tmp/pynad-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynad-2.2.0.tar", last modified: Mon Feb 14 13:46:00 2022, max compression
+gzip compressed data, was "pynad-3.0.0.tar", last modified: Sun Jun 25 14:53:22 2023, max compression
```

## Comparing `pynad-2.2.0.tar` & `pynad-3.0.0.tar`

### file list

```diff
@@ -1,26 +1,24 @@
-drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2022-02-14 13:46:00.292473 pynad-2.2.0/
--rw-rw-r--   0 rafael    (1000) rafael    (1000)    35152 2020-04-21 13:59:39.000000 pynad-2.2.0/LICENSE
--rw-rw-r--   0 rafael    (1000) rafael    (1000)       66 2022-02-14 13:45:35.000000 pynad-2.2.0/MANIFEST.in
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     6470 2022-02-14 13:46:00.292473 pynad-2.2.0/PKG-INFO
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     6013 2021-10-14 23:17:44.000000 pynad-2.2.0/README.rst
--rw-rw-r--   0 rafael    (1000) rafael    (1000)      607 2022-02-14 13:25:35.000000 pynad-2.2.0/changelog.txt
-drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2022-02-14 13:46:00.292473 pynad-2.2.0/pynad/
--rw-r--r--   0 rafael    (1000) rafael    (1000)      103 2021-10-14 15:15:54.000000 pynad-2.2.0/pynad/__init__.py
--rwxr--r--   0 rafael    (1000) rafael    (1000)     1548 2021-10-21 19:34:51.000000 pynad-2.2.0/pynad/aux_functions.py
--rw-r--r--   0 rafael    (1000) rafael    (1000)     1160 2021-02-26 12:43:44.000000 pynad-2.2.0/pynad/file.svg
--rw-r--r--   0 rafael    (1000) rafael    (1000)      720 2020-01-31 20:52:40.000000 pynad-2.2.0/pynad/folder.svg
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     9064 2022-02-14 13:12:13.000000 pynad-2.2.0/pynad/help.html
--rwxrwxr-x   0 rafael    (1000) rafael    (1000)    17281 2021-09-16 18:10:03.000000 pynad-2.2.0/pynad/ident.py
--rw-rw-r--   0 rafael    (1000) rafael    (1000)    11254 2021-10-14 23:42:01.000000 pynad-2.2.0/pynad/main_form.py
--rwxrwxr-x   0 rafael    (1000) rafael    (1000)     9452 2021-09-18 21:46:35.000000 pynad-2.2.0/pynad/metadata.py
--rwxrwxr-x   0 rafael    (1000) rafael    (1000)     2746 2021-09-18 19:20:24.000000 pynad-2.2.0/pynad/person.py
--rw-r--r--   0 rafael    (1000) rafael    (1000)    76748 2022-02-14 13:24:06.000000 pynad-2.2.0/pynad/pynad_app.py
-drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2022-02-14 13:46:00.292473 pynad-2.2.0/pynad.egg-info/
--rw-rw-r--   0 rafael    (1000) rafael    (1000)     6470 2022-02-14 13:46:00.000000 pynad-2.2.0/pynad.egg-info/PKG-INFO
--rw-rw-r--   0 rafael    (1000) rafael    (1000)      421 2022-02-14 13:46:00.000000 pynad-2.2.0/pynad.egg-info/SOURCES.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)        1 2022-02-14 13:46:00.000000 pynad-2.2.0/pynad.egg-info/dependency_links.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)       49 2022-02-14 13:46:00.000000 pynad-2.2.0/pynad.egg-info/entry_points.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)       23 2022-02-14 13:46:00.000000 pynad-2.2.0/pynad.egg-info/requires.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)        6 2022-02-14 13:46:00.000000 pynad-2.2.0/pynad.egg-info/top_level.txt
--rw-rw-r--   0 rafael    (1000) rafael    (1000)      104 2021-10-14 15:54:16.000000 pynad-2.2.0/pyproject.toml
--rw-rw-r--   0 rafael    (1000) rafael    (1000)      631 2022-02-14 13:46:00.292473 pynad-2.2.0/setup.cfg
+drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2023-06-25 14:53:22.956679 pynad-3.0.0/
+-rw-r--r--   0 rafael    (1000) rafael    (1000)    35152 2020-04-21 13:59:39.000000 pynad-3.0.0/LICENSE
+-rw-r--r--   0 rafael    (1000) rafael    (1000)       22 2023-06-25 13:22:31.000000 pynad-3.0.0/MANIFEST.in
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     4057 2023-06-25 14:53:22.956679 pynad-3.0.0/PKG-INFO
+-rw-r--r--   0 rafael    (1000) rafael    (1000)     3636 2023-06-25 14:51:28.000000 pynad-3.0.0/README.rst
+-rw-r--r--   0 rafael    (1000) rafael    (1000)      803 2023-06-25 13:21:18.000000 pynad-3.0.0/changelog.txt
+drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2023-06-25 14:53:22.956679 pynad-3.0.0/pynad/
+-rw-r--r--   0 rafael    (1000) rafael    (1000)      103 2023-06-25 14:09:36.000000 pynad-3.0.0/pynad/__init__.py
+-rw-r--r--   0 rafael    (1000) rafael    (1000)     2542 2023-06-13 23:56:24.000000 pynad-3.0.0/pynad/auxiliares.py
+-rw-r--r--   0 rafael    (1000) rafael    (1000)    11436 2023-06-25 14:11:15.000000 pynad-3.0.0/pynad/converter.py
+-rw-r--r--   0 rafael    (1000) rafael    (1000)    10210 2023-06-25 14:11:15.000000 pynad-3.0.0/pynad/copia_local.py
+-rw-r--r--   0 rafael    (1000) rafael    (1000)    12078 2023-06-25 14:11:15.000000 pynad-3.0.0/pynad/metadados.py
+-rw-r--r--   0 rafael    (1000) rafael    (1000)    20460 2023-06-25 14:11:15.000000 pynad-3.0.0/pynad/paineis.py
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)    24138 2023-06-25 14:11:15.000000 pynad-3.0.0/pynad/paineis_id.py
+-rw-r--r--   0 rafael    (1000) rafael    (1000)    10619 2023-06-25 14:47:47.000000 pynad-3.0.0/pynad/pynad.py
+drwxrwxr-x   0 rafael    (1000) rafael    (1000)        0 2023-06-25 14:53:22.956679 pynad-3.0.0/pynad.egg-info/
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)     4057 2023-06-25 14:53:22.000000 pynad-3.0.0/pynad.egg-info/PKG-INFO
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)      394 2023-06-25 14:53:22.000000 pynad-3.0.0/pynad.egg-info/SOURCES.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)        1 2023-06-25 14:53:22.000000 pynad-3.0.0/pynad.egg-info/dependency_links.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)       47 2023-06-25 14:53:22.000000 pynad-3.0.0/pynad.egg-info/entry_points.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)       13 2023-06-25 14:53:22.000000 pynad-3.0.0/pynad.egg-info/requires.txt
+-rw-rw-r--   0 rafael    (1000) rafael    (1000)        6 2023-06-25 14:53:22.000000 pynad-3.0.0/pynad.egg-info/top_level.txt
+-rw-r--r--   0 rafael    (1000) rafael    (1000)      104 2021-10-14 15:54:16.000000 pynad-3.0.0/pyproject.toml
+-rw-r--r--   0 rafael    (1000) rafael    (1000)      617 2023-06-25 14:53:22.956679 pynad-3.0.0/setup.cfg
```

### Comparing `pynad-2.2.0/LICENSE` & `pynad-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynad-2.2.0/README.rst` & `pynad-3.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,56 +1,54 @@
+Metadata-Version: 2.1
+Name: pynad
+Version: 3.0.0
+Summary: An application to manage Pnadc microdata and setup its panels
+Author: Rafael Guerreiro Osorio
+Author-email: rafael.osorio@ipea.gov.br
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+License-File: LICENSE
+
 #####
 pynad
 #####
 An application to download, sync, organize and prepare the microdata and metadata of the Brazilian National Household Survey, **Pesquisa Nacional por Amostra de Domicílios Contínua** - **Pnadc** - fielded by the Instituto Brasileiro de Geografia e Estatística, `IBGE <http://www.ibge.gov.br>`_.
 
 The **PNADC** is a rotating panel survey. The residential dwellings sampled for a panel are visited five times, quarterly. Every quarter a new panel starts, thus there are five active panels in visits 1 to 5. However, IBGE only disseminates Pnadc microdata as cross-section datasets, aggregating records from distinct panels. The *trimestral* and the *anual-trimestre* datasets are aggregates of the distinct visits of the five panels surveyed in a quarter; the *anual-visita* datasets are annual aggregates of first or fifth visit interviews, comprised by four panels visited for the first or fifth time in a year.
 
 ----------------
 What pynad does?
 ----------------
 **IBGE periodically releases new PNADC datasets and documents. Eventually, previously released datasets and documents are patched. Currently, there are more than a hundred files to download and monitor for updates.**
 
-Pynad ascertains one always have the latest versions of data and documents, and helps to keep track of the versions used in an application. It clones the *Microdados* folder of the Pnadc distributions at IBGE's `FTP server <ftp://ftp.ibge.gov.br/>`_ as a local archive, a compressed **zip** file, syncing it at user demand.
+Pynad ascertains one always have the latest versions of data and documents, and helps to keep track of the versions used in an application. It clones the *Microdados* folder of the Pnadc distributions at IBGE's `FTP server <ftp://ftp.ibge.gov.br/>`_ copying all its files to a local folder, syncing it at user demand.
 
 **PNADC datasets are disseminated as text files with fixed width records. The position of each variable in the record must be declared to load them. The full metadata (names and columns of variables, categories etc.) are in binary xls Excel files.**
 
-Pynad converts the original microdata to standard **csv** text files, conveniently organizes copies of the original *dicionários de variáveis*, and generates machine and human readable **json** text files containing all metadata. The new files are stored in the archive containing the local copy of the PNADC, in distinct folders.
+Pynad converts the original microdata to standard **csv** text files and/or **parquet** binary files; conveniently organizes copies of the original *dicionários de variáveis*; and generates machine and human readable **json** text files containing all metadata. The new files are stored in the archive containing the local copy of the PNADC, in distinct folders.
 
-When the local copy is synced, pynad updates the metadata and **csv** files on a need basis.
+When the local copy is synced, pynad updates the metadata and **csv** and/or **parquet** files on a need basis.
 
 **PNADC datasets are organized for use as a quarterly or annual cross-section survey, mixing records from 4 or 5 distinct panels. One panel has variables scattered in different datasets. Though dwellings are identified, households and individuals are not. Population weights are not available for the panels**
 
-Pynad creates another archive for panel files. It separates the panels retrieving their records from the cross-sectional datasets and generates a **csv** microdata file for each panel. Then pynad identifies the households and individuals in each dwelling and generates a **csv** microdata file with the keys for each panel.
-
-Finally, pynad joins the panels and identifiers, and reshapes the joined datasets as identified individual records. Original variables have up to five instances in the identified individual records. E.g. for literacy, v3001, the identified individual record has v3001_1, v3001_2 v3001_3, v3001_4, v3001_5.
-
-After reshaping, it calculates and adds panel population weights to the records. Then the records are split in variable blocks: basic, education, labour, income etc. A **csv** microdata file of identified individual records is created for each block of every panel.
+Pynad creates another archive for panel files. It separates the panels retrieving their records from the cross-sectional datasets, then pynad identifies the households and individuals in each dwelling and generates and generates a **parquet**  and/or a **csv**  microdata file for each panel.
+Original variables have up to five instances in the identified individual records. E.g. for literacy, v3001, the identified individual record has v3001_1, v3001_2 v3001_3, v3001_4, v3001_5.
 
-When the local copy is synced, and the metadata and **csv** files updated, pynad updates the panel files on a need basis.
+Pynad updates the panel files on a need basis.
 
 -------
 Install
 -------
 `Windows <https://docs.python.org/3/using/windows.html#install-layout-option>`_ users should add Python to the PATH environment variable.
 
 Use `pip <https://docs.python.org/3/installing/index.html#installing-index>`_ to install pynad.
 
+Type *pynad* in a terminal to run it.
+
 ************
 Requirements
 ************
-Four additional packages will be installed: `Tablib <https://pypi.org/project/tablib/>`_, `xlrd <https://pypi.org/project/xlrd/>`_, `xlwt <https://pypi.org/project/xlwt/>`_, `PyQt5 <https://pypi.org/project/PyQt5/>`_.
-
-A computer with **16GB RAM** is recommended, as it can use more than 12GB when processing large panels.
-
-Optionally, pynad's performance will improve if a command line compression utility is available.
-
-***********
-Performance
-***********
-IBGE disseminates microdata in text files with fixed width field records. Pynad does not load the content of the original microdata files as numeric data types. It operates with text records converted to comma separated values. Handling, writing and compressing text files, particularly those with lenghty records, takes time, around 10-20 minutes to process a panel. In the first use, some hours will be required to process the more than 30 panels available.
-
-Archives with compressed files have one major drawback: there is no fast and safe way to delete a compressed file. Compression utilities that offer a delete option actually replace the archive by a new one excluding the "deleted" files. Therefore, it takes more time to delete a small file from a large archive than to delete a large file.
-
-The standard Python package `zipfile <https://docs.python.org/3/library/zipfile.html?highlight=zipfile#module-zipfile>`_ does not have a method to delete files. Although it can be easily implemented - write a temporary archive excluding the undesirable files, exclude the old archive, and rename the temporary archive to replace it - its performance is very bad when compared to that of compression utilities such as `zip <http://infozip.sourceforge.net/Zip.html>`_ or `7zip <https://www.7-zip.org/>`_. In Linux, usually **zip** is already installed or is available in the software repositories, and **7zip** can be installed using the **p7zip-full** package. Windows users must make sure the utilitiy is on the system PATH.
+Two additional packages will be installed: `pyarrow <https://pypi.org/project/pyarrow/>`_, `xlrd <https://pypi.org/project/xlrd/>`_.
 
-Pynad will try to subprocess **zip** or **7zip** to delete files from the archives. If none is found, pynad will resort to the standard library to remove outdated files from the archives.
+At least 200GB free storage if generating uncompressed **csv** files.
```

### Comparing `pynad-2.2.0/changelog.txt` & `pynad-3.0.0/changelog.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
 Pynad
 
+v3.0.0 - Volta para interface com linha de comando; tira seleção de arquivos; operações com pyarrow e arquivos parquet; somente arquivo de painel deitado
+         e sem pesos BS; mais rápido
 v2.2.0 - Separação dos pesos de bootstrap em arquivos por domicílio; correção do comportamento de seleção de arquivos na árvore - exibe sempre os arquivos remotos, arquivos que existem na cópia local mas não no IBGE não são exibidos
 v2.1.0 - Resolvido problema do registro da seleção de arquivos para garantir que novos arquivos estejam sempre marcados para download
 v2.0.14 - Resolvidos problemas em arquivos de configuração do pacote para download com pip
 v2.0.0 - Primeira versão com interface gráfica
 v1.x.x - Versões inciais sem interface gráfica (quase todas tem algum bug)
```

### Comparing `pynad-2.2.0/pynad/metadata.py` & `pynad-3.0.0/pynad/metadados.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,179 +1,223 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-2020 - Rafael Guerreiro Osorio - Ipea.
+Organiza os metadados da Pnadc.
 
-pynad - métodos de extração de metadados
+pynad v3
+Ipea - 2023
+Rafael Guerreiro Osorio
 
 ROTINAS QUE DEPENDEM DE COMO O IBGE DIVULGA METADADOS
 """
-
+import json
 import re
-from io import BytesIO
-from pathlib import Path, PurePosixPath as pPath
-from zipfile import ZipFile, ZIP_DEFLATED
-from tablib import Dataset
-
-# constantes para os microdados da PNADC
-PNADCA = 'anual'
-PNADCT = 'trimestral'
-FTP_FOLDERS = {PNADCA: ('Trabalho_e_Rendimento',
-                        'Pesquisa_Nacional_por_Amostra_de_Domicilios_continua',
-                        'Anual', 'Microdados'),
-               PNADCT: ('Trabalho_e_Rendimento',
-                        'Pesquisa_Nacional_por_Amostra_de_Domicilios_continua',
-                        'Trimestral', 'Microdados')}
+import time
+import zipfile
+from shutil import rmtree
+from pathlib import Path
+import xlrd
+from .copia_local import COPIA_LOCAL, PNADCA, PNADCT, list_local_files
+from .auxiliares import elapsed, pausar, CRCLR
+
+
+DICTRI = 'dicionario_PNADC_microdados_trimestral.xls'
+
 
 # pastas especificas no IBGE
 TRIDOCS = 'Documentacao'
 CA_DOCS = 'Documentacao'
 CA_DATA = 'Dados'
 CA_VIS = 'Visita'
 CA_TRI = 'Trimestre'
 
 # nome para pastas das cópias locais e paineis
-ORI = 'originais'
 META = 'metadados'
-MICRO = 'microdados'
-REGPES = 'pessoas'
-REGIND = 'individuos'
-REGPID = 'chaves'
+METALIST = 'pnadc.microdados.dicionarios.json'
 
 # chaves dos dicionários de variáveis json
 _VPART = 'parte'  # parte do registro: identificação e controle etc.
 _VDESC = 'nome'  # nome da variável
 _VPER = 'periodo'  # periodo
-_VPOS = 'colunas'  # posição no arquivo original
+_VPOS = 'colunas'  # posição no arquivo COPIA_LOCALginal
 _VSIZE = 'bytes'  # bytes necessários para o tipo de dado
-_VCAT = 'valores'  # categorias ou valores
+_VCAT = 'valores'  # categCOPIA_LOCALas ou valores
 _VQUES = 'quesito'  # número da questão para variáveis do questionário
 _MISS = 'vazio'  # chave para "não aplicável" em _VCAT
 
 
-def _metadata_pnadc_anual(mirrorfile):
+def import_xls(xls):
+    """Importa um dicionário de variáveis e retorna em texto TSV."""
+    dicionario = xlrd.open_workbook(xls).sheet_by_index(0)
+    rows = dicionario.nrows
+    cols = dicionario.ncols
+    tsv = ''
+    for row in range(rows):
+        for col in range(cols):
+            try:
+                datum = str(int(
+                    dicionario.cell_value(row, col))).replace('\n', ' ')
+            except ValueError:
+                datum = str(
+                    dicionario.cell_value(row, col)).replace('\n', ' ')
+            tsv += datum + '\t'
+        tsv = tsv[:-1] + '\n'
+    return tsv
+
+
+def generate(folder):
+    """Gera ou atualiza os metadados."""
+    print('METADADOS\n')
+    start = time.time()
+    # é mais prático remover e gerar
+    # os metadados do que atualizá-los
+    try:
+        rmtree(Path(folder, META))
+    except FileNotFoundError:
+        pass
+    finally:
+        Path(folder, META).mkdir()
+    arquivos = [str(Path(folder, COPIA_LOCAL, arq['path'], arq['name']))
+                for arq in list_local_files(folder)]
+    anuais = metadata_pnadc_anual(folder, arquivos, start)
+    trimestrais = metadata_pnadc_trimestral(folder, arquivos, start)
+    microdados = []
+    for anual in anuais:
+        processados = []
+        target = Path(folder, META, Path(anual[1]).name)
+        if anual[1] not in processados:
+            processados.append(anual[1])
+            with open(anual[1], 'rb') as src:
+                with open(target, 'wb') as tgt:
+                    tgt.write(src.read())
+        if anual[2][0] not in processados:
+            processados.append(anual[2][0])
+            with open(anual[2][0], 'w', encoding='utf-8') as tgt:
+                tgt.write(json.dumps(anual[2][1]))
+        microdados.append((anual[0], anual[1], anual[2][0]))
+    if trimestrais:
+        with open(trimestrais[0][2][0], 'w', encoding='utf-8') as tgt:
+            tgt.write(json.dumps(trimestrais[0][2][1]))
+        for tri in trimestrais:
+            microdados.append((tri[0], tri[1], tri[2][0]))
+        target = Path(folder, META, METALIST)
+        with open(target, 'w', encoding='utf-8') as tgt:
+            tgt.write(json.dumps(microdados))
+    print(f'{CRCLR}Metadados gerados em {elapsed(start)}\n')
+    pausar()
+
+
+def metadata_pnadc_anual(folder, arquivos, start):
     """
     Extrai e organiza metadados da pnadc anual.
 
     Esta rotina depende de como o IBGE organiza os
     arquivos para divulgação
 
     Em dezembro de 2019 a estrutura de disseminação da pnadc
     anual mudou radicalmente
 
     Há pastas para:
      - 5 visitas (dicionario por visita e por ano)
      - 4 trimestres (dicionário por trimestre vale para todos os anos)
     """
-    archive = ZipFile(mirrorfile, 'a', ZIP_DEFLATED)
-    microdados = _metadata_pnadc_anual_arquivos(archive.namelist())
+    microdados = metadata_pnadc_anual_arquivos(folder, arquivos)
     for microdado in microdados:
+        print(f'{CRCLR}Gerando metadados {elapsed(start)}', end='')
         # lê o dicionário correspondente
-        temp = BytesIO(archive.read(microdado[1]))
-        doc = Dataset()
-        doc.load(temp.getvalue(), format='xls')
-        dicionario = _metadata_pnadc_vars(doc.export('tsv'))
-
-        # acrescenta à lista
+        dicionario = metadata_pnadc_vars(import_xls(microdado[1]))
         nome = Path(microdado[0]).name
         if 'trimestre' in nome:
             dicid = nome[:-4].split('_')[2]
         else:
-            dicid = '.'.join(nome[:-4].split('_')[1:3])
-        target = f'variaveis.pnadc.anual.{dicid}.json'
-        microdado[2] = [str(pPath(META, target)), dicionario]
-    archive.close()
+            dicid = '.'.join((nome[:-4].split('_')[2],
+                              nome[:-4].split('_')[1]))
+        target = f'pnadc.variaveis.anual.{dicid}.json'
+        microdado[2] = [str(Path(folder, META, target)), dicionario]
     return microdados
 
 
-def _metadata_pnadc_anual_arquivos(zipitems):
+def metadata_pnadc_anual_arquivos(folder, arquivos):
+    """Identifica arquivos de microdados anuais."""
     microdados = []
     for vis in range(1, 6):
-        datafolder = pPath(ORI, PNADCA, CA_VIS, f'{CA_VIS}_{vis}', CA_DATA)
-        docsfolder = pPath(ORI, PNADCA, CA_VIS, f'{CA_VIS}_{vis}', CA_DOCS)
-        docfiles = [item for item in zipitems
+        datafolder = Path(folder, COPIA_LOCAL, PNADCA, CA_VIS,
+                          f'{CA_VIS}_{vis}', CA_DATA)
+        docsfolder = Path(folder, COPIA_LOCAL, PNADCA, CA_VIS,
+                          f'{CA_VIS}_{vis}', CA_DOCS)
+        docfiles = [item for item in arquivos
                     if str(docsfolder) in item
                     and 'dicionario' in item
                     and item.endswith('xls')]
-        datafiles = [item for item in zipitems
+        datafiles = [item for item in arquivos
                      if str(datafolder) in item
                      and item.endswith('zip')]
+
+        # relaciona arquivos de microdados com dicionarios de variaveis
         for doc in docfiles:
             anodoc = Path(doc).name.split('_')[3]
             microdados.extend([[item, doc, '', PNADCA]
                                for item in datafiles
                                if (Path(item).name.split('_')[1]
                                    == anodoc and f'{CA_VIS.lower()}{vis}'
                                    in item) or
                                (Path(item).name.split('_')[1]
                                 in ('2013', '2014') and
                                 f'{CA_VIS.lower()}{vis}'
                                 in item and anodoc == '2012')])
     for tri in range(1, 5):
-        datafolder = pPath(ORI, PNADCA, CA_TRI, f'{CA_TRI}_{tri}', CA_DATA)
-        docsfolder = pPath(ORI, PNADCA, CA_TRI, f'{CA_TRI}_{tri}', CA_DOCS)
-        docfiles = [item for item in zipitems
+        datafolder = Path(folder, COPIA_LOCAL, PNADCA, CA_TRI,
+                          f'{CA_TRI}_{tri}', CA_DATA)
+        docsfolder = Path(folder, COPIA_LOCAL, PNADCA, CA_TRI,
+                          f'{CA_TRI}_{tri}', CA_DOCS)
+        docfiles = [item for item in arquivos
                     if str(docsfolder) in item
                     and 'dicionario' in item
                     and item.endswith('xls')]
-        datafiles = [item for item in zipitems
+        datafiles = [item for item in arquivos
                      if str(datafolder) in item
                      and item.endswith('zip')]
         if docfiles:
             doc = docfiles[0]
             microdados.extend([[item, doc, '', PNADCA]
                                for item in datafiles])
     return microdados
 
 
-def _metadata_pnadc_trimestral(mirrorfile):
+def metadata_pnadc_trimestral(folder, arquivos, start):
     """
     Extrai e organiza metadados da pnadc trimestral.
 
     Esta rotina depende de como o IBGE organiza os
     arquivos para divulgação
     """
-    archive = ZipFile(mirrorfile, 'a', ZIP_DEFLATED)
-
     # apenas um dicionário para a pnadc trimestral
-    file = [file for file in archive.namelist() if
-            all(stub in file for stub
-                in (ORI, PNADCT, TRIDOCS, 'Dicionario_e_input'))]
-
-    if not file:
-        archive.close()
-        return None
-
-    file = file[0]
-
-    # ler o arquivo zip do dicionário e obter metadados
-    buffer = BytesIO(archive.read(file))
-    file = ZipFile(buffer)
-    diciori = [item for item in file.namelist()
-               if 'dicionario' in item][0]
-    original = BytesIO(file.read(diciori))
-
-    # le o dicionario com tablib e converte para tsv
-    doc = Dataset()
-    doc.load(original.getvalue(), format='xls')
-    dicionario = _metadata_pnadc_vars(doc.export('tsv'))
-    target = str(pPath(META, 'variaveis.pnadc.trimestral.json'))
+    archive = [file for file in arquivos if
+               all(stub in file for stub
+                   in (COPIA_LOCAL, PNADCT, TRIDOCS,
+                       'Dicionario_e_input'))][0:1]
+    if not archive:
+        return []
+    with zipfile.ZipFile(archive[0]) as zpf:
+        zpf.extract(DICTRI, str(Path(folder, META)))
+    dicionario = metadata_pnadc_vars(import_xls(
+        str(Path(folder, META, DICTRI))))
+    target = str(Path(folder, META, 'pnadc.variaveis.trimestral.json'))
 
     # lista com os arquivos de microdados trimestrais
-    arquivos = archive.namelist()
-    arquivos.remove('pynad.json')
-    microdados = [[item, diciori, [target, dicionario, original], PNADCT]
-                  for item in arquivos
-                  if ORI in item and PNADCT in item and
-                  item.split('/')[2].isnumeric()]
-    archive.close()
+    microdados = [[arq, str(Path(folder, META, DICTRI)),
+                   [target, dicionario], PNADCT]
+                  for arq in arquivos
+                  if COPIA_LOCAL in arq and PNADCT in arq and
+                  any(parte.isnumeric() for parte in Path(arq).parts)]
+    print(f'{CRCLR}Gerando metadados {elapsed(start)}', end='')
     return microdados
 
 
-def _metadata_pnadc_vars(contents):
+def metadata_pnadc_vars(contents):
     """Depende da estrutura dos dicionários de variáveis."""
     def __clean_label(label):
         label = label.replace('"', '').strip()
         label = label.replace('\n', ' ')
         label = re.sub(' +', ' ', label)
         try:
             label = int(float(label))
@@ -206,15 +250,15 @@
     meta = {}
     curvar = None
 
     # seção do questionário
     parte = ''
 
     # pula linhas de cabeçalho e processa
-    rows = contents.split('\r\n')[3:-1]
+    rows = contents.split('\n')[3:-1]
     for row in rows:
 
         # line breaks, double spaces e outras coisas
         # limpar campos para processar linhas
         fields = [__clean_label(field) for field in row.split('\t')]
 
         # linha com informação de "parte" do questionário
@@ -260,16 +304,36 @@
                     or any(item in fields[5].lower() for item in especial)):
                 meta[curvar][_VCAT][fields[5]] = str(fields[6]).lower()
             elif fields[5] or fields[6]:
                 meta[curvar][_VCAT] = ', '.join([item.lower()
                                                  for item in fields[5:7]
                                                  if item])
 
-        # linha de categoria
+        # linha de categCOPIA_LOCALa
         elif not fields[0] and not fields[1]:
             if not fields[5]:
                 fields[5] = _MISS
             try:
                 meta[curvar][_VCAT][fields[5]] = fields[6].strip().lower()
             except TypeError:
-                print(curvar, fields)
+                # INSPECIONAR AQUI SE ESTIVEREM FALTANDO CATEGCOPIA_LOCALAS
+                # print(curvar, fields)
+                pass
     return meta
+
+
+def csv_name(file, keep_ext=False):
+    """Retorna o nome do arquivo a partir do original e tipo de pnad."""
+    name = str(Path(file).name)
+    # originalmente era só csv, mas podem ser zip ou parquet
+    ext = name[-name[::-1].find('.'):]
+    if str(Path(COPIA_LOCAL, PNADCA)) in file:
+        stub = '.'.join((name[:-4].split('_')[2],
+                         name[:-4].split('_')[1]))
+        pnad = PNADCA
+    else:
+        stub = name[:-4].split('_')
+        stub = f'{stub[1][2:]}.{stub[1][1]}'
+        pnad = PNADCT
+    if keep_ext:
+        return f'pnadc.microdados.{pnad}.{stub}.{ext}'
+    return f'pnadc.microdados.{pnad}.{stub}.csv'
```

### Comparing `pynad-2.2.0/setup.cfg` & `pynad-3.0.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 [metadata]
 name = pynad
-version = 2.2.0
+version = 3.0.0
 author = Rafael Guerreiro Osorio
 author_email = rafael.osorio@ipea.gov.br
 description = An application to manage Pnadc microdata and setup its panels
 long_description = file: README.rst
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 	Operating System :: OS Independent
 
 [options]
 include_package_data = True
 packages = pynad
 python_requires = >=3.6
 install_requires = 
-	tablib
+	pyarrow
 	xlrd
-	xlwt
-	pyqt5
 
 [options.entry_points]
 gui_scripts = 
-	pynad = pynad.pynad_app: pynad_app
+	pynad = pynad.pynad: main_script
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

