# Comparing `tmp/bib2x-0.4.0.tar.gz` & `tmp/bib2x-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\products\bibpres\bib2x_github - Kopie\dist\.tmp-_8917u2h\bib2x-0.4.0.tar", last modified: Mon Mar 27 19:32:34 2023, max compression
+gzip compressed data, was "bib2x-0.4.2.tar", last modified: Mon May  6 17:24:12 2024, max compression
```

## Comparing `bib2x-0.4.0.tar` & `bib2x-0.4.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 19:32:34.451041 bib2x-0.4.0/
--rw-rw-rw-   0        0        0     1520 2023-03-08 17:26:03.000000 bib2x-0.4.0/LICENSE
--rw-rw-rw-   0        0        0     5436 2023-03-27 19:32:34.450040 bib2x-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     3936 2023-03-27 19:16:38.000000 bib2x-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-27 19:32:34.403029 bib2x-0.4.0/bib2x/
--rw-rw-rw-   0        0        0      542 2023-03-10 20:29:20.000000 bib2x-0.4.0/bib2x/__init__.py
--rw-rw-rw-   0        0        0     3174 2023-03-27 18:57:14.000000 bib2x-0.4.0/bib2x/bib2x.py
--rw-rw-rw-   0        0        0    18580 2023-03-10 20:29:05.000000 bib2x-0.4.0/bib2x/texfile.py
-drwxrwxrwx   0        0        0        0 2023-03-27 19:32:34.425035 bib2x-0.4.0/bib2x/texhandler/
--rw-rw-rw-   0        0        0      556 2023-03-10 20:28:31.000000 bib2x-0.4.0/bib2x/texhandler/__init__.py
--rw-rw-rw-   0        0        0     2691 2023-03-10 20:28:08.000000 bib2x-0.4.0/bib2x/texhandler/handler.py
--rw-rw-rw-   0        0        0     7996 2023-03-27 19:02:11.000000 bib2x-0.4.0/bib2x/texhandler/html.py
--rw-rw-rw-   0        0        0     4584 2023-03-27 17:52:55.000000 bib2x-0.4.0/bib2x/texhandler/json.py
--rw-rw-rw-   0        0        0     5265 2023-03-10 20:28:18.000000 bib2x-0.4.0/bib2x/texhandler/memory.py
-drwxrwxrwx   0        0        0        0 2023-03-27 19:32:34.413032 bib2x-0.4.0/bib2x.egg-info/
--rw-rw-rw-   0        0        0     5436 2023-03-27 19:32:34.000000 bib2x-0.4.0/bib2x.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      451 2023-03-27 19:32:34.000000 bib2x-0.4.0/bib2x.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 19:32:34.000000 bib2x-0.4.0/bib2x.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-03-27 19:32:34.000000 bib2x-0.4.0/bib2x.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       12 2023-03-27 19:32:34.000000 bib2x-0.4.0/bib2x.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-27 19:32:34.451041 bib2x-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     2330 2023-03-27 19:26:23.000000 bib2x-0.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-27 19:32:34.449041 bib2x-0.4.0/tests/
--rw-rw-rw-   0        0        0      398 2023-03-08 17:08:25.000000 bib2x-0.4.0/tests/__init__.py
--rw-rw-rw-   0        0        0     7079 2023-03-27 19:04:23.000000 bib2x-0.4.0/tests/test_bib2x_html.py
--rw-rw-rw-   0        0        0     6419 2023-03-27 18:59:44.000000 bib2x-0.4.0/tests/test_bib2x_json.py
--rw-rw-rw-   0        0        0     2487 2023-03-27 18:59:17.000000 bib2x-0.4.0/tests/test_bib2x_main.py
+drwxrwxrwx   0        0        0        0 2024-05-06 17:24:12.501791 bib2x-0.4.2/
+-rw-rw-rw-   0        0        0     1520 2024-05-06 17:08:29.000000 bib2x-0.4.2/LICENSE
+-rw-rw-rw-   0        0        0     5436 2024-05-06 17:24:12.500792 bib2x-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3936 2024-05-06 17:08:29.000000 bib2x-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 17:24:12.482788 bib2x-0.4.2/bib2x/
+-rw-rw-rw-   0        0        0      568 2024-05-06 17:12:17.000000 bib2x-0.4.2/bib2x/__init__.py
+-rw-rw-rw-   0        0        0     3083 2024-05-06 17:13:13.000000 bib2x-0.4.2/bib2x/bib2x.py
+-rw-rw-rw-   0        0        0     9216 2024-05-06 17:08:29.000000 bib2x-0.4.2/bib2x/tex.db
+-rw-rw-rw-   0        0        0    18118 2024-05-06 17:08:29.000000 bib2x-0.4.2/bib2x/texfile.py
+drwxrwxrwx   0        0        0        0 2024-05-06 17:24:12.494791 bib2x-0.4.2/bib2x/texhandler/
+-rw-rw-rw-   0        0        0      541 2024-05-06 17:08:29.000000 bib2x-0.4.2/bib2x/texhandler/__init__.py
+-rw-rw-rw-   0        0        0     2591 2024-05-06 17:08:29.000000 bib2x-0.4.2/bib2x/texhandler/handler.py
+-rw-rw-rw-   0        0        0     7818 2024-05-06 17:08:29.000000 bib2x-0.4.2/bib2x/texhandler/html.py
+-rw-rw-rw-   0        0        0     4433 2024-05-06 17:08:29.000000 bib2x-0.4.2/bib2x/texhandler/json.py
+-rw-rw-rw-   0        0        0     5099 2024-05-06 17:08:29.000000 bib2x-0.4.2/bib2x/texhandler/memory.py
+drwxrwxrwx   0        0        0        0 2024-05-06 17:24:12.499791 bib2x-0.4.2/bib2x.egg-info/
+-rw-rw-rw-   0        0        0     5436 2024-05-06 17:24:12.000000 bib2x-0.4.2/bib2x.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2024-05-06 17:24:12.000000 bib2x-0.4.2/bib2x.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 17:24:12.000000 bib2x-0.4.2/bib2x.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-06 17:24:12.000000 bib2x-0.4.2/bib2x.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       12 2024-05-06 17:24:12.000000 bib2x-0.4.2/bib2x.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 17:24:12.501791 bib2x-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     2406 2024-05-06 17:24:05.000000 bib2x-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 17:24:12.498792 bib2x-0.4.2/tests/
+-rw-rw-rw-   0        0        0      398 2024-05-06 17:08:29.000000 bib2x-0.4.2/tests/__init__.py
+-rw-rw-rw-   0        0        0     7079 2024-05-06 17:08:29.000000 bib2x-0.4.2/tests/test_bib2x_html.py
+-rw-rw-rw-   0        0        0     6419 2024-05-06 17:08:29.000000 bib2x-0.4.2/tests/test_bib2x_json.py
+-rw-rw-rw-   0        0        0     2487 2024-05-06 17:08:29.000000 bib2x-0.4.2/tests/test_bib2x_main.py
```

### Comparing `bib2x-0.4.0/LICENSE` & `bib2x-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bib2x-0.4.0/PKG-INFO` & `bib2x-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bib2x
-Version: 0.4.0
+Version: 0.4.2
 Summary: A BibTex parser and converter
 Home-page: http://bib2x.readthedocs.org/
 Download-URL: http://pypi.python.org/pypi/bib2x
 Author: dkrajzew
 Author-email: d.krajzewicz@gmail.com
 License: BSD
 Project-URL: Documentation, https://bib2x.readthedocs.io/
```

### Comparing `bib2x-0.4.0/README.md` & `bib2x-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `bib2x-0.4.0/bib2x/bib2x.py` & `bib2x-0.4.2/bib2x/bib2x.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-from __future__ import print_function
-# ===================================================================
-# bib2x - A BibTex parser and converter.
-#
-# bib2x.py - Main module
-#
-# (c) Daniel Krajzewicz 2011-2014, 2022-2023
-# daniel@krajzewicz.de
-# - https://github.com/dkrajzew/bib2x
-# - http://www.krajzewicz.de/docs/bib2x/index.html
-# - http://www.krajzewicz.de
-# 
-# Available under the BSD license.
-# ===================================================================
-
-
-# --- imports -------------------------------------------------------
-import sys, os
-sys.path.append(os.path.dirname(os.path.realpath(__file__)))
-from optparse import OptionParser
-try: import texfile
-except: from . import texfile
-try: import texhandler
-except: from . import texhandler
-try:
-    import texhandler
-    import texhandler.json
-    import texhandler.html
-except:
-    pass
-
-# --- functions -----------------------------------------------------
-# --- main
-def main(arguments=None):
-    """Main method
-    
-    The application reads the file defined by --input / -i _&lt;BIBTEX_FILE&gt;_ and saves the contents
-    to the file defined using the option --output / -o _&lt;FILE&gt;_, converting them to the 
-    format defined using the option --format / -f _&lt;FORMAT&gt;_.
-    
-    Args:
-        arguments (List[str]): The command line arguments, parsed as options using OptionParser.
-
-
-    Options
-    -------
-    
-    The following options must be set:
-
-    --input / -i _&lt;BIBTEX_FILE&gt;_:
-        The BibTeX file to load
-    
-    --output / -o _&lt;FILE&gt;_:
-        The file to write
-    
-    The following options are optional:
-    
-    --format / -f _&lt;FORMAT&gt;_:
-        The type of file to write ['json']
-    
-    
-    """
-    # build options
-    optParser = OptionParser(usage="bib2x [options]", version="bib2x 0.4.0")
-    optParser.add_option("-i", "--input", dest="input", default=None, help="The BibTeX file to load")
-    optParser.add_option("-o", "--output", dest="output", default=None, help="The file to write")
-    optParser.add_option("-f", "--format", dest="format", default="json", help="The type of file to write ['json']")
-    options, remaining_args = optParser.parse_args(args=arguments)
-    # check options
-    if options.input is None:
-        optParser.error("Input file name is missing, please use the option '--input' / '-i'.")
-    if options.output is None:
-        optParser.error("Output file name is missing, please use the option '--output' / '-o'.")
-    if options.format!="json" and options.format!="html":
-        optParser.error("Unknown output format; only 'json' and 'html' are supported.")
-    # process
-    texF = texfile.TeXfile()
-    content = texF.read2string(options.input)
-    fdo = open(options.output, "w")
-    handler = None
-    if options.format=="json":
-        handler = texhandler.json.JSONexportingTeXhandler(fdo)
-    elif options.format=="html":
-        handler = texhandler.html.HTMLexportingTeXhandler(fdo)
-    texF.parse(content, handler)
-    
-
-
-# -- main check
-if __name__ == '__main__':
-    main(sys.argv[1:]) # pragma: no cover
+from __future__ import print_function
+# ===================================================================
+# bib2x - A BibTex parser and converter.
+#
+# bib2x.py - Main module
+#
+# (c) Daniel Krajzewicz 2011-2014, 2022-2023
+# daniel@krajzewicz.de
+# - https://github.com/dkrajzew/bib2x
+# - http://www.krajzewicz.de/docs/bib2x/index.html
+# - http://www.krajzewicz.de
+# 
+# Available under the BSD license.
+# ===================================================================
+
+
+# --- imports -------------------------------------------------------
+import sys, os
+sys.path.append(os.path.dirname(os.path.realpath(__file__)))
+from optparse import OptionParser
+try: import texfile
+except: from . import texfile
+try: import texhandler
+except: from . import texhandler
+try:
+    import texhandler
+    import texhandler.json
+    import texhandler.html
+except:
+    pass
+
+# --- functions -----------------------------------------------------
+# --- main
+def main(arguments=None):
+    """Main method
+    
+    The application reads the file defined by --input / -i _&lt;BIBTEX_FILE&gt;_ and saves the contents
+    to the file defined using the option --output / -o _&lt;FILE&gt;_, converting them to the 
+    format defined using the option --format / -f _&lt;FORMAT&gt;_.
+    
+    Args:
+        arguments (List[str]): The command line arguments, parsed as options using OptionParser.
+
+
+    Options
+    -------
+    
+    The following options must be set:
+
+    --input / -i _&lt;BIBTEX_FILE&gt;_:
+        The BibTeX file to load
+    
+    --output / -o _&lt;FILE&gt;_:
+        The file to write
+    
+    The following options are optional:
+    
+    --format / -f _&lt;FORMAT&gt;_:
+        The type of file to write ['json']
+    
+    
+    """
+    # build options
+    optParser = OptionParser(usage="bib2x [options]", version="bib2x 0.4.2")
+    optParser.add_option("-i", "--input", dest="input", default=None, help="The BibTeX file to load")
+    optParser.add_option("-o", "--output", dest="output", default=None, help="The file to write")
+    optParser.add_option("-f", "--format", dest="format", default="json", help="The type of file to write ['json']")
+    options, remaining_args = optParser.parse_args(args=arguments)
+    # check options
+    if options.input is None:
+        optParser.error("Input file name is missing, please use the option '--input' / '-i'.")
+    if options.output is None:
+        optParser.error("Output file name is missing, please use the option '--output' / '-o'.")
+    if options.format!="json" and options.format!="html":
+        optParser.error("Unknown output format; only 'json' and 'html' are supported.")
+    # process
+    texF = texfile.TeXfile()
+    content = texF.read2string(options.input)
+    fdo = open(options.output, "w")
+    handler = None
+    if options.format=="json":
+        handler = texhandler.json.JSONexportingTeXhandler(fdo)
+    elif options.format=="html":
+        handler = texhandler.html.HTMLexportingTeXhandler(fdo)
+    texF.parse(content, handler)
+    
+
+
+# -- main check
+if __name__ == '__main__':
+    main(sys.argv[1:]) # pragma: no cover
```

