# Comparing `tmp/multiform-validator-0.0.6.tar.gz` & `tmp/multiform_validator-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiform-validator-0.0.6.tar", last modified: Wed Mar 27 06:45:48 2024, max compression
+gzip compressed data, was "multiform_validator-0.0.7.tar", last modified: Mon May  6 06:31:18 2024, max compression
```

## Comparing `multiform-validator-0.0.6.tar` & `multiform_validator-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 06:45:48.296776 multiform-validator-0.0.6/
--rw-rw-rw-   0        0        0     1074 2024-03-15 22:10:05.000000 multiform-validator-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     4373 2024-03-27 06:45:48.296776 multiform-validator-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3705 2024-03-27 06:41:10.000000 multiform-validator-0.0.6/README.md
--rw-rw-rw-   0        0        0      638 2024-03-27 06:44:14.000000 multiform-validator-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-27 06:45:48.296776 multiform-validator-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-27 06:45:47.864962 multiform-validator-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-03-27 06:45:48.249940 multiform-validator-0.0.6/src/multiform_validator/
--rw-rw-rw-   0        0        0      389 2023-10-18 00:54:32.000000 multiform-validator-0.0.6/src/multiform_validator/__init__.py
--rw-rw-rw-   0        0        0     2222 2024-03-27 06:37:56.000000 multiform-validator-0.0.6/src/multiform_validator/cnpjValidator.py
--rw-rw-rw-   0        0        0     2496 2024-03-27 06:38:21.000000 multiform-validator-0.0.6/src/multiform_validator/cpfValidator.py
--rw-rw-rw-   0        0        0     2700 2024-03-27 06:38:41.000000 multiform-validator-0.0.6/src/multiform_validator/getOnlyEmail.py
--rw-rw-rw-   0        0        0     1132 2024-03-27 06:38:57.000000 multiform-validator-0.0.6/src/multiform_validator/identifyFlagCard.py
--rw-rw-rw-   0        0        0      679 2024-03-27 06:39:14.000000 multiform-validator-0.0.6/src/multiform_validator/isCreditCardValid.py
--rw-rw-rw-   0        0        0      706 2024-03-27 06:39:21.000000 multiform-validator-0.0.6/src/multiform_validator/isEmail.py
--rw-rw-rw-   0        0        0     1461 2024-03-27 06:39:26.000000 multiform-validator-0.0.6/src/multiform_validator/passwordStrengthTester.py
--rw-rw-rw-   0        0        0     1139 2024-03-27 06:39:38.000000 multiform-validator-0.0.6/src/multiform_validator/validateBRPhoneNumber.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:45:48.296776 multiform-validator-0.0.6/src/multiform_validator.egg-info/
--rw-rw-rw-   0        0        0     4373 2024-03-27 06:45:47.000000 multiform-validator-0.0.6/src/multiform_validator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      600 2024-03-27 06:45:47.000000 multiform-validator-0.0.6/src/multiform_validator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 06:45:47.000000 multiform-validator-0.0.6/src/multiform_validator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-03-27 06:45:47.000000 multiform-validator-0.0.6/src/multiform_validator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-06 06:31:18.915777 multiform_validator-0.0.7/
+-rw-rw-rw-   0        0        0     1074 2024-03-15 22:10:05.000000 multiform_validator-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     4027 2024-05-06 06:31:18.897799 multiform_validator-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3277 2024-05-06 06:21:19.000000 multiform_validator-0.0.7/README.md
+-rw-rw-rw-   0        0        0      728 2024-05-06 06:19:31.000000 multiform_validator-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-06 06:31:18.916765 multiform_validator-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-06 06:31:18.600974 multiform_validator-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2024-05-06 06:31:18.866872 multiform_validator-0.0.7/src/multiform_validator/
+-rw-rw-rw-   0        0        0      389 2023-10-18 00:54:32.000000 multiform_validator-0.0.7/src/multiform_validator/__init__.py
+-rw-rw-rw-   0        0        0     2222 2024-03-27 06:37:56.000000 multiform_validator-0.0.7/src/multiform_validator/cnpjValidator.py
+-rw-rw-rw-   0        0        0     2496 2024-04-19 06:28:03.000000 multiform_validator-0.0.7/src/multiform_validator/cpfValidator.py
+-rw-rw-rw-   0        0        0     2700 2024-03-27 06:38:41.000000 multiform_validator-0.0.7/src/multiform_validator/getOnlyEmail.py
+-rw-rw-rw-   0        0        0     1132 2024-03-27 06:38:57.000000 multiform_validator-0.0.7/src/multiform_validator/identifyFlagCard.py
+-rw-rw-rw-   0        0        0      679 2024-03-27 06:39:14.000000 multiform_validator-0.0.7/src/multiform_validator/isCreditCardValid.py
+-rw-rw-rw-   0        0        0     1258 2024-05-06 06:23:22.000000 multiform_validator-0.0.7/src/multiform_validator/isEmail.py
+-rw-rw-rw-   0        0        0     1461 2024-03-27 06:39:26.000000 multiform_validator-0.0.7/src/multiform_validator/passwordStrengthTester.py
+-rw-rw-rw-   0        0        0     1139 2024-03-27 06:39:38.000000 multiform_validator-0.0.7/src/multiform_validator/validateBRPhoneNumber.py
+drwxrwxrwx   0        0        0        0 2024-05-06 06:31:18.897799 multiform_validator-0.0.7/src/multiform_validator.egg-info/
+-rw-rw-rw-   0        0        0     4027 2024-05-06 06:31:18.000000 multiform_validator-0.0.7/src/multiform_validator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      600 2024-05-06 06:31:18.000000 multiform_validator-0.0.7/src/multiform_validator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 06:31:18.000000 multiform_validator-0.0.7/src/multiform_validator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-06 06:31:18.000000 multiform_validator-0.0.7/src/multiform_validator.egg-info/top_level.txt
```

### Comparing `multiform-validator-0.0.6/LICENSE` & `multiform_validator-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `multiform-validator-0.0.6/PKG-INFO` & `multiform_validator-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: multiform-validator
-Version: 0.0.6
-Summary: Multiform-validator package
+Version: 0.0.7
+Summary: Multilingual library made for validation, various form fields, such as: email, cpf, cnpj, credit card, and much more.
 Author: Gabriel Logan
 Project-URL: Homepage, https://github.com/gabriel-logan/multiform-validator/tree/main/packages/python
 Project-URL: Bug Tracker, https://github.com/gabriel-logan/multiform-validator/tree/main/packages/python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -14,16 +14,14 @@
 
 # Multiform-validator
 
 [![PyPI version](https://badge.fury.io/py/multiform-validator.svg)](https://badge.fury.io/py/multiform-validator)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI downloads](https://img.shields.io/pypi/dm/multiform-validator.svg?style=flat-square)](https://pypistats.org/packages/multiform-validator)
 
-# Library is in testing period
-
 This package provides Python functions to validate various forms fields.
 
 Documentation: https://github.com/gabriel-logan/multiform-validator
 
 Feel free to find bugs and report them to me. Your feedback is highly appreciated. Hugs from Gabriel Logan!
 
 If you want to help me, you can buy me a coffee (:
@@ -36,14 +34,18 @@
 
 ### Installation
 
 ```bash
 pip install multiform-validator
 ```
 
+# Data Validator
+
+This package contains various modules for validating different types of data. Below are the available validation modules:
+
 # Avaliable for while
 
 - **cnpjValidator**: CNPJ validation.
 - **cpfValidator**: CPF validation.
 - **getOnlyEmail**: Extracts only the email or emails address from a string.
 - **identifyFlagCard**: Identifies the flag of a credit card.
 - **isCreditCardValid**: Credit card validation.
@@ -60,46 +62,36 @@
     isCreditCardValid,
     isEmail,
     passwordStrengthTester,
     validateBRPhoneNumber
 )
 ```
 
