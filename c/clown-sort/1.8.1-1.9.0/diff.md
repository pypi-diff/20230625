# Comparing `tmp/clown_sort-1.8.1.tar.gz` & `tmp/clown_sort-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clown_sort-1.8.1.tar", max compression
+gzip compressed data, was "clown_sort-1.9.0.tar", max compression
```

## Comparing `clown_sort-1.8.1.tar` & `clown_sort-1.9.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     3405 2023-06-20 05:50:48.559552 clown_sort-1.8.1/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.8.1/LICENSE
--rw-r--r--   0        0        0     9322 2023-06-20 05:48:55.384657 clown_sort-1.8.1/README.md
--rw-r--r--   0        0        0     4215 2023-06-20 05:47:05.935055 clown_sort-1.8.1/clown_sort/__init__.py
--rw-r--r--   0        0        0     7987 2023-06-03 00:19:42.985646 clown_sort-1.8.1/clown_sort/config.py
--rw-r--r--   0        0        0     9021 2023-06-02 20:58:04.234216 clown_sort-1.8.1/clown_sort/filename_extractor.py
--rw-r--r--   0        0        0     4711 2023-05-27 16:06:01.553047 clown_sort-1.8.1/clown_sort/files/image_file.py
--rw-r--r--   0        0        0     3069 2023-06-15 23:22:00.182053 clown_sort-1.8.1/clown_sort/files/pdf_file.py
--rw-r--r--   0        0        0    12052 2023-06-20 03:19:34.507174 clown_sort-1.8.1/clown_sort/files/sortable_file.py
--rwxr-xr-x   0        0        0     3456 2023-06-15 23:17:52.887054 clown_sort-1.8.1/clown_sort/sort_selector.py
--rw-r--r--   0        0        0    11758 2023-06-20 03:19:34.507783 clown_sort-1.8.1/clown_sort/sorting_rules/crypto.csv
--rw-r--r--   0        0        0     3506 2023-04-24 00:53:03.331251 clown_sort-1.8.1/clown_sort/util/argument_parser.py
--rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.8.1/clown_sort/util/constants.py
--rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.8.1/clown_sort/util/dict_helper.py
--rw-r--r--   0        0        0     3705 2023-06-20 03:19:34.508422 clown_sort-1.8.1/clown_sort/util/filesystem_helper.py
--rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.8.1/clown_sort/util/logging.py
--rw-r--r--   0        0        0     3427 2023-05-27 22:16:38.822426 clown_sort-1.8.1/clown_sort/util/rich_helper.py
--rw-r--r--   0        0        0      667 2023-05-27 16:06:01.554255 clown_sort-1.8.1/clown_sort/util/string_helper.py
--rw-r--r--   0        0        0     1712 2023-06-20 05:50:48.565217 clown_sort-1.8.1/pyproject.toml
--rw-r--r--   0        0        0    10744 1970-01-01 00:00:00.000000 clown_sort-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0     3534 2023-06-25 02:58:48.184419 clown_sort-1.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.9.0/LICENSE
+-rw-r--r--   0        0        0     9287 2023-06-25 02:54:41.522424 clown_sort-1.9.0/README.md
+-rw-r--r--   0        0        0     4431 2023-06-25 02:54:41.522832 clown_sort-1.9.0/clown_sort/__init__.py
+-rw-r--r--   0        0        0     8073 2023-06-25 02:54:41.523241 clown_sort-1.9.0/clown_sort/config.py
+-rw-r--r--   0        0        0     9021 2023-06-02 20:58:04.234216 clown_sort-1.9.0/clown_sort/filename_extractor.py
+-rw-r--r--   0        0        0     4832 2023-06-25 02:54:41.523569 clown_sort-1.9.0/clown_sort/files/image_file.py
+-rw-r--r--   0        0        0      392 2023-06-24 02:14:02.169664 clown_sort-1.9.0/clown_sort/files/import pdfplumber.py
+-rw-r--r--   0        0        0     3766 2023-06-25 02:56:51.220186 clown_sort-1.9.0/clown_sort/files/pdf_file.py
+-rw-r--r--   0        0        0    12052 2023-06-20 03:19:34.507174 clown_sort-1.9.0/clown_sort/files/sortable_file.py
+-rwxr-xr-x   0        0        0     3456 2023-06-15 23:17:52.887054 clown_sort-1.9.0/clown_sort/sort_selector.py
+-rw-r--r--   0        0        0    11873 2023-06-25 02:54:41.524264 clown_sort-1.9.0/clown_sort/sorting_rules/crypto.csv
+-rw-r--r--   0        0        0     4181 2023-06-25 02:54:44.150613 clown_sort-1.9.0/clown_sort/util/argument_parser.py
+-rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.9.0/clown_sort/util/constants.py
+-rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.9.0/clown_sort/util/dict_helper.py
+-rw-r--r--   0        0        0     3705 2023-06-20 03:19:34.508422 clown_sort-1.9.0/clown_sort/util/filesystem_helper.py
+-rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.9.0/clown_sort/util/logging.py
+-rw-r--r--   0        0        0     3427 2023-05-27 22:16:38.822426 clown_sort-1.9.0/clown_sort/util/rich_helper.py
+-rw-r--r--   0        0        0      667 2023-05-27 16:06:01.554255 clown_sort-1.9.0/clown_sort/util/string_helper.py
+-rw-r--r--   0        0        0     1712 2023-06-25 02:58:48.188486 clown_sort-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0    10709 1970-01-01 00:00:00.000000 clown_sort-1.9.0/PKG-INFO
```

### Comparing `clown_sort-1.8.1/CHANGELOG.md` & `clown_sort-1.9.0/CHANGELOG.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # NEXT RELEASE
 
