# Comparing `tmp/crypto-screening-1.0.1.tar.gz` & `tmp/crypto-screening-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-1.0.1.tar", last modified: Fri Jun 23 16:58:41 2023, max compression
+gzip compressed data, was "crypto-screening-1.0.2.tar", last modified: Sun Jun 25 15:39:07 2023, max compression
```

## Comparing `crypto-screening-1.0.1.tar` & `crypto-screening-1.0.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 16:58:41.588214 crypto-screening-1.0.1/
--rw-rw-rw-   0        0        0       74 2023-06-23 16:58:41.000000 crypto-screening-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2085 2023-06-23 16:58:41.588214 crypto-screening-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1264 2023-06-23 16:52:27.000000 crypto-screening-1.0.1/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.0.1/build.py
-drwxrwxrwx   0        0        0        0 2023-06-23 16:58:41.568107 crypto-screening-1.0.1/crypto_screening/
--rw-rw-rw-   0        0        0     6694 2023-06-23 16:52:27.000000 crypto-screening-1.0.1/crypto_screening/base.py
--rw-rw-rw-   0        0        0    17327 2023-06-23 16:52:27.000000 crypto-screening-1.0.1/crypto_screening/collect.py
--rw-rw-rw-   0        0        0    12461 2023-06-23 16:52:27.000000 crypto-screening-1.0.1/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      781 2023-06-23 16:52:27.000000 crypto-screening-1.0.1/crypto_screening/document.py
--rw-rw-rw-   0        0        0      194 2023-06-23 16:52:27.000000 crypto-screening-1.0.1/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0      180 2023-06-23 16:52:27.000000 crypto-screening-1.0.1/crypto_screening/hints.py
--rw-rw-rw-   0        0        0     2665 2023-06-23 16:52:27.000000 crypto-screening-1.0.1/crypto_screening/interval.py
--rw-rw-rw-   0        0        0    32685 2023-06-23 16:52:27.000000 crypto-screening-1.0.1/crypto_screening/ohlcv.py
--rw-rw-rw-   0        0        0    24532 2023-06-23 16:52:27.000000 crypto-screening-1.0.1/crypto_screening/orderbook.py
--rw-rw-rw-   0        0        0    34310 2023-06-23 16:52:27.000000 crypto-screening-1.0.1/crypto_screening/screener.py
--rw-rw-rw-   0        0        0    11995 2023-06-23 16:52:27.000000 crypto-screening-1.0.1/crypto_screening/symbols.py
-drwxrwxrwx   0        0        0        0 2023-06-23 16:58:41.587215 crypto-screening-1.0.1/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2085 2023-06-23 16:58:41.000000 crypto-screening-1.0.1/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      599 2023-06-23 16:58:41.000000 crypto-screening-1.0.1/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 16:58:41.000000 crypto-screening-1.0.1/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-06-23 16:58:41.000000 crypto-screening-1.0.1/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-23 16:58:41.000000 crypto-screening-1.0.1/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-06-23 16:58:41.000000 crypto-screening-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       73 2023-06-23 16:55:08.000000 crypto-screening-1.0.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 16:58:41.588214 crypto-screening-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-06-23 16:52:27.000000 crypto-screening-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 15:39:07.889730 crypto-screening-1.0.2/
+-rw-rw-rw-   0        0        0       98 2023-06-25 15:39:07.000000 crypto-screening-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2085 2023-06-25 15:39:07.888713 crypto-screening-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1264 2023-06-23 16:52:27.000000 crypto-screening-1.0.2/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-1.0.2/build.py
+drwxrwxrwx   0        0        0        0 2023-06-25 15:39:07.870714 crypto-screening-1.0.2/crypto_screening/
+-rw-rw-rw-   0        0        0     6694 2023-06-23 16:52:27.000000 crypto-screening-1.0.2/crypto_screening/base.py
+-rw-rw-rw-   0        0        0    23575 2023-06-25 15:15:52.000000 crypto-screening-1.0.2/crypto_screening/collect.py
+-rw-rw-rw-   0        0        0    12461 2023-06-25 15:33:45.000000 crypto-screening-1.0.2/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      860 2023-06-25 14:10:00.000000 crypto-screening-1.0.2/crypto_screening/document.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-1.0.2/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0      180 2023-06-23 16:52:27.000000 crypto-screening-1.0.2/crypto_screening/hints.py
+-rw-rw-rw-   0        0        0     2665 2023-06-23 16:52:27.000000 crypto-screening-1.0.2/crypto_screening/interval.py
+-rw-rw-rw-   0        0        0    32685 2023-06-25 15:28:31.000000 crypto-screening-1.0.2/crypto_screening/ohlcv.py
+-rw-rw-rw-   0        0        0    24555 2023-06-25 15:03:52.000000 crypto-screening-1.0.2/crypto_screening/orderbook.py
+-rw-rw-rw-   0        0        0     2392 2023-06-25 15:15:52.000000 crypto-screening-1.0.2/crypto_screening/process.py
+-rw-rw-rw-   0        0        0    34516 2023-06-25 15:38:04.000000 crypto-screening-1.0.2/crypto_screening/screener.py
+-rw-rw-rw-   0        0        0     9867 2023-06-25 14:09:42.000000 crypto-screening-1.0.2/crypto_screening/symbols.py
+drwxrwxrwx   0        0        0        0 2023-06-25 15:39:07.887713 crypto-screening-1.0.2/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2085 2023-06-25 15:39:07.000000 crypto-screening-1.0.2/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      627 2023-06-25 15:39:07.000000 crypto-screening-1.0.2/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 15:39:07.000000 crypto-screening-1.0.2/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-06-25 15:39:07.000000 crypto-screening-1.0.2/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-25 15:39:07.000000 crypto-screening-1.0.2/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-06-25 15:39:07.000000 crypto-screening-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       73 2023-06-23 16:55:08.000000 crypto-screening-1.0.2/requirements-dev.txt
+-rw-rw-rw-   0        0        0       64 2023-06-23 16:55:08.000000 crypto-screening-1.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 15:39:07.889730 crypto-screening-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-06-25 15:39:00.000000 crypto-screening-1.0.2/setup.py
```

### Comparing `crypto-screening-1.0.1/PKG-INFO` & `crypto-screening-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.0.1
+Version: 1.0.2
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.0.1/README.md` & `crypto-screening-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.0.1/build.py` & `crypto-screening-1.0.2/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.0.1/crypto_screening/base.py` & `crypto-screening-1.0.2/crypto_screening/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.0.1/crypto_screening/dataset.py` & `crypto-screening-1.0.2/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.0.1/crypto_screening/document.py` & `crypto-screening-1.0.2/crypto_screening/document.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from crypto_screening.ohlcv import *
 # noinspection PyUnresolvedReferences
 from crypto_screening.collect import *
 # noinspection PyUnresolvedReferences
 from crypto_screening.screener import *
 # noinspection PyUnresolvedReferences
 from crypto_screening.exchanges import *
