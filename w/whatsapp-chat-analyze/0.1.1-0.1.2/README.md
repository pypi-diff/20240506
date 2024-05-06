# Comparing `tmp/whatsapp_chat_analyze-0.1.1.tar.gz` & `tmp/whatsapp_chat_analyze-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whatsapp_chat_analyze-0.1.1.tar", max compression
+gzip compressed data, was "whatsapp_chat_analyze-0.1.2.tar", max compression
```

## Comparing `whatsapp_chat_analyze-0.1.1.tar` & `whatsapp_chat_analyze-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-05-06 04:15:09.959026 whatsapp_chat_analyze-0.1.1/README.md
--rw-r--r--   0        0        0      898 2024-05-06 04:30:18.970168 whatsapp_chat_analyze-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-06 04:30:18.970846 whatsapp_chat_analyze-0.1.1/whatsapp_chat_analyze/__init__.py
--rwxr-xr-x   0        0        0    10778 2024-05-06 04:27:52.831627 whatsapp_chat_analyze-0.1.1/whatsapp_chat_analyze/cli.py
--rw-r--r--   0        0        0     1036 1970-01-01 00:00:00.000000 whatsapp_chat_analyze-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1682 2024-05-06 04:35:18.706328 whatsapp_chat_analyze-0.1.2/README.md
+-rw-r--r--   0        0        0      898 2024-05-06 04:36:39.949573 whatsapp_chat_analyze-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-06 04:36:39.950136 whatsapp_chat_analyze-0.1.2/whatsapp_chat_analyze/__init__.py
+-rwxr-xr-x   0        0        0    10780 2024-05-06 04:36:33.023041 whatsapp_chat_analyze-0.1.2/whatsapp_chat_analyze/cli.py
+-rw-r--r--   0        0        0     2718 1970-01-01 00:00:00.000000 whatsapp_chat_analyze-0.1.2/PKG-INFO
```

### Comparing `whatsapp_chat_analyze-0.1.1/pyproject.toml` & `whatsapp_chat_analyze-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "whatsapp-chat-analyze"
-version = "0.1.1"
+version = "0.1.2"
 description = "Ingest and analyze WhatsApp chat data, and plot beautiful visualizations."
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/tddschn/whatsapp-chat-analyze"
 repository = "https://github.com/tddschn/whatsapp-chat-analyze"
 classifiers = ["Topic :: Utilities"]
```

### Comparing `whatsapp_chat_analyze-0.1.1/whatsapp_chat_analyze/cli.py` & `whatsapp_chat_analyze-0.1.2/whatsapp_chat_analyze/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,16 @@
     df,
     output_base_name: str,
     plot_type: str,
     chat_name: str | None = None,
     plotly: bool = False,
 ):
     title_suffix = " | Made by Teddy (teddysc.me)"
-    title_prefix = f"{chat_name} |" if chat_name else ""
+    title_prefix = f"{chat_name} | " if chat_name else ""
+
     import matplotlib.pyplot as plt
 
     if plot_type == "message_count":
         print(f'Plotting "{plot_type}"')
         df["Author"].value_counts().plot(kind="bar")
         plt.title(title_prefix + "Message Counts" + title_suffix)
         plt.ylabel("Number of Messages")
```

