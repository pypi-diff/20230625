# Comparing `tmp/gpubs-2.tar.gz` & `tmp/gpubs-3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpubs-2.tar", last modified: Fri Jun 23 09:33:36 2023, max compression
+gzip compressed data, was "gpubs-3.tar", last modified: Fri Jun 23 21:26:59 2023, max compression
```

## Comparing `gpubs-2.tar` & `gpubs-3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-06-23 09:33:36.675703 gpubs-2/
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)       28 2023-06-23 03:40:04.000000 gpubs-2/MANIFEST.in
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      261 2023-06-23 09:33:36.675703 gpubs-2/PKG-INFO
-drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-06-23 09:33:36.675703 gpubs-2/gpubs/
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      129 2023-06-23 03:11:20.000000 gpubs-2/gpubs/__init__.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)       18 2023-06-23 09:33:36.000000 gpubs-2/gpubs/_version.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)    14654 2023-06-23 09:16:16.000000 gpubs-2/gpubs/api.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1829 2023-06-21 14:00:14.000000 gpubs-2/gpubs/fetch.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      210 2023-06-21 02:49:51.000000 gpubs-2/gpubs/log.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     5743 2023-06-21 13:08:21.000000 gpubs-2/gpubs/models.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     3279 2023-06-21 14:09:08.000000 gpubs-2/gpubs/parse.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1292 2023-06-21 13:33:20.000000 gpubs-2/gpubs/reference.py
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1939 2023-06-21 02:50:26.000000 gpubs-2/gpubs/search_words.py
-drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-06-23 09:33:36.675703 gpubs-2/gpubs.egg-info/
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      261 2023-06-23 09:33:36.000000 gpubs-2/gpubs.egg-info/PKG-INFO
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      411 2023-06-23 09:33:36.000000 gpubs-2/gpubs.egg-info/SOURCES.txt
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)        1 2023-06-23 09:33:36.000000 gpubs-2/gpubs.egg-info/dependency_links.txt
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)       76 2023-06-23 09:33:36.000000 gpubs-2/gpubs.egg-info/requires.txt
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)        6 2023-06-23 09:33:36.000000 gpubs-2/gpubs.egg-info/top_level.txt
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)      359 2023-06-23 05:04:20.000000 gpubs-2/release-info.json
-drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-06-23 09:33:36.675703 gpubs-2/scripts/
--rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     4101 2023-06-21 02:46:43.000000 gpubs-2/scripts/create_search_terms_file.sh
--rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     5195 2023-06-21 02:46:43.000000 gpubs-2/scripts/download_pubs.sh
--rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     1892 2023-06-21 02:46:43.000000 gpubs-2/scripts/search.awk
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)       38 2023-06-23 09:33:36.675703 gpubs-2/setup.cfg
--rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1164 2023-06-23 04:40:13.000000 gpubs-2/setup.py
+drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-06-23 21:26:59.471773 gpubs-3/
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)       28 2023-06-23 03:40:04.000000 gpubs-3/MANIFEST.in
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      261 2023-06-23 21:26:59.471773 gpubs-3/PKG-INFO
+drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-06-23 21:26:59.471773 gpubs-3/gpubs/
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      129 2023-06-23 03:11:20.000000 gpubs-3/gpubs/__init__.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)       18 2023-06-23 21:26:59.000000 gpubs-3/gpubs/_version.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)    15302 2023-06-23 21:11:44.000000 gpubs-3/gpubs/api.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1829 2023-06-21 14:00:14.000000 gpubs-3/gpubs/fetch.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      210 2023-06-21 02:49:51.000000 gpubs-3/gpubs/log.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     6583 2023-06-23 20:45:43.000000 gpubs-3/gpubs/models.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     3989 2023-06-23 21:12:15.000000 gpubs-3/gpubs/parse.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1292 2023-06-21 13:33:20.000000 gpubs-3/gpubs/reference.py
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1939 2023-06-21 02:50:26.000000 gpubs-3/gpubs/search_words.py
+drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-06-23 21:26:59.471773 gpubs-3/gpubs.egg-info/
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      261 2023-06-23 21:26:59.000000 gpubs-3/gpubs.egg-info/PKG-INFO
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      411 2023-06-23 21:26:59.000000 gpubs-3/gpubs.egg-info/SOURCES.txt
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)        1 2023-06-23 21:26:59.000000 gpubs-3/gpubs.egg-info/dependency_links.txt
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)       76 2023-06-23 21:26:59.000000 gpubs-3/gpubs.egg-info/requires.txt
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)        6 2023-06-23 21:26:59.000000 gpubs-3/gpubs.egg-info/top_level.txt
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)      359 2023-06-23 21:26:38.000000 gpubs-3/release-info.json
+drwxr-xr-x   0 krobasky  (1000) krobasky  (1000)        0 2023-06-23 21:26:59.471773 gpubs-3/scripts/
+-rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     4101 2023-06-21 02:46:43.000000 gpubs-3/scripts/create_search_terms_file.sh
+-rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     5195 2023-06-21 02:46:43.000000 gpubs-3/scripts/download_pubs.sh
+-rwxr-xr-x   0 krobasky  (1000) krobasky  (1000)     1892 2023-06-21 02:46:43.000000 gpubs-3/scripts/search.awk
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)       38 2023-06-23 21:26:59.471773 gpubs-3/setup.cfg
+-rw-r--r--   0 krobasky  (1000) krobasky  (1000)     1164 2023-06-23 04:40:13.000000 gpubs-3/setup.py
```

### Comparing `gpubs-2/gpubs/api.py` & `gpubs-3/gpubs/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 from gpubs.models import ReferenceData
 from gpubs.log import msg1, msg2
 from gpubs.reference import download_gene_symbols, extract_gene_data
 from gpubs.search_words import fetch_brown_corpus, create_stop_words, read_search_stop, filter_search_terms
 from gpubs.fetch import check_disk_space, download_file, verify_md5
