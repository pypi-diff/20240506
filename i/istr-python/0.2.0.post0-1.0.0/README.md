# Comparing `tmp/istr_python-0.2.0.post0.tar.gz` & `tmp/istr_python-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "istr_python-0.2.0.post0.tar", last modified: Wed May  1 15:46:05 2024, max compression
+gzip compressed data, was "istr_python-1.0.0.tar", last modified: Mon May  6 13:49:54 2024, max compression
```

## Comparing `istr_python-0.2.0.post0.tar` & `istr_python-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 15:46:05.685639 istr_python-0.2.0.post0/
--rw-rw-rw-   0        0        0    13136 2024-05-01 15:46:05.683754 istr_python-0.2.0.post0/PKG-INFO
--rw-rw-rw-   0        0        0    12151 2024-05-01 07:19:51.000000 istr_python-0.2.0.post0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 15:46:05.648793 istr_python-0.2.0.post0/istr/
--rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-0.2.0.post0/istr/__init__.py
--rw-rw-rw-   0        0        0    20752 2024-05-01 06:41:58.000000 istr_python-0.2.0.post0/istr/istr.py
-drwxrwxrwx   0        0        0        0 2024-05-01 15:46:05.681995 istr_python-0.2.0.post0/istr_python.egg-info/
--rw-rw-rw-   0        0        0    13136 2024-05-01 15:46:05.000000 istr_python-0.2.0.post0/istr_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2024-05-01 15:46:05.000000 istr_python-0.2.0.post0/istr_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 15:46:05.000000 istr_python-0.2.0.post0/istr_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-01 15:46:05.000000 istr_python-0.2.0.post0/istr_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      660 2024-05-01 15:45:57.000000 istr_python-0.2.0.post0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-01 15:46:05.685639 istr_python-0.2.0.post0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-01 15:46:05.668731 istr_python-0.2.0.post0/tests/
--rw-rw-rw-   0        0        0    13111 2024-04-30 11:45:24.000000 istr_python-0.2.0.post0/tests/test_istr.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:49:54.787606 istr_python-1.0.0/
+-rw-rw-rw-   0        0        0    15702 2024-05-06 13:49:54.785577 istr_python-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    14565 2024-05-06 13:47:27.000000 istr_python-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 13:49:54.759491 istr_python-1.0.0/istr/
+-rw-rw-rw-   0        0        0       50 2024-04-17 12:23:20.000000 istr_python-1.0.0/istr/__init__.py
+-rw-rw-rw-   0        0        0    24194 2024-05-06 11:38:16.000000 istr_python-1.0.0/istr/istr.py
+drwxrwxrwx   0        0        0        0 2024-05-06 13:49:54.783062 istr_python-1.0.0/istr_python.egg-info/
+-rw-rw-rw-   0        0        0    15702 2024-05-06 13:49:54.000000 istr_python-1.0.0/istr_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2024-05-06 13:49:54.000000 istr_python-1.0.0/istr_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 13:49:54.000000 istr_python-1.0.0/istr_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-06 13:49:54.000000 istr_python-1.0.0/istr_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      658 2024-05-06 13:49:48.000000 istr_python-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 13:49:54.787606 istr_python-1.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-06 13:49:54.781067 istr_python-1.0.0/tests/
+-rw-rw-rw-   0        0        0    16198 2024-05-06 11:40:02.000000 istr_python-1.0.0/tests/test_istr.py
```

### Comparing `istr_python-0.2.0.post0/PKG-INFO` & `istr_python-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: istr-python
-Version: 0.2.0.post0
+Version: 1.0.0
 Summary: istr - strings you can count on
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/istr
 Project-URL: Repository, https://github.com/salabim/istr
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-<img src="https://www.salabim.org/istr_logo.png" width=500>
+ <img src="https://www.salabim.org/istr_logo.png" width=500>
 
-## Introduction
+### Introduction
 
 The istr module has exactly one class: istr.
 
 With this it is possible to interpret strings as if they were integers.
 
-This can be very handy for solving puzzles, but also for other purposes.</br>
-For instance the
-famous send more money puzzle
+This can be very handy for solving puzzles, but also for other purposes.
+For instance the famous send more money puzzle, where each letter has to be replaced by a unique digit (0-9)
+
 ```
   S E N D
   M O R E
 --------- +
 M O N E Y
 ```
 can be nicely, albeit not very efficient, coded as:
@@ -37,280 +37,404 @@
     if m and ((s|e|n|d) + (m|o|r|e) == (m|o|n|e|y)):
         print(f' {s|e|n|d}')
         print(f' {m|o|r|e}')
         print('-----')
         print(f'{m|o|n|e|y}')
 ```
 
-And it is a nice demonstration of extending a class (str) with extra and changed functionality.
+Of, if we want to add all the digits in a string:
+
+```
+sum_digits = sum(istr('9282334'))  # answer 31
+```
+
+And the module is a demonstration of extending a class (str) with extra and changed functionality.
 
-## Installation
+### Installation
 Installing istr with pip is easy.
 ```
 $ pip install istr-python
 ```
 or when you want to upgrade,
 ```
 $ pip install istr-python --upgrade
 ```
 Alternatively, istr.py can be just copied into you current work directory from GitHub (https://github.com/salabim/istr).
 
 No dependencies!
 
-## Usage
+### Usage
+#### Start
+
 Just start with
 
 ```
 from istr import istr
 ```
 
-Now we can define some istrs:
+#### Use istrs as if the were int
+
+We can define an istr:
 ```
 four = istr('4')
 five = istr('5')
 ```
-Then we can do
+The variables `four`  and `five` can now be used as if they were int:
+
 ```
-x= four * five
+twenty = four * five
 ```
 , after which x is `istr('20')`
 
-And now we can do
+The same can be done with
+
+```
+twenty = 4 * five
+```
+
+or
+
+```
+twenty = four * 5
+```
+
+And now `twenty` can be used as if it was an int as well. So:
+
 ```
-print(x == 20)
-print(x == '20')
+twenty - four
 ```
-resulting in two times `True`. That's because istrs instances are treated as int, although they are strings.
 
-That means that we can also say
+is `istr('16')`
+
+We can do all the usual arithmetic operations on istrs, e.g.
+
 ```
-print(x < 30)
-print(x >= '10')
+-four + (twenty / 2)
+```
+
+is `istr('6')`
+
+And we can test for equality, So:
+
 ```
-again resulting in two times `True`.
+twenty == 20
+```
+is True.
+
+But as istrs are also strings. So
+
+```
+twenty == '20'
+```
+
+is also True!
+
+For the order comparisons (<=, <, >, >=), the istr is always interpreted as an int:
+
+That means that  both
+```
+twenty < 30
+twenty >= '10' # here '10' is converted to 10 for the comparison
+```
+are `True`.
 
 In contrast to an ordinary string
 ```
 print(four + five)
 ```
 prints `9`, as istr are treated as ints.
 
-Please note that `four` and `five` could have also be initialized with
+Please note that `four`  could have also been initialized with
 ```
 four = istr(4)
-five = istr(5)
 ```
 or even
 ```
 four, five = istr(4, 5)
 ```
 
-But how can we concatenate istrs? Just use the or operator (|): 
+> [!NOTE]
+>
+> All calculations are strictly integer calculations. That means that if a float variale is ever produced it will be converted to an int.
+> Also divisions are always floor divisions!
+
+#### Use istrs as string
+
+We should realize that istrs are in fact strings.
+
+In order to concatenate two istrs (or an istr and a str), we cannot use the `four + five` operator as
+
+that would be `istr(9)`.
+
+In order to concatenate istrs,  we use the or operator (`|`). So
+
 ```
-print(four | five)
+four | five
 ```
-will output `45`.
-
-And the result is again an istr.
+will be `istr(`45`).
 
 That means that
 ```
 (four | five) / 3
 ```
 is `istr('9')`.
 
-In order to repeat a string in the usual sense, you cannot use `3 * four`, as that woud be `12`. 
+In order to repeat a string in the usual sense, you cannot use `3 * four`, as that would be `12`. 
+
+In order to repeat we use the matrix multiplication operator (`@`). So
+
+ `3 @ four`
+
+ is istr(`444`). As is `four @ 3`.
+
+> [!NOTE]
+>
+> It is not allowed to use the `@` operator for two istrs. So, `four @ five` raises a TypeError.
+
+#### istrs that can't be interpreted as an int
 
-We use the matrix multiplication operator (@) for this. So `3 @ four` is `444`. As is `four @ 3`.
+Although usualy, istrs are to be interpreted as an int, that's not a requirement.
+
+So
 
-Also allowed are
 ```
-abs(four)
--four 
+istr('abc')
 ```
 
-The bool operator works on the integer value of an istr. So
-`bool(istr('0'))` ==> `False`
-`bool(istr('1'))` ==> `True`
-The code
+or
+
+```
+istr(1,2,3)
+```
+
+are accepted.
+
+But, we can't do any arithmetic with them. 
+
+If we try
+
 ```
-if istr('0'):
-    print('True')
-else:
-    print('False')
+istr('abc') + 5
 ```
-will print `False`
 
-For the in operator, an istr is treated as an ordinary string, although it is possible to use ints as well:
+a TypeError will be raised.
+
+That holds for any arithmetic we try.
+
+If we want to test if an istr can be interpreted (and thus used in an arithmetic expression). we can use the `is_int()` method. So
+
+```ìstr(20).is_int()```
+
+is `True`, wherea
+
+```ìstr('abc').is_int()```
+
+is `False`.
+
+
+
+The bool operator works normally on the integer value of an istr. So
+
+`bool(istr('0'))` ==> `False`
+`bool(istr('1'))` ==> `True`
+
+If the istr can't be interpreted as an int, the string will be used to test. So
+
+`bool(istr('abc'))` ==> `False`
+`bool(istr(''))` ==> `True`
+
+#### Other operators
+
+For the `in` operator, an istr is treated as an ordinary string, although it is possible to use ints as well:
+
 ```
 '34' in istr(1234)
 34 in istr(1234)
 ```
 On the left hand side an istr is always treated as a string:
 ```
 istr(1234) in '01234566890ABCDEF'
 ```
 
-Note that all calculations are strictly integer calculations. That means that if a float variale is ever produced it will be converted to an int.
-Also divisions are always floor divisions!
-
-There's a special case for `istr('')`. This is a proper empty string, but also represents the value of 0.
-That is to allow for `istr('').join(i for i in '01234)'`, resulting in `istr('01234')`.
-
 Sorting a list of istrs is based on the integer value, not the string. So
 
-`' '.join(sorted('1 3 2 4 5 6 11 7 9 8 10 12 0'.split()))`
+```
+' '.join(sorted('1 3 2 4 5 6 11 7 9 8 10 12 0'.split()))
+```
 
 is
 
-`'0 1 10 11 2 3 4 5 6 7 8 9'`
+```
+'0 1 10 11 2 3 4 5 6 7 8 9'
+```
 
 ,whereas
 
-`' '.join(sorted(istr('1 3 2 4 5 6 11 7 9 8 10 12 0'.split())))`
+```
+' '.join(sorted(istr('1 3 2 4 5 6 11 7 9 8 10 12 0'.split()))
+```
 
 is 
 
-`'0 1 2 3 4 5 6 7 8 9 10 11'`
+```
+'0 1 2 3 4 5 6 7 8 9 10 11'
+```
 