+# 1.9.0
+* Parse text from images in PDFs (some PDFs have no text only images)
+* Improve `extract_text_from_files` functionality
+
 ### 1.8.1
 * Actually make `extract_text_from_files` executable
 
 # 1.8.0
 * Add a script to extract files
 * More default sort rules
```

### Comparing `clown_sort-1.8.1/LICENSE` & `clown_sort-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clown_sort-1.8.1/README.md` & `clown_sort-1.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -132,15 +132,19 @@
 pipx install clown_sort[gui]
 ```
 
 ![](doc/manual_select_box.png)
 
 
 ## One Off Extractions
-Sometimes you just want to see the extracted text from a PDF or image and aren't trying to sort anything. There is a convenience script ou can use to extract text from a single file, multiple files, or all the files in a given directory. Just run `extract_text_from_files MY_FILE` to extract a single file. As an example for extracting multiple files and/or directories:
+`extract_text_from_files` (installed at the same time) is a convenient script you can use to extract text from a single file, multiple files, or all the files in a given directory using Google's best in class Tesseract library.
+
+![](doc/extract_text_from_files_help.png)
+
+As an example for extracting multiple files and/or directories:
 
 ```
 extract_text_from_files MY_FILE1 MY_FILE2 SOME_DIR3
 ```
 
 This will parse and display the text in `MY_FILE1`, `MY_FILE2`, and all the files in `SOME_DIR3`.
```

### Comparing `clown_sort-1.8.1/clown_sort/__init__.py` & `clown_sort-1.9.0/clown_sort/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import sys
+from argparse import Namespace
 from glob import glob
 from os import environ, getcwd, path
 from pathlib import Path
 from typing import List, Union
 
 from dotenv import load_dotenv
 
 # load_dotenv() should be called as soon as possible (before parsing local classes) but not for pytest
 if not environ.get('INVOKED_BY_PYTEST', False):
     for dotenv_file in [path.join(dir, '.clown_sort') for dir in [getcwd(), Path.home()]]:
         if path.exists(dotenv_file):
             load_dotenv(dotenv_path=dotenv_file)
             break
 
+from clown_sort.util.argument_parser import extraction_parser
 from clown_sort.config import Config
 from clown_sort.files.image_file import ImageFile
 from clown_sort.files.pdf_file import PdfFile
 from clown_sort.files.sortable_file import SortableFile
 from clown_sort.sort_selector import process_file_with_popup
 from clown_sort.util.filesystem_helper import (IMAGE_FILE_EXTENSIONS, files_in_dir, is_image,
       is_pdf, set_timestamp_based_on_screenshot_filename)
@@ -41,27 +43,29 @@
             file_to_sort.sort_file()
 
 
 def extract_text_from_files() -> None:
     """
     Extract text from a single file or from all files in a given directory. Can accept
     multiple paths as arguments on the command line.
-
-    TODO: replace with an option parser
     """
+    args: Namespace = extraction_parser.parse_args()
     console.line()
+    files_to_process = []
 
-    if len(sys.argv) <= 1:
-        print("Provide at least one filename to extract.")
-        sys.exit()
+    if args.debug:
+        Config.enable_debug_mode()
 
-    files_to_process = []
+    for file_or_dir in args.file_or_dir:
+        file_path = Path(file_or_dir)
 
-    for file_path in sys.argv[1:]:
-        if Path(file_path).is_dir():
+        if not file_path.exists():
+            console.print(f"File '{file_path}' doesn't exist!")
+            sys.exit()
+        elif file_path.is_dir():
             files_to_process.extend(files_in_dir(file_path))
         else:
             files_to_process.append(file_path)
 
     for file_path in files_to_process:
         build_sortable_file(file_path).print_extracted_text()
         console.line(2)
```

### Comparing `clown_sort-1.8.1/clown_sort/config.py` & `clown_sort-1.9.0/clown_sort/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,15 @@
         if '--version' in sys.argv:
             print(f"{PACKAGE_NAME} {version(PACKAGE_NAME)}")
             sys.exit()
 
         args: Namespace = parser.parse_args()
 
         if args.debug:
-            Config.debug = True
-            set_log_level('DEBUG')
+            cls.enable_debug_mode()
 
         rules_csvs = args.rules_csv or DEFAULT_RULES_CSV_PATHS
         rules_csvs = [CRYPTO_RULES_CSV_PATH if arg == CRYPTO else arg for arg in rules_csvs]
         log.debug(f"Rules CSVs: {rules_csvs}")
 
         screenshots_dir = Path(args.screenshots_dir).expanduser()
         destination_dir = Path(args.destination_dir or args.screenshots_dir).expanduser()
@@ -135,14 +134,19 @@
 
     @classmethod
     def get_sort_dirs(cls) -> List[str]:
         """Returns a list of the subdirectories already created for sorted images."""
         return sorted(subdirs_of_dir(cls.sorted_screenshots_dir), key=lambda d: d.lower())
 
     @classmethod
+    def enable_debug_mode(cls) -> None:
+        Config.debug = True
+        set_log_level('DEBUG')
+
+    @classmethod
     def _load_rules_csv(cls, file_path: Union[Path, str]) -> List[SortRule]:
         with open(Path(file_path), mode='r') as csvfile:
             return [
                 SortRule(row['folder'], re.compile(row['regex'], re.IGNORECASE | re.MULTILINE))
                 for row in csv.DictReader(
                     filter(lambda _row: len(_row) > 0 and _row.lstrip()[0] != '#', csvfile),
                     delimiter=','
```

### Comparing `clown_sort-1.8.1/clown_sort/filename_extractor.py` & `clown_sort-1.9.0/clown_sort/filename_extractor.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.8.1/clown_sort/files/image_file.py` & `clown_sort-1.9.0/clown_sort/files/image_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 OCR:  https://pypi.org/project/pytesseract/
 EXIF: https://blog.matthewgove.com/2022/05/13/how-to-bulk-edit-your-photos-exif-data-with-10-lines-of-python/
 Tags: https://exiftool.org/TagNames/EXIF.html
 """
 import io
 import re
 from pathlib import Path
-from typing import Optional
+from typing import Optional, Union
 
 import pytesseract
 from PIL import Image
 from PIL.ExifTags import TAGS
 
 from clown_sort.config import Config
 from clown_sort.filename_extractor import FilenameExtractor
@@ -77,31 +77,15 @@
         return _thumbnail_bytes.getvalue()
 
     def extracted_text(self) -> Optional[str]:
         """Use Tesseract to OCR the text in the image, which is returned as a string."""
         if self.text_extraction_attempted:
             return self._extracted_text
 
-        try:
-            self._extracted_text = pytesseract.image_to_string(self.pillow_image_obj())
-        except OSError as e:
-            if 'truncated' in str(e):
-                console.print(warning_text(f"Truncated image file! '{self.file_path}'!"))
-            else:
-                console.print_exception()
-                console.print(f"Error while extracting '{self.file_path}'!", style='bright_red')
-                raise e
-        except Exception as e:
-            console.print_exception()
-            console.print(f"Error while extracting '{self.file_path}'!", style='bright_red')
-            raise e
-
-        if self._extracted_text is not None:
-            self._extracted_text = self._extracted_text.strip()
-
+        self._extracted_text = ImageFile.extract_text(self.pillow_image_obj(), str(self.file_path))
         self.text_extraction_attempted = True
         return self._extracted_text
 
     def exif_dict(self) -> dict:
         """Return a key/value list of exif tags where keys are strings."""
         raw_exif_tags = self.pillow_image_obj().getexif()
         return {TAGS[k]: v for k,v in raw_exif_tags.items()}
@@ -119,7 +103,27 @@
 
     def __repr__(self) -> str:
         return f"ImageFile('{self.file_path}')"
 
     # def __rich_console__(self, console: Console, options: ConsoleOptions) -> RenderResult:
     #     super().__rich_console__(console, options)
     #     log.debug(f"RAW EXIF: {self.raw_exif_dict()}")
+
+    @staticmethod
+    def extract_text(image: Image.Image, image_name: str) -> Optional[str]:
+        text = None
+
+        try:
+            text = pytesseract.image_to_string(image)
+        except OSError as e:
+            if 'truncated' in str(e):
+                console.print(warning_text(f"Truncated image file! '{image_name}'!"))
+            else:
+                console.print_exception()
+                console.print(f"Error while extracting '{image_name}'!", style='bright_red')
+                raise e
+        except Exception as e:
+            console.print_exception()
+            console.print(f"Error while extracting '{image_name}'!", style='bright_red')
+            raise e
+
+        return None if text is None else text.strip()
```

### Comparing `clown_sort-1.8.1/clown_sort/files/sortable_file.py` & `clown_sort-1.9.0/clown_sort/files/sortable_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.8.1/clown_sort/sort_selector.py` & `clown_sort-1.9.0/clown_sort/sort_selector.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.8.1/clown_sort/sorting_rules/crypto.csv` & `clown_sort-1.9.0/clown_sort/sorting_rules/crypto.csv`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 folder,regex
 1mdb,1mdb|jho[-_\s.]*low|Victor[-_\s.]*Hoo
 3ac,3ac|Three[-_\s.]*Arrows[-_\s.]*Capital|su[-_\s.]*zhu|zhu[-_\s.]*su|kyle[-_\s.]*davies|OPNX
 A16Z,a16z|Andreessen|Packym|Arianna[-_\s1]*Simpson|Ben[-_\s.]*Horowitz|\bAXS\b
 Aave,\bAave
 Abra,\bAbra\b|\bPlutus\b|\bBarhydt
-AAX,\baax
+AAX,\bAAX
 Algorand,\bAlgorand|\b[$#]ALGO\b
 Arbitrum,Arbitrum|[$#]ARB\b
 Amber Group,Amber[-_\s.]*Group|\btiantian\b|\bkullander\b|\btony[-_\s.]*he\b|\bbo[-_\s.]*shen\b
 Aptos,\bAptos\b
 Art,occult
 Atomic Wallet,Atomic[-_\s.]*Wallet
 Avalanche,\bAvax|AVAX\b|avalanche|\bava[-_\s.]*labs
 Banks,SEBA[^a-z]|Credit[-_\s.]*Suisse|SJMBT|Sygnum|Celtic[-_\s.]*Bank|\bMercury\b|Choice[-_\s.]*Financial[-_\s.]*Group|\$FRC|Commercium[-_\s.]*Financial|\bmetabank|\bHBAN\b|Huntington[-_\s.]*Bancshares|United[-_\s.]*Texas|\bUTB\b|Craig[-_\s.]*Sellars
 Bankless,Bankless|David[-_\s.]*Hoffman
 Biconomy,\bBiconomy|Omchain
 Binary Options,binary[-_\s.]*options
-Binance,binance|\bbiconomy|\bbnb\b|\bbsc\b|\bcz\b|\bbifinity\b|binaryx|\bbillance|changpeng|\bjoselito\b|\bpaysafe|\bSwipe[-_\s.]*(IO|Wallet)|\bkeyway|\bkey[-_\s.]*vision|\bTrustWallet\b|BUSD\b|\boztures|Kaiser[-_\s.]*Ng|InvestByBit|Swyftx|Guangying[-_\s.]*Chen|\bcoley\b|\bBAM\b|\bFlowbank|\bnuvei\b|\borum\b|Worldpay|Bijie[-_\s.]*(Network|Tech)|Venus[-_\s.]*(Protocol|Community)
+Binance,bi(nance|conomy|llance|finity|naryx)|\b(BNB|BSC|BUSD|Cpz|CZ|Changpeng|joselito|paysafe|keyway|TrustWallet|Coley|nuvei|orum|Worldpay|Winind)\b|\bSwipe[-_\s.]*(IO|Wallet)|\bkey[-_\s.]*vision|\boztures|Kaiser[-_\s.]*Ng|InvestByBit|Swyftx|Guangying[-_\s.]*Chen|\bBAM[-_\s.]*(Trading|Management)\b|\bFlowbank|Bijie[-_\s.]*(Network|Tech)|Venus[-_\s.]*(Protocol|Community)|Merit[-_\s.]*Peak|(Optic|Blockone|Winind|Unison)[-_\s.]*Technolog
 Bitdeer,Bitdeer
 BitGet,Bitget
 Bithumb,\bbithumb
 Bitmain,Bitmain
 BitMex,Bitmex|Arthur[-_\s.]*Hayes
 Bitstamp,Bitstamp
 Bittrex,Bittrex|Ritchie[-_\s.]*Lai|Kiran[-_\s.]*Raj|John[-_\s.]*Roth\b|\bAquila\b
@@ -42,30 +42,30 @@
 CMCC Global,CMCC[-_\s.]*Global
 Coinbase,Coinbase|\$COIN|brian[-_\s.]*armstrong|grewal\b|Asiff[-_\s.]*Hirji|\bbalaji|Fred[-_\s.]*Ehrsam|\bremitly\b|\$RELY\b
 Coinflex,Mark[-_\s.]*Lamb|Roger[-_\s.]*Ver|coinflex|Doug[-_\s.]*Polk|OPNX|flexusd|Leslie[-_\s.]*Lamb|dougpolkvids
 CoinLoan,coinloan|Faliushin\b
 CompoundFi,compoundfi|leshner|\bgonen\b
 ConsenSys,ConsenSys
 Cross River Bank,\bCRB|Cross[-_\s.]*River|Prestige[-_\s.]*Capital|\bbae[-_\s.]*communications|Zenfi\b|PeerIQ|\bupstart\b|\bUPST\b|\bLeumi\b|Hapoalim|BetterFin|\bMANTL\b|\bLvnv|\bKabbage|\bAFRM\b|\bMomnt
-Crypto.com,crypto[._]?com|CDC|[$#]CRO|\sCRO\s|Doug(las)?[-_\s.]*Ching\b
+Crypto.com,crypto[._]?com|CDC|[$#]CRO|\sCRO\s|Doug(las)?[-_\s.]*Ching\b|Bobby[-_\s.]*Bao\b|Gary[-_\s.]*Or\b|Marszalek|Rafael[-_\s.]*Melo\b
 CUBI,\bCUBI\b|Customers[-_\s.]*Ban(k|corp)
 Cumberland,cumberland
 Custodia,custodia\b|caitlin[-_\s.]*long
 dalle,craiyon|midjourney|\bdall[-_\s.]*e\b
 DCG,DCG|digital[-_\s.]*currency[-_\s.]*group|sh?ill?bert|Grayscale|GBTC|\bkraines\b|hq[-_\s.]*digital|Alana[-_\s.]*Ackerson|Jennifer[-_\s.]*Mitrenga|Emily[-_\s.]*(Heather[-_\s.]*)?Goodman|Founders[-_\s.]*Liquidity[-_\s.]*Fund
 DeFi,\bdefi\b|decentralized[-_\s.]*finance
 Dragonfly Capital,Dragonfly[-_\s.]*Capital
 DWF,DWF|Andrey[-_\s.]*Grachev|\bgrachev\b
 Evolve Bank,getevolved|\bevolve[-_\s.]*bank\b
 Effective Altruism,\bE\.?A\.?\b|effective[-_\s.]*altruism
 El Salvador,El[-_\s.]*Salvador|Bukele|Max[-_\s.]*Keiser
 Elon Musk,\bTesla\b|\bTSLA\b|\bElon\b|\bElmo\b
 EOS,\bEOS\b|\bBlumer\b|\bLarimer\b|@B1\b|Block[-_\.\s]One
 Evertas,\bEvertas\b|Ryan[-_\s.]*Lackey
-Euler Finance,\beuler\b
+Euler Finance,\bEuler\b
 FalconX,falconx
 First Digital,First[-_\s.]*Digital\b
 Flip Filipkowski,filipkowski
 Finblox,finblox
 Fireblocks,fireblocks
 Frax,\bFrax\b|\bFRX|[\b#$]FXS
 Friedlander Group,Friedlander|Agro[-_\s.]*Bank|\ball[-_\s.]*year\b|\bbrock\b|brockpierce|litvishhocker|Yecheskel|Swift[-_\s.]*Staffing
@@ -114,61 +114,61 @@
 Nexo,\bNexo\b|Antoni[-_\s.]*Trenchev|Georgi[-_\s.]*Shulev|Lydia[-_\s.]*Shuleva|\bNDS[-_\s.]*EOD\b
 NFTs,crypto[-_\s.]*punk|pudgy[-_\s.]*penguin
 OKX,oke?[cx]|star[-_\s.]*xu|\blennix[-_\s.]*lai\b|\bOKcoin|\bHong[-_\s.]*Fang\b
 Olympus DAO,\bOlympus\b|OlympusDAO|\bOHM\b
 Ooki DAO,\bOoki(DAO)?\b
 OneCoin,\bOne(Coin|Life)\b
 OpenPayd,openpayd|CFD\s?Team
-OpenSea,OpenSea
+OpenSea,OpenSea\b
 PAG,\bpag\b|Weijian[-_\s.]*Shan
 Paradigm,Fred[-_\s.]*Ehrsam|paradigm\b
 Paxful,paxful|Ray[-_\s.]*(Youssef|Savant)|Artur[-_\s.]*Schaback
 Paxos,paxos|BUSD|USDP|PAXG
-Payrnet,payrnet|railsr|railsbank
+Payrnet,Payrnet|Rails(r|bank)\b
 Pi,\$PI[^\w]|Pi[-_\s.]*Network
 Politics,\bted[-_\s.]*cruz
-Prime Trust,Prime[-\s_]*Trust|\bBanq\b|Scott\bPurcell|(Planet|Fortress)[-\s_]*(Xyz|Trust|NFT)|George[-\s_]*Georgiades|Kevin[-\s_]*Lehtiniitty|PrimeX\b|\bSroge\b|\banonalyx
+Prime Trust,Prime[-\s_]*Trust|\b(Banq|PrimeX|Sroge|anonalyx)\b|Scott[-\s_]*Purcell|(Planet|Fortress)[-\s_]*(Xyz|Trust|NFT)|George[-\s_]*Georgiades|Kevin[-\s_]*Lehtiniitty
 PVBC,PVBC|BankProv
 Quadriga,Quadriga|Gerald[-_\s.]*Cotten|0xsifu\b|michael[-_\s.]*patryn|wonderland|daniele[-_\s.]*sesta\b
-Revolut,revolut[^\w]
+Revolut,\bRevolut\b
 Ripple,XRP|garlinghouse|\bripple\b
 RIOT,[$#]RIOT\b|Riot[-\s_]*(Block|Platform)|Bioptix
 Safemoon,Safemoon
 Satoshi,Satoshi|Nakamoto
-SEC,\bSEC(\b|Gov)|\b(Gary)?Gensler|CFTC|Securities.{0,6}Exchange.{0,6}Commission
+SEC,\bSEC(Gov)?\b|\b(Gary)?Gensler|CFTC|Securities.{0,6}Exchange.{0,6}Commission
 Signature Bank,SBNY|Signature[-_\s.]*Bank|Signet|Scott[-_\s.]*Shay\b|(Joseph|Joe)[-_\s.]*DePaolo|\bKushner\b
 Silicon Valley Bank,si?vb|Silicon[-_\s.]*Valley[-_\s.]*Bank
 Silk Road,Silk[-_\s.]*Road|\bulbricht|\bDPR\b
 Silvergate,\$SI|Silvergate|Alan[-_\s.]*Lane|Eisele|\bSEN\b|SENnetwork|Rebecca[-_\s.]*Rettig
-Skrill,\bskrill
-Solana,Solana|Serum
-Stellar,\bstellar\b
+Skrill,\bSkrill\b
+Solana,(Solana|Serum)\b
+Stellar,\bStellar\b|[$#]?XLM
 Stifel Bank,\bStifel\b|[#$]SF\b
 Symbolic Capital,Symbolic[-_\s.]*Capital|Lev[-_\s]Livnev
 Synapse,Synapse(fi|labs|protocol)?\b
 TerraLuna,\bluna\b|do[-_\s.]*kwon|stablekwon|\bTerra(form|Luna)?\b|Macedo|\bLuna[-_\s.]*Foundation\b|Mirror[-_\s.]*Protocol
-Tether,\btether\b|usdt|paolo\b|paoloardoino|friedberg|\bhoegner|Noble[-_\s.]*Bank|\bDeltec[^\']|b(e|i)tfinex[^e]|\bbrock([-_\s.]*pierce)?\b|Clearstone[-_\s.]*Global|Capital[-_\s.]*Union|Noblex|SJMBT|Global[-_\s.]*Trad(ing|e)[-_\s.]*Solutions|(dig|i)finex|BFXNA|BFXWW|[$#]Leo\b|Phil[-_\s.]*Potter|Stablehouse|Samson[-_\s.]*Mow|Gabor[-_\s.]*Gurbacs|XBTO|Paul[-_\s.]*Eisma|Philippe[-_\s.]*Bekhazi|\b(Master|Real)coin\b|Reeve[-_\s.]*Collins|\bdevasini\b|phil(ip)?[-_\s.]*potter\b|van[-_\s.]*der[-_\s.]*velde|Perpetual[-_\s.]*Action[-_\s.]*Group|\burwhatyouknow|global[-_\s.]*trade[-_\s.]*solutions|reginald[-_\s.]*fowler|renrenbee\b|\bludovicus|Amos[-_\s.]*Ltd|William[-_\s.]*Quigley|Sunlot\b|\bD10e\b|\bGoCoin\b|Blade[-_\s.]*payments|Five[-_\s.]*Delta|\bXfire\b|\bPlaysino\b|\bEvertune|\bGamesTV|\bethfinex|coinapult|gabriel[-_\s.]*sukenik|R(ondell|[ho][ho]n)[-_\s.]*(Clyde)?[-_\s.]*Monroe|\bTuxia\b|\bIGEL\b|\bInfomatec|Mainstreet[-_\s.]*Partners|\bMallers\b|Far[-_\s.]*Eastern[-_\s.]*International|\b(Chesham|Sinopec|SFP)\b|White[-_\s.]*Plains[-_\s.]*Capital|BANK[-_\s.]*OF[-_\s.]*COMMUNICATIONS
+Tether,\b(BFXNA|BFXWW|Chesham|Coinapult|D10e|Devasini|GoCoin|Evertune|Friedberg|GamesTV|Hoegner|IGEL|Infomatec|Ludovicus|(Master|Real)coin|Mallers|Noblex|Paolo(Ardoino)?|Playsino|Renrenbee|SFP|Sinopec|SJMBT|Stablehouse|Sunlot|Tether|Tuxia|urwhatyouknow|USDT|XBTO|Xfire)\b|Noble[-_\s.]*Bank|\bDeltec[^\']|\b(B[ei]t|i|Digi?|Eth)finex[^e']|\bbrock([-_\s.]*pierce)?\b|Clearstone[-_\s.]*Global|Capital[-_\s.]*Union|Global[-_\s.]*Trad(ing|e)[-_\s.]*Solutions|[$#]LEO\b|Phil[-_\s.]*Potter|Samson[-_\s.]*Mow|Gabor[-_\s.]*Gurbacs|Paul[-_\s.]*Eisma|Philippe[-_\s.]*Bekhazi|Reeve[-_\s.]*Collins|phil(ip)?[-_\s.]*potter\b|Van[-_\s.]*der[-_\s.]*Velde|Perpetual[-_\s.]*Action[-_\s.]*Group|Global[-_\s.]*Trade[-_\s.]*Solutions|reginald[-_\s.]*fowler|Amos[-_\s.]*Ltd|William[-_\s.]*Quigley|Blade[-_\s.]*payments|Five[-_\s.]*Delta|gabriel[-_\s.]*sukenik|R(ondell|[ho][ho]n)[-_\s.]*(Clyde)?[-_\s.]*Monroe|Mainstreet[-_\s.]*Partners|Far[-_\s.]*Eastern[-_\s.]*International|White[-_\s.]*Plains[-_\s.]*Capital|BANK[-_\s.]*OF[-_\s.]*COMMUNICATIONS
 Tornado Cash,tornado[-_\s.]*cash
-Transactive Systems UAB,Transactive
+Transactive Systems UAB,Transactive[-_\s.]*Systems
 Tron,\btron\b|tron(block|[-_\s.]*)?chain|trondao|TRX\b
 TrueUSD,TUSD|TrueUSD|TrueFi|TrustExplorer|Techteryx
 Vauld,Vauld
 VCs,venture[-_\s.]*capital|\bVCs?\b|calacanis|@jason\b|david[-_\s.]*sacks|\bthiel\b|sequoia|founders[-_\s.]*fund|Valar[-_\s.]*Ventures|6th[-_\s.]*Man[-_\s.]*Ventures|Northzone|Warburg[-_\s.]*Serres|Alan[-_\s.]*Howard|Tiger[-_\s.]*Global
 Vitalik Buterin,\bvitalik\b
-Voyager,voyager
+Voyager,Voyager\b
 Wanxiang Group,wanxiang|\bFeng[-_\s.]*Xiao
 Wallet Addresses BCH,bitcoincash:q.*\b
 Wallet Addresses Bitcoin,\b(bc1|[13])[a-zA-HJ-NP-Z0-9]{25,39}\b
 Wallet Addresses Cardano,\baddr1[a-z0-9]+\b
 Wallet Addresses Cosmos,\bcosmos[a-zA-Z0-9_.-]{10,}\b
 Wallet Addresses Dash,\bX[1-9A-HJ-NP-Za-km-z]{33}
 Wallet Addresses Doge,\bD[a-zA-Z0-9_.-]{33}
 Wallet Addresses Ethereum,0x[a-fA-F0-9]{40}
 Wallet Addresses Monero,\b[48][0-9AB][1-9A-HJ-NP-Za-km-z]{93}
 Wallet Addresses Polkadot,\b1[0-9a-zA-Z]{47}
 Wallet Addresses Ripple,\br[0-9a-zA-Z]{33}
 Wallet Addresses Stellar,\bG[0-9A-Z]{40,60}\b
 Waves,sasha35625|sasha\.waves|\bvires|sasha[-_\s.]*ivanov|boris[-_\s.]*titov|[$#]waves\b
-Wintermute,wintermute|\bbebop\b
-Wirecard,wirecard|\bmarsalek\b|\bBafin\b
+Wintermute,Wintermute|\b(Bebop|Evgeny)\b
+Wirecard,\b(Bafin|Marsalek|Wirecard)\b|Markus[-_\s.]*Braun
 Worldcoin,Worldcoin|\borb\b
 Wyre,\bwyre|sendwyre|\bLead[-_\s.]*Bank\b|Steven[-_\s.]*Huynh
```

### Comparing `clown_sort-1.8.1/clown_sort/util/argument_parser.py` & `clown_sort-1.9.0/clown_sort/util/argument_parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+Parse arguments for both the main sort_screenshots() as well as extract_text_from_files().
+"""
 from argparse import ArgumentParser
 from os import environ
 from pathlib import Path
 
 from rich_argparse_plus import RichHelpFormatterPlus
 
 from clown_sort.util.constants import (DEFAULT_SCREENSHOTS_DIR, DEFAULT_DESTINATION_DIR,
@@ -67,7 +70,21 @@
                     help="don't preserve the original screenshots in the Processed/ folder")
 
 parser.add_argument('--show-rules', action='store_true',
                     help='display the sorting rules and exit')
 
 parser.add_argument('--debug', action='store_true',
                     help='turn on debug level logging')
+
+
+############################################
+# Parse args for extract_text_from_files() #
+############################################
+
+extraction_parser = ArgumentParser(
+    formatter_class=RichHelpFormatterPlus,
+    description="Extract the text from one or more files or directories.",
+    epilog="If any of the FILE_OR_DIRs is a directory all files in that directory will be extracted."
+)
+
+extraction_parser.add_argument('file_or_dir', nargs='+', metavar='FILE_OR_DIR')
+extraction_parser.add_argument('--debug', action='store_true', help='turn on debug level logging')
```

### Comparing `clown_sort-1.8.1/clown_sort/util/constants.py` & `clown_sort-1.9.0/clown_sort/util/constants.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.8.1/clown_sort/util/filesystem_helper.py` & `clown_sort-1.9.0/clown_sort/util/filesystem_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.8.1/clown_sort/util/rich_helper.py` & `clown_sort-1.9.0/clown_sort/util/rich_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.8.1/clown_sort/util/string_helper.py` & `clown_sort-1.9.0/clown_sort/util/string_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.8.1/pyproject.toml` & `clown_sort-1.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clown_sort"
-version = "1.8.1"
+version = "1.9.0"
 description = "Sort screenshots based on rules or through individual review."
 authors = ["Michel de Cryptadamus <michel@cryptadamus.com>"]
 readme = "README.md"
 packages = [{include = "clown_sort"}]
 homepage = "https://github.com/michelcrypt4d4mus/clown_sort"
 
 include = [
@@ -38,15 +38,15 @@
 rich = "^13.0.1"
 piexif = "^1.1.3"
 pillow = "^9.4.0"
 filedate = "^2.0"
 python-dotenv = "^0.21.1"
 rich-argparse-plus = "^0.3.1.4"
 pyexiftool = "^0.5.5"
-pypdf = "^3.4.1"
+pypdf = "^3.8.0"
 pycryptodome = {version = "^3.17", optional = true}
 PyMuPDF = {version = "^1.22.3", optional = true}
 
 [tool.poetry.extras]
 pdf = ['pycryptodome', 'PyMuPDF']
 gui = ['PySimpleGUI']
```

### Comparing `clown_sort-1.8.1/PKG-INFO` & `clown_sort-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clown-sort
-Version: 1.8.1
+Version: 1.9.0
 Summary: Sort screenshots based on rules or through individual review.
 Home-page: https://github.com/michelcrypt4d4mus/clown_sort
 Keywords: ocr,organization,organizer,screenshot,rename,sort
 Author: Michel de Cryptadamus
 Author-email: michel@cryptadamus.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -20,15 +20,15 @@
 Requires-Dist: PySimpleGUI (>=4.60.4,<5.0.0) ; extra == "gui"
 Requires-Dist: exif (>=1.5.0,<2.0.0)
 Requires-Dist: filedate (>=2.0,<3.0)
 Requires-Dist: piexif (>=1.1.3,<2.0.0)
 Requires-Dist: pillow (>=9.4.0,<10.0.0)
 Requires-Dist: pycryptodome (>=3.17,<4.0) ; extra == "pdf"
 Requires-Dist: pyexiftool (>=0.5.5,<0.6.0)
-Requires-Dist: pypdf (>=3.4.1,<4.0.0)
+Requires-Dist: pypdf (>=3.8.0,<4.0.0)
 Requires-Dist: pytesseract (>=0.3.10,<0.4.0)
 Requires-Dist: python-dotenv (>=0.21.1,<0.22.0)
 Requires-Dist: rich (>=13.0.1,<14.0.0)
 Requires-Dist: rich-argparse-plus (>=0.3.1.4,<0.4.0.0)
 Description-Content-Type: text/markdown
 
 ![Python Version](https://img.shields.io/pypi/pyversions/clown_sort)
@@ -165,15 +165,19 @@
 pipx install clown_sort[gui]
 ```
 
 ![](doc/manual_select_box.png)
 
 
 ## One Off Extractions
-Sometimes you just want to see the extracted text from a PDF or image and aren't trying to sort anything. There is a convenience script ou can use to extract text from a single file, multiple files, or all the files in a given directory. Just run `extract_text_from_files MY_FILE` to extract a single file. As an example for extracting multiple files and/or directories:
+`extract_text_from_files` (installed at the same time) is a convenient script you can use to extract text from a single file, multiple files, or all the files in a given directory using Google's best in class Tesseract library.
+
+![](doc/extract_text_from_files_help.png)
+
+As an example for extracting multiple files and/or directories:
 
 ```
 extract_text_from_files MY_FILE1 MY_FILE2 SOME_DIR3
 ```
 
 This will parse and display the text in `MY_FILE1`, `MY_FILE2`, and all the files in `SOME_DIR3`.
```