-from gpubs.parse import get_pub_df
+from gpubs.parse import parse_pubs
 
 def create_gene_reference_data(m: ReferenceData):
     
     raw_gene_info_filepath = os.path.join(m.raw_path(), m.gene_info_filename)
     reference_gene_symbols_filepath = os.path.join(m.reference_path(), m.gene_symbols_filename)
     reference_gene_synonyms_filepath = os.path.join(m.reference_path(), m.gene_synonyms_filename)
     dbxref_path = m.dbxref_path()
@@ -146,47 +146,60 @@
     if final_file is not None:
         with open(final_file, "w") as f:
             f.writelines('\n'.join(final_terms))
     msg2(verbose, f"Created {final_file}")
     return final_terms
 
 
-def fetch_abstracts(m: ReferenceData):
+def fetch_abstracts(m: ReferenceData, get_updates: bool = False):
+    """ Downloads files from m.ncbi_ftp_host. 
+
+    ARGS:
+
+      get_updates: If True then download the updatefiles, otherwise get the baseline. See : https://ftp.ncbi.nlm.nih.gov/pubmed/baseline/README.txt
+
+    """
     import subprocess
     
     num_files = m.num_abstract_xml_files
     refresh = m.refresh_abstract_xml_files
+    ftp_host = m.ncbi_ftp_host
     download_dir = m.pub_inpath()
     verbose = m.verbose
+    if get_updates:
+        download_dir = os.path.join(download_dir, m.abstract_updatefiles_inpath)
+        ftp_path = m.ncbi_ftp_updatefiles_path
+        msg2(verbose, f"! Getting update files, download_dir={download_dir}.")
+    else:
+        ftp_path = m.ncbi_ftp_baseline_path
     
     """ This can probably be done faster with download_files.sh """ 
     msg2(verbose, f"Download Directory: {download_dir}")
     msg2(verbose, f"Number of abstracts to ensure have been downloaded: {num_files}")
     msg2(verbose, f"Refresh: {refresh}")
 
-    # FTP settings
-    ftp_host = "ftp.ncbi.nlm.nih.gov"
-    ftp_path = "/pubmed/baseline/"
 
     # Retrieve file names and find the largest number
     #file_list = subprocess.check_output(['curl', '-s', f"ftp://{ftp_host}{ftp_path}"]).decode().splitlines()
     
     output = subprocess.check_output(['curl', '-s', f"ftp://{ftp_host}{ftp_path}"]).decode()