-## Using other values for istr than numeric value or str
+#### Using other values for istr than numeric value or str
 Apart from with simple numeric (to be interpreted as an int) or str, istr can be initialized with
 several other types:
 
-- if a dict (or subtype of dict), the same type dict will be returned with all values istr'ed
+- if a dict (or subtype of dict), the same type dict will be returned with all *values* istr'ed
 
-    `istr({0: 0, 1: 1, 2: 4})` ==> `{0: istr('0'), 1: istr('1'), 2: istr('4')}`
+    ```
+    istr({0: 0, 1: 1, 2: 4}) ==> {0: istr('0'), 1: istr('1'), 2: istr('4')}
+    ```
 
 - if an iterator, the iterator will be mapped with istr
 
-    `istr(i * i for i in range(3))` ==> `<map object>`
-
-    `list(istr(i * i for i in range(3)))` ==> `[istr('0'), istr('1'), istr('4')]`
+    ```
+    istr(i * i for i in range(3)) ==> <map object>
+    list(istr(i * i for i in range(3))) ==> [istr('0'), istr('1'), istr('4')]
+    ```
 
 - if an iterable, the same type will be returned with all elements istr'ed
 
-    `istr([0, 1, 4])` ==> `[istr('0'), istr('1'), istr('4')]`
-
-    `istr((0, 1, 4))` ==> `(istr('0'), istr('1'), istr('4'))`
-
-    `istr({0, 1, 4})` ==> `{istr('4'), istr('0'), istr('1')} ## or similar`
+    ```
+    istr([0, 1, 4]) ==> [istr('0'), istr('1'), istr('4')]
+    istr((0, 1, 4)) ==> (istr('0'), istr('1'), istr('4'))
+    istr({0, 1, 4}) ==> `{istr('4'), istr('0'), istr('1')}  # or similar
+    ```
 
 - if a range, an istr.range instance will be returned
-    
-    `istr(range(3))` ==> `istr.range(3)`
+  
+    ```
+  istr(range(3))` ==> `istr.range(3)
+    list(istr(range(3)))` ==> `[istr('0'), istr('1'), istr('2')]
+  len(istr(range(3)))` ==> `3
+  ```
 
-    `list(istr(range(3)))` ==> `[istr('0'), istr('1'), istr('2')]`
+- if an istr.range instance, the same istr.range will be returned
 
-    `len(istr(range(3)))` ==> `3`
+- if an istr, the same istr will be used
 
-- if an istr.range instance, the same istr.range will be returned
+    ```
+    istr(istr('4')) ==> istr ('4')
+    ```
 
-## More than one parameter for istr
+#### More than one parameter for istr
 It is possible to give more than one parameter, in which case a tuple
 of the istrs of the parameters will be returned, which can be handy
 to unpack multiple values, e.g.
 
-`a, b, c = istr(5, 6, 7)` ==> `a=istr('5') , b=istr('6'), c=istr('7')`
+```
+a, b, c = istr(5, 6, 7) ==> a=istr('5') , b=istr('6'), c=istr('7') 
+```
 
-## test for even/odd
-It is possible to test for even/odd with the
+#### test for even/odd
+It is possible to test for even/odd (provided the istt can be interpreted as an int) with the
 
 `is_even` and `is_odd` method, e.g.
 
 ```
-print(istr(4).is_even())
-print(istr(5).is_odd())
+istr(4).is_even()) ==> True
+istr(5).is_odd()) ==> True
 ```
-This will print `True` twice.
-
-## reverse an istr
+#### reverse an istr
 The method `istr.reversed()` will return the an istr with the reversed content:
 ```
-print(repr(istr(456).reversed()))
-print(repr(istr('0456').reversed()))
-```
-result:
-```
-istr('654')
-istr('6540')
+istr(456).reversed() ==> istr('654')
+istr('0456').reversed() ==> istr('6540')
 ```
 The same can -of course- be achieved with
 ```
-print(repr(istr(456)[::-1]))
-print(repr(istr('0456')[::-1]))
+istr(456)[::-1] ==> istr('654')
+istr('0456')[::-1] ==> istr('6540')
 ```
-Note that is impossible to reverse a negative istr.
+> [!NOTE]
+>
+> It is possible to reverse a negative istr, but the result can't be interpreted as an int anymore.
+>
+> ```
+> istr(-456) ==> TypeError
+> ```
 
-## enumerate with istrs
+#### enumerate with istrs
 
 The `istr.enumerate` method can be used just as the builtin enumerate function.
 The iteration counter however is an istr rather than an int. E.g. 
+
 ```
     for i,c in istr.enumerate('abc'):
         print(f'{repr(i)} {c}')
 ```
 prints
 ```
 istr('0') a
 istr('1') b
 istr('2') c
 ```
 
-## concatenate an iterable
+#### concatenate an iterable
 
 The `istr.concat` method can be useful to map all items of an iterable
 to `istr` and then concatenate these.
 
-`list(istr.concat(((1,2),(3,4)))` ==> `istr([12,34])`
+`
 
-`list(istr.concat(itertools.permutations(range(3),2)))` ==> `[istr('01'), istr('02'), istr('10'), istr('12'), istr('20'), istr('21')]` 
+```
+list(istr.concat(((1,2),(3,4))) ==> istr([12,34])
+list(istr.concat(itertools.permutations(range(3),2))) ==> 
+    [istr('01'), istr('02'), istr('10'), istr('12'), istr('20'), istr('21')] 
+```
 
-## generate istr with digits
+#### generate istr with digits
 
 The class method `digits` can be used to return an istr of digits according to a given specification.
 The method takes either no or a number of arguments.
 
 If no arguments are given, the result will be istr('0123456789').
 
 The given argument(s) result in a range of digits.
 
 - `<n>` ==> n
-- `<n-m> ==> n, n+1, ..., m
+- `<n-m>` ==> n, n+1, ..., m
 - `-n>` ==> 0, 1, ... n
 - `n->` ==> n, n+1, ..., 9
 - `''` ==> 0, 1, ..., 9
 
-(n and m must be digit between 0 and 9)
+(n and m must be digits between 0 and 9)
 
 The final result is an istr composed of the given range(s).
 
 Here are some examples:
 
-- `istr.digits()` ==> `istr('0123456789')`
-- `istr.digits('')` ==> `istr('0123456789')`
-- `istr.digits('1')` ==> `istr('1')`
-- `istr.digits('3-')` ==> `istr('3456789')`
-- `istr.digits('-3')` ==> `istr('0123')`
-- `istr('1-4', '6', '8-9')` ==> `istr('1234689')`
-- `istr('1', '1-2', '1-3')` ==> `istr('11213')`
+```
+istr.digits() ==> istr('0123456789')
+istr.digits('') ==> istr('0123456789')
+istr.digits('1') ==> istr('1')
+istr.digits('3-') ==> istr('3456789')
+istr.digits('-3') ==> istr('0123')
+istr('1-4', '6', '8-9') ==> istr('1234689')
+istr('1', '1-2', '1-3') ==> istr('11213')
+```
 
 
-## Subclassing istr
+#### Subclassing istr
 When a class is derived from istr, all methods will return that newly derived class. 
 
 E.g.
 ```
 class jstr(istr):
     ...
     
 print(repr(jstr(4) * jstr(5)))
 ```
 will print `jstr('20')`
 
-## Changing the way repr works
+#### Changing the way repr works
 
 It is possible to control the way an `istr` instance will be repr'ed.
 
 By default, the `istr('5')` is represented as `istr('5')`.
 
 With the istr.repr_mode() context manager, that can be changed:
 ```
@@ -326,15 +450,31 @@
 ```
 This will print
 ```
 '5'
 5
 istr('5')
 ```
-Note that the way an `istr` is represented is determined at initialization.
+If the repr_mode is `'int'` and the istr can't be interpreted as an int the string `nan` (not a number) will be returned:
+
+```
+ with istr.repr_mode('int'):
+    abc = istr('abc')
+    print(repr(abc))
+```
+
+This will print
+
+```
+nan
+```
+
+> [!NOTE]
+>
+> The way an `istr` is represented is determined at initialization.
 
 It is also possible to set the repr mode without a context manager:
 
 ```
 istr.repr_mode('str')
 five = istr('5')
 print(repr(five))
@@ -345,21 +485,21 @@
 ```
 Finally, the current repr mode can be queried with `istr.repr_mode()`. So upon start:
 ```
 print(repr(istr.repr_mode()))
 ```
 will output `istr`.
 
-## Changing the base system
+#### Changing the base system
 
 By default, `istr` works in base 10. However it is possible to change the base system with the `istr.base()` context manager / method.
 
 Any base between 2 and 36 may be used.
 
-Note that the integer is always stored in base 10 mode, but the string
+Note that the integer is **always** stored in base 10 mode, but the string
 representation will reflect the chosen base (at time of initialization).
 
 Some examples:
 ```
 with istr.base(16):
     a = istr('7fff')
     print(int(a))
@@ -387,100 +527,118 @@
 ```
 Finally, the current base can be queried with `istr.base()`, so upon start:
 ```
 print(istr.base())
 ```
 will result in `10`.
 
-## Changing the format of the string
-
-By default, `istr` does not change the way an istr is stored when a str is to initialize:
+#### Changing the format of the string
 
-`repr('4'))` ==> `istr('4')`
+When an  istr is initialized with a string the istr will be just stored as such.
 
-`repr(' 4'))` ==> `istr(' 4')`
-
-`repr('4  '))` ==> `istr('4  ')`
+```
+repr('4')) ==> istr('4')
+repr(' 4')) ==> istr(' 4')
+repr('4  ')) ==> istr('4  ')
+```
 
-For initializing with an int (or other numeric) value, the string is simply the str representation
+For initializing with an int (or other numeric) value, the string is by default simply the str representation
 
-`repr(4))` ==> `istr('4')`
+```
+repr(4)) ==> istr('4')
+```
 
-With the `istr.format()` context manager this behavior can be changed.
+ With the `istr.int_format()` context manager this behavior can be changed.
 If the format specifier is a number, most likely a single digit, that
 will be the minimum number of characters in the string:
+
 ```
-with istr.format('3'):
+with istr.int_format('3'):
     print(repr(istr(1)))
     print(repr(istr(12)))
     print(repr(istr(123)))
     print(repr(istr(1234)))
 ```
 will print
 ```
 istr('  1')
 istr(' 12')
 istr('123')
 istr('1234')
 ```
 If the string starts with a `0`, the string will be zero filled:
 ```
-with istr.format('03'):
+with istr.int_format('03'):
     print(repr(istr(1)))
     print(repr(istr(12)))
     print(repr(istr(123)))
     print(repr(istr(1234)))
 ```
 will print
 ```
 istr('001')
 istr('012')
 istr('123')
 istr('1234')
 ```
-Note that if a format other than the default `''` is used, the string will reformatted even if the `istr` is specified with a string:
-```
-with istr.format('03'):
-    print(repr(istr('  12 ')))
-```
-will result in `istr('0012')`
+> [!NOTE]
+>
+>  if a string is used to initialize an istr AND that string can be interpreted as an int. the string will reformatted:
+>
+> ```
+> with istr.int_format('03'):
+>     print(repr(istr('  12 ')))
+> ```
+>
+> will result in
+>
+> ```
+> istr('0012')
+> ```
+
+> [!NOTE]
+>
+> For bases other than 10, the string will never be reformatted!
 
-Remark: For bases other than 10, the string will never be reformatted!
+### Overview of operations
 
-## Operations
-----------------------------
-```
 The table below shows whether the string or the int version of istr is applied.
 
