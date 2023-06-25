# Comparing `tmp/volvisualizer-1.1.2-py3-none-any.whl.zip` & `tmp/volvisualizer-1.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 27328 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-14 14:38 volvisualizer/__init__.py
+Zip file size: 27397 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-25 19:00 volvisualizer/__init__.py
 -rw-rw-rw-  2.0 fat    26576 b- defN 22-Mar-16 10:04 volvisualizer/graph.py
 -rw-rw-rw-  2.0 fat    11866 b- defN 23-Jun-14 14:40 volvisualizer/market_data.py
--rw-rw-rw-  2.0 fat    25959 b- defN 23-Jun-14 14:48 volvisualizer/market_data_prep.py
+-rw-rw-rw-  2.0 fat    26180 b- defN 23-Jun-25 18:28 volvisualizer/market_data_prep.py
 -rw-rw-rw-  2.0 fat     2857 b- defN 22-Mar-16 09:22 volvisualizer/utils.py
 -rw-rw-rw-  2.0 fat    30001 b- defN 22-Mar-15 16:13 volvisualizer/vol_methods.py
 -rw-rw-rw-  2.0 fat    13496 b- defN 22-Mar-16 09:22 volvisualizer/volatility.py
 -rw-rw-rw-  2.0 fat     3914 b- defN 23-Jun-14 14:38 volvisualizer/volatility_params.py
--rw-rw-rw-  2.0 fat     1089 b- defN 23-Jun-14 14:58 volvisualizer-1.1.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      727 b- defN 23-Jun-14 14:58 volvisualizer-1.1.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-14 14:58 volvisualizer-1.1.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-Jun-14 14:58 volvisualizer-1.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1093 b- defN 23-Jun-14 14:58 volvisualizer-1.1.2.dist-info/RECORD
-13 files, 117707 bytes uncompressed, 25502 bytes compressed:  78.3%
+-rw-rw-rw-  2.0 fat     1089 b- defN 23-Jun-25 19:05 volvisualizer-1.1.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      727 b- defN 23-Jun-25 19:05 volvisualizer-1.1.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-25 19:05 volvisualizer-1.1.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-Jun-25 19:05 volvisualizer-1.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1093 b- defN 23-Jun-25 19:05 volvisualizer-1.1.3.dist-info/RECORD
+13 files, 117928 bytes uncompressed, 25571 bytes compressed:  78.3%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: volvisualizer/volatility.py
 Comment: 
 
 Filename: volvisualizer/volatility_params.py
 Comment: 
 
-Filename: volvisualizer-1.1.2.dist-info/LICENSE
+Filename: volvisualizer-1.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: volvisualizer-1.1.2.dist-info/METADATA
+Filename: volvisualizer-1.1.3.dist-info/METADATA
 Comment: 
 