+    msg2(verbose, f"file_list curl: curl -s ftp://{ftp_host}{ftp_path}")
     file_list = [line.split()[-1] for line in output.splitlines() if line.endswith(".xml.gz")]
 
     msg2(verbose, f"Total number of NCBI abstract XML files: {len(file_list)}")
     latest_files = [file_name for file_name in file_list if file_name.startswith("pubmed23n") and file_name.endswith(".xml.gz")]
     latest_files.sort(reverse=True)
     latest_files = latest_files[:num_files]
     msg2(verbose, f"latest_files {num_files}: {latest_files}")
 
     # Check if enough files are available
+    import sys
     if len(latest_files) == 0:
         msg1(verbose, "Error: Insufficient number of files available!")
-        exit(1)
+        sys.exit(1)
 
     # Calculate total predicted size
     total_size = 0
     for file_name in latest_files:
         response = subprocess.check_output(['curl', '-sI', f"ftp://{ftp_host}{ftp_path}{file_name}"]).decode()
         file_size = int(response.split("Content-Length: ")[1].split("\r")[0])
         total_size += file_size
@@ -234,36 +247,39 @@
 
         # Check MD5
         verify_md5(file_path, md5_file_path, verbose)
 
     total_size_human = subprocess.check_output(['numfmt', '--to=iec-i', '--suffix=B', str(total_size)]).decode().strip()
     msg2(verbose, f"Total size of abstract files: {total_size_human}")
 
-def create_pubcsv_dataset(m: ReferenceData) -> List:
-    """ Takes about 14min for 30 (2 per minute) """
+def create_pubcsv_dataset(m: ReferenceData, parse_updates: bool = False) -> List:
+    """ Takes about 14min for 30 (2-3 per minute) 
+
+    ARGS:
+
+      parse_updates: If True then parse the updatefiles, otherwise parse the baseline. See : https://ftp.ncbi.nlm.nih.gov/pubmed/baseline/README.txt
+      
+    """
+    import os
     
     abstract_length_threshold = m.abstract_length_threshold
     pub_inpath = m.pub_inpath()
+    pub_updatefiles_inpath = os.path.join(m.pub_inpath(), m.abstract_updatefiles_inpath)
+    if parse_updates:
+        pub_inpath = os.path.join(pub_inpath, m.abstract_updatefiles_inpath)
     pub_outpath = m.pub_outpath()
     verbose = m.verbose
-
-    import os
-    import glob
     
     csv_list = []
+
     # Iterate through files in the directory
-    for filepath in glob.glob(os.path.join(pub_inpath, "pubmed*.xml.gz")):
-        msg2(verbose, f"Converting file {filepath}")
-        if os.path.isfile(filepath):
-            filename = os.path.basename(filepath)
-            df = get_pub_df(filename=filename, inpath=pub_inpath, outpath= pub_outpath, prune=True, length_threshold = abstract_length_threshold, verbose = verbose)
-            csv_filepath = os.path.join(pub_outpath, f"{filename}.csv")
-            df.to_csv(csv_filepath, header=False, index=False, sep="\t")
-            msg2(verbose, f"Wrote file:{csv_filepath}")
-            csv_list.append(csv_filepath)
+    csv_list = parse_pubs(inpath=pub_inpath, outpath=pub_outpath, length_threshold = abstract_length_threshold, csv_list=csv_list, verbose=verbose)
+
+    # Repeat for 'updatefiles'
+    csv_list = parse_pubs(inpath=pub_updatefiles_inpath, outpath=pub_outpath, length_threshold = abstract_length_threshold, csv_list=csv_list, verbose=verbose)
             
     return(csv_list)
 
 def create_gene_files(m: ReferenceData):
     """ Calls the search.awk script in gpubs/scripts """
     
     filtered_terms_file = os.path.join(m.search_path(), m.filtered_terms_filename)
```

### Comparing `gpubs-2/gpubs/fetch.py` & `gpubs-3/gpubs/fetch.py`

 * *Files identical despite different names*

### Comparing `gpubs-2/gpubs/models.py` & `gpubs-3/gpubs/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,20 +18,27 @@
         # make directory structure
         os.makedirs(self.version_root, exist_ok=True)
         os.makedirs(self.raw_path(), exist_ok=True)
         os.makedirs(self.reference_path(), exist_ok=True)
         os.makedirs(self.dbxref_path(), exist_ok=True)
         os.makedirs(self.search_path(), exist_ok=True)
         os.makedirs(self.pub_inpath(), exist_ok=True)