-operator/function   int  str  Example
-----------------------------
-+                    x        istr(20) + 3 ==> istr('23')
-_                    x        istr(20) - 3 ==> istr('17')
-*                    x        istr(20) * 3 ==> istr('60')
-/                    x        istr(20) / 3 ==> istr('6')
-//                   x        istr(20) // 3 ==> istr('6')
-%                    x        istr(20) % 3 ==> istr('2')
-divmod               x        divmod(istr(20), 3) ==> (istr('6'), istr('2'))
-**                   x        istr(2) ** 3 ==> istr('8')
-@                         x   istr(20) @ 3 ==> istr('202020')
-==                   x    x   istr(20) == 20 ==> True | istr(20) == '20' ==> True
-|                         x   istr(20) | 5 ==> istr('205')
-abs                  x        abs(istr(-20)) ==> istr('20')
-bool                 x        bool(istr(' 0 ')) ==> False
-<=, <, >, >=         x        istr('100') > istr('2') ==> True
-slicing              x        istr(12345)[1:3] ==> istr('23')
-iterate                   x   [x for x in istr(20)] ==> [istr('2'), istr('0')
-len                       x   len(istr(' 20 ')) ==> 4
-count                     x   istr(100),count('0') ==> 2
-index                     x   istr(' 100 ').index('0') ==> 2
-----------------------------
 ```
-## Test script
+operator/function   int  str   Example
+-----------------------------------------------------------------------------------------
++                    x         istr(20) + 3 ==> istr('23')
+_                    x         istr(20) - 3 ==> istr('17')
+*                    x         istr(20) * 3 ==> istr('60')
+/                    x         istr(20) / 3 ==> istr('6')
+//                   x         istr(20) // 3 ==> istr('6')
+%                    x         istr(20) % 3 ==> istr('2')
+divmod               x         divmod(istr(20), 3) ==> (istr('6'), istr('2'))
+**                   x         istr(2) ** 3 ==> istr('8')
+@                         x    istr(20) @ 3 ==> istr('202020')
+==                   x    x    istr(20) == 20 ==> True | istr(20) == '20' ==> True
+|                         x    istr(20) | 5 ==> istr('205')
+abs                  x         abs(istr(-20)) ==> istr('20')
+bool                 x    x *) bool(istr(' 0 ')) ==> False | istr('') ==> False
+<=, <, >, >=         x         istr('100') > istr('2') ==> True
+slicing                   x    istr(12345)[1:3] ==> istr('23')
+iterate                   x    [x for x in istr(20)] ==> [istr('2'), istr('0')
+len                       x    len(istr(' 20 ')) ==> 4
+count                     x    istr(100),count('0') ==> 2
+index                     x    istr(' 100 ').index('0') ==> 2
+split                     x    istr('1 2').split() ==> (istr('1'), istr('2'))
+other string methods      x    istr('aAbBcC').lower() ==> istr('aabbcc')
+                               istr('aAbBcC').islower() ==> False
+                               istr('  abc   ').strip() ==> istr('abc')
+-----------------------------------------------------------------------------------------
+*) str is applied if is_int() is False
+```
+### Test script
 There's an extensive pytest script in the `\tests` directory.
 
-This script also shows clearly the ways istr can be used.
+This script also shows clearly the ways istr can be used, including several edge cases. Highly recommended to have a look at.
 
-## Badges
+### Badges
 ![PyPI](https://img.shields.io/pypi/v/istr-python) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/istr-python) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/istr-python)
 
 ![PyPI - License](https://img.shields.io/pypi/l/istr-python) ![Black](https://img.shields.io/badge/code%20style-black-000000.svg) 
- ![GitHub last commit](https://img.shields.io/github/last-commit/salabim/istr)
+![GitHub last commit](https://img.shields.io/github/last-commit/salabim/istr)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `istr_python-0.2.0.post0/README.md` & `istr_python-1.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-<img src="https://www.salabim.org/istr_logo.png" width=500>
+ <img src="https://www.salabim.org/istr_logo.png" width=500>
 
-## Introduction
+### Introduction
 
 The istr module has exactly one class: istr.
 
 With this it is possible to interpret strings as if they were integers.
 
-This can be very handy for solving puzzles, but also for other purposes.</br>
-For instance the
-famous send more money puzzle
+This can be very handy for solving puzzles, but also for other purposes.
+For instance the famous send more money puzzle, where each letter has to be replaced by a unique digit (0-9)
+
 ```
   S E N D
   M O R E
 --------- +
 M O N E Y
 ```
 can be nicely, albeit not very efficient, coded as:
@@ -24,280 +24,404 @@
     if m and ((s|e|n|d) + (m|o|r|e) == (m|o|n|e|y)):
         print(f' {s|e|n|d}')
         print(f' {m|o|r|e}')
         print('-----')
         print(f'{m|o|n|e|y}')
 ```
 
-And it is a nice demonstration of extending a class (str) with extra and changed functionality.
+Of, if we want to add all the digits in a string:
+
+```
+sum_digits = sum(istr('9282334'))  # answer 31
+```
+
+And the module is a demonstration of extending a class (str) with extra and changed functionality.
 
-## Installation
+### Installation
 Installing istr with pip is easy.
 ```
 $ pip install istr-python
 ```
 or when you want to upgrade,
 ```
 $ pip install istr-python --upgrade
 ```
 Alternatively, istr.py can be just copied into you current work directory from GitHub (https://github.com/salabim/istr).
 
 No dependencies!
 
-## Usage
+### Usage
+#### Start
+
 Just start with
 
 ```
 from istr import istr
 ```
 
-Now we can define some istrs:
+#### Use istrs as if the were int
+
+We can define an istr:
 ```
 four = istr('4')
 five = istr('5')
 ```
-Then we can do
+The variables `four`  and `five` can now be used as if they were int:
+
 ```
-x= four * five
+twenty = four * five
 ```
 , after which x is `istr('20')`
 
-And now we can do
+The same can be done with
+
+```
+twenty = 4 * five
+```
+
+or
+
+```
+twenty = four * 5
+```
+
+And now `twenty` can be used as if it was an int as well. So:
+
 ```
-print(x == 20)
-print(x == '20')
+twenty - four
 ```
-resulting in two times `True`. That's because istrs instances are treated as int, although they are strings.
 
-That means that we can also say
+is `istr('16')`
+
+We can do all the usual arithmetic operations on istrs, e.g.
+
 ```
-print(x < 30)
-print(x >= '10')
+-four + (twenty / 2)
+```
+
+is `istr('6')`
+
+And we can test for equality, So:
+
 ```
-again resulting in two times `True`.
+twenty == 20
+```
+is True.
+
+But as istrs are also strings. So
+
+```
+twenty == '20'
+```
+
+is also True!
+
+For the order comparisons (<=, <, >, >=), the istr is always interpreted as an int:
+
+That means that  both
+```
+twenty < 30
+twenty >= '10' # here '10' is converted to 10 for the comparison
+```
+are `True`.
 
 In contrast to an ordinary string
 ```
 print(four + five)
 ```
 prints `9`, as istr are treated as ints.
 
-Please note that `four` and `five` could have also be initialized with
+Please note that `four`  could have also been initialized with
 ```
 four = istr(4)
-five = istr(5)
 ```
 or even
 ```
 four, five = istr(4, 5)
 ```
 
-But how can we concatenate istrs? Just use the or operator (|): 
+> [!NOTE]
+>
+> All calculations are strictly integer calculations. That means that if a float variale is ever produced it will be converted to an int.
+> Also divisions are always floor divisions!
+
+#### Use istrs as string
+
+We should realize that istrs are in fact strings.
+
+In order to concatenate two istrs (or an istr and a str), we cannot use the `four + five` operator as
+
+that would be `istr(9)`.
+
+In order to concatenate istrs,  we use the or operator (`|`). So
+
 ```
-print(four | five)
+four | five
 ```
-will output `45`.
-
-And the result is again an istr.
+will be `istr(`45`).
 
 That means that
 ```
 (four | five) / 3
 ```
 is `istr('9')`.
 
-In order to repeat a string in the usual sense, you cannot use `3 * four`, as that woud be `12`. 
+In order to repeat a string in the usual sense, you cannot use `3 * four`, as that would be `12`. 
+
+In order to repeat we use the matrix multiplication operator (`@`). So
+
+ `3 @ four`
+
+ is istr(`444`). As is `four @ 3`.
+
+> [!NOTE]
+>
+> It is not allowed to use the `@` operator for two istrs. So, `four @ five` raises a TypeError.
+
+#### istrs that can't be interpreted as an int
 
-We use the matrix multiplication operator (@) for this. So `3 @ four` is `444`. As is `four @ 3`.
+Although usualy, istrs are to be interpreted as an int, that's not a requirement.
+
+So
 
-Also allowed are
 ```
-abs(four)
--four 
+istr('abc')
 ```
 
-The bool operator works on the integer value of an istr. So
-`bool(istr('0'))` ==> `False`
-`bool(istr('1'))` ==> `True`
-The code
+or
+
+```
+istr(1,2,3)
+```
+
+are accepted.
+
+But, we can't do any arithmetic with them. 
+
+If we try
+
 ```
-if istr('0'):
-    print('True')
-else:
-    print('False')
+istr('abc') + 5
 ```
-will print `False`
 
-For the in operator, an istr is treated as an ordinary string, although it is possible to use ints as well:
+a TypeError will be raised.
+
+That holds for any arithmetic we try.
+
+If we want to test if an istr can be interpreted (and thus used in an arithmetic expression). we can use the `is_int()` method. So
+
+```ìstr(20).is_int()```
+
+is `True`, wherea
+
+```ìstr('abc').is_int()```
+
+is `False`.
+
+
+
+The bool operator works normally on the integer value of an istr. So
+
+`bool(istr('0'))` ==> `False`
+`bool(istr('1'))` ==> `True`
+
+If the istr can't be interpreted as an int, the string will be used to test. So
+
+`bool(istr('abc'))` ==> `False`
+`bool(istr(''))` ==> `True`
+
+#### Other operators
+
+For the `in` operator, an istr is treated as an ordinary string, although it is possible to use ints as well:
+
 ```
 '34' in istr(1234)
 34 in istr(1234)
 ```
 On the left hand side an istr is always treated as a string:
 ```
 istr(1234) in '01234566890ABCDEF'
 ```
 
-Note that all calculations are strictly integer calculations. That means that if a float variale is ever produced it will be converted to an int.
-Also divisions are always floor divisions!
-
-There's a special case for `istr('')`. This is a proper empty string, but also represents the value of 0.
-That is to allow for `istr('').join(i for i in '01234)'`, resulting in `istr('01234')`.
-
 Sorting a list of istrs is based on the integer value, not the string. So
 
-`' '.join(sorted('1 3 2 4 5 6 11 7 9 8 10 12 0'.split()))`
+```
+' '.join(sorted('1 3 2 4 5 6 11 7 9 8 10 12 0'.split()))
+```
 
 is
 
-`'0 1 10 11 2 3 4 5 6 7 8 9'`
+```
+'0 1 10 11 2 3 4 5 6 7 8 9'
+```
 
 ,whereas
 
-`' '.join(sorted(istr('1 3 2 4 5 6 11 7 9 8 10 12 0'.split())))`
+```
+' '.join(sorted(istr('1 3 2 4 5 6 11 7 9 8 10 12 0'.split()))
+```
 
 is 
 
-`'0 1 2 3 4 5 6 7 8 9 10 11'`
+```
+'0 1 2 3 4 5 6 7 8 9 10 11'
+```
 
-## Using other values for istr than numeric value or str
+#### Using other values for istr than numeric value or str
 Apart from with simple numeric (to be interpreted as an int) or str, istr can be initialized with
 several other types:
 
-- if a dict (or subtype of dict), the same type dict will be returned with all values istr'ed
+- if a dict (or subtype of dict), the same type dict will be returned with all *values* istr'ed
 
-    `istr({0: 0, 1: 1, 2: 4})` ==> `{0: istr('0'), 1: istr('1'), 2: istr('4')}`
+    ```
+    istr({0: 0, 1: 1, 2: 4}) ==> {0: istr('0'), 1: istr('1'), 2: istr('4')}
+    ```
 
 - if an iterator, the iterator will be mapped with istr
 
-    `istr(i * i for i in range(3))` ==> `<map object>`
-
-    `list(istr(i * i for i in range(3)))` ==> `[istr('0'), istr('1'), istr('4')]`
+    ```
+    istr(i * i for i in range(3)) ==> <map object>
+    list(istr(i * i for i in range(3))) ==> [istr('0'), istr('1'), istr('4')]
+    ```
 
 - if an iterable, the same type will be returned with all elements istr'ed
 
-    `istr([0, 1, 4])` ==> `[istr('0'), istr('1'), istr('4')]`
-
-    `istr((0, 1, 4))` ==> `(istr('0'), istr('1'), istr('4'))`
-
-    `istr({0, 1, 4})` ==> `{istr('4'), istr('0'), istr('1')} ## or similar`
+    ```
+    istr([0, 1, 4]) ==> [istr('0'), istr('1'), istr('4')]
+    istr((0, 1, 4)) ==> (istr('0'), istr('1'), istr('4'))
+    istr({0, 1, 4}) ==> `{istr('4'), istr('0'), istr('1')}  # or similar
+    ```
 
 - if a range, an istr.range instance will be returned
-    
-    `istr(range(3))` ==> `istr.range(3)`
+  
+    ```
+  istr(range(3))` ==> `istr.range(3)
+    list(istr(range(3)))` ==> `[istr('0'), istr('1'), istr('2')]
+  len(istr(range(3)))` ==> `3
+  ```
 
-    `list(istr(range(3)))` ==> `[istr('0'), istr('1'), istr('2')]`
+- if an istr.range instance, the same istr.range will be returned
 
-    `len(istr(range(3)))` ==> `3`
+- if an istr, the same istr will be used
 
-- if an istr.range instance, the same istr.range will be returned
+    ```
+    istr(istr('4')) ==> istr ('4')
+    ```
 
-## More than one parameter for istr
+#### More than one parameter for istr
 It is possible to give more than one parameter, in which case a tuple
 of the istrs of the parameters will be returned, which can be handy
 to unpack multiple values, e.g.
 
-`a, b, c = istr(5, 6, 7)` ==> `a=istr('5') , b=istr('6'), c=istr('7')`
+```
+a, b, c = istr(5, 6, 7) ==> a=istr('5') , b=istr('6'), c=istr('7') 
+```
 
-## test for even/odd
-It is possible to test for even/odd with the
+#### test for even/odd
+It is possible to test for even/odd (provided the istt can be interpreted as an int) with the
 
 `is_even` and `is_odd` method, e.g.
 
 ```
-print(istr(4).is_even())
-print(istr(5).is_odd())
+istr(4).is_even()) ==> True
+istr(5).is_odd()) ==> True
 ```
-This will print `True` twice.
-
-## reverse an istr
+#### reverse an istr
 The method `istr.reversed()` will return the an istr with the reversed content:
 ```
-print(repr(istr(456).reversed()))
-print(repr(istr('0456').reversed()))
-```
-result:
-```
-istr('654')
-istr('6540')
+istr(456).reversed() ==> istr('654')
+istr('0456').reversed() ==> istr('6540')
 ```
 The same can -of course- be achieved with
 ```
-print(repr(istr(456)[::-1]))
-print(repr(istr('0456')[::-1]))
+istr(456)[::-1] ==> istr('654')
+istr('0456')[::-1] ==> istr('6540')
 ```
-Note that is impossible to reverse a negative istr.
+> [!NOTE]
+>
+> It is possible to reverse a negative istr, but the result can't be interpreted as an int anymore.
+>
+> ```
+> istr(-456) ==> TypeError
+> ```
 
-## enumerate with istrs
+#### enumerate with istrs
 
 The `istr.enumerate` method can be used just as the builtin enumerate function.
 The iteration counter however is an istr rather than an int. E.g. 
+
 ```
     for i,c in istr.enumerate('abc'):
         print(f'{repr(i)} {c}')
 ```
 prints
 ```
 istr('0') a
 istr('1') b
 istr('2') c
 ```
 
-## concatenate an iterable
+#### concatenate an iterable
 
 The `istr.concat` method can be useful to map all items of an iterable
 to `istr` and then concatenate these.
 
-`list(istr.concat(((1,2),(3,4)))` ==> `istr([12,34])`
+`
 
-`list(istr.concat(itertools.permutations(range(3),2)))` ==> `[istr('01'), istr('02'), istr('10'), istr('12'), istr('20'), istr('21')]` 
+```
+list(istr.concat(((1,2),(3,4))) ==> istr([12,34])
+list(istr.concat(itertools.permutations(range(3),2))) ==> 
+    [istr('01'), istr('02'), istr('10'), istr('12'), istr('20'), istr('21')] 
+```
 
-## generate istr with digits
+#### generate istr with digits
 
 The class method `digits` can be used to return an istr of digits according to a given specification.
 The method takes either no or a number of arguments.
 
 If no arguments are given, the result will be istr('0123456789').
 
 The given argument(s) result in a range of digits.
 
 - `<n>` ==> n
-- `<n-m> ==> n, n+1, ..., m
+- `<n-m>` ==> n, n+1, ..., m
 - `-n>` ==> 0, 1, ... n
 - `n->` ==> n, n+1, ..., 9
 - `''` ==> 0, 1, ..., 9
 
-(n and m must be digit between 0 and 9)
+(n and m must be digits between 0 and 9)
 
 The final result is an istr composed of the given range(s).
 
 Here are some examples:
 
-- `istr.digits()` ==> `istr('0123456789')`
-- `istr.digits('')` ==> `istr('0123456789')`
-- `istr.digits('1')` ==> `istr('1')`
-- `istr.digits('3-')` ==> `istr('3456789')`
-- `istr.digits('-3')` ==> `istr('0123')`
-- `istr('1-4', '6', '8-9')` ==> `istr('1234689')`
-- `istr('1', '1-2', '1-3')` ==> `istr('11213')`
+```
+istr.digits() ==> istr('0123456789')
+istr.digits('') ==> istr('0123456789')
+istr.digits('1') ==> istr('1')
+istr.digits('3-') ==> istr('3456789')
+istr.digits('-3') ==> istr('0123')
+istr('1-4', '6', '8-9') ==> istr('1234689')
+istr('1', '1-2', '1-3') ==> istr('11213')
+```
 
 
-## Subclassing istr
+#### Subclassing istr
 When a class is derived from istr, all methods will return that newly derived class. 
 
 E.g.
 ```
 class jstr(istr):
     ...
     
 print(repr(jstr(4) * jstr(5)))
 ```
 will print `jstr('20')`
 
-## Changing the way repr works
+#### Changing the way repr works
 
 It is possible to control the way an `istr` instance will be repr'ed.
 
 By default, the `istr('5')` is represented as `istr('5')`.
 
 With the istr.repr_mode() context manager, that can be changed:
 ```
@@ -313,15 +437,31 @@
 ```
 This will print
 ```
 '5'
 5
 istr('5')
 ```
-Note that the way an `istr` is represented is determined at initialization.
+If the repr_mode is `'int'` and the istr can't be interpreted as an int the string `nan` (not a number) will be returned:
+
+```
+ with istr.repr_mode('int'):
+    abc = istr('abc')
+    print(repr(abc))
+```
+
+This will print
+
+```
+nan
+```
+
+> [!NOTE]
+>
+> The way an `istr` is represented is determined at initialization.
 
 It is also possible to set the repr mode without a context manager:
 
 ```
 istr.repr_mode('str')
 five = istr('5')
 print(repr(five))
@@ -332,21 +472,21 @@
 ```
 Finally, the current repr mode can be queried with `istr.repr_mode()`. So upon start:
 ```
 print(repr(istr.repr_mode()))
 ```
 will output `istr`.
 
-## Changing the base system
+#### Changing the base system
 
 By default, `istr` works in base 10. However it is possible to change the base system with the `istr.base()` context manager / method.
 
 Any base between 2 and 36 may be used.
 
-Note that the integer is always stored in base 10 mode, but the string
+Note that the integer is **always** stored in base 10 mode, but the string
 representation will reflect the chosen base (at time of initialization).
 
 Some examples:
 ```
 with istr.base(16):
     a = istr('7fff')
     print(int(a))
@@ -374,100 +514,118 @@
 ```
 Finally, the current base can be queried with `istr.base()`, so upon start:
 ```
 print(istr.base())
 ```
 will result in `10`.
 
-## Changing the format of the string
-
-By default, `istr` does not change the way an istr is stored when a str is to initialize:
+#### Changing the format of the string
 
-`repr('4'))` ==> `istr('4')`
+When an  istr is initialized with a string the istr will be just stored as such.
 
-`repr(' 4'))` ==> `istr(' 4')`
-
-`repr('4  '))` ==> `istr('4  ')`
+```
+repr('4')) ==> istr('4')
+repr(' 4')) ==> istr(' 4')
+repr('4  ')) ==> istr('4  ')
+```
 
-For initializing with an int (or other numeric) value, the string is simply the str representation
+For initializing with an int (or other numeric) value, the string is by default simply the str representation
 
-`repr(4))` ==> `istr('4')`
+```
+repr(4)) ==> istr('4')
+```
 
-With the `istr.format()` context manager this behavior can be changed.
+ With the `istr.int_format()` context manager this behavior can be changed.
 If the format specifier is a number, most likely a single digit, that
 will be the minimum number of characters in the string:
+
 ```
