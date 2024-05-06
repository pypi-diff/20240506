# Comparing `tmp/LexBuilder-1.0.2.tar.gz` & `tmp/lexbuilder-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LexBuilder-1.0.2.tar", last modified: Mon Jan  8 20:03:17 2024, max compression
+gzip compressed data, was "lexbuilder-1.1.0.tar", last modified: Mon May  6 17:43:03 2024, max compression
```

## Comparing `LexBuilder-1.0.2.tar` & `lexbuilder-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-01-08 20:03:17.233305 LexBuilder-1.0.2/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1096 2024-01-08 18:53:21.000000 LexBuilder-1.0.2/LICENSE
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-01-08 20:03:17.233305 LexBuilder-1.0.2/LexBuilder/
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     3323 2024-01-08 18:50:01.000000 LexBuilder-1.0.2/LexBuilder/BaseLexer.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1722 2024-01-08 19:42:35.000000 LexBuilder-1.0.2/LexBuilder/PyLexer.py
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       62 2024-01-08 19:42:43.000000 LexBuilder-1.0.2/LexBuilder/__init__.py
-drwxrwxr-x   0 alexander  (1000) alexander  (1000)        0 2024-01-08 20:03:17.233305 LexBuilder-1.0.2/LexBuilder.egg-info/
--rw-r--r--   0 alexander  (1000) alexander  (1000)     2016 2024-01-08 20:03:17.000000 LexBuilder-1.0.2/LexBuilder.egg-info/PKG-INFO
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      241 2024-01-08 20:03:17.000000 LexBuilder-1.0.2/LexBuilder.egg-info/SOURCES.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)        1 2024-01-08 20:03:17.000000 LexBuilder-1.0.2/LexBuilder.egg-info/dependency_links.txt
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       11 2024-01-08 20:03:17.000000 LexBuilder-1.0.2/LexBuilder.egg-info/top_level.txt
--rw-r--r--   0 alexander  (1000) alexander  (1000)     2016 2024-01-08 20:03:17.233305 LexBuilder-1.0.2/PKG-INFO
--rw-rw-r--   0 alexander  (1000) alexander  (1000)     1592 2024-01-08 20:03:12.000000 LexBuilder-1.0.2/README.md
--rw-rw-r--   0 alexander  (1000) alexander  (1000)       38 2024-01-08 20:03:17.233305 LexBuilder-1.0.2/setup.cfg
--rw-rw-r--   0 alexander  (1000) alexander  (1000)      630 2024-01-08 20:03:12.000000 LexBuilder-1.0.2/setup.py
+drwxrwxr-x   0 alexander554  (1000) alexander554  (1000)        0 2024-05-06 17:43:03.582765 lexbuilder-1.1.0/
+-rw-rw-r--   0 alexander554  (1000) alexander554  (1000)     1096 2024-01-08 18:53:21.000000 lexbuilder-1.1.0/LICENSE
+drwxrwxr-x   0 alexander554  (1000) alexander554  (1000)        0 2024-05-06 17:43:03.579765 lexbuilder-1.1.0/LexBuilder/
+-rw-rw-r--   0 alexander554  (1000) alexander554  (1000)     3503 2024-05-06 17:23:53.000000 lexbuilder-1.1.0/LexBuilder/BaseCppLexer.py
+-rw-rw-r--   0 alexander554  (1000) alexander554  (1000)     3284 2024-05-06 17:23:53.000000 lexbuilder-1.1.0/LexBuilder/BasePyLexer.py
+-rw-rw-r--   0 alexander554  (1000) alexander554  (1000)     3537 2024-05-06 17:39:59.000000 lexbuilder-1.1.0/LexBuilder/Builder.py
+-rw-rw-r--   0 alexander554  (1000) alexander554  (1000)      117 2024-05-06 17:21:27.000000 lexbuilder-1.1.0/LexBuilder/__init__.py
+drwxrwxr-x   0 alexander554  (1000) alexander554  (1000)        0 2024-05-06 17:43:03.581765 lexbuilder-1.1.0/LexBuilder.egg-info/
+-rw-r--r--   0 alexander554  (1000) alexander554  (1000)     2766 2024-05-06 17:43:03.000000 lexbuilder-1.1.0/LexBuilder.egg-info/PKG-INFO
+-rw-rw-r--   0 alexander554  (1000) alexander554  (1000)      270 2024-05-06 17:43:03.000000 lexbuilder-1.1.0/LexBuilder.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexander554  (1000) alexander554  (1000)        1 2024-05-06 17:43:03.000000 lexbuilder-1.1.0/LexBuilder.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexander554  (1000) alexander554  (1000)       11 2024-05-06 17:43:03.000000 lexbuilder-1.1.0/LexBuilder.egg-info/top_level.txt
+-rw-r--r--   0 alexander554  (1000) alexander554  (1000)     2766 2024-05-06 17:43:03.582765 lexbuilder-1.1.0/PKG-INFO
+-rw-rw-r--   0 alexander554  (1000) alexander554  (1000)     2337 2024-05-06 17:39:59.000000 lexbuilder-1.1.0/README.md
+-rw-rw-r--   0 alexander554  (1000) alexander554  (1000)       38 2024-05-06 17:43:03.582765 lexbuilder-1.1.0/setup.cfg
+-rw-rw-r--   0 alexander554  (1000) alexander554  (1000)      634 2024-05-06 17:40:34.000000 lexbuilder-1.1.0/setup.py
```

### Comparing `LexBuilder-1.0.2/LICENSE` & `lexbuilder-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `LexBuilder-1.0.2/LexBuilder/BaseLexer.py` & `lexbuilder-1.1.0/LexBuilder/BasePyLexer.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,29 +18,28 @@
     def __str__(self):
         return f'Token({self.type}, {self.value})'
 
     def __repr__(self):
         return self.__str__()
 
 
-# Define a lexer to tokenize the input
 class Lexer:
      def __init__(self, text):
          self.text = text
          self.pos = 0
          self.current_char = self.text[self.pos]
 
      def advance(self):
          self.pos += 1
          if self.pos < len(self.text):
              self.current_char = self.text[self.pos]
          else:
              self.current_char = None
 
-     def return_pos(self, pos):
+     def change_pos(self, pos):
          self.pos = pos
          if self.pos < len(self.text):
              self.current_char = self.text[self.pos]
          else:
              self.current_char = None
 
      def skip_whitespace(self):
```

