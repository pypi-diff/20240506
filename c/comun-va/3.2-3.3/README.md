# Comparing `tmp/comun_va-3.2.tar.gz` & `tmp/comun_va-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comun_va-3.2.tar", last modified: Fri Mar 22 10:33:13 2024, max compression
+gzip compressed data, was "comun_va-3.3.tar", last modified: Mon May  6 13:06:02 2024, max compression
```

## Comparing `comun_va-3.2.tar` & `comun_va-3.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 10:33:13.322568 comun_va-3.2/
--rw-rw-rw-   0        0        0       53 2024-03-22 10:33:13.321571 comun_va-3.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-22 10:33:13.320567 comun_va-3.2/comun_va.egg-info/
--rw-rw-rw-   0        0        0       53 2024-03-22 10:33:13.000000 comun_va-3.2/comun_va.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      179 2024-03-22 10:33:13.000000 comun_va-3.2/comun_va.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 10:33:13.000000 comun_va-3.2/comun_va.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-03-22 10:33:13.000000 comun_va-3.2/comun_va.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-03-22 10:33:13.000000 comun_va-3.2/comun_va.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8850 2024-03-22 09:15:18.000000 comun_va-3.2/comun_va.py
--rw-rw-rw-   0        0        0       42 2024-03-22 10:33:13.322568 comun_va-3.2/setup.cfg
--rw-rw-rw-   0        0        0      216 2024-03-22 09:15:18.000000 comun_va-3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:06:02.648731 comun_va-3.3/
+-rw-rw-rw-   0        0        0       53 2024-05-06 13:06:02.647725 comun_va-3.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-06 13:06:02.646423 comun_va-3.3/comun_va.egg-info/
+-rw-rw-rw-   0        0        0       53 2024-05-06 13:06:02.000000 comun_va-3.3/comun_va.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2024-05-06 13:06:02.000000 comun_va-3.3/comun_va.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 13:06:02.000000 comun_va-3.3/comun_va.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-06 13:06:02.000000 comun_va-3.3/comun_va.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-06 13:06:02.000000 comun_va-3.3/comun_va.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8885 2024-05-06 13:01:57.000000 comun_va-3.3/comun_va.py
+-rw-rw-rw-   0        0        0       42 2024-05-06 13:06:02.648731 comun_va-3.3/setup.cfg
+-rw-rw-rw-   0        0        0      216 2024-05-06 13:05:09.000000 comun_va-3.3/setup.py
```

### Comparing `comun_va-3.2/comun_va.py` & `comun_va-3.3/comun_va.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,22 +57,22 @@
         mssql = comun_sqlsrv.Sql(mssql_srv, database, user, passwd)
         query = f"""
                 INSERT INTO T_VA_API_LOG
                 (FECHA_HORA, ENDPOINT, RESULTADO, DATO_RECIBIDO, PREDICCION_VA, NOMBRE_IMAGEN, COD_BAR, ERROR, PORCENTAJE_ACIERTO)
                 VALUES (%s, %s, %s, %s, %s, %s, %s, %s, %s);
                 """
         query_values = (self.date_time,
-                        self.endpoint_name,
-                        self.result,
-                        self.endpoint_data_received,
-                        self.prediction,
-                        self.img_name,
+                        str(self.endpoint_name),
+                        str(self.result),
+                        str(self.endpoint_data_received),
+                        str(self.prediction),
+                        str(self.img_name),
                         str(self.bar_code),
-                        self.error,
-                        self.match_score)
+                        str(self.error),
+                        str(self.match_score))
         mssql.ejecutar(query, query_values)
         mssql.cerrar_conexion()
 
     def send_email_info(self, smtp_host: str, email_subject: str, receiver: list):
         """
         Send an email with VA information
         :param smtp_host: IP and port of the smtp server, example: "10.10.10.5:587"
```