-with istr.format('3'):
+with istr.int_format('3'):
     print(repr(istr(1)))
     print(repr(istr(12)))
     print(repr(istr(123)))
     print(repr(istr(1234)))
 ```
 will print
 ```
 istr('  1')
 istr(' 12')
 istr('123')
 istr('1234')
 ```
 If the string starts with a `0`, the string will be zero filled:
 ```
-with istr.format('03'):
+with istr.int_format('03'):
     print(repr(istr(1)))
     print(repr(istr(12)))
     print(repr(istr(123)))
     print(repr(istr(1234)))
 ```
 will print
 ```
 istr('001')
 istr('012')
 istr('123')
 istr('1234')
 ```
-Note that if a format other than the default `''` is used, the string will reformatted even if the `istr` is specified with a string:
-```
-with istr.format('03'):
-    print(repr(istr('  12 ')))
-```
-will result in `istr('0012')`
+> [!NOTE]
+>
+>  if a string is used to initialize an istr AND that string can be interpreted as an int. the string will reformatted:
+>
+> ```
+> with istr.int_format('03'):
+>     print(repr(istr('  12 ')))
+> ```
+>
+> will result in
+>
+> ```
+> istr('0012')
+> ```
+
+> [!NOTE]
+>
+> For bases other than 10, the string will never be reformatted!
 
-Remark: For bases other than 10, the string will never be reformatted!
+### Overview of operations
 
-## Operations
-----------------------------
-```
 The table below shows whether the string or the int version of istr is applied.
 