### Comparing `bib2x-0.4.0/bib2x/texfile.py` & `bib2x-0.4.2/bib2x/texfile.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,463 +1,463 @@
-from __future__ import print_function
-# ===================================================================
-# bib2x - A BibTex parser and converter.
-#
-# texfile.py - A BibTex-file representation
-#
-# (c) Daniel Krajzewicz 2011-2014, 2022-2023
-# daniel@krajzewicz.de
-# - https://github.com/dkrajzew/bib2x
-# - http://www.krajzewicz.de/docs/bib2x/index.html
-# - http://www.krajzewicz.de
-# 
-# Available under the BSD license.
-# ===================================================================
-
-
-# --- imports -------------------------------------------------------
-import os
-import sys
-import re
-import sqlite3
-
-
-# --- debugging options ---------------------------------------------
-DEBUG_SPECIAL_RECOGNITION = False
-DEBUG_SPECIAL_CODING = False
-DEBUG_UNKNOWN_CMD = False
-
-
-# --- classes -------------------------------------------------------
-class TeXfile:
-    """A class representing a BibTeX file"""
-    
-    def __init__(self):
-        """Initialisation
-        
-        Todo:
-            Extract DB entries and set them up as Python definitions?
-        """
-        self._stringMap = {}
-        self._stringMapKeys = []
-        DB = os.path.join(os.path.dirname(__file__), 'tex.db')
-        conn = sqlite3.connect(DB)
-        cur = conn.cursor()
-        cur.execute('SELECT * FROM styles')
-        self._tex_styles = cur.fetchall()
-        cur.execute('SELECT * FROM stylesp')
-        self._tex_styles_pref = cur.fetchall()
-        cur.execute('SELECT * FROM conv')
-        self._tex_conv = cur.fetchall()
-        cur.execute('SELECT * FROM repl')
-        self._tex_repl = cur.fetchall()
-        
-
-    def _decodeCommand(self, cmd, optArgs, content, ret):
-        if DEBUG_SPECIAL_RECOGNITION: print ("decode: '" + cmd + "/" + content + "'")
-        if cmd=='\\':
-            if DEBUG_SPECIAL_RECOGNITION: print (">!3")
-            return content, False
-        for t in self._tex_styles:
-            if cmd == t[0]:
-                r = str(t[1])
-                r = r.replace("%s", content)
-                r = r.replace("%a", optArgs)
-                if DEBUG_SPECIAL_RECOGNITION: print (">" + r)
-                return r, False
-        for t in self._tex_styles_pref:
-            if cmd == t[0]:
-                if DEBUG_SPECIAL_RECOGNITION: print (">!1")
-                ret["pref"] = True
-                return "", False
-        for t in self._tex_conv:
-            if cmd.startswith(t[0]):
-                r = str(t[1].strip())
-                if DEBUG_SPECIAL_RECOGNITION: print (">" + r + cmd[len(t[0]):])
-                removeSpaces = t[0][1].isalpha()
-                return r + cmd[len(t[0]):], removeSpaces
-        cmd2 = cmd + content
-        for t in self._tex_conv:
-            if cmd2.startswith(t[0]):
-                r = str(t[1].strip())
-                if DEBUG_SPECIAL_RECOGNITION: print (">" + r + cmd2[len(t[0]):])
-                return r + cmd2[len(t[0]):], False
-        ret["unfound"] = True
-        if DEBUG_UNKNOWN_CMD: print ("Unknown cmd '%s'" % cmd)
-        if cmd[0]=='\\':
-            return cmd[1:], False
-        return cmd, False
-        
-
-    def _decodeCommand2(self, cmd, optArgs, content, w, beg, end, currPos):
-        ret = {}
-        r, s = self._decodeCommand(cmd, optArgs, content, ret)
-        if "pref" in ret:
-            for i in self._tex_styles_pref:
-                if cmd==i[0]:
-                    beg = beg + len(cmd)
-                    while w[beg]==' ' or w[beg]=='\n':
-                        beg = beg + 1
-                    r, e = self._tex2html(w, beg, end)
-                    if DEBUG_SPECIAL_RECOGNITION: print ("> " + str(i[1]) + r + str(i[2]))
-                    return str(i[1]) + r + str(i[2]), end
-        if "unfound" in ret and currPos<end-1 and w[currPos]=='\\':
-            cmd = cmd + w[currPos+1:currPos+2]
-            r, s = self._decodeCommand(cmd, optArgs, "", ret)
-            currPos += 2
-        if s:
-            if DEBUG_SPECIAL_RECOGNITION: print ("here's s")
-            currPos = self._skipSpaces(w, currPos)
-        return r, currPos
-        
-    
-    def _findMatchingBracket(self, w, beg, o="{", c="}"):
-        i = beg
-        l = 0
-        while i<len(w):
-            if w[i]==o:
-                l = l + 1
-            if w[i]==c:
-                l = l - 1
-                if l==0:
-                    return i
-            i = i + 1
-        print ("error: Missing closing bracket '%s'" % w[beg:])
-        return len(w)
-        
-        
-    def _skipSpaces(self, w, i):
-        while i<len(w) and w[i].isspace():
-            i = i + 1
-        return i
-
-
-    def _tex2html(self, w, beg=0, end=-1):
-        #print "%s %s %s" % (w, beg, end)
-        i = beg
-        if end<0:
-            end = len(w)
-        else:
-            end = min(len(w), end)
-        r = ""
-        while i<end:
-            if w[i]=='\\':
-                procB = i
-                cmdEnd = -1
-                optArgs = ""
-                i = i + 1
-                e1 = False
-                while i<end and not e1:
-                    if not e1 and w[i]=='[':
-                        # optional parameter
-                        cmdEnd = i
-                        q = self._findMatchingBracket(w, i, "[", "]")
-                        optArgs = ", " + w[i+1:q]
-                        if DEBUG_SPECIAL_CODING: print ("2a: %s %s %s" % (procB, i, optArgs))
-                        i = q + 1
-                    if not e1 and w[i]=='{':
-                        # escaped command, with a bracketed parameter
-                        if DEBUG_SPECIAL_CODING: print ("2: %s %s %s" % (procB, i, w))
-                        q = self._findMatchingBracket(w, i)
-                        dec, e = self._tex2html(w, i+1, q)
-                        if cmdEnd<0: cmdEnd = i
-                        t1, i = self._decodeCommand2(w[procB:cmdEnd].strip(), optArgs, dec, w, beg, end, i)
-                        r = r + t1
-                        i = q + 1
-                        e1 = True                    
-                    if not e1 and w[i]=='|':
-                        # escaped command, with a bracketed parameter
-                        if DEBUG_SPECIAL_CODING: print ("2b: %s %s %s" % (procB, i, w))
-                        q = w.find('|', i+1)
-                        dec, e = self._tex2html(w, i+1, q)
-                        if cmdEnd<0: cmdEnd = i
-                        t1, i = self._decodeCommand2(w[procB:cmdEnd].strip(), optArgs, dec, w, beg, end, i)
-                        r = r + t1
-                        i = q + 1
-                        e1 = True
-                    if not e1 and w[i]=='\\' and i==procB+1:
-                        if DEBUG_SPECIAL_CODING: print ("1b: %s %s %s %s %s" % (procB, i, w, len(w), end))
-                        r = r + "<br/>"
-                        i = self._skipSpaces(w, i + 1)
-                        e1 = True 
-                    if not e1 and (w[i]==' ' or w[i]=='\\' or (i>=procB+2 and not w[i].isalpha() and w[procB+1].isalpha())):
-                        # escaped command, closed by a trailing blank
-                        if DEBUG_SPECIAL_CODING: print ("1: %s %s %s %s %s" % (procB, i, w, len(w), end))
-                        t1, i = self._decodeCommand2(w[procB:i].strip(), optArgs, "", w, beg, end, i)
-                        r = r + t1
-                        e1 = True
-                    if not e1:
-                        i = i + 1
-                if i==end and not e1:
-                    if DEBUG_SPECIAL_CODING: print ("3: %s %s %s %s %s" % (procB, i, w, len(w), end))
-                    t1, i = self._decodeCommand2(w[procB:i].strip(), optArgs, "", w, beg, end, i)
-                    r = r + t1
-            elif w[i]=='{':
-                q = self._findMatchingBracket(w, i)
-                if DEBUG_SPECIAL_CODING: print ("4: %s %s %s" % (i, q, w[i+1:q]))
-                dec, i = self._tex2html(w, i+1, q)
-                if DEBUG_SPECIAL_CODING: print ("t1: %s %s %s %s" % ("hallo", i, w[i-2:i+2], dec))
-                r = r + dec
-                i = q + 1
-                if DEBUG_SPECIAL_CODING: print ("t2: %s %s %s %s %s" % ("hallo", i, w[i-2:i+2], end, r))
-            elif w[i]=='$':
-                q = w.find('$', i+1)
-                if q<0:
-                    print ("unclosed special character $")
-                    q = i
-                if DEBUG_SPECIAL_CODING: print ("5: %s %s %s" % (i, q, w[i+1:q]))
-                dec, i = self._tex2html(w, i+1, q)
-                r = r + dec
-                i = q + 1
-            else:
-                if w[i]=='\n':
-                    r = r + ' '
-                else:
-                    r = r + w[i]                    
-                i = i + 1
-        for t in self._tex_repl:
-            r = r.replace(str(t[0]), str(t[1]))
-        r2 = ""
-        html = False
-        for j in range(0, len(r)):
-            if r[j]=='<':
-                html = True
-            elif r[j]=='>':
-                html = False
-            if r[j]=='"' and not html:
-                r2 = r2 + "&quot;"
-            elif r[j]=="'" and not html:
-                r2 = r2 + "&rsquo;"
-            else:
-                r2 = r2 + r[j]
-        r = r2            
-        r = re.sub("\s+" , " ", r)
-        return r, i    
-                
-
-    def _splitHTMLaware(self, what):
-        """Splits the given string at ';' and ',', assuring that a split
-             is not done if the occured ';' belongs to a HTML-encoded special
-             character
-        
-        Args:
-            what (str): The string to split
-            
-        Returns:
-            (List[str]): The split string
-        """
-        ret = []
-        b = 0
-        isHTML = False
-        for i in range(0, len(what)):
-            if what[i]=='&':
-                isHTML = True
-            if what[i]==',' or (what[i]==';' and not isHTML):
-                ret.append(what[b:i].strip())
-                b = i+1
-            if what[i]==';':
-                isHTML = False
-        ret.append(what[b:].strip())
-        return ret
-                    
-
-    def _convValue(self, value, lastItem):
-        # this may be the document ending bracket
-        if lastItem and value[-1]=="}":
-            value = value[:-1]
-        if value in self._stringMap:
-            value = self._stringMap[value]
-        else:
-            value, e = self._tex2html(value)
-            value = value.replace('"', "\\\"")
-            b = value.find("\\")
-            while b>=0:
-                if b<len(value)-1 and value[b+1:b+2]!='\\' and value[b+1:b+2]!='"':
-                    value = value[:b] + '\\' + value[b:]
-                    b = value.find("\\", b+2)
-                else:
-                    b = value.find("\\", b+1)
-        return value
-    
-    
-    def _escaped(self, src, i):
-        if i==0:
-            return False
-        return src[i-1]=='\\'
-
-
-    def _getNext(self, src, i):
-        i1 = src.find("=", i)
-        if i1<0:
-            return "", "", -1, False
-        key = src[i:i1].strip().lower();
-        i1 += 1
-        i2 = i1
-        no = 0
-        odelim = ""
-        cdelim = ""
-        completeValue = ""
-        while True:
-            if not src[i2:i2+1].isspace():
-                if no==0 and odelim=="":
-                    i1 = i2
-                    if src[i2:i2+1]=="{":
-                        odelim = "{"
-                        cdelim = "}"
-                    elif src[i2:i2+1]=='"':
-                        odelim = '"'
-                        cdelim = '"'
-                        i2 += 1
-                    else:
-                        odelim = ","
-                        cdelim = ","
-                        i1 = i1 - 1
-                if src[i2:i2+1]==odelim and (i2==0 or src[i2-1:i2]!="\\"):
-                    no = no + 1
-            if (src[i2:i2+1]=='#' and no==0 and not self._escaped(src, i2)):
-                if DEBUG_SPECIAL_CODING: print ("%s %s %s" % (src[i2-2:i2+2], src[i2-1:i2], self._escaped(src, i2)))
-                value = src[i1+1:i2].strip()
-                completeValue = completeValue + self._convValue(value, cdelim=="," and len(src)==i2)
-                i1 = i2 + 1
-                i2 = i2 + 1
-                if i2>=len(src):
-                    return key, completeValue, i2+1, True
-                no = 0
-                odelim = ""
-                cdelim = ""
-            elif len(src)==i2 or (src[i2:i2+1]==cdelim and (i2==0 or src[i2-1:i2]!="\\")):
-                no = no - 1
-                if len(src)==i2 or no==0:
-                    value = src[i1+1:i2]#.strip()
-                    if odelim=='{':
-                        value = value.strip()
-                    #print "        %s %s" % (value, len(src))
-                    completeValue = completeValue + self._convValue(value, cdelim=="," and len(src)==i2)
-                    while i2<len(src):
-                        i2 = i2 + 1
-                        if src[i2-1]=='#':
-                            break
-                        if src[i2-1]==',' or src[i2-1]=='}':
-                            return key, completeValue, i2+1, True    
-                    if i2==len(src):
-                        return key, completeValue, i2+1, True
-                    no = 0
-                    odelim = ""
-                    cdelim = ""
-            i2 += 1
-
-
-
-    def read2string(self, file, skipComments=True, convertSpaces=True):
-        """Reads the file optionally discarding comments and replacing tabs by spaces
-        
-        Args:
-            file (str): The name of the file to read
-            skipComments (bool): Whether comments shall be removed
-            convertSpaces (bool): Whether tabs shall be converted to spaces
-        
-        Returns:
-            (str): The file contents, optionally stripped and without tabs
-        """
-        fdi = open(file)
-        c = []
-        for l in fdi.readlines():
-            if skipComments:
-                if len(l)>0 and l[0]=='%':
-                    continue
-            c.append(l)
-        fdi.close()
-        c = " ".join(c)
-        if convertSpaces:
-            c = c.replace("\t", " ")
-        return c
-
-
-
-    def parse(self, c, handler):
-        handler.startDocument()
-        b1 = 0
-        while b1<len(c):
-            b1 = c.find("@", b1)
-            if b1<0:
-                break;
-            i1 = c.find("{", b1+1)
-            if i1<0:
-                break;
-            e1 = self._findMatchingBracket(c, i1)
-            e = c[b1+1:e1+1]
-            i1 = e.find("{")
-            b1 = e1
-            entryType = e[:i1].strip()
-            if entryType.lower()=="string" or entryType.lower()=="comment":
-                t = e[i1+1:-1]
-                b = t.find("=")
-                key = t[:b].strip()
-                value = t[b+1:].strip()
-                if value[0]=='"' and value[-1]=='"':
-                    value = value[1:-1]
-                v, e = self._tex2html(value)
-            if entryType.lower()=="string":
-                handler.addStringDefinition(key, v)
-                self._stringMap[key], e = self._tex2html(value)
-                self._stringMapKeys.append(key)
-                self._stringMapKeys.sort(key=lambda x: len(x))
-                self._stringMapKeys.reverse()
-                continue
-            if entryType.lower()=="comment":
-                handler.addComment(key, value)
-                continue
-            i2 = e.find(",", i1)
-            entryID = e[i1+1:i2]
-            print ("%s %s" % (entryID, i1))
-            handler.startEntry(entryID)
-            handler.addField(entryID, "bibtex-type", entryType)
-            haveNext = True
-            i2 += 1
-            while haveNext:
-                key, value, i2, haveNext = self._getNext(e, i2)
-                if haveNext:
-                    hadOne = True
-                    if key=="keywords":
-                        w = self._splitHTMLaware(value)
-                        handler.addField(entryID, key, w)
-                    elif key=="author" or key=="editor":            
-                        value = value.replace(" AND ", " and ")
-                        if value.find(" and ")>=0:
-                            w = value.split(" and ")
-                        else:
-                            w = [ value ]
-                        handler.addField(entryID, key, w)
-                    elif key=="file":
-                        value = value.replace("http//", "http://").replace("http\\:", "http:").replace("http\\\\:", "http:")
-                        a1 = value.find(':')
-                        a2 = value.rfind(':')            
-                        w = [ value[:a1], value[a1+1:a2], value[a2+1:] ]
-                        if len(w)==3 and len(w[1])!=0:# and w[2].lower()=="url":
-                            pairs = []
-                            pairs.append(["name", w[0]])                        
-                            pairs.append(["url", w[1]])                        
-                            handler.addField2(entryID, key, pairs)
-                        else:
-                            hadOne = False
-                    elif key=="year":
-                        a1 = value.find('.')
-                        if a1>=0: value = value[value.rfind(".")+1:]
-                        a1 = value.find('-')
-                        if a1>=0: value = value[:a1]
-                        a1 = value.find('&') # ndash/mdash - should maybe be split so that the information is preserved, but sorting is possible
-                        if a1>=0: value = value[:a1]
-                        year = 0
-                        try: year = int(value)
-                        except: pass
-                        handler.addField(entryID, key, year)
-                    elif key=="pages":
-                        value = value.replace("--", "&ndash;")
-                        value = value.replace("-", "&ndash;")
-                        value = value.replace(" ", "")
-                        handler.addField(entryID, key, value)
-                    else:
-                        handler.addField(entryID, key, value)
-                    if e[i2:i2+1]==",":
-                        i2 += 1
-            handler.closeEntry(entryID)
+from __future__ import print_function
+# ===================================================================
+# bib2x - A BibTex parser and converter.
+#
+# texfile.py - A BibTex-file representation
+#
+# (c) Daniel Krajzewicz 2011-2014, 2022-2023
+# daniel@krajzewicz.de
+# - https://github.com/dkrajzew/bib2x
+# - http://www.krajzewicz.de/docs/bib2x/index.html
+# - http://www.krajzewicz.de
+# 
+# Available under the BSD license.
+# ===================================================================
+
+
+# --- imports -------------------------------------------------------
+import os
+import sys
+import re
+import sqlite3
+
+
+# --- debugging options ---------------------------------------------
+DEBUG_SPECIAL_RECOGNITION = False
+DEBUG_SPECIAL_CODING = False
+DEBUG_UNKNOWN_CMD = False
+
+
+# --- classes -------------------------------------------------------
+class TeXfile:
+    """A class representing a BibTeX file"""
+    
+    def __init__(self):
+        """Initialisation
+        
+        Todo:
+            Extract DB entries and set them up as Python definitions?
+        """
+        self._stringMap = {}
+        self._stringMapKeys = []
+        DB = os.path.join(os.path.dirname(__file__), 'tex.db')
+        conn = sqlite3.connect(DB)
+        cur = conn.cursor()
+        cur.execute('SELECT * FROM styles')
+        self._tex_styles = cur.fetchall()
+        cur.execute('SELECT * FROM stylesp')
+        self._tex_styles_pref = cur.fetchall()
+        cur.execute('SELECT * FROM conv')
+        self._tex_conv = cur.fetchall()
+        cur.execute('SELECT * FROM repl')
+        self._tex_repl = cur.fetchall()
+        
+
+    def _decodeCommand(self, cmd, optArgs, content, ret):
+        if DEBUG_SPECIAL_RECOGNITION: print ("decode: '" + cmd + "/" + content + "'")
+        if cmd=='\\':
+            if DEBUG_SPECIAL_RECOGNITION: print (">!3")
+            return content, False
+        for t in self._tex_styles:
+            if cmd == t[0]:
+                r = str(t[1])
+                r = r.replace("%s", content)
+                r = r.replace("%a", optArgs)
+                if DEBUG_SPECIAL_RECOGNITION: print (">" + r)
+                return r, False
+        for t in self._tex_styles_pref:
+            if cmd == t[0]:
+                if DEBUG_SPECIAL_RECOGNITION: print (">!1")
+                ret["pref"] = True
+                return "", False
+        for t in self._tex_conv:
+            if cmd.startswith(t[0]):
+                r = str(t[1].strip())
+                if DEBUG_SPECIAL_RECOGNITION: print (">" + r + cmd[len(t[0]):])
+                removeSpaces = t[0][1].isalpha()
+                return r + cmd[len(t[0]):], removeSpaces
+        cmd2 = cmd + content
+        for t in self._tex_conv:
+            if cmd2.startswith(t[0]):
+                r = str(t[1].strip())
+                if DEBUG_SPECIAL_RECOGNITION: print (">" + r + cmd2[len(t[0]):])
+                return r + cmd2[len(t[0]):], False
+        ret["unfound"] = True
+        if DEBUG_UNKNOWN_CMD: print ("Unknown cmd '%s'" % cmd)
+        if cmd[0]=='\\':
+            return cmd[1:], False
+        return cmd, False
+        
+
+    def _decodeCommand2(self, cmd, optArgs, content, w, beg, end, currPos):
+        ret = {}
+        r, s = self._decodeCommand(cmd, optArgs, content, ret)
+        if "pref" in ret:
+            for i in self._tex_styles_pref:
+                if cmd==i[0]:
+                    beg = beg + len(cmd)
+                    while w[beg]==' ' or w[beg]=='\n':
+                        beg = beg + 1
+                    r, e = self._tex2html(w, beg, end)
+                    if DEBUG_SPECIAL_RECOGNITION: print ("> " + str(i[1]) + r + str(i[2]))
+                    return str(i[1]) + r + str(i[2]), end
+        if "unfound" in ret and currPos<end-1 and w[currPos]=='\\':
+            cmd = cmd + w[currPos+1:currPos+2]
+            r, s = self._decodeCommand(cmd, optArgs, "", ret)
+            currPos += 2
+        if s:
+            if DEBUG_SPECIAL_RECOGNITION: print ("here's s")
+            currPos = self._skipSpaces(w, currPos)
+        return r, currPos
+        
+    
+    def _findMatchingBracket(self, w, beg, o="{", c="}"):
+        i = beg
+        l = 0
+        while i<len(w):
+            if w[i]==o:
+                l = l + 1
+            if w[i]==c:
+                l = l - 1
+                if l==0:
+                    return i
+            i = i + 1
+        print ("error: Missing closing bracket '%s'" % w[beg:])
+        return len(w)
+        
+        
+    def _skipSpaces(self, w, i):
+        while i<len(w) and w[i].isspace():
+            i = i + 1
+        return i
+
+
+    def _tex2html(self, w, beg=0, end=-1):
+        #print "%s %s %s" % (w, beg, end)
+        i = beg
+        if end<0:
+            end = len(w)
+        else:
+            end = min(len(w), end)
+        r = ""
+        while i<end:
+            if w[i]=='\\':
+                procB = i
+                cmdEnd = -1
+                optArgs = ""
+                i = i + 1
+                e1 = False
+                while i<end and not e1:
+                    if not e1 and w[i]=='[':
+                        # optional parameter
+                        cmdEnd = i
+                        q = self._findMatchingBracket(w, i, "[", "]")
+                        optArgs = ", " + w[i+1:q]
+                        if DEBUG_SPECIAL_CODING: print ("2a: %s %s %s" % (procB, i, optArgs))
+                        i = q + 1
+                    if not e1 and w[i]=='{':
+                        # escaped command, with a bracketed parameter
+                        if DEBUG_SPECIAL_CODING: print ("2: %s %s %s" % (procB, i, w))
+                        q = self._findMatchingBracket(w, i)
+                        dec, e = self._tex2html(w, i+1, q)
+                        if cmdEnd<0: cmdEnd = i
+                        t1, i = self._decodeCommand2(w[procB:cmdEnd].strip(), optArgs, dec, w, beg, end, i)
+                        r = r + t1
+                        i = q + 1
+                        e1 = True                    
+                    if not e1 and w[i]=='|':
+                        # escaped command, with a bracketed parameter
+                        if DEBUG_SPECIAL_CODING: print ("2b: %s %s %s" % (procB, i, w))
+                        q = w.find('|', i+1)
+                        dec, e = self._tex2html(w, i+1, q)
+                        if cmdEnd<0: cmdEnd = i
+                        t1, i = self._decodeCommand2(w[procB:cmdEnd].strip(), optArgs, dec, w, beg, end, i)
+                        r = r + t1
+                        i = q + 1
+                        e1 = True
+                    if not e1 and w[i]=='\\' and i==procB+1:
+                        if DEBUG_SPECIAL_CODING: print ("1b: %s %s %s %s %s" % (procB, i, w, len(w), end))
+                        r = r + "<br/>"
+                        i = self._skipSpaces(w, i + 1)
+                        e1 = True 
+                    if not e1 and (w[i]==' ' or w[i]=='\\' or (i>=procB+2 and not w[i].isalpha() and w[procB+1].isalpha())):
+                        # escaped command, closed by a trailing blank
+                        if DEBUG_SPECIAL_CODING: print ("1: %s %s %s %s %s" % (procB, i, w, len(w), end))
+                        t1, i = self._decodeCommand2(w[procB:i].strip(), optArgs, "", w, beg, end, i)
+                        r = r + t1
+                        e1 = True
+                    if not e1:
+                        i = i + 1
+                if i==end and not e1:
+                    if DEBUG_SPECIAL_CODING: print ("3: %s %s %s %s %s" % (procB, i, w, len(w), end))
+                    t1, i = self._decodeCommand2(w[procB:i].strip(), optArgs, "", w, beg, end, i)
+                    r = r + t1
+            elif w[i]=='{':
+                q = self._findMatchingBracket(w, i)
+                if DEBUG_SPECIAL_CODING: print ("4: %s %s %s" % (i, q, w[i+1:q]))
+                dec, i = self._tex2html(w, i+1, q)
+                if DEBUG_SPECIAL_CODING: print ("t1: %s %s %s %s" % ("hallo", i, w[i-2:i+2], dec))
+                r = r + dec
+                i = q + 1
+                if DEBUG_SPECIAL_CODING: print ("t2: %s %s %s %s %s" % ("hallo", i, w[i-2:i+2], end, r))
+            elif w[i]=='$':
+                q = w.find('$', i+1)
+                if q<0:
+                    print ("unclosed special character $")
+                    q = i
+                if DEBUG_SPECIAL_CODING: print ("5: %s %s %s" % (i, q, w[i+1:q]))
+                dec, i = self._tex2html(w, i+1, q)
+                r = r + dec
+                i = q + 1
+            else:
+                if w[i]=='\n':
+                    r = r + ' '
+                else:
+                    r = r + w[i]                    
+                i = i + 1
+        for t in self._tex_repl:
+            r = r.replace(str(t[0]), str(t[1]))
+        r2 = ""
+        html = False
+        for j in range(0, len(r)):
+            if r[j]=='<':
+                html = True
+            elif r[j]=='>':
+                html = False
+            if r[j]=='"' and not html:
+                r2 = r2 + "&quot;"
+            elif r[j]=="'" and not html:
+                r2 = r2 + "&rsquo;"
+            else:
+                r2 = r2 + r[j]
+        r = r2            
+        r = re.sub("\s+" , " ", r)
+        return r, i    
+                
+
+    def _splitHTMLaware(self, what):
+        """Splits the given string at ';' and ',', assuring that a split
+             is not done if the occured ';' belongs to a HTML-encoded special
+             character
+        
+        Args:
+            what (str): The string to split
+            
+        Returns:
+            (List[str]): The split string
+        """
+        ret = []
+        b = 0
+        isHTML = False
+        for i in range(0, len(what)):
+            if what[i]=='&':
+                isHTML = True
+            if what[i]==',' or (what[i]==';' and not isHTML):
+                ret.append(what[b:i].strip())
+                b = i+1
+            if what[i]==';':
+                isHTML = False
+        ret.append(what[b:].strip())
+        return ret
+                    
+
+    def _convValue(self, value, lastItem):
+        # this may be the document ending bracket
+        if lastItem and value[-1]=="}":
+            value = value[:-1]
+        if value in self._stringMap:
+            value = self._stringMap[value]
+        else:
+            value, e = self._tex2html(value)
+            value = value.replace('"', "\\\"")
+            b = value.find("\\")
+            while b>=0:
+                if b<len(value)-1 and value[b+1:b+2]!='\\' and value[b+1:b+2]!='"':
+                    value = value[:b] + '\\' + value[b:]
+                    b = value.find("\\", b+2)
+                else:
+                    b = value.find("\\", b+1)
+        return value
+    
+    
+    def _escaped(self, src, i):
+        if i==0:
+            return False
+        return src[i-1]=='\\'
+
+
+    def _getNext(self, src, i):
+        i1 = src.find("=", i)
+        if i1<0:
+            return "", "", -1, False
+        key = src[i:i1].strip().lower();
+        i1 += 1
+        i2 = i1
+        no = 0
+        odelim = ""
+        cdelim = ""
+        completeValue = ""
+        while True:
+            if not src[i2:i2+1].isspace():
+                if no==0 and odelim=="":
+                    i1 = i2
+                    if src[i2:i2+1]=="{":
+                        odelim = "{"
+                        cdelim = "}"
+                    elif src[i2:i2+1]=='"':
+                        odelim = '"'
+                        cdelim = '"'
+                        i2 += 1
+                    else:
+                        odelim = ","
+                        cdelim = ","
+                        i1 = i1 - 1
+                if src[i2:i2+1]==odelim and (i2==0 or src[i2-1:i2]!="\\"):
+                    no = no + 1
+            if (src[i2:i2+1]=='#' and no==0 and not self._escaped(src, i2)):
+                if DEBUG_SPECIAL_CODING: print ("%s %s %s" % (src[i2-2:i2+2], src[i2-1:i2], self._escaped(src, i2)))
+                value = src[i1+1:i2].strip()
+                completeValue = completeValue + self._convValue(value, cdelim=="," and len(src)==i2)
+                i1 = i2 + 1
+                i2 = i2 + 1
+                if i2>=len(src):
+                    return key, completeValue, i2+1, True
+                no = 0
+                odelim = ""
+                cdelim = ""
+            elif len(src)==i2 or (src[i2:i2+1]==cdelim and (i2==0 or src[i2-1:i2]!="\\")):
+                no = no - 1
+                if len(src)==i2 or no==0:
+                    value = src[i1+1:i2]#.strip()
+                    if odelim=='{':
+                        value = value.strip()
+                    #print "        %s %s" % (value, len(src))
+                    completeValue = completeValue + self._convValue(value, cdelim=="," and len(src)==i2)
+                    while i2<len(src):
+                        i2 = i2 + 1
+                        if src[i2-1]=='#':
+                            break
+                        if src[i2-1]==',' or src[i2-1]=='}':
+                            return key, completeValue, i2+1, True    
+                    if i2==len(src):
+                        return key, completeValue, i2+1, True
+                    no = 0
+                    odelim = ""
+                    cdelim = ""
+            i2 += 1
+
+
+
+    def read2string(self, file, skipComments=True, convertSpaces=True):
+        """Reads the file optionally discarding comments and replacing tabs by spaces
+        
+        Args:
+            file (str): The name of the file to read
+            skipComments (bool): Whether comments shall be removed
+            convertSpaces (bool): Whether tabs shall be converted to spaces
+        
+        Returns:
+            (str): The file contents, optionally stripped and without tabs
+        """
+        fdi = open(file)
+        c = []
+        for l in fdi.readlines():
+            if skipComments:
+                if len(l)>0 and l[0]=='%':
+                    continue
+            c.append(l)
+        fdi.close()
+        c = " ".join(c)
+        if convertSpaces:
+            c = c.replace("\t", " ")
+        return c
+
+
+
+    def parse(self, c, handler):
+        handler.startDocument()
+        b1 = 0
+        while b1<len(c):
+            b1 = c.find("@", b1)
+            if b1<0:
+                break;
+            i1 = c.find("{", b1+1)
+            if i1<0:
+                break;
+            e1 = self._findMatchingBracket(c, i1)
+            e = c[b1+1:e1+1]
+            i1 = e.find("{")
+            b1 = e1
+            entryType = e[:i1].strip()
+            if entryType.lower()=="string" or entryType.lower()=="comment":
+                t = e[i1+1:-1]
+                b = t.find("=")
+                key = t[:b].strip()
+                value = t[b+1:].strip()
+                if value[0]=='"' and value[-1]=='"':
+                    value = value[1:-1]
+                v, e = self._tex2html(value)
+            if entryType.lower()=="string":
+                handler.addStringDefinition(key, v)
+                self._stringMap[key], e = self._tex2html(value)
+                self._stringMapKeys.append(key)
+                self._stringMapKeys.sort(key=lambda x: len(x))
+                self._stringMapKeys.reverse()
+                continue
+            if entryType.lower()=="comment":
+                handler.addComment(key, value)
+                continue
+            i2 = e.find(",", i1)
+            entryID = e[i1+1:i2]
+            print ("%s %s" % (entryID, i1))
+            handler.startEntry(entryID)
+            handler.addField(entryID, "bibtex-type", entryType)
+            haveNext = True
+            i2 += 1
+            while haveNext:
+                key, value, i2, haveNext = self._getNext(e, i2)
+                if haveNext:
+                    hadOne = True
+                    if key=="keywords":
+                        w = self._splitHTMLaware(value)
+                        handler.addField(entryID, key, w)
+                    elif key=="author" or key=="editor":            
+                        value = value.replace(" AND ", " and ")
+                        if value.find(" and ")>=0:
+                            w = value.split(" and ")
+                        else:
+                            w = [ value ]
+                        handler.addField(entryID, key, w)
+                    elif key=="file":
+                        value = value.replace("http//", "http://").replace("http\\:", "http:").replace("http\\\\:", "http:")
+                        a1 = value.find(':')
+                        a2 = value.rfind(':')            
+                        w = [ value[:a1], value[a1+1:a2], value[a2+1:] ]
+                        if len(w)==3 and len(w[1])!=0:# and w[2].lower()=="url":
+                            pairs = []
+                            pairs.append(["name", w[0]])                        
+                            pairs.append(["url", w[1]])                        
+                            handler.addField2(entryID, key, pairs)
+                        else:
+                            hadOne = False
+                    elif key=="year":
+                        a1 = value.find('.')
+                        if a1>=0: value = value[value.rfind(".")+1:]
+                        a1 = value.find('-')
+                        if a1>=0: value = value[:a1]
+                        a1 = value.find('&') # ndash/mdash - should maybe be split so that the information is preserved, but sorting is possible
+                        if a1>=0: value = value[:a1]
+                        year = 0
+                        try: year = int(value)
+                        except: pass
+                        handler.addField(entryID, key, year)
+                    elif key=="pages":
+                        value = value.replace("--", "&ndash;")
+                        value = value.replace("-", "&ndash;")
+                        value = value.replace(" ", "")
+                        handler.addField(entryID, key, value)
+                    else:
+                        handler.addField(entryID, key, value)
+                    if e[i2:i2+1]==",":
+                        i2 += 1
+            handler.closeEntry(entryID)
         handler.endDocument()
