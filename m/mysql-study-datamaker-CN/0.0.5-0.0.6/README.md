# Comparing `tmp/mysql_study_datamaker_cn-0.0.5.tar.gz` & `tmp/mysql_study_datamaker_cn-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysql_study_datamaker_cn-0.0.5.tar", last modified: Tue Apr 30 06:19:57 2024, max compression
+gzip compressed data, was "mysql_study_datamaker_cn-0.0.6.tar", last modified: Mon May  6 08:42:54 2024, max compression
```

## Comparing `mysql_study_datamaker_cn-0.0.5.tar` & `mysql_study_datamaker_cn-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 06:19:57.794355 mysql_study_datamaker_cn-0.0.5/
--rw-rw-rw-   0        0        0     1091 2024-04-28 07:59:25.000000 mysql_study_datamaker_cn-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      912 2024-04-30 06:19:57.791611 mysql_study_datamaker_cn-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      495 2024-04-30 06:17:18.000000 mysql_study_datamaker_cn-0.0.5/README.md
--rw-rw-rw-   0        0        0      407 2024-04-30 06:17:18.000000 mysql_study_datamaker_cn-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-30 06:19:57.794355 mysql_study_datamaker_cn-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-30 06:19:57.758290 mysql_study_datamaker_cn-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-04-30 06:19:57.774902 mysql_study_datamaker_cn-0.0.5/src/mysql_study_datamaker_CN/
--rw-rw-rw-   0        0        0      112 2024-04-30 06:19:49.000000 mysql_study_datamaker_cn-0.0.5/src/mysql_study_datamaker_CN/__init__.py
--rw-rw-rw-   0        0        0     9784 2024-04-30 06:14:50.000000 mysql_study_datamaker_cn-0.0.5/src/mysql_study_datamaker_CN/datamaker.py
--rw-rw-rw-   0        0        0     1501 2024-04-23 04:28:09.000000 mysql_study_datamaker_cn-0.0.5/src/mysql_study_datamaker_CN/new_family.txt
--rw-rw-rw-   0        0        0    28630 2024-04-23 04:24:33.000000 mysql_study_datamaker_cn-0.0.5/src/mysql_study_datamaker_CN/new_names.txt
-drwxrwxrwx   0        0        0        0 2024-04-30 06:19:57.789129 mysql_study_datamaker_cn-0.0.5/src/mysql_study_datamaker_CN.egg-info/
--rw-rw-rw-   0        0        0      912 2024-04-30 06:19:57.000000 mysql_study_datamaker_cn-0.0.5/src/mysql_study_datamaker_CN.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2024-04-30 06:19:57.000000 mysql_study_datamaker_cn-0.0.5/src/mysql_study_datamaker_CN.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 06:19:57.000000 mysql_study_datamaker_cn-0.0.5/src/mysql_study_datamaker_CN.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-30 06:19:57.000000 mysql_study_datamaker_cn-0.0.5/src/mysql_study_datamaker_CN.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 08:42:54.291696 mysql_study_datamaker_cn-0.0.6/
+-rw-rw-rw-   0        0        0     1091 2024-04-28 07:59:25.000000 mysql_study_datamaker_cn-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      912 2024-05-06 08:42:54.291696 mysql_study_datamaker_cn-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      495 2024-04-30 06:17:18.000000 mysql_study_datamaker_cn-0.0.6/README.md
+-rw-rw-rw-   0        0        0      407 2024-05-06 08:42:06.000000 mysql_study_datamaker_cn-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 08:42:54.291696 mysql_study_datamaker_cn-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-06 08:42:54.259017 mysql_study_datamaker_cn-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 08:42:54.277227 mysql_study_datamaker_cn-0.0.6/src/mysql_study_datamaker_CN/
+-rw-rw-rw-   0        0        0      619 2024-05-06 08:41:18.000000 mysql_study_datamaker_cn-0.0.6/src/mysql_study_datamaker_CN/__init__.py
+-rw-rw-rw-   0        0        0    10385 2024-05-06 08:41:18.000000 mysql_study_datamaker_cn-0.0.6/src/mysql_study_datamaker_CN/datamaker.py
+-rw-rw-rw-   0        0        0     1501 2024-04-23 04:28:09.000000 mysql_study_datamaker_cn-0.0.6/src/mysql_study_datamaker_CN/new_family.txt
+-rw-rw-rw-   0        0        0    28630 2024-04-23 04:24:33.000000 mysql_study_datamaker_cn-0.0.6/src/mysql_study_datamaker_CN/new_names.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 08:42:54.291696 mysql_study_datamaker_cn-0.0.6/src/mysql_study_datamaker_CN.egg-info/
+-rw-rw-rw-   0        0        0      912 2024-05-06 08:42:54.000000 mysql_study_datamaker_cn-0.0.6/src/mysql_study_datamaker_CN.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2024-05-06 08:42:54.000000 mysql_study_datamaker_cn-0.0.6/src/mysql_study_datamaker_CN.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 08:42:54.000000 mysql_study_datamaker_cn-0.0.6/src/mysql_study_datamaker_CN.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-06 08:42:54.000000 mysql_study_datamaker_cn-0.0.6/src/mysql_study_datamaker_CN.egg-info/top_level.txt
```

### Comparing `mysql_study_datamaker_cn-0.0.5/LICENSE` & `mysql_study_datamaker_cn-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mysql_study_datamaker_cn-0.0.5/PKG-INFO` & `mysql_study_datamaker_cn-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql_study_datamaker_CN
-Version: 0.0.5
+Version: 0.0.6
 Summary: Generate some data and convert it to MySQL language.
 Author-email: Kavin <scratch_test@126.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `mysql_study_datamaker_cn-0.0.5/src/mysql_study_datamaker_CN/datamaker.py` & `mysql_study_datamaker_cn-0.0.6/src/mysql_study_datamaker_CN/datamaker.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,16 @@
     """
     这个类的目的是为了在学习 MySQL 语言时，创建表结构后，需要很多插入的数据来进行学习测试；
     DataMaker会根据指定的数量生成指定多的随机项，且支持自定义顺序；
     当前的版本只会生成一个 txt 文本，注意最后一行的","要替换成";"才能够插入数据；
     xxx 是你的 MySQL 表名，需要替换，很傻瓜很简单的一个类
     """
 
-    def __init__(self, N, args=("姓名", "年龄", "性别", "生日", "部门"), left=1950, right=2000, department=None, gender="int", a=0, b=150):
+    def __init__(self, N, args=("姓名", "年龄", "性别", "生日", "部门"), left=1950, right=2000,
+                 department=None, gender="int", a=0, b=150, file=None):
         """
         __information：数据字典
         N：数据个数
         args：字段列表，目前只支持：姓名,年龄,部门,生日,性别,分数
         left:出生日期左边界，默认情况下不允许小于 1950 （如有需求可自行修改源代码中的判定）
         right:出生日期有边界，默认情况下不允许小于当前年 （自动判定当前年份，拒绝未来人）
         department：默认给了：‘销售部,技术部,售后部,企划部,咨询部,人事部,财务部’，如果需要重新定义部门，需要写字符串，用','分割；
@@ -24,26 +25,37 @@
             en：英文的 M F
             english：英文的 Male  Female
         a：考试分数的随机，最小值；
         b:考试分数的随机，最大值；
         分数只要识别前两个字符是分数就可以，如果想创建多个分数的学生信息，可以写成：
         ("姓名", "年龄", "性别",  "分数1", "分数2", "分数3")
         考试分数默认是 ； 0~150 分，则 a 就是 0， b：就是 150，做了判定修改，支持 b < a
+        file：文件名，写入以 x 格式，所以创建后，再次生成会报文件已存在的错误，建议写入当前日期时间，模式为：None或者'date'，
+              如果是None则使用 "_mysql_date.txt" , 如果是 "date" 则以此刻时间为基准，也可以自定义名直接写；
         """
         self.__informations = {}
 
         self.__N = N
         self.__args = args
         self.__left = left
         self.__right = right
         self.__department = department
         self.__gender = gender
         self.__a = a
         self.__b = b
 
+        if file is None:
+            self.file = "_mysql_date.txt"
+        elif not isinstance(file, str):
+            raise TypeError("'file' should be a str")
+        elif file.lower() == "date":
+            now = datetime.now()
+            self.file = f"{now.year}{now.month:>02}{now.day:>02} {now.hour:>02}.{now.minute:>02}.{now.second:>02}.txt"
+        else:
+            self.file = file
         self.get_info()
 
     def get_name(self):
         """
         返回随机生成的姓名系统，总共有 300个姓氏，3579个名字；
         如果超过 1,073,700 个姓名，就一定会有重复的名字出现；
         因为没有做去重处理，所以就算生成 2 个随机姓名也有重复出现的概率！
@@ -188,32 +200,31 @@
             result += next(v) + ","
         result = result[:-1]
         if not result:
             raise StopIteration
         return result
 
     @classmethod
-    def create_insertinto(cls, self, file="_mysql_insert.txt"):
+    def create_insertinto(cls, self):
         """
         需要先生成一个DataMaker对象，来创建指定数量和字段，再调用该方法，写入到一个txt文本中；
         :param self: 生成的对象
         :param file: txt文件名
         :return: None
         """
-        with open(file, "x", encoding="utf-8") as f:
+        with open("insert_into_" + self.file, "x", encoding="utf-8") as f:
             f.write("insert into xxx values \n")
             id = 1
             for line in self:
                 comment = "(" + str(id) + "," + line + "),\n"
                 id += 1
                 f.write(comment)
 
 
 if __name__ == '__main__':
     """
     下面是案例，直接运行可以获得测试代码，生成15个随机数据；
     """
-    now = datetime.now()
-    file_name = f"{now.year}{now.month:>02}{now.day:>02} {now.hour:>02}.{now.minute:>02}.{now.second:>02}.txt"
-    one = DataMaker(15, ("姓名", "年龄", "性别",  "分数1", "分数2", "分数3"), gender="cn")
-    DataMaker.create_insertinto(one, file_name)
+    args = ("姓名", "年龄", "性别")
+    one = DataMaker(15, args, left=2010, gender="cn", file='date')
+    DataMaker.create_insertinto(one)
```

### Comparing `mysql_study_datamaker_cn-0.0.5/src/mysql_study_datamaker_CN/new_family.txt` & `mysql_study_datamaker_cn-0.0.6/src/mysql_study_datamaker_CN/new_family.txt`

 * *Files identical despite different names*

### Comparing `mysql_study_datamaker_cn-0.0.5/src/mysql_study_datamaker_CN/new_names.txt` & `mysql_study_datamaker_cn-0.0.6/src/mysql_study_datamaker_CN/new_names.txt`

 * *Files identical despite different names*

### Comparing `mysql_study_datamaker_cn-0.0.5/src/mysql_study_datamaker_CN.egg-info/PKG-INFO` & `mysql_study_datamaker_cn-0.0.6/src/mysql_study_datamaker_CN.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysql_study_datamaker_CN
-Version: 0.0.5
+Version: 0.0.6
 Summary: Generate some data and convert it to MySQL language.
 Author-email: Kavin <scratch_test@126.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

