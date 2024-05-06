# Comparing `tmp/squelch-0.2.0.tar.gz` & `tmp/squelch-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "squelch-0.2.0.tar", max compression
+gzip compressed data, was "squelch-0.3.0.tar", max compression
```

## Comparing `squelch-0.2.0.tar` & `squelch-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2018-06-22 07:09:46.422789 squelch-0.2.0/LICENSE
--rw-r--r--   0        0        0     2607 2024-04-17 18:59:58.698301 squelch-0.2.0/README.md
--rw-r--r--   0        0        0      721 2024-04-20 10:42:03.743440 squelch-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    19166 2024-04-20 10:42:31.867731 squelch-0.2.0/squelch/__init__.py
--rw-r--r--   0        0        0     4513 2024-04-15 12:20:52.730110 squelch-0.2.0/squelch/__main__.py
--rw-r--r--   0        0        0     3459 1970-01-01 00:00:00.000000 squelch-0.2.0/setup.py
--rw-r--r--   0        0        0     3435 1970-01-01 00:00:00.000000 squelch-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2018-06-22 07:09:46.422789 squelch-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5919 2024-05-06 18:59:51.634075 squelch-0.3.0/README.md
+-rw-r--r--   0        0        0      721 2024-05-06 18:59:51.634075 squelch-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    29979 2024-05-06 18:59:51.634075 squelch-0.3.0/squelch/__init__.py
+-rw-r--r--   0        0        0     6698 2024-05-06 18:59:51.634075 squelch-0.3.0/squelch/__main__.py
+-rw-r--r--   0        0        0     6863 1970-01-01 00:00:00.000000 squelch-0.3.0/setup.py
+-rw-r--r--   0        0        0     6747 1970-01-01 00:00:00.000000 squelch-0.3.0/PKG-INFO
```

### Comparing `squelch-0.2.0/LICENSE` & `squelch-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `squelch-0.2.0/pyproject.toml` & `squelch-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "squelch"
-version = "0.2.0"
+version = "0.3.0"
 description = "Simple SQL REPL Command Handler"
 authors = ["Paul Breen <pbree@bas.ac.uk>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/paul-breen/squelch"
 homepage = "https://github.com/paul-breen/squelch"
 documentation = "https://github.com/paul-breen/squelch/blob/main/README.md"
```

### Comparing `squelch-0.2.0/squelch/__main__.py` & `squelch-0.3.0/squelch/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import sys
 import argparse
 import logging
 
 from squelch import Squelch, __version__, PROGNAME, DEF_CONF_FILE
 
+STATE_OPTS = ['set','pset']
+NON_CONF_OPTS = STATE_OPTS
+
 logging.basicConfig()
 logger = logging.getLogger(PROGNAME)
 
 def parse_cmdln():
     """
     Parse the command line
 
@@ -27,14 +30,16 @@
 
 "The string form of the URL is dialect[+driver]://user:password@host/dbname[?key=value..], where dialect is a database name such as mysql, oracle, postgresql, etc., and driver the name of a DBAPI, such as psycopg2, pyodbc, cx_oracle, etc. Alternatively, the URL can be an instance of URL."
 """
 
     parser = argparse.ArgumentParser(description='Squelch is a Simple SQL REPL Command Handler.', epilog=epilog, formatter_class=argparse.RawDescriptionHelpFormatter, prog=PROGNAME)
     parser.add_argument('-c', '--conf-file', help=f"The full path to a JSON configuration file.  It defaults to {DEF_CONF_FILE}.")
     parser.add_argument('-u', '--url', help='The database connection URL, as required by sqlalchemy.create_engine().')