-Filename: volvisualizer-1.1.2.dist-info/WHEEL
+Filename: volvisualizer-1.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: volvisualizer-1.1.2.dist-info/top_level.txt
+Filename: volvisualizer-1.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: volvisualizer-1.1.2.dist-info/RECORD
+Filename: volvisualizer-1.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## volvisualizer/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.1.2"
+__version__ = "1.1.3"
```

## volvisualizer/market_data_prep.py

```diff
@@ -745,39 +745,46 @@
         """
 
         # If the ticker is not valid return zero
         if ticker == '^SPX':
             try:
                 div_yield = cls._spx_div_yield()
             except ValueError:
-                print("No dividend data for "+ticker)
+                print("No dividend data for SPX")
                 div_yield = '0.0%'
         else:
             try:
                 div_yield = cls._stock_dividend_yield(ticker)
             except ValueError:
                 print("No dividend data for "+ticker)
                 div_yield = '0.0%'
 
-        return np.round(float(div_yield.rstrip('%'))/100, 5)
+        try: 
+            result = np.round(float(div_yield.rstrip('%'))/100, 5)
+        except ValueError:
+            print("No valid dividend data for "+ticker)
+            result = 0.0
+
+        return result
 
 
     @staticmethod
     def _stock_dividend_yield(ticker):
 
-        url = 'https://ycharts.com/companies/'+ticker+'/dividend_yield'
+        url = 'https://stockanalysis.com/stocks/'+ticker+'/dividend/'
 
-        urlopener = UrlOpener()
-        response = urlopener.open(url)
+        r = requests.get(url)
 
-        html_doc = response.text
+        html_doc = r.text
 
-        data = pd.read_html(html_doc)
+        tree = html.fromstring(html_doc)
+        
+        parse = tree.xpath("//*[contains(text(), 'Dividend Yield')]/div/text()")
 
-        return data[0]['Value'][0]
+        return [str(p) for p in parse][0].replace('\n','')
 
 
     @staticmethod
     def _spx_div_yield():
 
         url = 'https://www.multpl.com/s-p-500-dividend-yield'
```

## Comparing `volvisualizer-1.1.2.dist-info/LICENSE` & `volvisualizer-1.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `volvisualizer-1.1.2.dist-info/METADATA` & `volvisualizer-1.1.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volvisualizer
-Version: 1.1.2
+Version: 1.1.3
 Summary: Extract and visualize implied volatility from option data.
 Home-page: https://github.com/GBERESEARCH/volvisualizer
 Author: GBERESEARCH
 Author-email: gberesearch@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

## Comparing `volvisualizer-1.1.2.dist-info/RECORD` & `volvisualizer-1.1.3.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-volvisualizer/__init__.py,sha256=JhNfc49cF1z8HnPYAyTem2s5Sn4s2XfgPp_HRwRQSfQ,23
+volvisualizer/__init__.py,sha256=MNg8Ih17kliJwlnU9Nip6ZLjE9MDf-ibrAgQJVctAy4,23
 volvisualizer/graph.py,sha256=y6LePLlhdGJCkqg-WgpAHHH42PKkr2Bq5oQ_HRWCeZ0,26576
 volvisualizer/market_data.py,sha256=bmjzmB8HJMCPcQRnlvFvmDLzTYGlsDgXebQDqN_t8Kk,11866
-volvisualizer/market_data_prep.py,sha256=rqN1IAYE5keWLz3hVuer4RIori2u-8CxMtvcJE7iBJM,25959
+volvisualizer/market_data_prep.py,sha256=Thf4vYGC2RReN7b2m-GbyaXzY870-diySS1drI270QU,26180
 volvisualizer/utils.py,sha256=KkZn7dNsGDVuOkpQ04AVMAMUMF3l5XjbqyIoKWJK-mI,2857
 volvisualizer/vol_methods.py,sha256=GLJsL6LCEsl9JNXMfvrh1RZbZ778VmVJOfgC0aKbWvA,30001
 volvisualizer/volatility.py,sha256=euBLvjKd9ieBu0XkRFiLB5lAmf52MRJjkM2fLrwHVWE,13496
 volvisualizer/volatility_params.py,sha256=g2iiXI1Cbiz4ISDv8JGZyCNwOb81NxZtSAmUX6AEnuk,3914
-volvisualizer-1.1.2.dist-info/LICENSE,sha256=AE-WWqzPtajuHJajyfzO6uPCKh1DW3MqA1NXcnBImL0,1089
-volvisualizer-1.1.2.dist-info/METADATA,sha256=qPdTlvkmvr1PsWp43zIV4_uKSDA4FwbCp_89Z9c46F4,727
-volvisualizer-1.1.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-volvisualizer-1.1.2.dist-info/top_level.txt,sha256=Tfyh9PL2rX9P1DsThRUSnziSAZJU3o43o73eAOUHCMc,14
-volvisualizer-1.1.2.dist-info/RECORD,,
+volvisualizer-1.1.3.dist-info/LICENSE,sha256=AE-WWqzPtajuHJajyfzO6uPCKh1DW3MqA1NXcnBImL0,1089
+volvisualizer-1.1.3.dist-info/METADATA,sha256=dxdnFpj4c7A4TCsvPwJ4yDZmo-GQENeH-UIBDINPVho,727
+volvisualizer-1.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+volvisualizer-1.1.3.dist-info/top_level.txt,sha256=Tfyh9PL2rX9P1DsThRUSnziSAZJU3o43o73eAOUHCMc,14
+volvisualizer-1.1.3.dist-info/RECORD,,
```