```

### Comparing `bib2x-0.4.0/bib2x/texhandler/html.py` & `bib2x-0.4.2/bib2x/texhandler/html.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,179 +1,179 @@
-from __future__ import print_function
-# ===================================================================
-# bib2x - A BibTex parser and converter.
-#
-# html.py - A HTML exporting BibTeX handler
-#
-# (c) Daniel Krajzewicz 2011-2014, 2022-2023
-# daniel@krajzewicz.de
-# - https://github.com/dkrajzew/bib2x
-# - http://www.krajzewicz.de/docs/bib2x/index.html
-# - http://www.krajzewicz.de
-# 
-# Available under the BSD license.
-# ===================================================================
-
-
-# --- format definitions --------------------------------------------
-formats = {
-    "periodical":       "<b>%title%</b>, ?month:%month% ?%year%.",
-    "article":          "%authorREP%. <b>%title%</b>. <i>%journal%</i>?, volume:%volume%??, number:(%number%)??, pages::%pages%??, month:%month%? %year%.",
-    "book":             "%authorREP%. <b>%title%</b>?volume:, volume %volume%??series: of %series%?. %publisher%?address:, %address%??edition:, %edition% edition?, ?month:%month% ?%year%.",
-    "booklet":          "%authorREP%. <b>%title%</b>. ?howpublished:%howpublished%, ??address: %address%, ??month:%month% ?%year%.",
-    "conference":       "%authorREP%. <b>%title%</b>. In: ?editor:%editorREP%, editor, ?<i>%booktitle%</i>?volume:, volume %volume%??series: of %series%??pages:, pages %pages%??address:, %address%?, ?month:%month% ?%year%. ?organization:%organization%, ??publisher:%publisher%?.",
-    "electronic":       "%authorREP%. <b>%title%</b>. ?howpublished:%howpublished%, ??month:%month% ?%year%.",
-    "inbook":           "%authorREP%. <b>%title%</b>?volume:, volume %volume%??series: of %series%??type:, %type%??chapter: %chapter%??pages:, %pages%??publisher:, %publisher%??address:, %address%??edition:, %edition% edition?, ?month:%month% ?%year%.",
-    "incollection":     "%authorREP%. <b>%title%</b>. In: ?editor:%editorREP%, editor, ?<i>%booktitle%</i>?volume:, volume %volume%??series: of %series%??type:, %type%??chapter: %chapter%??pages:, %pages%?.?publisher: %publisher%??address:, %address%??edition:, %edition% edition?, ?month:%month% ?%year%.",
-    "inproceedings":    "%authorREP%. <b>%title%</b>. In: ?editor:%editorREP%, editor, ?<i>%booktitle%</i>?volume:, volume %volume%??series: of %series%??pages:, %pages%??address:, %address%?, ?month:%month% ?%year%. ?organization:%organization%, ??publisher:%publisher%.?",
-    "manual":           "%authorREP%. <b>%title%</b>. ?organization:%organization%??address:, %address%??edition:, %edition% edition?, ?month:%month% ?%year%.",
-    "mastersthesis":    "%authorREP%. <b>%title%</b>. ?type:%type%, ?%school%?address:, %address%?, ?month:%month% ?%year%.",
-    "misc":             "%authorREP%. <b>%title%</b>. ?howpublished:%howpublished%, ??month:%month% ?%year%.",
-    "patent":           "%authorREP%. <b>%title%</b>. %year%.",
-    "phdthesis":        "%authorREP%. <b>%title%</b>. ?type:%type%, ?%school%?address:, %address%?, ?month:%month% ?%year%.",
-    "proceedings":      "%editorREP%, editor. <b>%title%</b>?volume:, volume %volume%??series: of %series%??pages:, %pages%??address:, %address%?, ?month:%month% ?%year%. ?organization:%organization%, ??publisher:%publisher%?.",
-    "standard":         "%authorREP%. <b>%title%</b>. ?howpublished:%howpublished%, ??month:%month% ?%year%.",
-    "techreport":       "%authorREP%. <b>%title%</b>. ?type:%type%??number: %number%??type:, ??institution:%institution%, ??address:%address%, ??month:%month% ?%year%.",
-    "unpublished":      "%authorREP%. <b>%title%</b>. ?month:%month% ?%year%."
-}
-
-
-# --- classes -------------------------------------------------------
-class HTMLexportingTeXhandler:
-    """A BibTex handler that exports entries as HTML."""
-
-    def __init__(self, fdo):
-        """Constructor
-        
-        Args:
-            fdo (file descriptor): The file to write to
-        """
-        self._fdo = fdo
-        self._stringMap = {}
-        self._currentBibTeXKey = None
-        self._currentAttrs = {}
-    
-    
-    def startDocument(self):
-        """Called at the begin of a document's processing"""
-        self._fdo.write("<ul>\n")
-    
-    
-    def addStringDefinition(self, key, value):
-        """Adds the definition of a string
-        
-        Args:
-            key (str): The shortcut for the string.
-            value (str): The value of the string.
-        """
-        self._stringMap[key] = value
-        
-    
-    def addComment(self, key, value):
-        """Adds a comment
-        
-        Args:
-            key (str): The name of the comment?
-            value (str): The value of the comment
-        
-        todo: Check semantics
-        """
-        pass
-
-    
-    def startEntry(self, entryID):
-        """Called if a new entry is started to being parsed.
-        
-        Args:
-            entryID (str): The ID (key) of the entry
-        """
-        self._currentBibTeXKey = entryID
-        self._currentAttrs = {}
-
-
-    def addField(self, entryID, key, value):
-        """Called if a new attribute of an entry shall be added.
-        
-        Args:
-            entryID (str): The ID (key) of the entry
-            key (str): The name of the attribute
-            value (str): The value of the attribute
-        """
-        self._currentAttrs[key] = value
-
-
-    def addField2(self, entryID, key, pairs):
-        """Called if a new attribute consisting of multiple named fields shall be added.
-        
-        This is only used when parsing JabRef file-fields.
-        
-        Args:
-            entryID (str): The ID (key) of the entry
-            key (str): The name of the attribute
-            pairs (List[Tuple[str, str]]): The value of the attribute
-        """
-        self._currentAttrs[key] = pairs
-
-
-    def fillTemplate(self, tpl, fields):
-        """Parses the template and fills it with the given values
-        
-        Args:
-            tpl (str): The entry-type specific template to fill
-            fields (dict): The dictionary of the entry's attributes
-        """
-        ret = ""
-        tmp = ""
-        isOpt = False
-        hadAll = False
-        i = 0
-        while i<len(tpl):
-            if tpl[i]=='?':
-                if isOpt:
-                    isOpt = False
-                    if hadAll:
-                        ret += tmp
-                else:
-                    isOpt = True
-                    hadAll = True
-                    tmp = ""
-            elif tpl[i]=='%':
-                b = i + 1
-                e = b
-                while tpl[e]!="%" and e<len(tpl):
-                    e += 1
-                k = tpl[b:e]
-                if k not in fields:
-                    hadAll = False
-                    if not isOpt:
-                        print ("Missing required attribute '%s' in %s" % (k, self._currentBibTeXKey))
-                elif isOpt:
-                    tmp += str(fields[k])
-                else:
-                    ret += str(fields[k])
-                i = e
-            elif isOpt:
-                tmp += tpl[i]
-            else:
-                ret += tpl[i]
-            i += 1
-        return ret
-
-
-    def closeEntry(self, entryID):
-        """Closes the entry
-        
-        Args:
-            entryID (str): The ID (key) of the entry
-        """
-        bibtexType = "article" if "bibtex-type" not in self._currentAttrs else self._currentAttrs["bibtex-type"].lower()
-        self._currentAttrs["authorREP"] = ", ".join(self._currentAttrs["author"]) if "author" in self._currentAttrs else ""
-        self._currentAttrs["editorREP"] = ", ".join(self._currentAttrs["editor"]) if "editor" in self._currentAttrs else ""
-        tpl = formats[bibtexType]
-        ret = "<li>" + self.fillTemplate(tpl, self._currentAttrs) + "</li>\n"
-        self._fdo.write(ret)
-
-
-    def endDocument(self):
-        """Called after parsing a document"""
-        self._fdo.write("</ul>\n")
+from __future__ import print_function
+# ===================================================================
+# bib2x - A BibTex parser and converter.
+#
+# html.py - A HTML exporting BibTeX handler
+#
+# (c) Daniel Krajzewicz 2011-2014, 2022-2023
+# daniel@krajzewicz.de
+# - https://github.com/dkrajzew/bib2x
+# - http://www.krajzewicz.de/docs/bib2x/index.html
+# - http://www.krajzewicz.de
+# 
+# Available under the BSD license.
+# ===================================================================
+
+
+# --- format definitions --------------------------------------------
+formats = {
+    "periodical":       "<b>%title%</b>, ?month:%month% ?%year%.",
+    "article":          "%authorREP%. <b>%title%</b>. <i>%journal%</i>?, volume:%volume%??, number:(%number%)??, pages::%pages%??, month:%month%? %year%.",
+    "book":             "%authorREP%. <b>%title%</b>?volume:, volume %volume%??series: of %series%?. %publisher%?address:, %address%??edition:, %edition% edition?, ?month:%month% ?%year%.",
+    "booklet":          "%authorREP%. <b>%title%</b>. ?howpublished:%howpublished%, ??address: %address%, ??month:%month% ?%year%.",
+    "conference":       "%authorREP%. <b>%title%</b>. In: ?editor:%editorREP%, editor, ?<i>%booktitle%</i>?volume:, volume %volume%??series: of %series%??pages:, pages %pages%??address:, %address%?, ?month:%month% ?%year%. ?organization:%organization%, ??publisher:%publisher%?.",
+    "electronic":       "%authorREP%. <b>%title%</b>. ?howpublished:%howpublished%, ??month:%month% ?%year%.",
+    "inbook":           "%authorREP%. <b>%title%</b>?volume:, volume %volume%??series: of %series%??type:, %type%??chapter: %chapter%??pages:, %pages%??publisher:, %publisher%??address:, %address%??edition:, %edition% edition?, ?month:%month% ?%year%.",
+    "incollection":     "%authorREP%. <b>%title%</b>. In: ?editor:%editorREP%, editor, ?<i>%booktitle%</i>?volume:, volume %volume%??series: of %series%??type:, %type%??chapter: %chapter%??pages:, %pages%?.?publisher: %publisher%??address:, %address%??edition:, %edition% edition?, ?month:%month% ?%year%.",
+    "inproceedings":    "%authorREP%. <b>%title%</b>. In: ?editor:%editorREP%, editor, ?<i>%booktitle%</i>?volume:, volume %volume%??series: of %series%??pages:, %pages%??address:, %address%?, ?month:%month% ?%year%. ?organization:%organization%, ??publisher:%publisher%.?",
+    "manual":           "%authorREP%. <b>%title%</b>. ?organization:%organization%??address:, %address%??edition:, %edition% edition?, ?month:%month% ?%year%.",
+    "mastersthesis":    "%authorREP%. <b>%title%</b>. ?type:%type%, ?%school%?address:, %address%?, ?month:%month% ?%year%.",
+    "misc":             "%authorREP%. <b>%title%</b>. ?howpublished:%howpublished%, ??month:%month% ?%year%.",
+    "patent":           "%authorREP%. <b>%title%</b>. %year%.",
+    "phdthesis":        "%authorREP%. <b>%title%</b>. ?type:%type%, ?%school%?address:, %address%?, ?month:%month% ?%year%.",
+    "proceedings":      "%editorREP%, editor. <b>%title%</b>?volume:, volume %volume%??series: of %series%??pages:, %pages%??address:, %address%?, ?month:%month% ?%year%. ?organization:%organization%, ??publisher:%publisher%?.",
+    "standard":         "%authorREP%. <b>%title%</b>. ?howpublished:%howpublished%, ??month:%month% ?%year%.",
+    "techreport":       "%authorREP%. <b>%title%</b>. ?type:%type%??number: %number%??type:, ??institution:%institution%, ??address:%address%, ??month:%month% ?%year%.",
+    "unpublished":      "%authorREP%. <b>%title%</b>. ?month:%month% ?%year%."
+}
+
+
+# --- classes -------------------------------------------------------
+class HTMLexportingTeXhandler:
+    """A BibTex handler that exports entries as HTML."""
+
+    def __init__(self, fdo):
+        """Constructor
+        
+        Args:
+            fdo (file descriptor): The file to write to
+        """
+        self._fdo = fdo
+        self._stringMap = {}
+        self._currentBibTeXKey = None
+        self._currentAttrs = {}
+    
+    
+    def startDocument(self):
+        """Called at the begin of a document's processing"""
+        self._fdo.write("<ul>\n")
+    
+    
+    def addStringDefinition(self, key, value):
+        """Adds the definition of a string
+        
+        Args:
+            key (str): The shortcut for the string.
+            value (str): The value of the string.
+        """
+        self._stringMap[key] = value
+        
+    
+    def addComment(self, key, value):
+        """Adds a comment
+        
+        Args:
+            key (str): The name of the comment?
+            value (str): The value of the comment
+        
+        todo: Check semantics
+        """
+        pass
+
+    
+    def startEntry(self, entryID):
+        """Called if a new entry is started to being parsed.
+        
+        Args:
+            entryID (str): The ID (key) of the entry
+        """
+        self._currentBibTeXKey = entryID
+        self._currentAttrs = {}
+
+
+    def addField(self, entryID, key, value):
+        """Called if a new attribute of an entry shall be added.
+        
+        Args:
+            entryID (str): The ID (key) of the entry
+            key (str): The name of the attribute
+            value (str): The value of the attribute
+        """
+        self._currentAttrs[key] = value
+
+
+    def addField2(self, entryID, key, pairs):
+        """Called if a new attribute consisting of multiple named fields shall be added.
+        
+        This is only used when parsing JabRef file-fields.
+        
+        Args:
+            entryID (str): The ID (key) of the entry
+            key (str): The name of the attribute
+            pairs (List[Tuple[str, str]]): The value of the attribute
+        """
+        self._currentAttrs[key] = pairs
+
+
+    def fillTemplate(self, tpl, fields):
+        """Parses the template and fills it with the given values
+        
+        Args:
+            tpl (str): The entry-type specific template to fill
+            fields (dict): The dictionary of the entry's attributes
+        """
+        ret = ""
+        tmp = ""
+        isOpt = False
+        hadAll = False
+        i = 0
+        while i<len(tpl):
+            if tpl[i]=='?':
+                if isOpt:
+                    isOpt = False
+                    if hadAll:
+                        ret += tmp
+                else:
+                    isOpt = True
+                    hadAll = True
+                    tmp = ""
+            elif tpl[i]=='%':
+                b = i + 1
+                e = b
+                while tpl[e]!="%" and e<len(tpl):
+                    e += 1
+                k = tpl[b:e]
+                if k not in fields:
+                    hadAll = False
+                    if not isOpt:
+                        print ("Missing required attribute '%s' in %s" % (k, self._currentBibTeXKey))
+                elif isOpt:
+                    tmp += str(fields[k])
+                else:
+                    ret += str(fields[k])
+                i = e
+            elif isOpt:
+                tmp += tpl[i]
+            else:
+                ret += tpl[i]
+            i += 1
+        return ret
+
+
+    def closeEntry(self, entryID):
+        """Closes the entry
+        
+        Args:
+            entryID (str): The ID (key) of the entry
+        """
+        bibtexType = "article" if "bibtex-type" not in self._currentAttrs else self._currentAttrs["bibtex-type"].lower()
+        self._currentAttrs["authorREP"] = ", ".join(self._currentAttrs["author"]) if "author" in self._currentAttrs else ""
+        self._currentAttrs["editorREP"] = ", ".join(self._currentAttrs["editor"]) if "editor" in self._currentAttrs else ""
+        tpl = formats[bibtexType]
+        ret = "<li>" + self.fillTemplate(tpl, self._currentAttrs) + "</li>\n"
+        self._fdo.write(ret)
+
+
+    def endDocument(self):
+        """Called after parsing a document"""
+        self._fdo.write("</ul>\n")
```

### Comparing `bib2x-0.4.0/bib2x/texhandler/json.py` & `bib2x-0.4.2/bib2x/texhandler/json.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,151 +1,151 @@
-from __future__ import print_function
-# ===================================================================
-# bib2x - A BibTex parser and converter.
-#
-# json.py - A JSON exporting BibTeX handler
-#
-# (c) Daniel Krajzewicz 2011-2014, 2022-2023
-# daniel@krajzewicz.de
-# - https://github.com/dkrajzew/bib2x
-# - http://www.krajzewicz.de/docs/bib2x/index.html
-# - http://www.krajzewicz.de
-# 
-# Available under the BSD license.
-# ===================================================================
-
-
-# --- imports -------------------------------------------------------
-import os
-import sys
-sys.path.append(os.path.dirname(os.path.realpath(__file__)))
-
-import re
-import sqlite3
-try: from . import handler
-except: import handler
-
-
-# --- classes -------------------------------------------------------
-class JSONexportingTeXhandler(handler.BibTeXhandler):
-    """A BibTex handler that exports entries as JSON."""
-
-    def __init__(self, fdo):
-        """Constructor
-        
-        Args:
-            fdo (file descriptor): The file to write to
-        """
-        self._fdo = fdo
-        self._entry = ""
-        self._firstEntry = True
-        self._hadOne = False
-
-
-    def startDocument(self):
-        """Called at the begin of a document's processing"""
-        self._fdo.write("var bib={\n \"entries\":{\n")
-        pass
-    
-    
-    def addStringDefinition(self, key, value):
-        """Adds the definition of a string
-        
-        This implementation does nothing.
-        
-        Args:
-            key (str): The shortcut for the string
-            value (str): The value of the string
-        
-        Todo: 
-            check whether string definition should not be saved
-        """
-        pass
-        
-    
-    def addComment(self, key, value):
-        """Adds a comment
-        
-        This implementation does nothing.
-        
-        Args:
-            key (str): The name of the comment?
-            value (str): The value of the comment
-        """
-        pass
-
-    
-    def startEntry(self, entryID):
-        """Called if a new entry is started to being parsed.
-
-        Begins entry encoding by generating a named JSON map.
-        
-        Args:
-            entryID (str): The ID (key) of the entry
-        """
-        self._hadOne = False
-        self._entry = ""
-        self._entry = self._entry + '  "%s":{\n' % entryID
-
-
-    def addField(self, entryID, key, value):
-        """Called if a new attribute of an entry shall be added.
-        
-        Appends the attribute encoded as JSON to the current item's
-        definition.
-        
-        Args:
-            entryID (str): The ID (key) of the entry
-            key (str): The name of the attribute
-            value (str): The value of the attribute
-        """
-        if self._hadOne:
-            self._entry = self._entry + ",\n"
-        if isinstance(value, int):
-            self._entry = self._entry + '   "%s":%s' % (key, value)
-        elif isinstance(value, list):
-            self._entry = self._entry + '   "%s":%s' % (key, value)
-        else:
-            self._entry = self._entry + '   "%s":"%s"' % (key, value)
-        self._hadOne = True
-        
-
-    def addField2(self, entryID, key, pairs):
-        """Called if a new attribute consisting of multiple named fields shall be added.
-        
-        Opens a new attribute with the given name and appends
-        the pairs as key/value JSON objects inside it.
-        
-        Args:
-            entryID (str): The ID (key) of the entry
-            key (str): The name of the attribute
-            pairs (List[Tuple[str, str]]): The value of the attribute
-        """
-        if self._hadOne:
-            self._entry = self._entry + ",\n"
-        self._entry = self._entry + '   "%s":{' % (key)
-        r = []
-        for p in pairs:
-            r.append('"%s":"%s"' % (p[0], p[1]))
-        self._entry = self._entry + ",".join(r)
-        self._entry = self._entry + '}'
-        self._hadOne = True
-
-
-    def closeEntry(self, entryID):
-        """Closes the entry
-        
-        Args:
-            entryID (str): The ID (key) of the entry
-        """
-        if not self._firstEntry:
-            self._entry = ",\n" + self._entry
-        else:
-            self._firstEntry = False
-        self._entry = self._entry + "\n  }" 
-        self._fdo.write(self._entry) 
-
-
-    def endDocument(self):
-        """Called after parsing a document"""
-        self._fdo.write("\n }\n};\n")
-        
+from __future__ import print_function
+# ===================================================================
+# bib2x - A BibTex parser and converter.
+#
+# json.py - A JSON exporting BibTeX handler
+#
+# (c) Daniel Krajzewicz 2011-2014, 2022-2023
+# daniel@krajzewicz.de
+# - https://github.com/dkrajzew/bib2x
+# - http://www.krajzewicz.de/docs/bib2x/index.html
+# - http://www.krajzewicz.de
+# 
+# Available under the BSD license.
+# ===================================================================
+
+
+# --- imports -------------------------------------------------------
+import os
+import sys
+sys.path.append(os.path.dirname(os.path.realpath(__file__)))
+
+import re
+import sqlite3
+try: from . import handler
+except: import handler
+
+
+# --- classes -------------------------------------------------------
+class JSONexportingTeXhandler(handler.BibTeXhandler):
+    """A BibTex handler that exports entries as JSON."""
+
+    def __init__(self, fdo):
+        """Constructor
+        
+        Args:
+            fdo (file descriptor): The file to write to
+        """
+        self._fdo = fdo
+        self._entry = ""
+        self._firstEntry = True
+        self._hadOne = False
+
+
+    def startDocument(self):
+        """Called at the begin of a document's processing"""
+        self._fdo.write("var bib={\n \"entries\":{\n")
+        pass
+    
+    
+    def addStringDefinition(self, key, value):
+        """Adds the definition of a string
+        
+        This implementation does nothing.
+        
+        Args:
+            key (str): The shortcut for the string
+            value (str): The value of the string
+        
+        Todo: 
+            check whether string definition should not be saved
+        """
+        pass
+        
+    
+    def addComment(self, key, value):
+        """Adds a comment
+        
+        This implementation does nothing.
+        
+        Args:
+            key (str): The name of the comment?
+            value (str): The value of the comment
+        """
+        pass
+
+    
+    def startEntry(self, entryID):
+        """Called if a new entry is started to being parsed.
+
+        Begins entry encoding by generating a named JSON map.
+        
+        Args:
+            entryID (str): The ID (key) of the entry
+        """
+        self._hadOne = False
+        self._entry = ""
+        self._entry = self._entry + '  "%s":{\n' % entryID
+
+
+    def addField(self, entryID, key, value):
+        """Called if a new attribute of an entry shall be added.
+        
+        Appends the attribute encoded as JSON to the current item's
+        definition.
+        
+        Args:
+            entryID (str): The ID (key) of the entry
+            key (str): The name of the attribute
+            value (str): The value of the attribute
+        """
+        if self._hadOne:
+            self._entry = self._entry + ",\n"
+        if isinstance(value, int):
+            self._entry = self._entry + '   "%s":%s' % (key, value)
+        elif isinstance(value, list):
+            self._entry = self._entry + '   "%s":%s' % (key, value)
+        else:
+            self._entry = self._entry + '   "%s":"%s"' % (key, value)
+        self._hadOne = True
+        
+
+    def addField2(self, entryID, key, pairs):
+        """Called if a new attribute consisting of multiple named fields shall be added.
+        
+        Opens a new attribute with the given name and appends
+        the pairs as key/value JSON objects inside it.
+        
+        Args:
+            entryID (str): The ID (key) of the entry
+            key (str): The name of the attribute
+            pairs (List[Tuple[str, str]]): The value of the attribute
+        """
+        if self._hadOne:
+            self._entry = self._entry + ",\n"
+        self._entry = self._entry + '   "%s":{' % (key)
+        r = []
+        for p in pairs:
+            r.append('"%s":"%s"' % (p[0], p[1]))
+        self._entry = self._entry + ",".join(r)
+        self._entry = self._entry + '}'
+        self._hadOne = True
+
+
+    def closeEntry(self, entryID):
+        """Closes the entry
+        
+        Args:
+            entryID (str): The ID (key) of the entry
+        """
+        if not self._firstEntry:
+            self._entry = ",\n" + self._entry
+        else:
+            self._firstEntry = False
+        self._entry = self._entry + "\n  }" 
+        self._fdo.write(self._entry) 
+
+
+    def endDocument(self):
+        """Called after parsing a document"""
+        self._fdo.write("\n }\n};\n")
+
```

### Comparing `bib2x-0.4.0/bib2x/texhandler/memory.py` & `bib2x-0.4.2/bib2x/texhandler/memory.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,166 +1,166 @@
-from __future__ import print_function
-# ===================================================================
-# bib2x - A BibTex parser and converter.
-#
-# memory.py - A BibTeX handler keeping the contents in memory
-#
-# (c) Daniel Krajzewicz 2011-2014, 2022-2023
-# daniel@krajzewicz.de
-# - https://github.com/dkrajzew/bib2x
-# - http://www.krajzewicz.de/docs/bib2x/index.html
-# - http://www.krajzewicz.de
-# 
-# Available under the BSD license.
-# ===================================================================
-
-
-# --- imports -------------------------------------------------------
-import os
-import sys
-sys.path.append(os.path.dirname(os.path.realpath(__file__)))
-
-import re
-import sqlite3
-try: from . import handler
-except: import handler
-
-
-# --- classes -------------------------------------------------------
-class StoringTeXhandler(handler.BibTeXhandler):
-    """A BibTeX handler keeping the entries in memory"""
-    
-    def __init__(self):
-        """Constructor
-        """
-        self._entries = {}
-        self._entryIDs = []
-        self._stringMap = {}
-        self._stringMapKeys = []
-    
-        self._groupNames = []
-        self._groups = {}
-
-    
-    def startDocument(self):
-        """Called at the begin of a document's processing"""
-        pass
-    
-    
-    def addStringDefinition(self, key, value):
-        """Adds the definition of a string
-
-        Stores the definition in the self._stringMap dictionary.
-        
-        Args:
-            key (str): The shortcut for the string.
-            value (str): The value of the string.
-        
-        Todo: 
-            Remove self._stringMapKeys
-        """
-        self._stringMap[key] = value
-        self._stringMapKeys.append(key)
-
-    
-    def addComment(self, key, value):
-        """Adds a comment
-        
-        This implementation is somehow "magic" as it targets
-        parsing JabRef comments that contain a group assignment.
-        
-        Args:
-            key (str): The name of the comment?
-            value (str): The value of the comment.
-        
-        Todo: 
-            Extract JabRef-parsing.
-        """
-        if not value.strip().startswith("jabref-meta: groupstree"):
-            return
-        value = value[value.find("0"):]
-        lines = value.split("\n")
-        c = ""
-        tree = []
-        lastLevel = 0
-        for l in lines:
-            c = c + l.strip()
-            i = c.rfind(";")
-            #print "%s %s %s %s" % (i, len(c)-1, c[i-2], c[i-2-5:])
-            if i==len(c)-1 and len(c)>2 and c[i-1]!='\\':
-                d = c[:c.find("\\;")].strip()
-                level = int(d[:d.find(" ")])
-                name = d[d.find(":")+1:]
-                if level<=lastLevel:
-                    tree = tree[:-(lastLevel - level + 1)]
-                lastLevel = level
-                tree.append(name)
-        
-                if level!=0:
-                    d = c[c.find(";")+1:].strip()
-                    d = d[d.find(";")+1:d.rfind(";")]
-                    items = filter(None, d.split("\;"))
-                    gName = "/".join(tree)
-                    if gName not in self._groupNames:
-                        self._groupNames.append(gName)
-                    if gName not in self._groups:
-                        self._groups[gName] = []
-                    self._groups[gName].extend(items)
-                #print "------------\n" + c[:20]
-                c = ""
-    
-    
-    def startEntry(self, entryID):
-        """Called if a new entry is started to being parsed.
-
-        Begins entry by storing it in internal containers.
-        
-        Args:
-            entryID (str): The ID (key) of the entry
-        """
-        self._entries[entryID] = {}
-        self._entryIDs.append(entryID)
-
-
-    def addField(self, entryID, key, value):
-        """Called if a new attribute of an entry shall be added.
-        
-        Stores the attribute in the self._entries[entryID] dictionary.
-        
-        Args:
-            entryID (str): The ID (key) of the entry
-            key (str): The name of the attribute
-            value (str): The value of the attribute
-        """
-        self._entries[entryID][key] = value
-
-
-    def addField2(self, entryID, key, pairs):
-        """Called if a new attribute consisting of multiple named fields shall be added.
-        
-        Allocates a dictionary entry in self._entries[entryID] with the given key.
-        Inserts the given pairs as key/values into this dictionary.
-        
-        Args:
-            entryID (str): The ID (key) of the entry
-            key (str): The name of the attribute
-            pairs (List[Tuple[str, str]]): The value of the attribute
-        """
-        if ukey not in self._entries[entryID]:
-            self._entries[entryID][key] = {}
-        for p in pairs:
-            self._entries[entryID][key][p[0]] = p[1]
-
-    
-    def closeEntry(self, entryID):
-        """Closes the entry
-        
-        Args:
-            entryID (str): The ID (key) of the entry
-        """
-        pass
-
-
-    def endDocument(self):
-        """Called after parsing a document"""
-        pass
-        
+from __future__ import print_function
+# ===================================================================
+# bib2x - A BibTex parser and converter.
+#
+# memory.py - A BibTeX handler keeping the contents in memory
+#
+# (c) Daniel Krajzewicz 2011-2014, 2022-2023
+# daniel@krajzewicz.de
+# - https://github.com/dkrajzew/bib2x
+# - http://www.krajzewicz.de/docs/bib2x/index.html
+# - http://www.krajzewicz.de
+# 
+# Available under the BSD license.
+# ===================================================================
+
+
+# --- imports -------------------------------------------------------
+import os
+import sys
+sys.path.append(os.path.dirname(os.path.realpath(__file__)))
+
+import re
+import sqlite3
+try: from . import handler
+except: import handler
+
+
+# --- classes -------------------------------------------------------
+class StoringTeXhandler(handler.BibTeXhandler):
+    """A BibTeX handler keeping the entries in memory"""
+    
+    def __init__(self):
+        """Constructor
+        """
+        self._entries = {}
+        self._entryIDs = []
+        self._stringMap = {}
+        self._stringMapKeys = []
+    
+        self._groupNames = []
+        self._groups = {}
+
+    
+    def startDocument(self):
+        """Called at the begin of a document's processing"""
+        pass
+    
+    
+    def addStringDefinition(self, key, value):
+        """Adds the definition of a string
+
+        Stores the definition in the self._stringMap dictionary.
+        
+        Args:
+            key (str): The shortcut for the string.
+            value (str): The value of the string.
+        
+        Todo: 
+            Remove self._stringMapKeys
+        """
+        self._stringMap[key] = value
+        self._stringMapKeys.append(key)
+
+    
+    def addComment(self, key, value):
+        """Adds a comment
+        
+        This implementation is somehow "magic" as it targets
+        parsing JabRef comments that contain a group assignment.
+        
+        Args:
+            key (str): The name of the comment?
+            value (str): The value of the comment.
+        
+        Todo: 
+            Extract JabRef-parsing.
+        """
+        if not value.strip().startswith("jabref-meta: groupstree"):
+            return
+        value = value[value.find("0"):]
+        lines = value.split("\n")
+        c = ""
+        tree = []
+        lastLevel = 0
+        for l in lines:
+            c = c + l.strip()
+            i = c.rfind(";")
+            #print "%s %s %s %s" % (i, len(c)-1, c[i-2], c[i-2-5:])
+            if i==len(c)-1 and len(c)>2 and c[i-1]!='\\':
+                d = c[:c.find("\\;")].strip()
+                level = int(d[:d.find(" ")])
+                name = d[d.find(":")+1:]
+                if level<=lastLevel:
+                    tree = tree[:-(lastLevel - level + 1)]
+                lastLevel = level
+                tree.append(name)
+        
+                if level!=0:
+                    d = c[c.find(";")+1:].strip()
+                    d = d[d.find(";")+1:d.rfind(";")]
+                    items = filter(None, d.split("\;"))
+                    gName = "/".join(tree)
+                    if gName not in self._groupNames:
+                        self._groupNames.append(gName)
+                    if gName not in self._groups:
+                        self._groups[gName] = []
+                    self._groups[gName].extend(items)
+                #print "------------\n" + c[:20]
+                c = ""
+    
+    
+    def startEntry(self, entryID):
+        """Called if a new entry is started to being parsed.
+
+        Begins entry by storing it in internal containers.
+        
+        Args:
+            entryID (str): The ID (key) of the entry
+        """
+        self._entries[entryID] = {}
+        self._entryIDs.append(entryID)
+
+
+    def addField(self, entryID, key, value):
+        """Called if a new attribute of an entry shall be added.
+        
+        Stores the attribute in the self._entries[entryID] dictionary.
+        
+        Args:
+            entryID (str): The ID (key) of the entry
+            key (str): The name of the attribute
+            value (str): The value of the attribute
+        """
+        self._entries[entryID][key] = value
+
+
+    def addField2(self, entryID, key, pairs):
+        """Called if a new attribute consisting of multiple named fields shall be added.
+        
+        Allocates a dictionary entry in self._entries[entryID] with the given key.
+        Inserts the given pairs as key/values into this dictionary.
+        
+        Args:
+            entryID (str): The ID (key) of the entry
+            key (str): The name of the attribute
+            pairs (List[Tuple[str, str]]): The value of the attribute
+        """
+        if ukey not in self._entries[entryID]:
+            self._entries[entryID][key] = {}
+        for p in pairs:
+            self._entries[entryID][key][p[0]] = p[1]
+
+    
+    def closeEntry(self, entryID):
+        """Closes the entry
+        
+        Args:
+            entryID (str): The ID (key) of the entry
+        """
+        pass
+
+
+    def endDocument(self):
+        """Called after parsing a document"""
+        pass
+
```

### Comparing `bib2x-0.4.0/bib2x.egg-info/PKG-INFO` & `bib2x-0.4.2/bib2x.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bib2x
-Version: 0.4.0
+Version: 0.4.2
 Summary: A BibTex parser and converter
 Home-page: http://bib2x.readthedocs.org/
 Download-URL: http://pypi.python.org/pypi/bib2x
 Author: dkrajzew
 Author-email: d.krajzewicz@gmail.com
 License: BSD
 Project-URL: Documentation, https://bib2x.readthedocs.io/