+        os.makedirs(os.path.join(self.pub_inpath(),self.abstract_updatefiles_inpath), exist_ok=True)
         os.makedirs(self.pub_outpath(), exist_ok=True)
         os.makedirs(self.genes_outpath(), exist_ok=True)
         
         msg2(self.verbose, "Created directory structure.")
 
     ncbi_gene_info_url: str = "https://ftp.ncbi.nlm.nih.gov/gene/DATA/GENE_INFO/Mammalia/Homo_sapiens.gene_info.gz"
+
+    ncbi_ftp_host: str = "ftp.ncbi.nlm.nih.gov"
+
+    ncbi_ftp_baseline_path: str = "/pubmed/baseline/"
+
+    ncbi_ftp_updatefiles_path: str = "/pubmed/updatefiles/"
     
     data_root: str  = "data/"
     """ full path to where all the raw, reference, and generated data are stored """
     
     raw_data_path: str = "raw/"
     
     reference_data_path: str = "reference/"
@@ -60,21 +67,25 @@
     
     # may overlap somewhat with stop words
     custom_stop_words:List = ['ago', 'aim', 'amid', 'april', 'arch', 'bed', 'bite', 'bug', 'cage', 'co', 'crop',
                     'damage', 'danger', 'digit', 'et', 'fast', 'fat', 'fate', 'fire', 'flower', 'gap', 'genesis', 'gov', 'gpa', 'grasp',
                     'ii', 'inos', 'iv', 'killer', 'lab', 'lamp', 'laser', 'map', 'mask', 'mater', 'melt', 'mice', 'minor', 'miss', 'mv',
                     'nail', 'net', 'not', 'osf', 'pan', 'par', 'pha', 'rab', 'race', 'rain', 'rank',
                     'san', 'sand', 'se', 'sink', 'soft', 'spatial', 'spin', 'spp', 'steel', 'stop',
-                    'storm', 'tactile', 'tau', 'theta', 'tip', 'traits', 'via']
+                    'storm', 'tactile', 'tau', 'theta', 'tip', 'traits', 'via', 
+                              "apex", "app", "apps", "args", "ash", "bar", "bit", "cast", "cats", "cava", "cd", "clock", "coil", "cope", "cord", "delta", "eat", "eg", "fats", "fish", "fix", "flame", "flap", "fuse", "grid", "gum", "heal", "hip", "hits", "hub", "igm", "li", "maps", "mets", "mix", "mn", "ms", "nm", "nodal", "pigs", "prey", "pros", "pt", "pva", "ray", "sac", "scar", "sea", "sea", "sp", "steep", "tank", "tied", "toll", "trap", "wire"]
 
     search_terms_filename: str = "search_terms.txt"
     
     filtered_terms_filename: str = "filtered_terms.txt"
     
     abstract_inpath: str = "pubs/"
+
+    abstract_updatefiles_inpath: str = "updates/"
+    """ This path gets added on to abstract_inpath (or pub_inpath) """
     
     refresh_abstract_xml_files: bool = False
     """ Set to True to overwrite downloaded NCBI XML abstract files and checksum files """
     
     num_abstract_xml_files: int
     """ Number of NCBI XML files to download; Set this to -1 to get all abstracts """
```

### Comparing `gpubs-2/gpubs/reference.py` & `gpubs-3/gpubs/reference.py`

 * *Files identical despite different names*

### Comparing `gpubs-2/gpubs/search_words.py` & `gpubs-3/gpubs/search_words.py`

 * *Files identical despite different names*

### Comparing `gpubs-2/scripts/create_search_terms_file.sh` & `gpubs-3/scripts/create_search_terms_file.sh`

 * *Files identical despite different names*

### Comparing `gpubs-2/scripts/download_pubs.sh` & `gpubs-3/scripts/download_pubs.sh`

 * *Files identical despite different names*

### Comparing `gpubs-2/scripts/search.awk` & `gpubs-3/scripts/search.awk`

 * *Files identical despite different names*

### Comparing `gpubs-2/setup.py` & `gpubs-3/setup.py`

 * *Files identical despite different names*

