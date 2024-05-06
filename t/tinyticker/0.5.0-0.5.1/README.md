# Comparing `tmp/tinyticker-0.5.0.tar.gz` & `tmp/tinyticker-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyticker-0.5.0.tar", max compression
+gzip compressed data, was "tinyticker-0.5.1.tar", max compression
```

## Comparing `tinyticker-0.5.0.tar` & `tinyticker-0.5.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1068 2024-05-03 22:53:19.227821 tinyticker-0.5.0/LICENSE
--rw-r--r--   0        0        0     3863 2024-05-03 22:53:19.227821 tinyticker-0.5.0/README.md
--rw-r--r--   0        0        0      899 2024-05-03 22:53:19.227821 tinyticker-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      207 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/__init__.py
--rw-r--r--   0        0        0     5821 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/__main__.py
--rw-r--r--   0        0        0     1731 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/config.py
--rw-r--r--   0        0        0     9301 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/display.py
--rw-r--r--   0        0        0      345 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/paths.py
--rw-r--r--   0        0        0    15408 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/ticker.py
--rw-r--r--   0        0        0     3123 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/utils.py
--rw-r--r--   0        0        0      318 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/waveshare_lib/__init__.py
--rw-r--r--   0        0        0     1259 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/waveshare_lib/_base.py
--rw-r--r--   0        0        0     8376 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/waveshare_lib/epd2in13.py
--rw-r--r--   0        0        0    11895 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/waveshare_lib/epd2in13_V2.py
--rw-r--r--   0        0        0    14581 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/waveshare_lib/epd2in13_V3.py
--rw-r--r--   0        0        0    10457 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/waveshare_lib/epd2in13_V4.py
--rw-r--r--   0        0        0     5835 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/waveshare_lib/epd2in13b_V3.py
--rw-r--r--   0        0        0     6627 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/waveshare_lib/epd2in13b_V4.py
--rw-r--r--   0        0        0     5690 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/waveshare_lib/epd2in13bc.py
--rw-r--r--   0        0        0     3148 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/waveshare_lib/epdconfig.py
--rw-r--r--   0        0        0     1283 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/waveshare_lib/models.py
--rw-r--r--   0        0        0       95 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/web/__init__.py
--rw-r--r--   0        0        0     2547 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/web/__main__.py
--rw-r--r--   0        0        0     6931 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/web/app.py
--rw-r--r--   0        0        0     2909 2024-05-03 22:53:19.231821 tinyticker-0.5.0/tinyticker/web/command.py
--rw-r--r--   0        0        0   274777 2024-05-03 22:53:19.235821 tinyticker-0.5.0/tinyticker/web/templates/css/uikit.min.css
--rw-r--r--   0        0        0    12844 2024-05-03 22:53:19.235821 tinyticker-0.5.0/tinyticker/web/templates/images/apple-touch-icon.png
--rw-r--r--   0        0        0      742 2024-05-03 22:53:19.235821 tinyticker-0.5.0/tinyticker/web/templates/images/favicon-16x16.png
--rw-r--r--   0        0        0     1645 2024-05-03 22:53:19.235821 tinyticker-0.5.0/tinyticker/web/templates/images/favicon-32x32.png
--rw-r--r--   0        0        0    15092 2024-05-03 22:53:19.235821 tinyticker-0.5.0/tinyticker/web/templates/index.html
--rw-r--r--   0        0        0      787 2024-05-03 22:53:19.235821 tinyticker-0.5.0/tinyticker/web/templates/js/index.js
--rw-r--r--   0        0        0    65291 2024-05-03 22:53:19.235821 tinyticker-0.5.0/tinyticker/web/templates/js/uikit-icons.min.js
--rw-r--r--   0        0        0   136629 2024-05-03 22:53:19.235821 tinyticker-0.5.0/tinyticker/web/templates/js/uikit.min.js
--rw-r--r--   0        0        0     1369 2024-05-03 22:53:19.235821 tinyticker-0.5.0/tinyticker/web/templates/logfiles.html
--rw-r--r--   0        0        0     5111 1970-01-01 00:00:00.000000 tinyticker-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-06 08:53:00.961287 tinyticker-0.5.1/LICENSE
+-rw-r--r--   0        0        0     3863 2024-05-06 08:53:00.961287 tinyticker-0.5.1/README.md
+-rw-r--r--   0        0        0      899 2024-05-06 08:53:00.961287 tinyticker-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      207 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/__init__.py
+-rw-r--r--   0        0        0     6196 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/__main__.py
+-rw-r--r--   0        0        0     1773 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/config.py
+-rw-r--r--   0        0        0     8880 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/display.py
+-rw-r--r--   0        0        0      345 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/paths.py
+-rw-r--r--   0        0        0    15609 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/ticker.py
+-rw-r--r--   0        0        0     3123 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/utils.py
+-rw-r--r--   0        0        0      318 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/waveshare_lib/__init__.py
+-rw-r--r--   0        0        0     1259 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/waveshare_lib/_base.py
+-rw-r--r--   0        0        0     8376 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/waveshare_lib/epd2in13.py
+-rw-r--r--   0        0        0    11895 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/waveshare_lib/epd2in13_V2.py
+-rw-r--r--   0        0        0    14581 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/waveshare_lib/epd2in13_V3.py
+-rw-r--r--   0        0        0    10457 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/waveshare_lib/epd2in13_V4.py
+-rw-r--r--   0        0        0     5835 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/waveshare_lib/epd2in13b_V3.py
+-rw-r--r--   0        0        0     6627 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/waveshare_lib/epd2in13b_V4.py
+-rw-r--r--   0        0        0     5690 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/waveshare_lib/epd2in13bc.py
+-rw-r--r--   0        0        0     3148 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/waveshare_lib/epdconfig.py
+-rw-r--r--   0        0        0     1283 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/waveshare_lib/models.py
+-rw-r--r--   0        0        0       95 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/web/__init__.py
+-rw-r--r--   0        0        0     2547 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/web/__main__.py
+-rw-r--r--   0        0        0     7161 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/web/app.py
+-rw-r--r--   0        0        0     2909 2024-05-06 08:53:00.965288 tinyticker-0.5.1/tinyticker/web/command.py
+-rw-r--r--   0        0        0   274777 2024-05-06 08:53:00.969287 tinyticker-0.5.1/tinyticker/web/templates/css/uikit.min.css
+-rw-r--r--   0        0        0    12844 2024-05-06 08:53:00.969287 tinyticker-0.5.1/tinyticker/web/templates/images/apple-touch-icon.png
+-rw-r--r--   0        0        0      742 2024-05-06 08:53:00.969287 tinyticker-0.5.1/tinyticker/web/templates/images/favicon-16x16.png
+-rw-r--r--   0        0        0     1645 2024-05-06 08:53:00.969287 tinyticker-0.5.1/tinyticker/web/templates/images/favicon-32x32.png
+-rw-r--r--   0        0        0    13954 2024-05-06 08:53:00.969287 tinyticker-0.5.1/tinyticker/web/templates/index.html
+-rw-r--r--   0        0        0      787 2024-05-06 08:53:00.969287 tinyticker-0.5.1/tinyticker/web/templates/js/index.js
+-rw-r--r--   0        0        0    65291 2024-05-06 08:53:00.969287 tinyticker-0.5.1/tinyticker/web/templates/js/uikit-icons.min.js
+-rw-r--r--   0        0        0   136629 2024-05-06 08:53:00.969287 tinyticker-0.5.1/tinyticker/web/templates/js/uikit.min.js
+-rw-r--r--   0        0        0     1369 2024-05-06 08:53:00.969287 tinyticker-0.5.1/tinyticker/web/templates/logfiles.html
+-rw-r--r--   0        0        0     5111 1970-01-01 00:00:00.000000 tinyticker-0.5.1/PKG-INFO
```

### Comparing `tinyticker-0.5.0/LICENSE` & `tinyticker-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.0/README.md` & `tinyticker-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.0/pyproject.toml` & `tinyticker-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tinyticker"
-version = "0.5.0"
+version = "0.5.1"
 description = "A tiny Raspberry Pi powered ePaper ticker."
 authors = ["Loic Coyle <loic.coyle@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/loiccoyle/tinyticker"
 keywords = ["raspberry-pi", "ticker", "stock", "crypto", "epaper", "finance"]
```

### Comparing `tinyticker-0.5.0/tinyticker/__main__.py` & `tinyticker-0.5.1/tinyticker/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -80,31 +80,39 @@
     sequence = Sequence.from_tinyticker_config(tt_config)
     logger.debug(sequence)
 
     try:
         for ticker, resp in sequence.start():
             logger.debug("API len(historical): %s", len(resp.historical))
             logger.debug("API current_price: %s", resp.current_price)
-            delta = (
-                100
-                * (resp.current_price - resp.historical.iloc[0]["Open"])
-                / resp.historical.iloc[0]["Open"]
+            delta_range_start = resp.historical.iloc[0]["Open"]
+            delta_range = (
+                100 * (resp.current_price - delta_range_start) / delta_range_start
             )
+
+            top_string = f"{ticker.symbol}: $ {resp.current_price:.2f}"
+            if ticker.avg_buy_price is not None:
+                # calculate the delta from the average buy price
+                delta_abp = (
+                    100
+                    * (resp.current_price - ticker.avg_buy_price)
+                    / ticker.avg_buy_price
+                )
+                top_string += f" {delta_abp:+.2f}%"
+
             xlim = None
             # if incomplete data, leave space for the missing data
             if len(resp.historical) < ticker.lookback:
                 # the floats are to leave padding left and right of the edge candles
                 xlim = (-0.75, ticker.lookback - 0.25)
             logger.debug("xlim: %s", xlim)
             display.plot(
                 resp.historical,
-                resp.current_price,
-                top_string=f"{ticker.symbol}: $",
-                sub_string=f"{len(resp.historical)}x{ticker.interval}",
-                delta=delta,
+                top_string=top_string,
+                sub_string=f"{len(resp.historical)}x{ticker.interval} {delta_range:+.2f}%",
                 show=True,
                 xlim=xlim,
                 type=ticker._display_kwargs.pop("plot_type", "candle"),
                 **ticker._display_kwargs,
             )
     except Exception as exc:
         logger.error(exc, stack_info=True)
```

### Comparing `tinyticker-0.5.0/tinyticker/config.py` & `tinyticker-0.5.1/tinyticker/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     symbol: str = "SPY"
     interval: str = "1d"
     lookback: Optional[int] = None
     wait_time: Optional[int] = None
     plot_type: str = "candle"
     mav: Optional[int] = None
     volume: bool = False
+    avg_buy_price: Optional[float] = None
 
 
 @dc.dataclass
 class SequenceConfig:
     skip_outdated: bool = True
     skip_empty: bool = True
```

### Comparing `tinyticker-0.5.0/tinyticker/display.py` & `tinyticker-0.5.1/tinyticker/display.py`

 * *Files 4% similar despite different names*

```diff
@@ -186,32 +186,28 @@
         self._show_image(image, highlight_image)
         self._log.info("Display sleep.")
         self.epd.sleep()
 
     def plot(
         self,
         historical: pd.DataFrame,
-        current_price: Optional[float],
-        delta: Optional[float] = None,
         top_string: Optional[str] = None,
         sub_string: Optional[str] = None,
         show: bool = False,
         type: str = "candle",
         volume: bool = False,
         **kwargs,
     ) -> Tuple[Figure, Axes]:
         """Plot symbol historical data chart.
 
         Args:
             historical: API response, `pd.DataFrame` containing the historical
                 price of the symbol.
-            current_price: API response, the current price of the symbol.
-            delta: relative percentage change.
-            top_string: Contents of the top left string, the `current_price` will be
-                appended if provided.
+            top_string: Contents of the top left string, '{}' will be replaced with the current
+                price.
             sub_string: Contents of a smaller text box below `top_string`.
             show: display the plot on the ePaper display.
             type: the chart type, see `mplfinance.plot`.
             volume: also plot the trade volume data.
             **kwargs: passed to `mplfinance.plot`.
 
         Returns:
@@ -234,24 +230,19 @@
             ax=ax,
             update_width_config={"line_width": 1},
             style=STYLE_HIGHLIGHT if self.has_highlight else STYLE,
             volume=volume_ax,
             linecolor="k",
             **kwargs,
         )
+
         # Fall back to using the last closing price
-        if current_price is None:
-            current_price = historical.iloc[-1]["Close"]
-        if top_string is not None:
-            top_string += f" {current_price:.2f}"
-        else:
-            top_string = str(current_price)
+        if top_string is None:
+            top_string = str(historical["Close"].iloc[-1])
 
-        if delta is not None:
-            top_string += f" {delta:+.2f}%"
         ax.text(
             0,
             1,
             top_string,
             transform=ax.transAxes,
             fontsize=10,
             weight="bold",
```

### Comparing `tinyticker-0.5.0/tinyticker/ticker.py` & `tinyticker-0.5.1/tinyticker/ticker.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,25 +168,27 @@
         api_key: CryptoCompare API key, https://min-api.cryptocompare.com/pricing,
             required for fetching crypto prices.
         symbol_type: Either "crypto" or "stock".
         symbol:  Ticker or token identifier, "AAPL", "BTC", "ETH", "DOGE" ...
         interval: Data time interval.
         lookback: How many intervals to look back.
         wait_time: Time to wait in between API calls.
+        avg_buy_price: Average buy price of the asset.
         **kwargs: Extra args are provided to the `Display.plot` method.
     """
 
     def __init__(
         self,
         api_key: Optional[str] = None,
         symbol_type: str = "crypto",
         symbol: str = "BTC",
         interval: str = "1d",
         lookback: Optional[int] = None,
         wait_time: Optional[int] = None,
+        avg_buy_price: Optional[float] = None,
         **kwargs,
     ) -> None:
         self._log = logging.getLogger(__name__)
         if symbol_type not in SYMBOL_TYPES:
             raise ValueError(f"'symbol_type' not in {SYMBOL_TYPES}")
         self.symbol_type = symbol_type
         if interval not in INTERVAL_TIMEDELTAS.keys():
@@ -214,14 +216,15 @@
         else:
             self.wait_time = wait_time  # type: int
         self._log.debug("wait_time: %s", self.wait_time)
         self._symbol_type_map: Dict[str, Callable] = {
             "crypto": self._tick_crypto,
             "stock": self._tick_stock,
         }
+        self.avg_buy_price = avg_buy_price
         self._display_kwargs = kwargs
 
     @property
     def single_tick(self) -> Callable[[], Response]:
         """Perform a single tick.
 
         Returns:
@@ -357,14 +360,15 @@
                     symbol=ticker.symbol,
                     interval=ticker.interval,
                     lookback=ticker.lookback,
                     wait_time=ticker.wait_time,
                     plot_type=ticker.plot_type,
                     mav=ticker.mav,
                     volume=ticker.volume,
+                    avg_buy_price=ticker.avg_buy_price,
                 )
                 for ticker in tt_config.tickers
             ],
             skip_empty=tt_config.sequence.skip_empty,
             skip_outdated=tt_config.sequence.skip_outdated,
         )
```

### Comparing `tinyticker-0.5.0/tinyticker/utils.py` & `tinyticker-0.5.1/tinyticker/utils.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.0/tinyticker/waveshare_lib/_base.py` & `tinyticker-0.5.1/tinyticker/waveshare_lib/_base.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.0/tinyticker/waveshare_lib/epd2in13.py` & `tinyticker-0.5.1/tinyticker/waveshare_lib/epd2in13.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.0/tinyticker/waveshare_lib/epd2in13_V2.py` & `tinyticker-0.5.1/tinyticker/waveshare_lib/epd2in13_V2.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.0/tinyticker/waveshare_lib/epd2in13_V3.py` & `tinyticker-0.5.1/tinyticker/waveshare_lib/epd2in13_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.0/tinyticker/waveshare_lib/epd2in13_V4.py` & `tinyticker-0.5.1/tinyticker/waveshare_lib/epd2in13_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.0/tinyticker/waveshare_lib/epd2in13b_V3.py` & `tinyticker-0.5.1/tinyticker/waveshare_lib/epd2in13b_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.0/tinyticker/waveshare_lib/epd2in13b_V4.py` & `tinyticker-0.5.1/tinyticker/waveshare_lib/epd2in13b_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.0/tinyticker/waveshare_lib/epd2in13bc.py` & `tinyticker-0.5.1/tinyticker/waveshare_lib/epd2in13bc.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.0/tinyticker/waveshare_lib/epdconfig.py` & `tinyticker-0.5.1/tinyticker/waveshare_lib/epdconfig.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.0/tinyticker/waveshare_lib/models.py` & `tinyticker-0.5.1/tinyticker/waveshare_lib/models.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.0/tinyticker/web/__main__.py` & `tinyticker-0.5.1/tinyticker/web/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.0/tinyticker/web/app.py` & `tinyticker-0.5.1/tinyticker/web/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,20 @@
 
 def no_empty_str(data: str) -> Optional[str]:
     if data == "":
         return None
     return data
 
 
+def no_empty_float(data: str) -> Optional[float]:
+    if data == "":
+        return None
+    return float(data)
+
+
 def no_empty_int(data: str) -> Optional[int]:
     if data == "":
         return None
     return int(data)
 
 
 def str_to_bool(data: str) -> Optional[bool]:
@@ -104,14 +110,17 @@
         tickers["symbol_type"] = request.args.getlist("symbol_type")
         tickers["plot_type"] = request.args.getlist("plot_type")
         tickers["interval"] = request.args.getlist("interval")
         tickers["lookback"] = request.args.getlist("lookback", type=no_empty_int)
         tickers["wait_time"] = request.args.getlist("wait_time", type=no_empty_int)
         tickers["mav"] = request.args.getlist("mav", type=no_empty_int)
         tickers["volume"] = request.args.getlist("volume", type=str_to_bool)
+        tickers["avg_buy_price"] = request.args.getlist(
+            "avg_buy_price", type=no_empty_float
+        )
 
         sequence = SequenceConfig(
             skip_outdated=request.args.get("skip_outdated", False, type=bool),
             # NOTE: currently not toggleable from the web app
             skip_empty=request.args.get("skip_empty", True, type=bool),
         )
```

### Comparing `tinyticker-0.5.0/tinyticker/web/command.py` & `tinyticker-0.5.1/tinyticker/web/command.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.0/tinyticker/web/templates/css/uikit.min.css` & `tinyticker-0.5.1/tinyticker/web/templates/css/uikit.min.css`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.0/tinyticker/web/templates/images/apple-touch-icon.png` & `tinyticker-0.5.1/tinyticker/web/templates/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.0/tinyticker/web/templates/images/favicon-16x16.png` & `tinyticker-0.5.1/tinyticker/web/templates/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.0/tinyticker/web/templates/images/favicon-32x32.png` & `tinyticker-0.5.1/tinyticker/web/templates/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.0/tinyticker/web/templates/index.html` & `tinyticker-0.5.1/tinyticker/web/templates/index.html`

 * *Files 12% similar despite different names*

```diff
@@ -151,23 +151,20 @@
                       >
                       <select
                         class="uk-select"
                         id="symbol_type"
                         name="symbol_type"
                       >
                         {%- for symbol_type_option in symbol_type_options -%}
-                          {%- if symbol_type_option == ticker.symbol_type -%}
-                            <option value="{{ symbol_type_option }}" selected>
-                              {{ symbol_type_option }}
-                            </option>
-                          {%- else -%}
-                            <option value="{{ symbol_type_option }}">
-                              {{ symbol_type_option }}
-                            </option>
-                          {%- endif -%}
+                          <option
+                            value="{{ symbol_type_option }}"
+                            {% if symbol_type_option == ticker.symbol_type %}selected{% endif %}
+                          >
+                            {{ symbol_type_option }}
+                          </option>
                         {%- endfor -%}
                       </select>
                       <label class="uk-form-label" for="symbol">Symbol</label>
                       <input
                         class="uk-input"
                         type="text"
                         id="symbol"
@@ -175,116 +172,89 @@
                         value="{{ ticker.symbol }}"
                       />
                       <label class="uk-form-label" for="interval"
                         >Interval</label
                       >
                       <select class="uk-select" id="interval" name="interval">
                         {%- for interval_option in interval_options -%}
-                          {%- if interval_option == ticker.interval -%}
-                            <option value="{{ interval_option }}" selected>
-                              {{ interval_option }}
-                            </option>
-                          {%- else -%}
-                            <option value="{{ interval_option }}">
-                              {{ interval_option }}
-                            </option>
-                          {%- endif -%}
+                          <option
+                            value="{{ interval_option }}"
+                            {% if interval_option == ticker.interval %}selected{% endif %}
+                          >
+                            {{ interval_option }}
+                          </option>
                         {%- endfor -%}
                       </select>
                       <label class="uk-form-label" for="plot_type"
                         >Plot type</label
                       >
                       <select class="uk-select" id="plot_type" name="plot_type">
                         {%- for plot_type_option in plot_type_options -%}
-                          {%- if plot_type_option == ticker.plot_type -%}
-                            <option value="{{ plot_type_option }}" selected>
-                              {{ plot_type_option }}
-                            </option>
-                          {%- else -%}
-                            <option value="{{ plot_type_option }}">
-                              {{ plot_type_option }}
-                            </option>
-                          {%- endif -%}
+                          <option
+                            value="{{ plot_type_option }}"
+                            {% if plot_type_option == ticker.plot_type %}selected{% endif %}
+                          >
+                            {{ plot_type_option }}
+                          </option>
                         {%- endfor -%}
                       </select>
                       <label class="uk-form-label" for="lookback"
                         >Lookback</label
                       >
-                      {%- if ticker.lookback is none -%}
-                        {#- If the look back is None then it hasn't been set so use the default lookback for the interval #}
-                        <input
-                          class="uk-input"
-                          inputmode="numeric"
-                          id="lookback"
-                          name="lookback"
-                          min="1"
-                          placeholder="{{ interval_lookbacks[ticker.interval] }}"
-                        />
-                      {%- else -%}
-                        <input
-                          class="uk-input"
-                          inputmode="numeric"
-                          id="lookback"
-                          name="lookback"
-                          min="1"
-                          value="{{ ticker.lookback }}"
-                        />
-                      {%- endif -%}
+                      <input
+                        class="uk-input"
+                        inputmode="numeric"
+                        id="lookback"
+                        name="lookback"
+                        min="1"
+                        {#- If the look back is None then it has not been set so use the default lookback for the interval #}
+                        {% if ticker.lookback is none %}placeholder="{{ interval_lookbacks[ticker.interval] }}"{% else %}value="{{ ticker.lookback }}"{% endif %}
+                      />
                       <label class="uk-form-label" for="wait_time"
                         >Wait time (s)</label
                       >
-                      {%- if ticker.wait_time is none -%}
-                        {#- If the wait_time is None then it hasn't been set so use the default wait_time for the interval #}
-                        <input
-                          class="uk-input"
-                          inputmode="numeric"
-                          id="wait_time"
-                          name="wait_time"
-                          min="1"
-                          placeholder="{{ interval_wait_times[ticker.interval] }}"
-                        />
-                      {%- else -%}
-                        <input
-                          class="uk-input"
-                          inputmode="numeric"
-                          id="wait_time"
-                          name="wait_time"
-                          min="1"
-                          value="{{ ticker.wait_time }}"
-                        />
-                      {%- endif -%}
+                      <input
+                        class="uk-input"
+                        inputmode="numeric"
+                        id="wait_time"
+                        name="wait_time"
+                        min="1"
+                        {#- If the wait_time is None then it has not been set so use the default wait_time for the interval #}
+                        {% if ticker.wait_time is none %}placeholder="{{ interval_wait_times[ticker.interval] }}"{% else %}value="{{ ticker.wait_time }}"{% endif %}
+                      />
                       <label class="uk-form-label" for="mav"
                         >Moving average</label
                       >
-                      {%- if ticker.mav is none -%}
-                        <input
-                          class="uk-input"
-                          inputmode="numeric"
-                          id="mav"
-                          name="mav"
-                          min="1"
-                          placeholder="3"
-                        />
-                      {%- else -%}
-                        <input
-                          class="uk-input"
-                          inputmode="numeric"
-                          id="mav"
-                          name="mav"
-                          min="1"
-                          value="{{ ticker.mav }}"
-                        />
-                      {%- endif -%}
+                      <input
+                        class="uk-input"
+                        inputmode="numeric"
+                        id="mav"
+                        name="mav"
+                        min="1"
+                        {% if ticker.mav is none %}placeholder="3"{% else %}value="{{ ticker.mav }}"{% endif %}
+                      />
+                      <label class="uk-form-label" for="avg_buy_price"
+                        >Average buy price</label
+                      >
+                      <input
+                        class="uk-input"
+                        inputmode="numeric"
+                        id="avg_buy_price"
+                        name="avg_buy_price"
+                        min="0"
+                        value="{{ ticker.avg_buy_price if ticker.avg_buy_price is not none }}"
+                        uk-tooltip="Optional, used to display percentage change from buy price."
+                      />
                       <label class="uk-form-label" for="volume"
                         >Show trade volume
-                        {% if ticker.volume | default(False) %}
-                          <input type="hidden" name="volume" value="1" />
-                        {% else %}
-                          <input type="hidden" name="volume" value="0" />
-                        {% endif %}
+                        <input
+                          type="hidden"
+                          name="volume"
+                          value="{{ 1 if ticker.volume | default(false) else 0 }}"
+                        />
                         <input
                           class="uk-checkbox"
                           type="checkbox"
                           {% if ticker.volume | default(False) %}checked{% endif %}
                           onclick="this.previousElementSibling.value=1-this.previousElementSibling.value"
                         />
                       </label>
```

#### html2text {}

```diff
@@ -14,41 +14,38 @@
 {{ epd_model_option.desc }}
 {%- endif -%} {%- endfor -%}
 % if flip | default(False) %}checked{% endif %} />Flip display
 _C_r_y_p_t_o_C_o_m_p_a_r_e API key
 % if api_key %}value="{{ api_key }}"{% endif %} />
 ****** TTiicckkeerrss ******
 {%- for ticker in tickers -%}
-{%- for symbol_type_option in symbol_type_options -%} {%- if symbol_type_option
-== ticker.symbol_type -%}
-{{ symbol_type_option }}
-{%- else -%}
-{{ symbol_type_option }}
-{%- endif -%} {%- endfor -%}
-{%- for interval_option in interval_options -%} {%- if interval_option ==
-ticker.interval -%}
-{{ interval_option }}
-{%- else -%}
-{{ interval_option }}
-{%- endif -%} {%- endfor -%}
-{%- for plot_type_option in plot_type_options -%} {%- if plot_type_option ==
-ticker.plot_type -%}
-{{ plot_type_option }}
-{%- else -%}
-{{ plot_type_option }}
-{%- endif -%} {%- endfor -%}
-Lookback {%- if ticker.lookback is none -%} {#- If the look back is None then
-it hasn't been set so use the default lookback for the interval #} [lookback
-]{%- else -%} [{{ ticker.lookback }}]{%- endif -%} Wait time (s) {%- if
-ticker.wait_time is none -%} {#- If the wait_time is None then it hasn't been
-set so use the default wait_time for the interval #} [wait_time           ]{%-
-else -%} [{{ ticker.wait_time }}]{%- endif -%} Moving average {%- if ticker.mav
-is none -%} [mav                 ]{%- else -%} [{{ ticker.mav }}    ]{%- endif
--%} Show trade volume {% if ticker.volume | default(False) %} {% else %} {%
-endif %}
+{%- for symbol_type_option in symbol_type_options -%}
+% if symbol_type_option == ticker.symbol_type %}selected{% endif %} > {
+{ symbol_type_option }}
+{%- endfor -%}
+{%- for interval_option in interval_options -%}
+% if interval_option == ticker.interval %}selected{% endif %} > {
+{ interval_option }}
+{%- endfor -%}
+{%- for plot_type_option in plot_type_options -%}
+% if plot_type_option == ticker.plot_type %}selected{% endif %} > {
+{ plot_type_option }}
+{%- endfor -%}
+Lookback
+#- If the look back is None then it has not been set so use the default
+lookback for the interval #} {% if ticker.lookback is none %}placeholder="{
+{ interval_lookbacks[ticker.interval] }}"{% else %}value="{{ ticker.lookback
+}}"{% endif %} /> Wait time (s)
+#- If the wait_time is None then it has not been set so use the default
+wait_time for the interval #} {% if ticker.wait_time is none %}placeholder="{
+{ interval_wait_times[ticker.interval] }}"{% else %}value="{{ ticker.wait_time
+}}"{% endif %} /> Moving average
+% if ticker.mav is none %}placeholder="3"{% else %}value="{{ ticker.mav }}"{%
+endif %} /> Average buy price [{{ ticker.avg_buy_price if ticker.avg_buy_price
+is not none }}]Show trade volume
 % if ticker.volume | default(False) %}checked{% endif %}
 onclick="this.previousElementSibling.value=1-this.previousElementSibling.value"
 />
 {%- endfor -%}
 % if sequence.skip_outdated | default(True) %}checked{% endif %} />Skip tickers
 with outdated data Apply
 Command
```

### Comparing `tinyticker-0.5.0/tinyticker/web/templates/js/index.js` & `tinyticker-0.5.1/tinyticker/web/templates/js/index.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.0/tinyticker/web/templates/js/uikit-icons.min.js` & `tinyticker-0.5.1/tinyticker/web/templates/js/uikit-icons.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.0/tinyticker/web/templates/js/uikit.min.js` & `tinyticker-0.5.1/tinyticker/web/templates/js/uikit.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.0/tinyticker/web/templates/logfiles.html` & `tinyticker-0.5.1/tinyticker/web/templates/logfiles.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.5.0/PKG-INFO` & `tinyticker-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyticker
-Version: 0.5.0
+Version: 0.5.1
 Summary: A tiny Raspberry Pi powered ePaper ticker.
 Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT
 Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance
 Author: Loic Coyle
 Author-email: loic.coyle@hotmail.fr
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tinyticker Version: 0.5.0 Summary: A tiny Raspberry
+Metadata-Version: 2.1 Name: tinyticker Version: 0.5.1 Summary: A tiny Raspberry
 Pi powered ePaper ticker. Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance Author:
 Loic Coyle Author-email: loic.coyle@hotmail.fr Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

