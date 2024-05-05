# Comparing `tmp/coomer_favlink_generator-1.0.0.tar.gz` & `tmp/coomer_favlink_generator-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coomer_favlink_generator-1.0.0.tar", last modified: Sat May  4 00:51:14 2024, max compression
+gzip compressed data, was "coomer_favlink_generator-1.0.1.tar", last modified: Sun May  5 22:09:24 2024, max compression
```

## Comparing `coomer_favlink_generator-1.0.0.tar` & `coomer_favlink_generator-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-04 00:51:14.692674 coomer_favlink_generator-1.0.0/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1078 2024-05-04 00:30:07.000000 coomer_favlink_generator-1.0.0/LICENSE
--rw-r--r--   0 codespace  (1000) codespace  (1000)       90 2024-05-04 00:51:14.688673 coomer_favlink_generator-1.0.0/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2352 2024-05-04 00:50:03.000000 coomer_favlink_generator-1.0.0/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-04 00:51:14.680673 coomer_favlink_generator-1.0.0/coomer_favlink_generator/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-04 00:08:28.000000 coomer_favlink_generator-1.0.0/coomer_favlink_generator/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1702 2024-05-04 00:20:47.000000 coomer_favlink_generator-1.0.0/coomer_favlink_generator/link_generator.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-04 00:51:14.688673 coomer_favlink_generator-1.0.0/coomer_favlink_generator.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)       90 2024-05-04 00:51:14.000000 coomer_favlink_generator-1.0.0/coomer_favlink_generator.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      349 2024-05-04 00:51:14.000000 coomer_favlink_generator-1.0.0/coomer_favlink_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-04 00:51:14.000000 coomer_favlink_generator-1.0.0/coomer_favlink_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       90 2024-05-04 00:51:14.000000 coomer_favlink_generator-1.0.0/coomer_favlink_generator.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       25 2024-05-04 00:51:14.000000 coomer_favlink_generator-1.0.0/coomer_favlink_generator.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-04 00:51:14.692674 coomer_favlink_generator-1.0.0/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      334 2024-05-04 00:29:13.000000 coomer_favlink_generator-1.0.0/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-05 22:09:24.434515 coomer_favlink_generator-1.0.1/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1078 2024-05-04 00:30:07.000000 coomer_favlink_generator-1.0.1/LICENSE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)       90 2024-05-05 22:09:24.434515 coomer_favlink_generator-1.0.1/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2352 2024-05-04 00:50:03.000000 coomer_favlink_generator-1.0.1/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-05 22:09:24.430515 coomer_favlink_generator-1.0.1/coomer_favlink_generator/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2024-05-04 00:08:28.000000 coomer_favlink_generator-1.0.1/coomer_favlink_generator/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1705 2024-05-05 22:08:30.000000 coomer_favlink_generator-1.0.1/coomer_favlink_generator/link_generator.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-05 22:09:24.434515 coomer_favlink_generator-1.0.1/coomer_favlink_generator.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)       90 2024-05-05 22:09:24.000000 coomer_favlink_generator-1.0.1/coomer_favlink_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      349 2024-05-05 22:09:24.000000 coomer_favlink_generator-1.0.1/coomer_favlink_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-05 22:09:24.000000 coomer_favlink_generator-1.0.1/coomer_favlink_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       90 2024-05-05 22:09:24.000000 coomer_favlink_generator-1.0.1/coomer_favlink_generator.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       25 2024-05-05 22:09:24.000000 coomer_favlink_generator-1.0.1/coomer_favlink_generator.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-05 22:09:24.434515 coomer_favlink_generator-1.0.1/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      329 2024-05-05 22:08:30.000000 coomer_favlink_generator-1.0.1/setup.py
```

### Comparing `coomer_favlink_generator-1.0.0/LICENSE` & `coomer_favlink_generator-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `coomer_favlink_generator-1.0.0/README.md` & `coomer_favlink_generator-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `coomer_favlink_generator-1.0.0/coomer_favlink_generator/link_generator.py` & `coomer_favlink_generator-1.0.1/coomer_favlink_generator/link_generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     for item in data:
         # Check the service type and generate the appropriate link
         if item['service'] == 'onlyfans':
             link = f"https://coomer.su/onlyfans/user/{item['name']}"
         elif item['service'] == 'fansly':
             link = f"https://coomer.su/fansly/user/{item['id']}"
         # Adding candfans profiles to favorites doesn't even work in coomer but whatever
-        elif item['service'] == 'fansly':
+        elif item['service'] == 'candfans':
             link = f"https://coomer.su/candfans/user/{item['id']}"
         else:
             continue
         
         links.append(link)
     
     return links
@@ -46,8 +46,8 @@
     with open('coomer_links.txt', 'w') as output_file:
         for link in links:
             output_file.write(link + '\n')
 
 if __name__ == "__main__":
     main()
 
-    
+
```