-operator/function   int  str  Example
-----------------------------
-+                    x        istr(20) + 3 ==> istr('23')
-_                    x        istr(20) - 3 ==> istr('17')
-*                    x        istr(20) * 3 ==> istr('60')
-/                    x        istr(20) / 3 ==> istr('6')
-//                   x        istr(20) // 3 ==> istr('6')
-%                    x        istr(20) % 3 ==> istr('2')
-divmod               x        divmod(istr(20), 3) ==> (istr('6'), istr('2'))
-**                   x        istr(2) ** 3 ==> istr('8')
-@                         x   istr(20) @ 3 ==> istr('202020')
-==                   x    x   istr(20) == 20 ==> True | istr(20) == '20' ==> True
-|                         x   istr(20) | 5 ==> istr('205')
-abs                  x        abs(istr(-20)) ==> istr('20')
-bool                 x        bool(istr(' 0 ')) ==> False
-<=, <, >, >=         x        istr('100') > istr('2') ==> True
-slicing              x        istr(12345)[1:3] ==> istr('23')
-iterate                   x   [x for x in istr(20)] ==> [istr('2'), istr('0')
-len                       x   len(istr(' 20 ')) ==> 4
-count                     x   istr(100),count('0') ==> 2
-index                     x   istr(' 100 ').index('0') ==> 2
-----------------------------
 ```
-## Test script
+operator/function   int  str   Example
+-----------------------------------------------------------------------------------------
++                    x         istr(20) + 3 ==> istr('23')
+_                    x         istr(20) - 3 ==> istr('17')
+*                    x         istr(20) * 3 ==> istr('60')
+/                    x         istr(20) / 3 ==> istr('6')
+//                   x         istr(20) // 3 ==> istr('6')
+%                    x         istr(20) % 3 ==> istr('2')
+divmod               x         divmod(istr(20), 3) ==> (istr('6'), istr('2'))
+**                   x         istr(2) ** 3 ==> istr('8')
+@                         x    istr(20) @ 3 ==> istr('202020')
+==                   x    x    istr(20) == 20 ==> True | istr(20) == '20' ==> True
+|                         x    istr(20) | 5 ==> istr('205')
+abs                  x         abs(istr(-20)) ==> istr('20')
+bool                 x    x *) bool(istr(' 0 ')) ==> False | istr('') ==> False
+<=, <, >, >=         x         istr('100') > istr('2') ==> True
+slicing                   x    istr(12345)[1:3] ==> istr('23')
+iterate                   x    [x for x in istr(20)] ==> [istr('2'), istr('0')
+len                       x    len(istr(' 20 ')) ==> 4
+count                     x    istr(100),count('0') ==> 2
+index                     x    istr(' 100 ').index('0') ==> 2
+split                     x    istr('1 2').split() ==> (istr('1'), istr('2'))
+other string methods      x    istr('aAbBcC').lower() ==> istr('aabbcc')
+                               istr('aAbBcC').islower() ==> False
+                               istr('  abc   ').strip() ==> istr('abc')
+-----------------------------------------------------------------------------------------
+*) str is applied if is_int() is False
+```
+### Test script
 There's an extensive pytest script in the `\tests` directory.
 
-This script also shows clearly the ways istr can be used.
+This script also shows clearly the ways istr can be used, including several edge cases. Highly recommended to have a look at.
 
-## Badges
+### Badges
 ![PyPI](https://img.shields.io/pypi/v/istr-python) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/istr-python) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/istr-python)
 
 ![PyPI - License](https://img.shields.io/pypi/l/istr-python) ![Black](https://img.shields.io/badge/code%20style-black-000000.svg) 
- ![GitHub last commit](https://img.shields.io/github/last-commit/salabim/istr)
+![GitHub last commit](https://img.shields.io/github/last-commit/salabim/istr)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `istr_python-0.2.0.post0/istr/istr.py` & `istr_python-1.0.0/istr/istr.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,51 @@
-import functools
-import math
-
 #     _       _
 #    (_) ___ | |_  _ __
 #    | |/ __|| __|| '__|
 #    | |\__ \| |_ | |
 #    |_||___/ \__||_|
 # strings you can count on
 
-__version__ = "0.2.0"
+__version__ = "1.0.0"
 import functools
 import math
 
 """
 changelog
 
+version 1.0.0 2024-05-06
+------------------------
+With this version, istrs do not have to be interpretable as an int anymore.
+Only when arithmetic and friends are to be carried with an istr, that's a requirement.
+
+So now we can say
+    a = istr('1 2 3')
+    print(a.split())
+and get
+    [istr('1'), istr('2'), istr('3')]
+But
+    a = istr('1 2 3')
+    b = a + 1
+will raise
+    TypeError: unsupported operand for +: istr('1 2 3') and 1
+    
+It is possible to check if an istr can be interpreted as an int with the is_int method:
+    a = istr('1 2 3')
+    print(a.is_int()) 
+will give
+    False 
+    
+This also means that there is no reason for istr('') to be interpretable as 0. So it isn't anymore.
+And reversed() now also works with negative numbers, although the result can't be used in calculations.
+
+The method / context manager format has been renamed to int_format.
+
+The bool method now operates on the string if it can not be interpreted as an int.
+That means that bool(istr('')) is False. For any other istr where is_int() is True, bool will be True.
+
 version 0.2.0 2024-04-30
 ----------------------
 Added __iter__ method__ .
     So now,
         for c in istr('123'):
             ...
         results in c values that are istrs 
@@ -237,17 +264,19 @@
         it is possible to give more than one parameter, in which case a tuple
         of the istrs of the parameters will be returned, which can be handy
         to multiple assign, e.g.
             a, b, c = istr(5, 6, 7) ==> a=istr("5") , b=istr("6"), c=istr("7")"""
 
     __slots__ = ("_as_int", "_as_repr")
 
-    _format = ""
-    _mode = "istr"
+    _int_format = ""
+    _repr_mode = "istr"
     _base = 10
+    _nan = "nan"
+    _force_istr_repr = False
 
     @staticmethod
     def _to_base(number, base):
         if number < 0:
             raise ValueError(f"negative numbers are not allowed for base {base}")
         result = ""
         while number:
@@ -258,16 +287,38 @@
     @classmethod
     def _to_int(cls, value):
         try:
             if cls._base != 10 and isinstance(value, str):
                 return int(value, cls._base)
             else:
                 return int(value)
-        except (ValueError, TypeError):
-            raise ValueError(f"unable to convert {repr(value)} to int (base {cls._base})")
+        except:
+            return cls._nan
+
+    def _check_is_int(self, *args, right=False):
+        operator = args[len(args) == 2]
+        if len(args) == 2:
+            other = args[0]
+            if not self.is_int() or self._to_int(other) == self._nan:
+                self.__class__._force_istr_repr = True
+                if right:
+                    message = f"unsupported operand for {operator}: {repr(other)} and {repr(self)}"
+                else:
+                    message = f"unsupported operand for {operator}: {repr(self)} and {repr(other)}"
+                self.__class__._force_istr_repr = False
+                raise TypeError(message)
+        else:
+            if not self.is_int():
+                self.__class__._force_istr_repr = True
+                message = f"unsupported operand for {operator}: {repr(self)}"
+                self.__class__._force_istr_repr = False
+                raise TypeError(message)
+
+    def _rcheck_is_int(self, *args):
+        self._check_is_int(*args, right=True)
 
     def __new__(cls, *value):
         if len(value) == 0:
             raise TypeError("no parameter given")
         if len(value) == 1:
             value = value[0]  # normal case of 1 parameter
         if isinstance(value, range):
@@ -278,170 +329,208 @@
             return value
         if isinstance(value, dict):
             return type(value)((k, cls(v)) for k, v in value.items())
         if not isinstance(value, (str, type)) and hasattr(value, "__iter__"):
             if hasattr(value, "__next__"):
                 return map(functools.partial(cls), value)
             return type(value)(map(functools.partial(cls), value))
-        if value == "":
-            as_str = ""
-            as_int = 0
+
+        as_int = cls._to_int(value)
+        if isinstance(value, str):
+            as_str = value
         else:
-            as_int = cls._to_int(value)
-            if (cls._format == "" or cls._base != 10) and not isinstance(value, istr):
-                if isinstance(value, str):
-                    as_str = value
+            if as_int == cls._nan:
+                raise TypeError(f"incorrect value for {cls.__name__}: {repr(value)}")
+            if cls._int_format == "" or cls._base != 10:
+                if cls._base == 10:
+                    as_str = str(as_int)
                 else:
-                    if cls._base == 10:
-                        as_str = str(as_int)
-                    else:
-                        as_str = istr._to_base(as_int, cls._base)
+                    as_str = istr._to_base(as_int, cls._base)
             else:
-                as_str = f"{as_int:{cls._format}}"
+                as_str = f"{as_int:{cls._int_format}}"
 
         self = super().__new__(cls, as_str)
         self._as_int = as_int
-        if self._mode == "istr":
+        if self._repr_mode == "istr":
             self._as_repr = f"{cls.__name__}({repr(as_str)})"
-        elif self._mode == "int":
-            self._as_repr = repr(as_int)
+        elif self._repr_mode == "int":
+            self._as_repr = "nan" if as_int == self._nan else repr(as_int)
         else:
             self._as_repr = repr(as_str)
         return self
-              
+
     def __iter__(self):
         yield from self.__class__(super().__iter__())
 
     def __hash__(self):
         return hash((self.__class__, str(self)))
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
-            return self._as_int == other._as_int
+            if self.is_int() and other.is_int():
+                return self._as_int == other._as_int
         if isinstance(other, str):
             return super().__eq__(other)
         try:
             return self._as_int == self._to_int(other)
         except Exception:
             return False
 
     def __ne__(self, other):
         return not self == other
 
     def __contains__(self, other):
         return super().__contains__(str(other))
 
     def __repr__(self):
+        if self._force_istr_repr:
+            return f"{self.__class__.__name__}({super().__repr__()})"
         return self._as_repr
 
     def __le__(self, other):
+        self._check_is_int(other, "<=")
         return self._as_int <= self._to_int(other)
 
     def __lt__(self, other):
+        self._check_is_int(other, "<")
         return self._as_int < self._to_int(other)
 
     def __ge__(self, other):
+        self._check_is_int(other, ">=")
         return self._as_int >= self._to_int(other)
 
     def __gt__(self, other):
+        self._check_is_int(other, ">")
         return self._as_int > self._to_int(other)
 
     def __bool__(self):
-        return bool(self._as_int)
+        if self.is_int():
+            return bool(self._as_int)
+        return bool(str(self))
 
     def __add__(self, other):
+        self._check_is_int(other, "+")
         return self.__class__(self._as_int + self._to_int(other))
 
+    def __radd__(self, other):
+        self._rcheck_is_int(other, "+")
+        return self.__class__(self._to_int(other) + self._as_int)
+
     def __sub__(self, other):
+        self._check_is_int(other, "-")
         return self.__class__(self._as_int - self._to_int(other))
 
+    def __rsub__(self, other):
+        self._rcheck_is_int(other, "-")
+        return self.__class__(self._to_int(other) - self._as_int)
+
     def __mul__(self, other):
+        self._check_is_int(other, "*")
         return self.__class__(self._as_int * self._to_int(other))
 
+    def __rmul__(self, other):
+        self._rcheck_is_int(other, "*")
+        return self.__class__(self._to_int(other) * self._as_int)
+
     def __floordiv__(self, other):
+        self._check_is_int(other, "//")
         return self.__class__(self._as_int // self._to_int(other))
 
     def __rfloordiv__(self, other):
+        self._rcheck_is_int(other, "//")
         return self.__class__(self._to_int(other) // self._as_int)
 
     def __truediv__(self, other):
+        self._check_is_int(other, "/")
         return self.__class__(self._as_int // self._to_int(other))
 
     def __rtruediv__(self, other):
+        self._rcheck_is_int(other, "/")
         return self.__class__(self._to_int(other) // self._as_int)
 
     def __pow__(self, other):
+        self._check_is_int(other, "**")
         return self.__class__(self._as_int ** self._to_int(other))
 
     def __rpow__(self, other):
+        self._rcheck_is_int(other, "**")
         return self.__class__(self._to_int(other) ** self._as_int)
 
-    def __radd__(self, other):
-        return self.__class__(self._to_int(other) + self._as_int)
-
-    def __rsub__(self, other):
-        return self.__class__(self._to_int(other) - self._as_int)
-
-    def __rmul__(self, other):
-        return self.__class__(self._to_int(other) * self._as_int)
-
     def __mod__(self, other):
+        self._check_is_int(other, "%")
         return self.__class__(self._as_int % self._to_int(other))
 
     def __rmod__(self, other):
+        self._rcheck_is_int(other, "%")
         return self.__class__(self._to_int(other) % self._as_int)
 
     def __or__(self, other):
         return self.__class__("".join((self, self.__class__(other))))
 
     def __ror__(self, other):
         return self.__class__("".join((self.__class__(other), self)))
 
-    def __int__(self):
-        return int(self._as_int)
-
     def __round__(self):
+        self._check_is_int("round")
         return self.__class__(round(self._as_int))
 
+    def __int__(self):
+        if not self.is_int():
+            raise ValueError(f"invalid literal for int() with base 10: {repr(self)}")
+        return int(self._as_int)
+
     def __trunc__(self):
+        self._check_is_int("trunc")
         return self.__class__(math.trunc(self._as_int))
 
     def __floor__(self):
+        self._check_is_int("floor")
         return self.__class__(math.floor(self._as_int))
 
     def __ceil__(self):
+        self._check_is_int("ceil")
         return self.__class__(math.ceil(self._as_int))
 
     def __matmul__(self, other):
         return self.__class__(super().__mul__(other))
 
     def __rmatmul__(self, other):
         return self.__class__(super().__rmul__(other))
 
     def __divmod__(self, other):
+        self._check_is_int(other, "divmod")
         return self.__class__(divmod(self._as_int, self._to_int(other)))
 
     def __rdivmod__(self, other):
+        self._rcheck_is_int(other, "divmod")
         return self.__class__(divmod(self._to_int(other), self._as_int))
 
     def __neg__(self):
+        self._check_is_int("-")
         return self.__class__(-self._as_int)
 
     def __pos__(self):
+        self._check_is_int("+")
         return self
 
     def __abs__(self):
+        self._check_is_int("abs")
         return self.__class__(abs(self._as_int))
 
     def is_even(self):
+        self._check_is_int("is_even")
         return self._as_int % 2 == 0
 
     def is_odd(self):
+        self._check_is_int("is_odd")
         return self._as_int % 2 == 1
 
+    def is_int(self):
+        return self._as_int != self._nan
+
     def reversed(self):
         return self[::-1]
 
     def __getitem__(self, key):
         return self.__class__(super().__getitem__(key))
 
     @classmethod
@@ -450,53 +539,53 @@
 
     @classmethod
     def enumerate(cls, iterable, start=0):
         for i, value in enumerate(iterable, start):
             yield cls(i), value
 
     @classmethod
-    class format:
-        def __new__(cls, cls_format, format=None):
-            if format is None:
-                return cls_format._format
+    class int_format:
+        def __new__(cls, cls_int_format, int_format=None):
+            if int_format is None:
+                return cls_int_format._int_format
             return super().__new__(cls)
 
-        def __init__(self, cls, format):
-            self.saved_format = cls._format
+        def __init__(self, cls, int_format):
+            self.saved_int_format = cls._int_format
             self.saved_cls = cls
-            if not (isinstance(format, str) and all(x in "0123456789" for x in format)):
-                raise ValueError(f"{repr(format)} is incorrect format")
+            if not (isinstance(int_format, str) and all(x in "0123456789" for x in int_format)):
+                raise ValueError(f"{repr(int_format)} is incorrect int_format")
 
-            cls._format = format
+            cls._int_format = int_format
 
         def __enter__(self):
             ...
 
         def __exit__(self, exc_type, exc_value, exc_tb):
-            self.saved_cls._format = self.saved_format
+            self.saved_cls._int_format = self.saved_int_format
 
     @classmethod
     class repr_mode:
-        def __new__(cls, cls_mode, mode=None):
+        def __new__(cls, cls_repr_mode, mode=None):
             if mode is None:
-                return cls_mode._mode
-            if mode in ("istr", "str", "int"):
+                return cls_repr_mode._repr_mode
+            if mode in ("istr", "str", "int"):  # _istr is used only for TypeErrors
                 return super().__new__(cls)
             raise TypeError(f"mode not 'istr', 'str' or 'int', but {repr(mode)}")
 
         def __init__(self, cls, mode):
-            self.saved_mode = cls._mode
+            self.saved_repr_mode = cls._repr_mode
             self.saved_cls = cls
-            cls._mode = mode
+            cls._repr_mode = mode
 
         def __enter__(self):
             ...
 
         def __exit__(self, exc_type, exc_value, exc_tb):
-            self.saved_cls._mode = self.saved_mode
+            self.saved_cls._repr_mode = self.saved_repr_mode
 
     @classmethod
     class base:
         def __new__(cls, cls_base, base=None):
             if base is None:
                 return cls_base._base
             if 2 <= base <= 36:
@@ -513,84 +602,87 @@
 
         def __exit__(self, exc_type, exc_value, exc_tb):
             self.saved_cls._base = self.saved_base
 
     @classmethod
     def range(cls, start, stop=None, step=1):
         return _range(cls, start, stop, step)
-        
+
     @classmethod
     @functools.lru_cache
-    def digits(cls,*args):
-        '''
+    def digits(cls, *args):
+        """
         return an istr of istr'ed digits as specified with args
-        
+
         if no args, 0-9 will be used
-        
+
         all given args will be used
         each arg has to be either null string, <digit>, <digit>-<digit> or -<digit>
-        
+
         examples
         --------
         istr.digits() ==> istr('0123456789')
         istr.digits('') ==> istr('0123456789')
         istr.digits('1') ==> istr('1')
         istr.digits('3-') ==> istr('3456789')
         istr.digits('-3') ==> istr('0123')
         istr('1-4', '6', '8-9') ==> istr('1234689')
         istr('1', '1-2', '1-3') ==> istr('11213')
 
         Note
         ----
         A digit can occur more than once.
 
-        '''
-        result=[]
+        """
+        result = []
         if not args:
-            args=['0-9']
+            args = ["0-9"]
         for arg in args:
-            if arg.strip()=='':
-                arg='0-9'
-            pre,*post=arg.split('-')
-            if pre.strip()=='':
-                pre='0'
+            if arg.strip() == "":
+                arg = "0-9"
+            pre, *post = arg.split("-")
+            if pre.strip() == "":
+                pre = "0"
             try:
-                start=int(pre)
+                start = int(pre)
             except ValueError:
-                raise ValueError(f'incorrect specifier: {repr(arg)}')  
-            if not 0<=start<=9:
-                raise ValueError(f'incorrect specifier: {repr(arg)}')                
-            if len(post)>1:
-                raise ValueError(f'incorrect specifier: {repr(arg)}')
+                raise ValueError(f"incorrect specifier: {repr(arg)}")
+            if not 0 <= start <= 9:
+                raise ValueError(f"incorrect specifier: {repr(arg)}")
+            if len(post) > 1:
+                raise ValueError(f"incorrect specifier: {repr(arg)}")
             if post:
-                if post[0].strip()=="":
-                    post="9"
+                if post[0].strip() == "":
+                    post = "9"
                 try:
-                    stop=int(post[0])
+                    stop = int(post[0])
                 except ValueError:
-                    raise ValueError(f'incorrect specifier: {repr(arg)}')                    
-                if (not 0<=start<=9) or start>stop:
-                    raise ValueError(f'incorrect specifier: {repr(arg)}')
+                    raise ValueError(f"incorrect specifier: {repr(arg)}")
+                if (not 0 <= start <= 9) or start > stop:
+                    raise ValueError(f"incorrect specifier: {repr(arg)}")
             else:
-                stop=start
-            result.extend(range(start,stop+1))
-        return cls('').join(istr(result))
+                stop = start
+            result.extend(range(start, stop + 1))
+        return cls("").join(istr(result))
 
     def capitalize(self, *args, **kwargs):
         return self.__class__(super().capitalize(*args, **kwargs))
 
     def casefold(self, *args, **kwargs):
         return self.__class__(super().casefold(*args, **kwargs))
 
     def center(self, *args, **kwargs):
         return self.__class__(super().center(*args, **kwargs))
 
     def expandtabs(self, *args, **kwargs):
         return self.__class__(super().expandtabs(*args, **kwargs))
 
+    def format(self, *args, **kwargs):
+        return self.__class__(super().format(*args, **kwargs))
+
     def join(self, *args, **kwargs):
         return self.__class__(super().join(*args, **kwargs))
 
     def ljust(self, *args, **kwargs):
         return self.__class__(super().ljust(*args, **kwargs))
 
     def lower(self, *args, **kwargs):
@@ -642,19 +734,11 @@
         return self.__class__(super().upper(*args, **kwargs))
 
     def zfill(self, *args, **kwargs):
         return self.__class__(super().zfill(*args, **kwargs))
 
 
 def main():
-    print(repr(istr.digits()))
-    print(istr.digits('1-9'))
-    print(istr.digits('1'))
-    print(istr.digits('1-2', '6'))    
-    print(istr.digits('1-5', '7-9'))        
-    print(istr.digits('-5'))   
-    print(istr.digits('3-'))   
-    print(repr(divmod(istr(20),3)))
+    ...
 
 if __name__ == "__main__":
     main()
-
```

### Comparing `istr_python-0.2.0.post0/istr_python.egg-info/PKG-INFO` & `istr_python-1.0.0/istr_python.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: istr-python
-Version: 0.2.0.post0
+Version: 1.0.0
 Summary: istr - strings you can count on
 Author-email: Ruud van der Ham <rt.van.der.ham@gmail.com>
 Project-URL: Homepage, https://github.com/salabim/istr
 Project-URL: Repository, https://github.com/salabim/istr
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
-<img src="https://www.salabim.org/istr_logo.png" width=500>
+ <img src="https://www.salabim.org/istr_logo.png" width=500>
 
-## Introduction
+### Introduction
 
 The istr module has exactly one class: istr.
 
 With this it is possible to interpret strings as if they were integers.
 
-This can be very handy for solving puzzles, but also for other purposes.</br>
-For instance the
-famous send more money puzzle
+This can be very handy for solving puzzles, but also for other purposes.
+For instance the famous send more money puzzle, where each letter has to be replaced by a unique digit (0-9)
+
 ```
   S E N D
   M O R E
 --------- +
 M O N E Y
 ```
 can be nicely, albeit not very efficient, coded as:
@@ -37,280 +37,404 @@
     if m and ((s|e|n|d) + (m|o|r|e) == (m|o|n|e|y)):
         print(f' {s|e|n|d}')
         print(f' {m|o|r|e}')
         print('-----')
         print(f'{m|o|n|e|y}')
 ```
 
-And it is a nice demonstration of extending a class (str) with extra and changed functionality.
+Of, if we want to add all the digits in a string:
+
+```
+sum_digits = sum(istr('9282334'))  # answer 31
+```
+
+And the module is a demonstration of extending a class (str) with extra and changed functionality.
 
-## Installation
+### Installation
 Installing istr with pip is easy.
 ```
 $ pip install istr-python
 ```
 or when you want to upgrade,
 ```
 $ pip install istr-python --upgrade
 ```
 Alternatively, istr.py can be just copied into you current work directory from GitHub (https://github.com/salabim/istr).
 
 No dependencies!
 
-## Usage
+### Usage
+#### Start
+
 Just start with
 
 ```
 from istr import istr
 ```
 
-Now we can define some istrs:
+#### Use istrs as if the were int
+
+We can define an istr:
 ```
 four = istr('4')
 five = istr('5')
 ```
-Then we can do
+The variables `four`  and `five` can now be used as if they were int:
+
 ```
-x= four * five
+twenty = four * five
 ```
 , after which x is `istr('20')`
 
-And now we can do
+The same can be done with
+
+```
+twenty = 4 * five
+```
+
+or
+
+```
+twenty = four * 5
+```
+
+And now `twenty` can be used as if it was an int as well. So:
+
 ```
-print(x == 20)
-print(x == '20')
+twenty - four
 ```
-resulting in two times `True`. That's because istrs instances are treated as int, although they are strings.
 
-That means that we can also say
+is `istr('16')`
+
+We can do all the usual arithmetic operations on istrs, e.g.
+
 ```
-print(x < 30)
-print(x >= '10')
+-four + (twenty / 2)
+```
+
+is `istr('6')`
+
+And we can test for equality, So:
+
 ```
-again resulting in two times `True`.
+twenty == 20
+```
+is True.
+
+But as istrs are also strings. So
+
+```
+twenty == '20'
+```
+
+is also True!
+
+For the order comparisons (<=, <, >, >=), the istr is always interpreted as an int:
+
+That means that  both
+```
+twenty < 30
+twenty >= '10' # here '10' is converted to 10 for the comparison
+```
+are `True`.
 
 In contrast to an ordinary string
 ```
 print(four + five)
 ```
 prints `9`, as istr are treated as ints.
 
-Please note that `four` and `five` could have also be initialized with
+Please note that `four`  could have also been initialized with
 ```
 four = istr(4)
-five = istr(5)
 ```
 or even
 ```
 four, five = istr(4, 5)
 ```
 
-But how can we concatenate istrs? Just use the or operator (|): 
+> [!NOTE]
+>
+> All calculations are strictly integer calculations. That means that if a float variale is ever produced it will be converted to an int.
+> Also divisions are always floor divisions!
+
+#### Use istrs as string
+
+We should realize that istrs are in fact strings.
+
+In order to concatenate two istrs (or an istr and a str), we cannot use the `four + five` operator as
+
+that would be `istr(9)`.
+
+In order to concatenate istrs,  we use the or operator (`|`). So
+
 ```
-print(four | five)
+four | five
 ```
-will output `45`.
-
-And the result is again an istr.
+will be `istr(`45`).
 
 That means that
 ```
 (four | five) / 3
 ```
 is `istr('9')`.
 
-In order to repeat a string in the usual sense, you cannot use `3 * four`, as that woud be `12`. 
+In order to repeat a string in the usual sense, you cannot use `3 * four`, as that would be `12`. 
+
+In order to repeat we use the matrix multiplication operator (`@`). So
+
+ `3 @ four`
+
+ is istr(`444`). As is `four @ 3`.
+
+> [!NOTE]
+>
+> It is not allowed to use the `@` operator for two istrs. So, `four @ five` raises a TypeError.
+
+#### istrs that can't be interpreted as an int
 
-We use the matrix multiplication operator (@) for this. So `3 @ four` is `444`. As is `four @ 3`.
+Although usualy, istrs are to be interpreted as an int, that's not a requirement.
+
+So
 
-Also allowed are
 ```
-abs(four)
--four 
+istr('abc')
 ```
 
-The bool operator works on the integer value of an istr. So
-`bool(istr('0'))` ==> `False`
-`bool(istr('1'))` ==> `True`
-The code
+or
+
+```
+istr(1,2,3)
+```
+
+are accepted.
+
+But, we can't do any arithmetic with them. 
+
+If we try
+
 ```
-if istr('0'):
-    print('True')
-else:
-    print('False')
+istr('abc') + 5
 ```
-will print `False`
 
-For the in operator, an istr is treated as an ordinary string, although it is possible to use ints as well:
+a TypeError will be raised.
+
+That holds for any arithmetic we try.
+
+If we want to test if an istr can be interpreted (and thus used in an arithmetic expression). we can use the `is_int()` method. So
+
+```ìstr(20).is_int()```
+
+is `True`, wherea
+
+```ìstr('abc').is_int()```
+
+is `False`.
+
+
+
+The bool operator works normally on the integer value of an istr. So
+
+`bool(istr('0'))` ==> `False`
+`bool(istr('1'))` ==> `True`
+
+If the istr can't be interpreted as an int, the string will be used to test. So
+
+`bool(istr('abc'))` ==> `False`
+`bool(istr(''))` ==> `True`
+
+#### Other operators
+
+For the `in` operator, an istr is treated as an ordinary string, although it is possible to use ints as well:
+
 ```
 '34' in istr(1234)
 34 in istr(1234)
 ```
 On the left hand side an istr is always treated as a string:
 ```
 istr(1234) in '01234566890ABCDEF'
 ```
 
-Note that all calculations are strictly integer calculations. That means that if a float variale is ever produced it will be converted to an int.
-Also divisions are always floor divisions!
-
-There's a special case for `istr('')`. This is a proper empty string, but also represents the value of 0.
-That is to allow for `istr('').join(i for i in '01234)'`, resulting in `istr('01234')`.
-
 Sorting a list of istrs is based on the integer value, not the string. So
 
-`' '.join(sorted('1 3 2 4 5 6 11 7 9 8 10 12 0'.split()))`
+```
+' '.join(sorted('1 3 2 4 5 6 11 7 9 8 10 12 0'.split()))
+```
 
 is
 
-`'0 1 10 11 2 3 4 5 6 7 8 9'`
+```
+'0 1 10 11 2 3 4 5 6 7 8 9'
+```
 
 ,whereas
 
-`' '.join(sorted(istr('1 3 2 4 5 6 11 7 9 8 10 12 0'.split())))`
+```
+' '.join(sorted(istr('1 3 2 4 5 6 11 7 9 8 10 12 0'.split()))
+```
 
 is 
 
-`'0 1 2 3 4 5 6 7 8 9 10 11'`
+```
+'0 1 2 3 4 5 6 7 8 9 10 11'
+```
 
-## Using other values for istr than numeric value or str
+#### Using other values for istr than numeric value or str
 Apart from with simple numeric (to be interpreted as an int) or str, istr can be initialized with
 several other types:
 
-- if a dict (or subtype of dict), the same type dict will be returned with all values istr'ed
+- if a dict (or subtype of dict), the same type dict will be returned with all *values* istr'ed
 
-    `istr({0: 0, 1: 1, 2: 4})` ==> `{0: istr('0'), 1: istr('1'), 2: istr('4')}`
+    ```
+    istr({0: 0, 1: 1, 2: 4}) ==> {0: istr('0'), 1: istr('1'), 2: istr('4')}
+    ```
 
 - if an iterator, the iterator will be mapped with istr
 
-    `istr(i * i for i in range(3))` ==> `<map object>`
-
-    `list(istr(i * i for i in range(3)))` ==> `[istr('0'), istr('1'), istr('4')]`
+    ```
+    istr(i * i for i in range(3)) ==> <map object>
+    list(istr(i * i for i in range(3))) ==> [istr('0'), istr('1'), istr('4')]
+    ```
 
 - if an iterable, the same type will be returned with all elements istr'ed
 
-    `istr([0, 1, 4])` ==> `[istr('0'), istr('1'), istr('4')]`
-
-    `istr((0, 1, 4))` ==> `(istr('0'), istr('1'), istr('4'))`
-
-    `istr({0, 1, 4})` ==> `{istr('4'), istr('0'), istr('1')} ## or similar`
+    ```
+    istr([0, 1, 4]) ==> [istr('0'), istr('1'), istr('4')]
+    istr((0, 1, 4)) ==> (istr('0'), istr('1'), istr('4'))
+    istr({0, 1, 4}) ==> `{istr('4'), istr('0'), istr('1')}  # or similar
+    ```
 
 - if a range, an istr.range instance will be returned
-    
-    `istr(range(3))` ==> `istr.range(3)`
+  
+    ```
+  istr(range(3))` ==> `istr.range(3)
+    list(istr(range(3)))` ==> `[istr('0'), istr('1'), istr('2')]
+  len(istr(range(3)))` ==> `3
+  ```
 
-    `list(istr(range(3)))` ==> `[istr('0'), istr('1'), istr('2')]`
+- if an istr.range instance, the same istr.range will be returned
 
-    `len(istr(range(3)))` ==> `3`
+- if an istr, the same istr will be used
 
-- if an istr.range instance, the same istr.range will be returned
+    ```
+    istr(istr('4')) ==> istr ('4')
+    ```
 
-## More than one parameter for istr
+#### More than one parameter for istr
 It is possible to give more than one parameter, in which case a tuple
 of the istrs of the parameters will be returned, which can be handy
 to unpack multiple values, e.g.
 
-`a, b, c = istr(5, 6, 7)` ==> `a=istr('5') , b=istr('6'), c=istr('7')`
+```
+a, b, c = istr(5, 6, 7) ==> a=istr('5') , b=istr('6'), c=istr('7') 
+```
 
-## test for even/odd
-It is possible to test for even/odd with the
+#### test for even/odd
+It is possible to test for even/odd (provided the istt can be interpreted as an int) with the
 
 `is_even` and `is_odd` method, e.g.
 
 ```
-print(istr(4).is_even())
-print(istr(5).is_odd())
+istr(4).is_even()) ==> True
+istr(5).is_odd()) ==> True
 ```
-This will print `True` twice.
-
-## reverse an istr
+#### reverse an istr
 The method `istr.reversed()` will return the an istr with the reversed content:
 ```
-print(repr(istr(456).reversed()))
-print(repr(istr('0456').reversed()))
-```
-result:
-```
-istr('654')
-istr('6540')
+istr(456).reversed() ==> istr('654')
+istr('0456').reversed() ==> istr('6540')
 ```
 The same can -of course- be achieved with
 ```
-print(repr(istr(456)[::-1]))
-print(repr(istr('0456')[::-1]))
+istr(456)[::-1] ==> istr('654')
+istr('0456')[::-1] ==> istr('6540')
 ```
-Note that is impossible to reverse a negative istr.
+> [!NOTE]
+>
+> It is possible to reverse a negative istr, but the result can't be interpreted as an int anymore.
+>
+> ```
+> istr(-456) ==> TypeError
+> ```
 
-## enumerate with istrs
+#### enumerate with istrs
 
 The `istr.enumerate` method can be used just as the builtin enumerate function.
 The iteration counter however is an istr rather than an int. E.g. 
+
 ```
     for i,c in istr.enumerate('abc'):
         print(f'{repr(i)} {c}')
 ```
 prints
 ```
 istr('0') a
 istr('1') b
 istr('2') c
 ```
 
-## concatenate an iterable
+#### concatenate an iterable
 
 The `istr.concat` method can be useful to map all items of an iterable
 to `istr` and then concatenate these.
 
-`list(istr.concat(((1,2),(3,4)))` ==> `istr([12,34])`
+`
 
-`list(istr.concat(itertools.permutations(range(3),2)))` ==> `[istr('01'), istr('02'), istr('10'), istr('12'), istr('20'), istr('21')]` 
+```
+list(istr.concat(((1,2),(3,4))) ==> istr([12,34])
+list(istr.concat(itertools.permutations(range(3),2))) ==> 
+    [istr('01'), istr('02'), istr('10'), istr('12'), istr('20'), istr('21')] 
+```
 
-## generate istr with digits
+#### generate istr with digits
 
 The class method `digits` can be used to return an istr of digits according to a given specification.
 The method takes either no or a number of arguments.
 
 If no arguments are given, the result will be istr('0123456789').
 
 The given argument(s) result in a range of digits.
 
 - `<n>` ==> n
-- `<n-m> ==> n, n+1, ..., m
+- `<n-m>` ==> n, n+1, ..., m
 - `-n>` ==> 0, 1, ... n
 - `n->` ==> n, n+1, ..., 9
 - `''` ==> 0, 1, ..., 9
 
-(n and m must be digit between 0 and 9)
+(n and m must be digits between 0 and 9)
 
 The final result is an istr composed of the given range(s).
 
 Here are some examples:
 
-- `istr.digits()` ==> `istr('0123456789')`
-- `istr.digits('')` ==> `istr('0123456789')`
-- `istr.digits('1')` ==> `istr('1')`
-- `istr.digits('3-')` ==> `istr('3456789')`
-- `istr.digits('-3')` ==> `istr('0123')`
-- `istr('1-4', '6', '8-9')` ==> `istr('1234689')`
-- `istr('1', '1-2', '1-3')` ==> `istr('11213')`
+```
+istr.digits() ==> istr('0123456789')
+istr.digits('') ==> istr('0123456789')
+istr.digits('1') ==> istr('1')
+istr.digits('3-') ==> istr('3456789')
+istr.digits('-3') ==> istr('0123')
+istr('1-4', '6', '8-9') ==> istr('1234689')
+istr('1', '1-2', '1-3') ==> istr('11213')
+```
 
 
-## Subclassing istr
+#### Subclassing istr
 When a class is derived from istr, all methods will return that newly derived class. 
 
 E.g.
 ```
 class jstr(istr):
     ...
     
 print(repr(jstr(4) * jstr(5)))
 ```
 will print `jstr('20')`
 
-## Changing the way repr works
+#### Changing the way repr works
 
 It is possible to control the way an `istr` instance will be repr'ed.
 
 By default, the `istr('5')` is represented as `istr('5')`.
 
 With the istr.repr_mode() context manager, that can be changed:
 ```
@@ -326,15 +450,31 @@
 ```
 This will print
 ```
 '5'
 5
 istr('5')
 ```
-Note that the way an `istr` is represented is determined at initialization.
+If the repr_mode is `'int'` and the istr can't be interpreted as an int the string `nan` (not a number) will be returned:
+
+```
+ with istr.repr_mode('int'):
+    abc = istr('abc')
+    print(repr(abc))
+```
+
+This will print
+
+```
+nan
+```
+
+> [!NOTE]
+>
+> The way an `istr` is represented is determined at initialization.
 
 It is also possible to set the repr mode without a context manager:
 
 ```
 istr.repr_mode('str')
 five = istr('5')
 print(repr(five))
@@ -345,21 +485,21 @@
 ```
 Finally, the current repr mode can be queried with `istr.repr_mode()`. So upon start:
 ```
 print(repr(istr.repr_mode()))
 ```
 will output `istr`.
 
-## Changing the base system
+#### Changing the base system
 
 By default, `istr` works in base 10. However it is possible to change the base system with the `istr.base()` context manager / method.
 
 Any base between 2 and 36 may be used.
 
-Note that the integer is always stored in base 10 mode, but the string
+Note that the integer is **always** stored in base 10 mode, but the string
 representation will reflect the chosen base (at time of initialization).
 
 Some examples:
 ```
 with istr.base(16):
     a = istr('7fff')
     print(int(a))
@@ -387,100 +527,118 @@
 ```
 Finally, the current base can be queried with `istr.base()`, so upon start:
 ```
 print(istr.base())
 ```
 will result in `10`.
 
-## Changing the format of the string
-
-By default, `istr` does not change the way an istr is stored when a str is to initialize:
+#### Changing the format of the string
 
-`repr('4'))` ==> `istr('4')`
+When an  istr is initialized with a string the istr will be just stored as such.
 
-`repr(' 4'))` ==> `istr(' 4')`
-
-`repr('4  '))` ==> `istr('4  ')`
+```
+repr('4')) ==> istr('4')
+repr(' 4')) ==> istr(' 4')
+repr('4  ')) ==> istr('4  ')
+```
 
-For initializing with an int (or other numeric) value, the string is simply the str representation
+For initializing with an int (or other numeric) value, the string is by default simply the str representation
 
-`repr(4))` ==> `istr('4')`
+```
+repr(4)) ==> istr('4')
+```
 
-With the `istr.format()` context manager this behavior can be changed.
+ With the `istr.int_format()` context manager this behavior can be changed.
 If the format specifier is a number, most likely a single digit, that
 will be the minimum number of characters in the string:
+
 ```
-with istr.format('3'):
+with istr.int_format('3'):
     print(repr(istr(1)))
     print(repr(istr(12)))
     print(repr(istr(123)))
     print(repr(istr(1234)))
 ```
 will print
 ```
 istr('  1')
 istr(' 12')
 istr('123')
 istr('1234')
 ```
 If the string starts with a `0`, the string will be zero filled:
 ```
-with istr.format('03'):
+with istr.int_format('03'):
     print(repr(istr(1)))
     print(repr(istr(12)))
     print(repr(istr(123)))
     print(repr(istr(1234)))
 ```
 will print
 ```
 istr('001')
 istr('012')
 istr('123')
 istr('1234')
 ```
-Note that if a format other than the default `''` is used, the string will reformatted even if the `istr` is specified with a string:
-```
-with istr.format('03'):
-    print(repr(istr('  12 ')))
-```
-will result in `istr('0012')`
+> [!NOTE]
+>
+>  if a string is used to initialize an istr AND that string can be interpreted as an int. the string will reformatted:
+>
+> ```
+> with istr.int_format('03'):
+>     print(repr(istr('  12 ')))
+> ```
+>
+> will result in
+>
+> ```
+> istr('0012')
+> ```
+
+> [!NOTE]
+>
+> For bases other than 10, the string will never be reformatted!
 
-Remark: For bases other than 10, the string will never be reformatted!
+### Overview of operations
 
-## Operations
-----------------------------
-```
 The table below shows whether the string or the int version of istr is applied.
 
-operator/function   int  str  Example
-----------------------------
-+                    x        istr(20) + 3 ==> istr('23')
-_                    x        istr(20) - 3 ==> istr('17')
-*                    x        istr(20) * 3 ==> istr('60')
-/                    x        istr(20) / 3 ==> istr('6')
-//                   x        istr(20) // 3 ==> istr('6')
-%                    x        istr(20) % 3 ==> istr('2')
-divmod               x        divmod(istr(20), 3) ==> (istr('6'), istr('2'))
-**                   x        istr(2) ** 3 ==> istr('8')
-@                         x   istr(20) @ 3 ==> istr('202020')
-==                   x    x   istr(20) == 20 ==> True | istr(20) == '20' ==> True
-|                         x   istr(20) | 5 ==> istr('205')
-abs                  x        abs(istr(-20)) ==> istr('20')
-bool                 x        bool(istr(' 0 ')) ==> False
-<=, <, >, >=         x        istr('100') > istr('2') ==> True
-slicing              x        istr(12345)[1:3] ==> istr('23')
-iterate                   x   [x for x in istr(20)] ==> [istr('2'), istr('0')
-len                       x   len(istr(' 20 ')) ==> 4
-count                     x   istr(100),count('0') ==> 2
-index                     x   istr(' 100 ').index('0') ==> 2
-----------------------------
 ```
-## Test script
+operator/function   int  str   Example
+-----------------------------------------------------------------------------------------
++                    x         istr(20) + 3 ==> istr('23')
+_                    x         istr(20) - 3 ==> istr('17')
+*                    x         istr(20) * 3 ==> istr('60')
+/                    x         istr(20) / 3 ==> istr('6')
+//                   x         istr(20) // 3 ==> istr('6')
+%                    x         istr(20) % 3 ==> istr('2')
+divmod               x         divmod(istr(20), 3) ==> (istr('6'), istr('2'))
+**                   x         istr(2) ** 3 ==> istr('8')
+@                         x    istr(20) @ 3 ==> istr('202020')
+==                   x    x    istr(20) == 20 ==> True | istr(20) == '20' ==> True
+|                         x    istr(20) | 5 ==> istr('205')
+abs                  x         abs(istr(-20)) ==> istr('20')
+bool                 x    x *) bool(istr(' 0 ')) ==> False | istr('') ==> False
+<=, <, >, >=         x         istr('100') > istr('2') ==> True
+slicing                   x    istr(12345)[1:3] ==> istr('23')
+iterate                   x    [x for x in istr(20)] ==> [istr('2'), istr('0')
+len                       x    len(istr(' 20 ')) ==> 4
+count                     x    istr(100),count('0') ==> 2
+index                     x    istr(' 100 ').index('0') ==> 2
+split                     x    istr('1 2').split() ==> (istr('1'), istr('2'))
+other string methods      x    istr('aAbBcC').lower() ==> istr('aabbcc')
+                               istr('aAbBcC').islower() ==> False
+                               istr('  abc   ').strip() ==> istr('abc')
+-----------------------------------------------------------------------------------------
+*) str is applied if is_int() is False
+```
+### Test script
 There's an extensive pytest script in the `\tests` directory.
 
-This script also shows clearly the ways istr can be used.
+This script also shows clearly the ways istr can be used, including several edge cases. Highly recommended to have a look at.
 
-## Badges
+### Badges
 ![PyPI](https://img.shields.io/pypi/v/istr-python) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/istr-python) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/istr-python)
 
 ![PyPI - License](https://img.shields.io/pypi/l/istr-python) ![Black](https://img.shields.io/badge/code%20style-black-000000.svg) 
- ![GitHub last commit](https://img.shields.io/github/last-commit/salabim/istr)
+![GitHub last commit](https://img.shields.io/github/last-commit/salabim/istr)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `istr_python-0.2.0.post0/pyproject.toml` & `istr_python-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "istr-python"
 authors = [
     {name = "Ruud van der Ham", email = "rt.van.der.ham@gmail.com"}
 ]
 description = "istr - strings you can count on"
-version = "0.2.0-0"
+version = "1.0.0"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
 ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License",
```