### Comparing `LexBuilder-1.0.2/LexBuilder/PyLexer.py` & `lexbuilder-1.1.0/LexBuilder/Builder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from .BaseLexer import types, lexer
+from .BasePyLexer import types as pytypes, lexer as pylexer
+from .BaseCppLexer import types as cpptypes, lexer as cpplexer
 
 
 class Token:
     def __init__(self, name, value):
         self.name = name
         self.value = value
 
@@ -32,14 +33,49 @@
             else:
                 result3 += f'                     if token_value == "{value}":\n'
                 result3 += f'                         return Token({name}, "{value}")\n\n'
 
         return result1, result2, result3
 
 
-    def build_lexer(self):
+    def build(self):
         code1, code2, code3 = self.generate_code_for_tokens()
         with open("Lexer.py", "w", encoding="utf-8") as file:
             file.write("import sys\n\n\n")
-            file.write(types.format(code1) + "\n\n\n")
-            file.write(lexer.substitute(first=code2, second=code3) + "\n\n")
+            file.write(pytypes.format(code1) + "\n")
+            file.write(pylexer.substitute(first=code2, second=code3) + "\n\n")
 
+
+class CppBuilder:
+    def __init__(self, tokens):
+        self.tokens = tokens
+
+    def generate_code_for_tokens(self):
+        result1 = "\n"
+        result2 = ""
+        result3 = ""
+
+        for token in self.tokens:
+            name = token.name
+            value = token.value
+            result1 += f'string {name} = "{name}";\n'
+            if len(set(value)) == 1:
+                result1 += f'string {"_".join([name, name])} = "{"_".join([name, name])}";\n'
+                result2 += f"             if (current_char == '{list(set(value))[0]}') " + "{\n"
+                result2 += f'                 advance();\n'
+                result2 += f"                 if (current_char == '{list(set(value))[0]}') " + "{\n"
+                result2 += f'                     advance();\n'
+                result2 += f'                     return Token({"_".join([name, name])}, "{value}");\n'
+                result2 += f'                 ' + "} " + 'else ' + '{\n'
+                result2 += f'                     return Token({name}, "{value}");' + "\n                 }\n             }"
+            else:
+                result3 += f'                     if (token_value == "{value}") ' + '{\n'
+                result3 += f'                         return Token({name}, "{value}");' + '\n                     }\n'
+
+        return result1, result2, result3
+
+    def build(self):
+        code1, code2, code3 = self.generate_code_for_tokens()
+        with open("Lexer.h", "w", encoding="utf-8") as file:
+            file.write("#include <iostream>\n#include <string>\n\nusing namespace std;\n\n\n")
+            file.write(cpptypes.format(code1) + "\n")
+            file.write(cpplexer.substitute(first=code2, second=code3) + "\n\n")
```

### Comparing `LexBuilder-1.0.2/LexBuilder.egg-info/PKG-INFO` & `lexbuilder-1.1.0/LexBuilder.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,62 @@
 Metadata-Version: 2.1
 Name: LexBuilder