```

### Comparing `bib2x-0.4.0/setup.py` & `bib2x-0.4.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 # --- definitions ---------------------------------------------------
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="bib2x",
-    version="0.4.0",
+    version="0.4.2",
     author="dkrajzew",
     author_email="d.krajzewicz@gmail.com",
     description="A BibTex parser and converter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='http://bib2x.readthedocs.org/',
     download_url='http://pypi.python.org/pypi/bib2x',
@@ -37,14 +37,16 @@
         'Source': 'https://github.com/dkrajzew/bib2x',
         'Tracker': 'https://github.com/dkrajzew/bib2x/issues',
         'Discussions': 'https://github.com/dkrajzew/bib2x/discussions',
     },
     license='BSD',
     # add modules
     packages=setuptools.find_packages(),
+    package_data={'': ["tex.db"]},
+    #data_files=[('bib2x', ["tex.db"])],
     entry_points = {
         'console_scripts': [
             'bib2x = bib2x:main'
         ]
     },
     # see https://pypi.org/classifiers/
     classifiers=[
```

### Comparing `bib2x-0.4.0/tests/test_bib2x_html.py` & `bib2x-0.4.2/tests/test_bib2x_html.py`

 * *Files identical despite different names*

### Comparing `bib2x-0.4.0/tests/test_bib2x_json.py` & `bib2x-0.4.2/tests/test_bib2x_json.py`

 * *Files identical despite different names*

### Comparing `bib2x-0.4.0/tests/test_bib2x_main.py` & `bib2x-0.4.2/tests/test_bib2x_main.py`

 * *Files identical despite different names*