+    parser.add_argument('-S', '--set', help='Set state variable NAME to VALUE.', metavar='NAME=VALUE', nargs='*', action='extend')
+    parser.add_argument('-P', '--pset', help='Set printing state variable NAME to VALUE.', metavar='NAME=VALUE', nargs='*', action='extend')
     parser.add_argument('-v', '--verbose', help='Turn verbose messaging on.  The effects of this option are incremental.', action='count', default=0)
     parser.add_argument('-V', '--version', action='version', version=f"%(prog)s {__version__}")
 
     args = parser.parse_args()
 
     return args
 
@@ -60,41 +65,81 @@
         if args.verbose > 2:
             logging.getLogger().setLevel(logging.DEBUG)
 
 def update_conf_from_cmdln(conf, args):
     """
     Update the configuration from command line arguments
 
+    Options listed in NON_CONF_OPTS are not included in the configuration
+
     :param conf: The program's configuration
     :type conf: dict
     :param args: The parsed command line arguments object
     :type args: argparse.Namespace object
     :returns: The updated configuration
     :rtype: dict
     """
 
     opts = {}
 
     for k,v in vars(args).items():
-        if v:
-            opts[k] = v
+        if k not in NON_CONF_OPTS:
+            if v:
+                opts[k] = v
 
     logger.debug(f"overriding configuration with options: {opts}")
     conf.update(opts)
 
     return conf
 
+def set_state_from_cmdln(squelch, args, nv_sep='='):
+    """
+    Update the program's runtime state from command line arguments
+
+    Options listed in STATE_OPTS are used to set the program's runtime state
+
+    :param squelch: The instantiated Squelch object
+    :type squelch: Squelch
+    :param args: The parsed command line arguments object
+    :type args: argparse.Namespace object
+    :param nv_sep: The name/value separator in the option argument
+    :type nv_sep: str
+    """
+
+    for k,v in vars(args).items():
+        if k in STATE_OPTS:
+            if v:
+                # Multiple state options can be set hence this is a list
+                for nv_pair in v:
+                    try:
+                        name, value = nv_pair.split(nv_sep, maxsplit=2)
+                    except ValueError as e:
+                        print(f"A state variable must be expressed as NAME=VALUE.  For example, --set AUTOCOMMIT=on, --pset pager=off.", file=sys.stderr)
+
+                        if args.verbose > 1:
+                            raise
+                        else:
+                            sys.exit(1)
+
+                    # Construct command in form it would be issued in client
+                    logger.debug(f"setting {name} to {value}")
+                    cmd = fr"\{k} {name} {value}"
+                    state_text = squelch.set_state(cmd)
+
+                    if state_text:
+                        logger.debug(state_text)
+
 def consolidate_conf(squelch, args):
     """
     Consolidate the configuration from a conf file and command line arguments
 
     :param squelch: The instantiated Squelch object
     :type squelch: Squelch
-    :param args: The parsed command line arguments squelchect
-    :type args: argparse.Namespace squelchect
+    :param args: The parsed command line arguments object
+    :type args: argparse.Namespace object
     :returns: The consolidated configuration
     :rtype: dict
     """
 
     if args.conf_file:
         squelch.get_conf(file=args.conf_file)
 
@@ -105,14 +150,16 @@
     try:
         args.verbose = squelch.conf['verbose']
     except KeyError:
         pass
 
     configure_logging(args)
 
+    set_state_from_cmdln(squelch, args)
+
     return squelch.conf
 
 def connect(squelch, args):
     """
     Connect to the database
 
     The program exits if no valid database connection URL was specified
@@ -142,12 +189,19 @@
 
     args = parse_cmdln()
     squelch = Squelch()
     configure_logging(args)
     consolidate_conf(squelch, args)
 
     connect(squelch, args)
-    squelch.repl()
+
+    # Process queries on stdin if we were called as a one-shot, otherwise
+    # we drop into the interactive REPL
+    if not sys.stdin.isatty():
+        for line in sys.stdin:
+            squelch.process_input(squelch.clean_raw_input(line))
+    else:
+        squelch.repl()
 
 if __name__ == '__main__':
     main()
```