+# noinspection PyUnresolvedReferences
+from crypto_screening.process import *
 
 from crypto_screening.base import document
 
 class Documentation:
     """"""
 # end Documentation
```

### Comparing `crypto-screening-1.0.1/crypto_screening/interval.py` & `crypto-screening-1.0.2/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-1.0.1/crypto_screening/ohlcv.py` & `crypto-screening-1.0.2/crypto_screening/ohlcv.py`

 * *Files 0% similar despite different names*

```diff
@@ -595,15 +595,15 @@
     Using this class, you can create a screener object to
     screen the market ask and bid data for a specific asset in
     a specific exchange at real time.
 
     Parameters:
 
     - exchanges:
-        The data of exchanges and their tickers to screen.
+        The data of exchanges and their symbols to screen.
 
     - interval:
         The interval for the time between data points in the dataset.
 
     - delay:
         The delay to wait between each data fetching.
```

### Comparing `crypto-screening-1.0.1/crypto_screening/orderbook.py` & `crypto-screening-1.0.2/crypto_screening/orderbook.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,23 +19,23 @@
 from cryptofeed.feed import Feed
 from cryptofeed.types import OrderBook
 from cryptofeed.defines import L2_BOOK
 
 from crypto_screening.dataset import (
     BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME
 )
-from crypto_screening.symbols import Separator, adjust_symbol
+from crypto_screening.symbols import adjust_symbol, Separator
 from crypto_screening.screener import (
     BaseScreener, BaseMultiScreener,
     create_market_dataframe, MarketRecorder,
     structure_screener_datasets
 )
 from crypto_screening.hints import Number