-Version: 1.0.2
+Version: 1.1.0
 Summary: Library for automatic construction of lexers
 Author: Alexander554
 Author-email: gaa.28112008@gmail.com
-Keywords: python lexer
+Keywords: python c++ lexer
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # About LexBuilder:
-LexBuilder is a library for automatically building a lexer in Python. In the future, the library will be able to build lexers in major programming languages such as C++, Golang, Java/Kotlin, etc.
+LexBuilder is a library for automatically building a lexer in Python and C++. In the future, the library will be able to build lexers in major programming languages such as Golang, Java/Kotlin, etc.
 
 ## About Syntax:
-In order for the library to generate the Lexer.py file, you need to pass a list of tokens to the PyBuilder class.
-To declare a token, you need to import the Token() class from the PyLexer() class. You need to pass the token name and its value to the Token() class. Afterwards, add all the tokens we created to a list and pass it as an argument to the PyBuilder() class. By default, the lexer contains the tokens:
+In order for the library to generate the Lexer.py or Lexer.h file, you need to pass a list of tokens to the Builder class.
+To declare a token, you need to import the Token() class from the Builder() class. You need to pass the token name and its value to the Token() class. Afterwards, add all the tokens we created to a list and pass it as an argument to the PyBuilder() or CppBuilder class. By default, the lexer contains the tokens:
 
 ```python
 INT_NUMBER = "INT_NUMBER"
 FLOAT_NUMBER = "FLOAT_NUMBER"
 STRING = "STRING"
 PLUS = "PLUS"
 MINUS = "MINUS"
 VAR = "VAR"
 EOF = "EOF"
 ```
 ### Example of creating a list of tokens:
 ```python
-from LexBuilder.PyLexer import Token
+from LexBuilder.Builder import Token
 
 DIVIDE = Token("DIVIDE", "/")
 PRINT = Token("PRINT", "print")
 INPUT = Token("INPUT", "input")
 
 tokens = [DIVIDE, PRINT, INPUT]
 ```
-## Example:
+#
+## Python Example:
 ### Generate Lexer:
 ```python
-from LexBuilder.PyLexer import PyBuilder, Token
+from LexBuilder.Builder import PyBuilder, Token
 
 
 DIVIDE = Token("DIVIDE", "/")
 PRINT = Token("PRINT", "print")
 INPUT = Token("INPUT", "input")
 
 tokens = [DIVIDE, PRINT, INPUT]
 
 lexer = PyBuilder(tokens)
-lexer.build_lexer()
+lexer.build()
 ```
 
 ### Use Lexer:
 ```python
 from Lexer import *
 
 
@@ -71,7 +72,50 @@
 ```
 
 ```python
 Token(PRINT, "print")
 Token(STRING, "Hello, world!")
 Token(EOF, None)
 ```
+#
+## C++ Example:
+### Generate Lexer:
+```python
+from LexBuilder.Builder import CppBuilder, Token
+
+
+DIVIDE = Token("DIVIDE", "/")
+PRINT = Token("PRINT", "print")
+INPUT = Token("INPUT", "input")
+
+tokens = [DIVIDE, PRINT, INPUT]
+
+lexer = CppBuilder(tokens)
+lexer.build()
+```
+
+### Use Lexer:
+```cpp
+#include "Lexer.h"
+
+using namespace std;
+
+
+int main() {
+    string code = "5 + 5";
+    Lexer lexer(code);
+    Token current_token = lexer.get_next_token();
+    cout << current_token << endl;
+    while (current_token.type != EOF_TOKEN) {
+        current_token = lexer.get_next_token();
+        cout << current_token << endl;
+    }
+}
+
+```
+
+```python
+Token(INT_NUMBER, 5)
+Token(PLUS, +)
+Token(INT_NUMBER, 5)
+Token(EOF, )
+```
```

### Comparing `LexBuilder-1.0.2/PKG-INFO` & `lexbuilder-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,62 @@
 Metadata-Version: 2.1
 Name: LexBuilder