-# Data Validator
-
-This package contains various modules for validating different types of data. Below are the available validation modules:
+## Looking for contributions. 
 
 ## Available Validation Modules !!! STILL NOT AVALIABLE !!!
 
-- **cnpjValidator**: CNPJ validation.
-- **cpfValidator**: CPF validation.
-- **getOnlyEmail**: Extracts only the email or emails address from a string.
-- **identifyFlagCard**: Identifies the flag of a credit card.
 - **isAscii**: Checks if the string contains only ASCII characters.
 - **isBase64**: Checks if the string is a valid Base64 encoding.
 - **isCEP**: CEP validation (Brazilian postal code).
-- **isCreditCardValid**: Credit card validation.
 - **isDate**: Date format validation.
 - **isDecimal**: Checks if the number is a decimal.
-- **isEmail**: Email address validation format.
 - **isEmpty**: Checks if the string is empty.
 - **isMACAddress**: MAC address validation.
 - **isMD5**: Checks if the string is a valid MD5 hash.
 - **validatePassportNumber**: Passport number validation.
 - **isPort**: Port number validation.
 - **isPostalCode**: Postal code validation.
 - **isTime**: Time format validation.
-- **validateBRPhoneNumber**: Brazilian phone number validation.
 - **validateEmail**: Email address full validation.
 - **validatePassword**: Password validation.
 - **validatePhoneNumber**: Phone number validation.
 - **validateUsername**: Username validation.
 - **validateUSPhoneNumber**: US phone number validation.
 - **isNumber**: Checks if the value is a number.