-from crypto_screening.exchanges import EXCHANGES
-from crypto_screening.collect import find_name
+from crypto_screening.exchanges import EXCHANGES, EXCHANGE_NAMES
+from crypto_screening.process import find_string_value
 
 __all__ = [
     "MarketHandler",
     "MarketOrderbookScreener",
     "add_feeds",
     "MarketOrderbookRecorder",
     "OrderbookScreener",
@@ -160,23 +160,20 @@
         """
         Records the data from the crypto feed into the dataset.
 
         :param data: The data from the exchange.
         :param timestamp: The time of the request.
         """
 
-        exchange = find_name(
-            name=data.exchange, names=self.market.keys()
+        exchange = find_string_value(
+            value=data.exchange, values=self.market.keys()
         )
-        symbol = find_name(
-            name=adjust_symbol(
-                symbol=data.symbol,
-                separator=Separator.value
-            ),
-            names=exchange
+        symbol = find_string_value(
+            value=adjust_symbol(symbol=data.symbol),
+            values=exchange
         )
 
         dataset = (
             self.market.
             setdefault(exchange, {}).
             setdefault(symbol, create_orderbook_dataframe())
         )
@@ -227,22 +224,22 @@
 # end ExchangeFeed
 
 def add_feeds(
         handler: FeedHandler,
         data: Dict[str, Iterable[str]],
         fixed: Optional[bool] = False,
         amount: Optional[int] = 5,
-        separator: Optional[str] = Separator.value,
+        separator: Optional[str] = None,
         parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
 ) -> None:
     """
-    Adds the tickers to the handler for each exchange.
+    Adds the symbols to the handler for each exchange.
 
     :param handler: The handler object.
-    :param data: The data of the exchanges and tickers to add.
+    :param data: The data of the exchanges and symbols to add.
     :param parameters: The parameters for the exchanges.
     :param fixed: The value for fixed parameters to all exchanges.
     :param separator: The separator of the assets.
     :param amount: The maximum amount of symbols for each feed.
     """
 
     base_parameters = None
@@ -251,16 +248,20 @@
         parameters = parameters or {}
 
     else:
         base_parameters = parameters or {}
         parameters = {}
     # end if
 
+    if separator is None:
+        separator = Separator.value
+    # end if
+
     for exchange, symbols in data.items():
-        exchange = find_name(name=exchange, names=EXCHANGES.keys())
+        exchange = find_string_value(value=exchange, values=EXCHANGE_NAMES)
 
         symbols = [
             symbol.replace(separator, '-')
             for symbol in symbols
         ]
 
         if fixed:
@@ -492,22 +493,22 @@
         return screeners
     # end create_screeners
 
     def add_feeds(
             self,
             data: Dict[str, Iterable[str]],
             fixed: Optional[bool] = True,
-            separator: Optional[str] = Separator.value,
+            separator: Optional[str] = None,
             amount: Optional[int] = None,
             parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
     ) -> None:
         """
-        Adds the tickers to the handler for each exchange.
+        Adds the symbols to the handler for each exchange.
 
-        :param data: The data of the exchanges and tickers to add.
+        :param data: The data of the exchanges and symbols to add.
         :param parameters: The parameters for the exchanges.
         :param fixed: The value for fixed parameters to all exchanges.
         :param amount: The maximum amount of symbols for each feed.
         :param separator: The separator of the assets.
         """
 
         self.feeds_parameters = dict(
@@ -771,15 +772,15 @@
         limited: Optional[bool] = None,
         handler: Optional[FeedHandler] = None,
         market: Optional[Market] = None,
         amount: Optional[int] = None,
         refresh: Optional[Union[Number, dt.timedelta, bool]] = None,
         recorder: Optional[MarketOrderbookRecorder] = None,
         fixed: Optional[bool] = True,
-        separator: Optional[str] = Separator.value,
+        separator: Optional[str] = None,
         parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
 ) -> MarketOrderbookScreener:
     """
     Creates the market screener object for the data.
 
     :param data: The market data.
     :param handler: The handler object for the market data.
```

### Comparing `crypto-screening-1.0.1/crypto_screening/screener.py` & `crypto-screening-1.0.2/crypto_screening/screener.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,18 @@
 
 from multithreading import Caller, multi_threaded_call
 
 from crypto_screening.dataset import (
     DATE_TIME, save_dataset, load_dataset
 )
 from crypto_screening.hints import Number
+from crypto_screening.symbols import Separator
+from crypto_screening.process import find_string_value
 from crypto_screening.collect import (
-    find_name, validate_exchange, validate_symbol
+    validate_exchange, validate_symbol
 )
 
 __all__ = [
     "BaseScreener",
     "wait_for_update",
     "wait_for_initialization",
     "WaitingState",
@@ -492,16 +494,22 @@
         :param location: The saving location of the dataset.
 
         :return: The saving path for the dataset.
         """
 
         location = location or self.location
 
-        return (location + "/" if isinstance(location, str) else "") + (
-            f"{self.exchange.lower()}/{self.symbol.replace('/', '-')}.csv"
+        if location is None:
+            location = "."
+        # end if
+
+        return (
+            f"{location}/"
+            f"{self.exchange.lower()}/"
+            f"{self.symbol.replace(Separator.value, '-')}.csv"
         )
     # end dataset_path
 
     def save_dataset(self, location: Optional[str] = None) -> None:
         """
         Saves the data of the screener.
 
@@ -659,15 +667,17 @@
 
         :param exchange: The source name of the exchange.
         :param symbol: The symbol of the pair.
 
         :return: The dataset of the spread data.
         """
 
-        exchange = find_name(name=exchange, names=self.market.keys())
+        exchange = find_string_value(
+            value=exchange, values=self.market.keys()
+        )
 
         validate_exchange(
             exchange=exchange,
             exchanges=self.market.keys(),
             provider=self
         )
```

### Comparing `crypto-screening-1.0.1/crypto_screening/symbols.py` & `crypto-screening-1.0.2/crypto_screening/symbols.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,17 +19,15 @@
     "parts_to_pair",
     "pair_to_parts",
     "symbols_to_parts",
     "parts_to_symbol_parts",
     "parts_to_symbol_parts",
     "assets_to_symbols",
     "parts_to_symbols",
-    "Separator",
-    "filter_symbols",
-    "keep_symbols"
+    "Separator"
 ]
 
 class Separator:
     """A class to contain the separator value."""
 
     value = "/"
 # end Separator
@@ -131,34 +129,34 @@
         # end if
 
         return Pair(*parts)
     # end load
 
     def symbol(self) -> str:
         """
-        Gets the tickers of the chain.
+        Gets the symbols of the chain.
 
-        :return: The tickers of the trading chain.
+        :return: The symbols of the trading chain.
         """
 
         return pair_to_symbol(self)
-    # end tickers
+    # end symbols
 
     def json(self) -> Tuple[str, str]:
         """
         Converts the data into a json format.
 
         :return: The chain of assets.
         """
 
         return pair_to_parts(self)
     # end json
 # end Pair
 
-def pair_to_symbol(pair: Pair, separator: Optional[str] = Separator.value) -> str:
+def pair_to_symbol(pair: Pair, separator: Optional[str] = None) -> str:
     """
     Converts a pair of assets into a symbol.
 
     :param pair: The pair of assets.
     :param separator: The separator of the assets.
 
     :return: The symbol.
@@ -167,15 +165,15 @@
     if separator is None:
         separator = Separator.value
     # end if
 
     return f"{pair.base}{separator}{pair.quote}"
 # end pair_to_symbol
 
-def parts_to_symbol(base: str, quote: str, separator: Optional[str] = Separator.value) -> str:
+def parts_to_symbol(base: str, quote: str, separator: Optional[str] = None) -> str:
     """
     Converts a pair of assets into a symbol.
 
     :param base: The base assets.
     :param quote: The quote assets.
     :param separator: The separator of the assets.
 
@@ -185,15 +183,15 @@
     if separator is None:
         separator = Separator.value
     # end if
 
     return f"{base}{separator}{quote}"
 # end parts_to_symbol
 
-def symbol_to_pair(symbol: str, separator: Optional[str] = Separator.value) -> Pair:
+def symbol_to_pair(symbol: str, separator: Optional[str] = None) -> Pair:
     """
     Converts a pair of assets into a symbol.
 
     :param symbol: The symbol to convert into a pair object.
     :param separator: The separator of the assets.
 
     :return: The symbol.
@@ -226,45 +224,43 @@
 
     :return: The symbol.
     """
 
     return Pair(base, quote)
 # end parts_to_pair
 
-def symbol_to_parts(symbol: str, separator: Optional[str] = Separator.value) -> Tuple[str, str]:
+def symbol_to_parts(symbol: str, separator: Optional[str] = None) -> Tuple[str, str]:
     """
     Converts a pair of assets into a symbol.
 
     :param symbol: The symbol to convert into a pair object.
     :param separator: The separator of the assets.
 
     :return: The symbol.
     """
 
-    pair = symbol_to_pair(symbol=symbol, separator=separator)
-
-    return pair.base, pair.quote
+    return symbol_to_pair(symbol=symbol, separator=separator).parts
 # end symbol_to_parts
 
-def reverse_symbol(symbol: str, separator: Optional[str] = Separator.value) -> str:
+def reverse_symbol(symbol: str, separator: Optional[str] = None) -> str:
     """
     Converts a pair of assets into a symbol.
 
     :param symbol: The symbol to convert into a pair object.
     :param separator: The separator of the assets.
 
     :return: The symbol.
     """
 
-    base, quote = symbol_to_parts(symbol=symbol, separator=separator)
-
-    return parts_to_symbol(base=quote, quote=base)
+    return parts_to_symbol(
+        *symbol_to_parts(symbol=symbol, separator=separator)
+    )
 # end reverse_symbol
 
-def reverse_pair(pair: Pair, separator: Optional[str] = Separator.value) -> Pair:
+def reverse_pair(pair: Pair, separator: Optional[str] = None) -> Pair:
     """
     Converts a pair of assets into a symbol.
 
     :param pair: The pair of assets.
     :param separator: The separator of the assets.
 
     :return: The symbol.
@@ -286,40 +282,36 @@
 
     :return: The symbol.
     """
 
     return pair.base, pair.quote
 # end pair_to_parts
 
-def adjust_symbol(symbol: str, separator: Optional[str] = Separator.value) -> str:
+def adjust_symbol(symbol: str, separator: Optional[str] = None) -> str:
     """
     Adjusts the symbol of the asset.
 
     :param symbol: The symbol of the asset to adjust.
     :param separator: The separator of the assets.
 
     :return: The adjusted asset symbol.
     """
 
     if separator is None:
         separator = Separator.value
     # end if
 
-    if separator is None:
-        separator = Separator.value
-    # end if
-
-    return symbol.replace("-", separator)
+    return symbol.replace("-", separator).upper()
 # end adjust_symbol
 
 def symbols_to_parts(symbols: Dict[str, Dict[str, Any]]) -> Tuple[List[str], List[str]]:
     """
-    Collects the bases and quotes of the tickers.
+    Collects the bases and quotes of the symbols.
 
-    :param symbols: The tickers to separate.
+    :param symbols: The symbols to separate.
 
     :return: The separated bases and quotes.
     """
 
     quotes = []
     bases = []
 
@@ -340,21 +332,21 @@
 
 def parts_to_symbol_parts(
         bases: Iterable[str],
         quotes: Iterable[str],
         symbols: Optional[Dict[str, Dict[str, Any]]] = None
 ) -> List[Tuple[str, str]]:
     """
-    Collects the bases and quotes of the tickers.
+    Collects the bases and quotes of the symbols.
 
     :param bases: The bases to join.
     :param quotes: The quotes to join.
-    :param symbols: The tickers to separate.
+    :param symbols: The symbols to separate.
 
-    :return: The joined tickers.
+    :return: The joined symbols.
     """
 
     pairs = []
 
     for base in bases:
         for quote in quotes:
             if (
@@ -376,36 +368,36 @@
 
 def parts_to_symbols(
         bases: Iterable[str],
         quotes: Iterable[str],
         symbols: Optional[Dict[str, Dict[str, Any]]] = None
 ) -> List[str]:
     """
-    Collects the bases and quotes of the tickers.
+    Collects the bases and quotes of the symbols.
 
     :param bases: The bases to join.
     :param quotes: The quotes to join.
-    :param symbols: The tickers to separate.
+    :param symbols: The symbols to separate.
 
-    :return: The joined tickers.
+    :return: The joined symbols.
     """
 
     return [
         parts_to_symbol(*parts) for parts in
         (parts_to_symbol_parts(bases, quotes, symbols))
     ]
 # end parts_to_symbols
 
 def assets_to_symbols(assets: Iterable[str]) -> List[str]:
     """
-    Creates the tickers from the assets.
+    Creates the symbols from the assets.
 
-    :param assets: The asset to build the tickers from.
+    :param assets: The asset to build the symbols from.
 
-    :return: The list of tickers.
+    :return: The list of symbols.
     """
 
     tickers = []
 
     for base in assets:
         for quote in assets:
             ticker = parts_to_symbol(base, quote)
@@ -413,86 +405,8 @@
             if base != quote and reverse_symbol(ticker) not in tickers:
                 tickers.append(ticker)
             # end if
         # end for
     # end for
 
     return tickers
-# end assets_to_symbols
-
-def keep_symbols(
-        symbols: Iterable[str],
-        bases: Optional[Iterable[str]] = None,
-        quotes: Optional[Iterable[str]] = None,
-        included: Optional[Iterable[str]] = None
-) -> List[str]:
-    """
-    Removes all symbols with not matching base or quote.
-
-    :param symbols: The symbols to filter.
-    :param bases: The bases to include.
-    :param quotes: The quotes to include.
-    :param included: The symbols to include.
-
-    :return: The filtered symbols.
-    """
-
-    saved = []
-
-    quotes = quotes or []
-    bases = bases or []
-    excluded = included or []
-
-    for symbol in symbols:
-        if symbol in excluded:
-            saved.append(symbol)
-        # end if
-
-        base, quote = symbol_to_parts(symbol)
-
-        if (base in bases) or (quote in quotes):
-            saved.append(symbol)
-        # end if
-    # end for
-
-    return saved
-# end keep_symbols
-
-def filter_symbols(
-        symbols: Iterable[str],
-        bases: Optional[Iterable[str]] = None,
-        quotes: Optional[Iterable[str]] = None,
-        excluded: Optional[Iterable[str]] = None
-) -> List[str]:
-    """
-    Removes all symbols with the matching base or quote.
-
-    :param symbols: The symbols to filter.
-    :param bases: The bases to exclude.
-    :param quotes: The quotes to exclude.
-    :param excluded: The symbols to exclude.
-
-    :return: The filtered symbols.
-    """
-
-    saved = []
-
-    quotes = quotes or []
-    bases = bases or []
-    excluded = excluded or []
-
-    for symbol in symbols:
-        if symbol in excluded:
-            continue
-        # end if
-
-        base, quote = symbol_to_parts(symbol)
-
-        if (base in bases) or (quote in quotes):
-            continue
-        # end if
-
-        saved.append(symbol)
-    # end for
-
-    return saved
-# end filter_symbols
+# end assets_to_symbols
```

### Comparing `crypto-screening-1.0.1/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-1.0.2/crypto_screening.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 1.0.1
+Version: 1.0.2
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-1.0.1/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-1.0.2/crypto_screening.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 crypto_screening/dataset.py
 crypto_screening/document.py
 crypto_screening/exchanges.py
 crypto_screening/hints.py
 crypto_screening/interval.py
 crypto_screening/ohlcv.py
 crypto_screening/orderbook.py
+crypto_screening/process.py
 crypto_screening/screener.py
 crypto_screening/symbols.py
 crypto_screening.egg-info/PKG-INFO
 crypto_screening.egg-info/SOURCES.txt
 crypto_screening.egg-info/dependency_links.txt
 crypto_screening.egg-info/requires.txt
 crypto_screening.egg-info/top_level.txt
```

### Comparing `crypto-screening-1.0.1/pyproject.toml` & `crypto-screening-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '1.0.1'
+version = '1.0.2'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-1.0.1/setup.py` & `crypto-screening-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='1.0.1',
+        version='1.0.2',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