-Version: 1.0.2
+Version: 1.1.0
 Summary: Library for automatic construction of lexers
 Author: Alexander554
 Author-email: gaa.28112008@gmail.com
-Keywords: python lexer
+Keywords: python c++ lexer
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # About LexBuilder:
-LexBuilder is a library for automatically building a lexer in Python. In the future, the library will be able to build lexers in major programming languages such as C++, Golang, Java/Kotlin, etc.
+LexBuilder is a library for automatically building a lexer in Python and C++. In the future, the library will be able to build lexers in major programming languages such as Golang, Java/Kotlin, etc.
 
 ## About Syntax:
-In order for the library to generate the Lexer.py file, you need to pass a list of tokens to the PyBuilder class.
-To declare a token, you need to import the Token() class from the PyLexer() class. You need to pass the token name and its value to the Token() class. Afterwards, add all the tokens we created to a list and pass it as an argument to the PyBuilder() class. By default, the lexer contains the tokens:
+In order for the library to generate the Lexer.py or Lexer.h file, you need to pass a list of tokens to the Builder class.
+To declare a token, you need to import the Token() class from the Builder() class. You need to pass the token name and its value to the Token() class. Afterwards, add all the tokens we created to a list and pass it as an argument to the PyBuilder() or CppBuilder class. By default, the lexer contains the tokens:
 
 ```python
 INT_NUMBER = "INT_NUMBER"
 FLOAT_NUMBER = "FLOAT_NUMBER"
 STRING = "STRING"
 PLUS = "PLUS"
 MINUS = "MINUS"
 VAR = "VAR"
 EOF = "EOF"
 ```
 ### Example of creating a list of tokens:
 ```python
-from LexBuilder.PyLexer import Token
+from LexBuilder.Builder import Token
 
 DIVIDE = Token("DIVIDE", "/")
 PRINT = Token("PRINT", "print")
 INPUT = Token("INPUT", "input")
 
 tokens = [DIVIDE, PRINT, INPUT]
 ```
-## Example:
+#
+## Python Example:
 ### Generate Lexer:
 ```python
-from LexBuilder.PyLexer import PyBuilder, Token
+from LexBuilder.Builder import PyBuilder, Token
 
 
 DIVIDE = Token("DIVIDE", "/")
 PRINT = Token("PRINT", "print")
 INPUT = Token("INPUT", "input")
 
 tokens = [DIVIDE, PRINT, INPUT]
 
 lexer = PyBuilder(tokens)
-lexer.build_lexer()
+lexer.build()
 ```
 
 ### Use Lexer:
 ```python
 from Lexer import *
 
 
@@ -71,7 +72,50 @@
 ```
 
 ```python
 Token(PRINT, "print")
 Token(STRING, "Hello, world!")
 Token(EOF, None)
 ```
+#
+## C++ Example:
+### Generate Lexer:
+```python
+from LexBuilder.Builder import CppBuilder, Token
+
+
+DIVIDE = Token("DIVIDE", "/")
+PRINT = Token("PRINT", "print")
+INPUT = Token("INPUT", "input")
+
+tokens = [DIVIDE, PRINT, INPUT]
+
+lexer = CppBuilder(tokens)
+lexer.build()
+```
+
+### Use Lexer:
+```cpp
+#include "Lexer.h"
+
+using namespace std;
+
+
+int main() {
+    string code = "5 + 5";
+    Lexer lexer(code);
+    Token current_token = lexer.get_next_token();
+    cout << current_token << endl;
+    while (current_token.type != EOF_TOKEN) {
+        current_token = lexer.get_next_token();
+        cout << current_token << endl;
+    }
+}
+
+```
+
+```python
+Token(INT_NUMBER, 5)
+Token(PLUS, +)
+Token(INT_NUMBER, 5)
+Token(EOF, )
+```
```

### Comparing `LexBuilder-1.0.2/README.md` & `lexbuilder-1.1.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 # About LexBuilder:
-LexBuilder is a library for automatically building a lexer in Python. In the future, the library will be able to build lexers in major programming languages such as C++, Golang, Java/Kotlin, etc.
+LexBuilder is a library for automatically building a lexer in Python and C++. In the future, the library will be able to build lexers in major programming languages such as Golang, Java/Kotlin, etc.
 
 ## About Syntax:
-In order for the library to generate the Lexer.py file, you need to pass a list of tokens to the PyBuilder class.
-To declare a token, you need to import the Token() class from the PyLexer() class. You need to pass the token name and its value to the Token() class. Afterwards, add all the tokens we created to a list and pass it as an argument to the PyBuilder() class. By default, the lexer contains the tokens:
+In order for the library to generate the Lexer.py or Lexer.h file, you need to pass a list of tokens to the Builder class.
+To declare a token, you need to import the Token() class from the Builder() class. You need to pass the token name and its value to the Token() class. Afterwards, add all the tokens we created to a list and pass it as an argument to the PyBuilder() or CppBuilder class. By default, the lexer contains the tokens:
 
 ```python
 INT_NUMBER = "INT_NUMBER"
 FLOAT_NUMBER = "FLOAT_NUMBER"
 STRING = "STRING"
 PLUS = "PLUS"
 MINUS = "MINUS"
 VAR = "VAR"
 EOF = "EOF"
 ```
 ### Example of creating a list of tokens:
 ```python
-from LexBuilder.PyLexer import Token
+from LexBuilder.Builder import Token
 
 DIVIDE = Token("DIVIDE", "/")
 PRINT = Token("PRINT", "print")
 INPUT = Token("INPUT", "input")
 
 tokens = [DIVIDE, PRINT, INPUT]
 ```
-## Example:
+#
+## Python Example:
 ### Generate Lexer:
 ```python
-from LexBuilder.PyLexer import PyBuilder, Token
+from LexBuilder.Builder import PyBuilder, Token
 
 
 DIVIDE = Token("DIVIDE", "/")
 PRINT = Token("PRINT", "print")
 INPUT = Token("INPUT", "input")
 
 tokens = [DIVIDE, PRINT, INPUT]
 
 lexer = PyBuilder(tokens)
-lexer.build_lexer()
+lexer.build()
 ```
 
 ### Use Lexer:
 ```python
 from Lexer import *
 
 
@@ -57,7 +58,50 @@
 ```
 
 ```python
 Token(PRINT, "print")
 Token(STRING, "Hello, world!")
 Token(EOF, None)
 ```
+#
+## C++ Example:
+### Generate Lexer:
+```python
+from LexBuilder.Builder import CppBuilder, Token
+
+
+DIVIDE = Token("DIVIDE", "/")
+PRINT = Token("PRINT", "print")
+INPUT = Token("INPUT", "input")
+
+tokens = [DIVIDE, PRINT, INPUT]
+
+lexer = CppBuilder(tokens)
+lexer.build()
+```
+
+### Use Lexer:
+```cpp
+#include "Lexer.h"
+
+using namespace std;
+
+
+int main() {
+    string code = "5 + 5";
+    Lexer lexer(code);
+    Token current_token = lexer.get_next_token();
+    cout << current_token << endl;
+    while (current_token.type != EOF_TOKEN) {
+        current_token = lexer.get_next_token();
+        cout << current_token << endl;
+    }
+}
+
+```
+
+```python
+Token(INT_NUMBER, 5)
+Token(PLUS, +)
+Token(INT_NUMBER, 5)
+Token(EOF, )
+```
```

### Comparing `LexBuilder-1.0.2/setup.py` & `lexbuilder-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 setup(
   name='LexBuilder',
-  version='1.0.2',
+  version='1.1.0',
   author='Alexander554',
   author_email='gaa.28112008@gmail.com',
   description='Library for automatic construction of lexers',
   long_description=readme(),
   long_description_content_type='text/markdown',
   packages=find_packages(),
   install_requires=[''],
   classifiers=[
     'Programming Language :: Python :: 3.11',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent'
   ],
-  keywords='python lexer',
+  keywords='python c++ lexer',
   python_requires='>=3.7'
 )
```