-- **passwordStrengthTester**: Password strength test.
 - **validateName**: Name validation.
 - **validateSurname**: Surname validation.
 - **validateTextarea**: Textarea validation.
 
 ### For better information, read the documentation
 
 Feel free to explore the various functions and experiment with different inputs to understand their behavior. If you encounter any issues or have suggestions, don't hesitate to reach out to me. Your feedback is valuable and helps improve the package. Happy coding!
```

#### html2text {}

```diff
@@ -1,54 +1,50 @@
-Metadata-Version: 2.1 Name: multiform-validator Version: 0.0.6 Summary:
-Multiform-validator package Author: Gabriel Logan Project-URL: Homepage, https:
-//github.com/gabriel-logan/multiform-validator/tree/main/packages/python
-Project-URL: Bug Tracker, https://github.com/gabriel-logan/multiform-validator/
-tree/main/packages/python Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
-markdown License-File: LICENSE # Multiform-validator [![PyPI version](https://
-badge.fury.io/py/multiform-validator.svg)](https://badge.fury.io/py/multiform-
-validator) [![License: MIT](https://img.shields.io/badge/License-MIT-
-yellow.svg)](https://opensource.org/licenses/MIT) [![PyPI downloads](https://
-img.shields.io/pypi/dm/multiform-validator.svg?style=flat-square)](https://
-pypistats.org/packages/multiform-validator) # Library is in testing period This
-package provides Python functions to validate various forms fields.
-Documentation: https://github.com/gabriel-logan/multiform-validator Feel free
-to find bugs and report them to me. Your feedback is highly appreciated. Hugs
-from Gabriel Logan! If you want to help me, you can buy me a coffee (:
+Metadata-Version: 2.1 Name: multiform-validator Version: 0.0.7 Summary:
+Multilingual library made for validation, various form fields, such as: email,
+cpf, cnpj, credit card, and much more. Author: Gabriel Logan Project-URL:
+Homepage, https://github.com/gabriel-logan/multiform-validator/tree/main/
+packages/python Project-URL: Bug Tracker, https://github.com/gabriel-logan/
+multiform-validator/tree/main/packages/python Classifier: Programming Language
+:: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Requires-Python: >=3.7 Description-Content-
+Type: text/markdown License-File: LICENSE # Multiform-validator [![PyPI
+version](https://badge.fury.io/py/multiform-validator.svg)](https://
+badge.fury.io/py/multiform-validator) [![License: MIT](https://img.shields.io/
+badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![PyPI
+downloads](https://img.shields.io/pypi/dm/multiform-validator.svg?style=flat-
+square)](https://pypistats.org/packages/multiform-validator) This package
+provides Python functions to validate various forms fields. Documentation:
+https://github.com/gabriel-logan/multiform-validator Feel free to find bugs and
+report them to me. Your feedback is highly appreciated. Hugs from Gabriel
+Logan! If you want to help me, you can buy me a coffee (:
                                _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
-### Installation ```bash pip install multiform-validator ``` # Avaliable for
-while - **cnpjValidator**: CNPJ validation. - **cpfValidator**: CPF validation.
-- **getOnlyEmail**: Extracts only the email or emails address from a string. -
+### Installation ```bash pip install multiform-validator ``` # Data Validator
+This package contains various modules for validating different types of data.
+Below are the available validation modules: # Avaliable for while -
+**cnpjValidator**: CNPJ validation. - **cpfValidator**: CPF validation. -
+**getOnlyEmail**: Extracts only the email or emails address from a string. -
 **identifyFlagCard**: Identifies the flag of a credit card. -
 **isCreditCardValid**: Credit card validation. - **isEmail**: Email address
 validation format. - **passwordStrengthTester**: Password strength test. -
 **validateBRPhoneNumber**: Brazilian phone number validation. ```python from
 multiform_validator import ( cnpjIsValid, cpfIsValid, getOnlyEmail,
 identifyFlagCard, isCreditCardValid, isEmail, passwordStrengthTester,
-validateBRPhoneNumber ) ``` # Data Validator This package contains various
-modules for validating different types of data. Below are the available
-validation modules: ## Available Validation Modules !!! STILL NOT AVALIABLE !!!
-- **cnpjValidator**: CNPJ validation. - **cpfValidator**: CPF validation. -
-**getOnlyEmail**: Extracts only the email or emails address from a string. -
-**identifyFlagCard**: Identifies the flag of a credit card. - **isAscii**:
-Checks if the string contains only ASCII characters. - **isBase64**: Checks if
-the string is a valid Base64 encoding. - **isCEP**: CEP validation (Brazilian
-postal code). - **isCreditCardValid**: Credit card validation. - **isDate**:
-Date format validation. - **isDecimal**: Checks if the number is a decimal. -
-**isEmail**: Email address validation format. - **isEmpty**: Checks if the
-string is empty. - **isMACAddress**: MAC address validation. - **isMD5**:
-Checks if the string is a valid MD5 hash. - **validatePassportNumber**:
-Passport number validation. - **isPort**: Port number validation. -
-**isPostalCode**: Postal code validation. - **isTime**: Time format validation.
-- **validateBRPhoneNumber**: Brazilian phone number validation. -
-**validateEmail**: Email address full validation. - **validatePassword**:
-Password validation. - **validatePhoneNumber**: Phone number validation. -
-**validateUsername**: Username validation. - **validateUSPhoneNumber**: US
-phone number validation. - **isNumber**: Checks if the value is a number. -
-**passwordStrengthTester**: Password strength test. - **validateName**: Name
-validation. - **validateSurname**: Surname validation. - **validateTextarea**:
-Textarea validation. ### For better information, read the documentation Feel
-free to explore the various functions and experiment with different inputs to
+validateBRPhoneNumber ) ``` ## Looking for contributions. ## Available
+Validation Modules !!! STILL NOT AVALIABLE !!! - **isAscii**: Checks if the
+string contains only ASCII characters. - **isBase64**: Checks if the string is
+a valid Base64 encoding. - **isCEP**: CEP validation (Brazilian postal code). -
+**isDate**: Date format validation. - **isDecimal**: Checks if the number is a
+decimal. - **isEmpty**: Checks if the string is empty. - **isMACAddress**: MAC
+address validation. - **isMD5**: Checks if the string is a valid MD5 hash. -
+**validatePassportNumber**: Passport number validation. - **isPort**: Port
+number validation. - **isPostalCode**: Postal code validation. - **isTime**:
+Time format validation. - **validateEmail**: Email address full validation. -
+**validatePassword**: Password validation. - **validatePhoneNumber**: Phone
+number validation. - **validateUsername**: Username validation. -
+**validateUSPhoneNumber**: US phone number validation. - **isNumber**: Checks
+if the value is a number. - **validateName**: Name validation. -
+**validateSurname**: Surname validation. - **validateTextarea**: Textarea
+validation. ### For better information, read the documentation Feel free to
+explore the various functions and experiment with different inputs to
 understand their behavior. If you encounter any issues or have suggestions,
 don't hesitate to reach out to me. Your feedback is valuable and helps improve
 the package. Happy coding! # By - Gabriel Logan
```

### Comparing `multiform-validator-0.0.6/README.md` & `multiform_validator-0.0.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # Multiform-validator
 
 [![PyPI version](https://badge.fury.io/py/multiform-validator.svg)](https://badge.fury.io/py/multiform-validator)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI downloads](https://img.shields.io/pypi/dm/multiform-validator.svg?style=flat-square)](https://pypistats.org/packages/multiform-validator)
 
-# Library is in testing period
-
 This package provides Python functions to validate various forms fields.
 
 Documentation: https://github.com/gabriel-logan/multiform-validator
 
 Feel free to find bugs and report them to me. Your feedback is highly appreciated. Hugs from Gabriel Logan!
 
 If you want to help me, you can buy me a coffee (:
@@ -22,14 +20,18 @@
 
 ### Installation
 
 ```bash
 pip install multiform-validator
 ```
 
+# Data Validator
+
+This package contains various modules for validating different types of data. Below are the available validation modules:
+
 # Avaliable for while
 
 - **cnpjValidator**: CNPJ validation.
 - **cpfValidator**: CPF validation.
 - **getOnlyEmail**: Extracts only the email or emails address from a string.
 - **identifyFlagCard**: Identifies the flag of a credit card.
 - **isCreditCardValid**: Credit card validation.
@@ -46,46 +48,36 @@
     isCreditCardValid,
     isEmail,
     passwordStrengthTester,
     validateBRPhoneNumber
 )
 ```
 
-# Data Validator
-
-This package contains various modules for validating different types of data. Below are the available validation modules:
+## Looking for contributions. 
 
 ## Available Validation Modules !!! STILL NOT AVALIABLE !!!
 
-- **cnpjValidator**: CNPJ validation.
-- **cpfValidator**: CPF validation.
-- **getOnlyEmail**: Extracts only the email or emails address from a string.
-- **identifyFlagCard**: Identifies the flag of a credit card.
 - **isAscii**: Checks if the string contains only ASCII characters.
 - **isBase64**: Checks if the string is a valid Base64 encoding.
 - **isCEP**: CEP validation (Brazilian postal code).
-- **isCreditCardValid**: Credit card validation.
 - **isDate**: Date format validation.
 - **isDecimal**: Checks if the number is a decimal.
-- **isEmail**: Email address validation format.
 - **isEmpty**: Checks if the string is empty.
 - **isMACAddress**: MAC address validation.
 - **isMD5**: Checks if the string is a valid MD5 hash.
 - **validatePassportNumber**: Passport number validation.
 - **isPort**: Port number validation.
 - **isPostalCode**: Postal code validation.
 - **isTime**: Time format validation.
-- **validateBRPhoneNumber**: Brazilian phone number validation.
 - **validateEmail**: Email address full validation.
 - **validatePassword**: Password validation.
 - **validatePhoneNumber**: Phone number validation.
 - **validateUsername**: Username validation.
 - **validateUSPhoneNumber**: US phone number validation.
 - **isNumber**: Checks if the value is a number.
-- **passwordStrengthTester**: Password strength test.
 - **validateName**: Name validation.
 - **validateSurname**: Surname validation.
 - **validateTextarea**: Textarea validation.
 
 ### For better information, read the documentation
 
 Feel free to explore the various functions and experiment with different inputs to understand their behavior. If you encounter any issues or have suggestions, don't hesitate to reach out to me. Your feedback is valuable and helps improve the package. Happy coding!
```

#### html2text {}

```diff
@@ -1,47 +1,42 @@
 # Multiform-validator [![PyPI version](https://badge.fury.io/py/multiform-
 validator.svg)](https://badge.fury.io/py/multiform-validator) [![License: MIT]
 (https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/
 licenses/MIT) [![PyPI downloads](https://img.shields.io/pypi/dm/multiform-
 validator.svg?style=flat-square)](https://pypistats.org/packages/multiform-
-validator) # Library is in testing period This package provides Python
-functions to validate various forms fields. Documentation: https://github.com/
-gabriel-logan/multiform-validator Feel free to find bugs and report them to me.
-Your feedback is highly appreciated. Hugs from Gabriel Logan! If you want to
-help me, you can buy me a coffee (:
+validator) This package provides Python functions to validate various forms
+fields. Documentation: https://github.com/gabriel-logan/multiform-validator
+Feel free to find bugs and report them to me. Your feedback is highly
+appreciated. Hugs from Gabriel Logan! If you want to help me, you can buy me a
+coffee (:
                                _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
-### Installation ```bash pip install multiform-validator ``` # Avaliable for
-while - **cnpjValidator**: CNPJ validation. - **cpfValidator**: CPF validation.
-- **getOnlyEmail**: Extracts only the email or emails address from a string. -
+### Installation ```bash pip install multiform-validator ``` # Data Validator
+This package contains various modules for validating different types of data.
+Below are the available validation modules: # Avaliable for while -
+**cnpjValidator**: CNPJ validation. - **cpfValidator**: CPF validation. -
+**getOnlyEmail**: Extracts only the email or emails address from a string. -
 **identifyFlagCard**: Identifies the flag of a credit card. -
 **isCreditCardValid**: Credit card validation. - **isEmail**: Email address
 validation format. - **passwordStrengthTester**: Password strength test. -
 **validateBRPhoneNumber**: Brazilian phone number validation. ```python from
 multiform_validator import ( cnpjIsValid, cpfIsValid, getOnlyEmail,
 identifyFlagCard, isCreditCardValid, isEmail, passwordStrengthTester,
-validateBRPhoneNumber ) ``` # Data Validator This package contains various
-modules for validating different types of data. Below are the available
-validation modules: ## Available Validation Modules !!! STILL NOT AVALIABLE !!!
-- **cnpjValidator**: CNPJ validation. - **cpfValidator**: CPF validation. -
-**getOnlyEmail**: Extracts only the email or emails address from a string. -
-**identifyFlagCard**: Identifies the flag of a credit card. - **isAscii**:
-Checks if the string contains only ASCII characters. - **isBase64**: Checks if
-the string is a valid Base64 encoding. - **isCEP**: CEP validation (Brazilian
-postal code). - **isCreditCardValid**: Credit card validation. - **isDate**:
-Date format validation. - **isDecimal**: Checks if the number is a decimal. -
-**isEmail**: Email address validation format. - **isEmpty**: Checks if the
-string is empty. - **isMACAddress**: MAC address validation. - **isMD5**:
-Checks if the string is a valid MD5 hash. - **validatePassportNumber**:
-Passport number validation. - **isPort**: Port number validation. -
-**isPostalCode**: Postal code validation. - **isTime**: Time format validation.
-- **validateBRPhoneNumber**: Brazilian phone number validation. -
-**validateEmail**: Email address full validation. - **validatePassword**:
-Password validation. - **validatePhoneNumber**: Phone number validation. -
-**validateUsername**: Username validation. - **validateUSPhoneNumber**: US
-phone number validation. - **isNumber**: Checks if the value is a number. -
-**passwordStrengthTester**: Password strength test. - **validateName**: Name
-validation. - **validateSurname**: Surname validation. - **validateTextarea**:
-Textarea validation. ### For better information, read the documentation Feel
-free to explore the various functions and experiment with different inputs to
+validateBRPhoneNumber ) ``` ## Looking for contributions. ## Available
+Validation Modules !!! STILL NOT AVALIABLE !!! - **isAscii**: Checks if the
+string contains only ASCII characters. - **isBase64**: Checks if the string is
+a valid Base64 encoding. - **isCEP**: CEP validation (Brazilian postal code). -
+**isDate**: Date format validation. - **isDecimal**: Checks if the number is a
+decimal. - **isEmpty**: Checks if the string is empty. - **isMACAddress**: MAC
+address validation. - **isMD5**: Checks if the string is a valid MD5 hash. -
+**validatePassportNumber**: Passport number validation. - **isPort**: Port
+number validation. - **isPostalCode**: Postal code validation. - **isTime**:
+Time format validation. - **validateEmail**: Email address full validation. -
+**validatePassword**: Password validation. - **validatePhoneNumber**: Phone
+number validation. - **validateUsername**: Username validation. -
+**validateUSPhoneNumber**: US phone number validation. - **isNumber**: Checks
+if the value is a number. - **validateName**: Name validation. -
+**validateSurname**: Surname validation. - **validateTextarea**: Textarea
+validation. ### For better information, read the documentation Feel free to
+explore the various functions and experiment with different inputs to
 understand their behavior. If you encounter any issues or have suggestions,
 don't hesitate to reach out to me. Your feedback is valuable and helps improve
 the package. Happy coding! # By - Gabriel Logan
```

### Comparing `multiform-validator-0.0.6/pyproject.toml` & `multiform_validator-0.0.7/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 requires = [
     "setuptools>=61"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "multiform-validator"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Gabriel Logan" },
 ]
-description = "Multiform-validator package"
+description = "Multilingual library made for validation, various form fields, such as: email, cpf, cnpj, credit card, and much more."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `multiform-validator-0.0.6/src/multiform_validator/cnpjValidator.py` & `multiform_validator-0.0.7/src/multiform_validator/cnpjValidator.py`

 * *Files identical despite different names*

### Comparing `multiform-validator-0.0.6/src/multiform_validator/cpfValidator.py` & `multiform_validator-0.0.7/src/multiform_validator/cpfValidator.py`

 * *Files identical despite different names*

### Comparing `multiform-validator-0.0.6/src/multiform_validator/getOnlyEmail.py` & `multiform_validator-0.0.7/src/multiform_validator/getOnlyEmail.py`

 * *Files identical despite different names*

### Comparing `multiform-validator-0.0.6/src/multiform_validator/identifyFlagCard.py` & `multiform_validator-0.0.7/src/multiform_validator/identifyFlagCard.py`

 * *Files identical despite different names*

### Comparing `multiform-validator-0.0.6/src/multiform_validator/isCreditCardValid.py` & `multiform_validator-0.0.7/src/multiform_validator/isCreditCardValid.py`

 * *Files identical despite different names*

### Comparing `multiform-validator-0.0.6/src/multiform_validator/passwordStrengthTester.py` & `multiform_validator-0.0.7/src/multiform_validator/passwordStrengthTester.py`

 * *Files identical despite different names*

### Comparing `multiform-validator-0.0.6/src/multiform_validator/validateBRPhoneNumber.py` & `multiform_validator-0.0.7/src/multiform_validator/validateBRPhoneNumber.py`

 * *Files identical despite different names*

### Comparing `multiform-validator-0.0.6/src/multiform_validator.egg-info/PKG-INFO` & `multiform_validator-0.0.7/src/multiform_validator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: multiform-validator
-Version: 0.0.6
-Summary: Multiform-validator package
+Version: 0.0.7
+Summary: Multilingual library made for validation, various form fields, such as: email, cpf, cnpj, credit card, and much more.
 Author: Gabriel Logan
 Project-URL: Homepage, https://github.com/gabriel-logan/multiform-validator/tree/main/packages/python
 Project-URL: Bug Tracker, https://github.com/gabriel-logan/multiform-validator/tree/main/packages/python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -14,16 +14,14 @@
 
 # Multiform-validator
 
 [![PyPI version](https://badge.fury.io/py/multiform-validator.svg)](https://badge.fury.io/py/multiform-validator)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI downloads](https://img.shields.io/pypi/dm/multiform-validator.svg?style=flat-square)](https://pypistats.org/packages/multiform-validator)
 
-# Library is in testing period
-
 This package provides Python functions to validate various forms fields.
 
 Documentation: https://github.com/gabriel-logan/multiform-validator
 
 Feel free to find bugs and report them to me. Your feedback is highly appreciated. Hugs from Gabriel Logan!
 
 If you want to help me, you can buy me a coffee (:
@@ -36,14 +34,18 @@
 
 ### Installation
 
 ```bash
 pip install multiform-validator
 ```
 
+# Data Validator
+
+This package contains various modules for validating different types of data. Below are the available validation modules:
+
 # Avaliable for while
 
 - **cnpjValidator**: CNPJ validation.
 - **cpfValidator**: CPF validation.
 - **getOnlyEmail**: Extracts only the email or emails address from a string.
 - **identifyFlagCard**: Identifies the flag of a credit card.
 - **isCreditCardValid**: Credit card validation.
@@ -60,46 +62,36 @@
     isCreditCardValid,
     isEmail,
     passwordStrengthTester,
     validateBRPhoneNumber
 )
 ```
 
-# Data Validator
-
-This package contains various modules for validating different types of data. Below are the available validation modules:
+## Looking for contributions. 
 
 ## Available Validation Modules !!! STILL NOT AVALIABLE !!!
 
-- **cnpjValidator**: CNPJ validation.
-- **cpfValidator**: CPF validation.
-- **getOnlyEmail**: Extracts only the email or emails address from a string.
-- **identifyFlagCard**: Identifies the flag of a credit card.
 - **isAscii**: Checks if the string contains only ASCII characters.
 - **isBase64**: Checks if the string is a valid Base64 encoding.
 - **isCEP**: CEP validation (Brazilian postal code).
-- **isCreditCardValid**: Credit card validation.
 - **isDate**: Date format validation.
 - **isDecimal**: Checks if the number is a decimal.
-- **isEmail**: Email address validation format.
 - **isEmpty**: Checks if the string is empty.
 - **isMACAddress**: MAC address validation.
 - **isMD5**: Checks if the string is a valid MD5 hash.
 - **validatePassportNumber**: Passport number validation.
 - **isPort**: Port number validation.
 - **isPostalCode**: Postal code validation.
 - **isTime**: Time format validation.
-- **validateBRPhoneNumber**: Brazilian phone number validation.
 - **validateEmail**: Email address full validation.
 - **validatePassword**: Password validation.
 - **validatePhoneNumber**: Phone number validation.
 - **validateUsername**: Username validation.
 - **validateUSPhoneNumber**: US phone number validation.
 - **isNumber**: Checks if the value is a number.
-- **passwordStrengthTester**: Password strength test.
 - **validateName**: Name validation.
 - **validateSurname**: Surname validation.
 - **validateTextarea**: Textarea validation.
 
 ### For better information, read the documentation
 
 Feel free to explore the various functions and experiment with different inputs to understand their behavior. If you encounter any issues or have suggestions, don't hesitate to reach out to me. Your feedback is valuable and helps improve the package. Happy coding!
```

#### html2text {}

```diff
@@ -1,54 +1,50 @@
-Metadata-Version: 2.1 Name: multiform-validator Version: 0.0.6 Summary:
-Multiform-validator package Author: Gabriel Logan Project-URL: Homepage, https:
-//github.com/gabriel-logan/multiform-validator/tree/main/packages/python
-Project-URL: Bug Tracker, https://github.com/gabriel-logan/multiform-validator/
-tree/main/packages/python Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
-markdown License-File: LICENSE # Multiform-validator [![PyPI version](https://
-badge.fury.io/py/multiform-validator.svg)](https://badge.fury.io/py/multiform-
-validator) [![License: MIT](https://img.shields.io/badge/License-MIT-
-yellow.svg)](https://opensource.org/licenses/MIT) [![PyPI downloads](https://
-img.shields.io/pypi/dm/multiform-validator.svg?style=flat-square)](https://
-pypistats.org/packages/multiform-validator) # Library is in testing period This
-package provides Python functions to validate various forms fields.
-Documentation: https://github.com/gabriel-logan/multiform-validator Feel free
-to find bugs and report them to me. Your feedback is highly appreciated. Hugs
-from Gabriel Logan! If you want to help me, you can buy me a coffee (:
+Metadata-Version: 2.1 Name: multiform-validator Version: 0.0.7 Summary:
+Multilingual library made for validation, various form fields, such as: email,
+cpf, cnpj, credit card, and much more. Author: Gabriel Logan Project-URL:
+Homepage, https://github.com/gabriel-logan/multiform-validator/tree/main/
+packages/python Project-URL: Bug Tracker, https://github.com/gabriel-logan/
+multiform-validator/tree/main/packages/python Classifier: Programming Language
+:: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Requires-Python: >=3.7 Description-Content-
+Type: text/markdown License-File: LICENSE # Multiform-validator [![PyPI
+version](https://badge.fury.io/py/multiform-validator.svg)](https://
+badge.fury.io/py/multiform-validator) [![License: MIT](https://img.shields.io/
+badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) [![PyPI
+downloads](https://img.shields.io/pypi/dm/multiform-validator.svg?style=flat-
+square)](https://pypistats.org/packages/multiform-validator) This package
+provides Python functions to validate various forms fields. Documentation:
+https://github.com/gabriel-logan/multiform-validator Feel free to find bugs and
+report them to me. Your feedback is highly appreciated. Hugs from Gabriel
+Logan! If you want to help me, you can buy me a coffee (:
                                _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
-### Installation ```bash pip install multiform-validator ``` # Avaliable for
-while - **cnpjValidator**: CNPJ validation. - **cpfValidator**: CPF validation.
-- **getOnlyEmail**: Extracts only the email or emails address from a string. -
+### Installation ```bash pip install multiform-validator ``` # Data Validator
+This package contains various modules for validating different types of data.
+Below are the available validation modules: # Avaliable for while -
+**cnpjValidator**: CNPJ validation. - **cpfValidator**: CPF validation. -
+**getOnlyEmail**: Extracts only the email or emails address from a string. -
 **identifyFlagCard**: Identifies the flag of a credit card. -
 **isCreditCardValid**: Credit card validation. - **isEmail**: Email address
 validation format. - **passwordStrengthTester**: Password strength test. -
 **validateBRPhoneNumber**: Brazilian phone number validation. ```python from
 multiform_validator import ( cnpjIsValid, cpfIsValid, getOnlyEmail,
 identifyFlagCard, isCreditCardValid, isEmail, passwordStrengthTester,
-validateBRPhoneNumber ) ``` # Data Validator This package contains various
-modules for validating different types of data. Below are the available
-validation modules: ## Available Validation Modules !!! STILL NOT AVALIABLE !!!
-- **cnpjValidator**: CNPJ validation. - **cpfValidator**: CPF validation. -
-**getOnlyEmail**: Extracts only the email or emails address from a string. -
-**identifyFlagCard**: Identifies the flag of a credit card. - **isAscii**:
-Checks if the string contains only ASCII characters. - **isBase64**: Checks if
-the string is a valid Base64 encoding. - **isCEP**: CEP validation (Brazilian
-postal code). - **isCreditCardValid**: Credit card validation. - **isDate**:
-Date format validation. - **isDecimal**: Checks if the number is a decimal. -
-**isEmail**: Email address validation format. - **isEmpty**: Checks if the
-string is empty. - **isMACAddress**: MAC address validation. - **isMD5**:
-Checks if the string is a valid MD5 hash. - **validatePassportNumber**:
-Passport number validation. - **isPort**: Port number validation. -
-**isPostalCode**: Postal code validation. - **isTime**: Time format validation.
-- **validateBRPhoneNumber**: Brazilian phone number validation. -
-**validateEmail**: Email address full validation. - **validatePassword**:
-Password validation. - **validatePhoneNumber**: Phone number validation. -
-**validateUsername**: Username validation. - **validateUSPhoneNumber**: US
-phone number validation. - **isNumber**: Checks if the value is a number. -
-**passwordStrengthTester**: Password strength test. - **validateName**: Name
-validation. - **validateSurname**: Surname validation. - **validateTextarea**:
-Textarea validation. ### For better information, read the documentation Feel
-free to explore the various functions and experiment with different inputs to
+validateBRPhoneNumber ) ``` ## Looking for contributions. ## Available
+Validation Modules !!! STILL NOT AVALIABLE !!! - **isAscii**: Checks if the
+string contains only ASCII characters. - **isBase64**: Checks if the string is
+a valid Base64 encoding. - **isCEP**: CEP validation (Brazilian postal code). -
+**isDate**: Date format validation. - **isDecimal**: Checks if the number is a
+decimal. - **isEmpty**: Checks if the string is empty. - **isMACAddress**: MAC
+address validation. - **isMD5**: Checks if the string is a valid MD5 hash. -
+**validatePassportNumber**: Passport number validation. - **isPort**: Port
+number validation. - **isPostalCode**: Postal code validation. - **isTime**:
+Time format validation. - **validateEmail**: Email address full validation. -
+**validatePassword**: Password validation. - **validatePhoneNumber**: Phone
+number validation. - **validateUsername**: Username validation. -
+**validateUSPhoneNumber**: US phone number validation. - **isNumber**: Checks
+if the value is a number. - **validateName**: Name validation. -
+**validateSurname**: Surname validation. - **validateTextarea**: Textarea
+validation. ### For better information, read the documentation Feel free to
+explore the various functions and experiment with different inputs to
 understand their behavior. If you encounter any issues or have suggestions,
 don't hesitate to reach out to me. Your feedback is valuable and helps improve
 the package. Happy coding! # By - Gabriel Logan
```

### Comparing `multiform-validator-0.0.6/src/multiform_validator.egg-info/SOURCES.txt` & `multiform_validator-0.0.7/src/multiform_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

