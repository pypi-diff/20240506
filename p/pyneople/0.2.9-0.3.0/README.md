# Comparing `tmp/pyneople-0.2.9.tar.gz` & `tmp/pyneople-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyneople-0.2.9.tar", last modified: Mon Apr 29 05:15:20 2024, max compression
+gzip compressed data, was "pyneople-0.3.0.tar", last modified: Mon May  6 14:02:07 2024, max compression
```

## Comparing `pyneople-0.2.9.tar` & `pyneople-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:15:20.708717 pyneople-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-29 05:15:09.000000 pyneople-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-29 05:15:20.708717 pyneople-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-29 05:15:09.000000 pyneople-0.2.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-29 05:15:09.000000 pyneople-0.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 05:15:20.708717 pyneople-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-29 05:15:09.000000 pyneople-0.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:15:20.704717 pyneople-0.2.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:15:20.708717 pyneople-0.2.9/src/pyneople/
--rw-r--r--   0 runner    (1001) docker     (127)     8293 2024-04-29 05:15:09.000000 pyneople-0.2.9/src/pyneople/METADATA.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-29 05:15:09.000000 pyneople-0.2.9/src/pyneople/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41952 2024-04-29 05:15:09.000000 pyneople-0.2.9/src/pyneople/character.py
--rw-r--r--   0 runner    (1001) docker     (127)    12353 2024-04-29 05:15:09.000000 pyneople-0.2.9/src/pyneople/database_connecter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7326 2024-04-29 05:15:09.000000 pyneople-0.2.9/src/pyneople/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 05:15:20.708717 pyneople-0.2.9/src/pyneople.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-29 05:15:20.000000 pyneople-0.2.9/src/pyneople.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-29 05:15:20.000000 pyneople-0.2.9/src/pyneople.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 05:15:20.000000 pyneople-0.2.9/src/pyneople.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-29 05:15:20.000000 pyneople-0.2.9/src/pyneople.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:02:07.537819 pyneople-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-06 14:01:55.000000 pyneople-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-06 14:02:07.537819 pyneople-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-06 14:01:55.000000 pyneople-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-06 14:01:55.000000 pyneople-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 14:02:07.537819 pyneople-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-06 14:01:55.000000 pyneople-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:02:07.533819 pyneople-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:02:07.533819 pyneople-0.3.0/src/pyneople/
+-rw-r--r--   0 runner    (1001) docker     (127)     8406 2024-05-06 14:01:55.000000 pyneople-0.3.0/src/pyneople/METADATA.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-06 14:01:55.000000 pyneople-0.3.0/src/pyneople/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39741 2024-05-06 14:01:55.000000 pyneople-0.3.0/src/pyneople/character.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22685 2024-05-06 14:01:55.000000 pyneople-0.3.0/src/pyneople/database_connecter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-05-06 14:01:55.000000 pyneople-0.3.0/src/pyneople/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:02:07.537819 pyneople-0.3.0/src/pyneople.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-06 14:02:07.000000 pyneople-0.3.0/src/pyneople.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-06 14:02:07.000000 pyneople-0.3.0/src/pyneople.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 14:02:07.000000 pyneople-0.3.0/src/pyneople.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 14:02:07.000000 pyneople-0.3.0/src/pyneople.egg-info/top_level.txt
```

### Comparing `pyneople-0.2.9/LICENSE` & `pyneople-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyneople-0.2.9/PKG-INFO` & `pyneople-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pyneople
-Version: 0.2.9
+Version: 0.3.0
 Summary: Neople Open API wrapper for data analyst
 Home-page: https://github.com/ippo252525/pyneople
 Author: ippo252525
 Author-email: ippo252525@gmail.com
 Project-URL: Bug Tracker, https://github.com/ippo252525/pyneople/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyneople
 Neople Open API wrapper for data analyst
 
 ## Getting Started
```

### Comparing `pyneople-0.2.9/setup.py` & `pyneople-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyneople",
-    version="0.2.9",
+    version="0.3.0",
     author="ippo252525",
     author_email="ippo252525@gmail.com",
     description="Neople Open API wrapper for data analyst",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ippo252525/pyneople",
     project_urls={
@@ -18,9 +18,9 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
-    python_requires=">=3.8",
+    python_requires=">=3.9",
 )
```

### Comparing `pyneople-0.2.9/src/pyneople/METADATA.py` & `pyneople-0.3.0/src/pyneople/METADATA.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,14 +172,21 @@
     'dark_element_damage': '암속성 피해',
     'bleed_damage': '출혈 피해',
     'poison_damage': '중독 피해',
     'burn_damage': '화상 피해',
     'electrocution_damage': '감전 피해'
  }
 
+GROWINFO_NAME = {
+        "level" : "level",
+        "exp_rate" : "expRate",
+        "option" : "options"
+}
+
+
 BASE_EQUIPMENT_NAME = {
     'item_name' :'itemName',
     'item_available_level' :'itemAvailableLevel',
     'item_rarity' :'itemRarity',
     'reinforce' :'reinforce',
     'amplification_name' :'amplificationName',
     'refine' :'refine', 
@@ -190,16 +197,16 @@
 EQUIPMENT_NAME = {
     'upgrade_info' : 'upgrade_info',
     'mist_gear' :  'mist_gear',
     'grow_info' : 'grow_info'
 }
 
 WEAPON_NAME = {
-    'bakal_info' : 'bakal_info',
-    'asrahan_info':'asrahan_info'
+    'bakal_info' : 'fusionOption',
+    'asrahan_info':'asrahanOption'
 }
 
 AVATAR_NAME = {
         'item_name' : "itemName",
         'item_rarity' : "itemRarity",
         'option_ability' : "optionAbility",
         'emblems' : 'emblems'
```

### Comparing `pyneople-0.2.9/src/pyneople/character.py` & `pyneople-0.3.0/src/pyneople/character.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import datetime
 import urllib.parse
 from typing import Iterable, Union
 from .functions import get_request, explain_enchant
 from .METADATA import SERVER_NAME_2_ID, CHARACTER_SEARCH_NAME, \
-                    CHARACTER_INFORMATION_NAME, STATUS_NAME, EQUIPMENT_LIST, AVATAR_LIST, PLATINUM_AVATAR_LIST, BASE_EQUIPMENT_NAME, EQUIPMENT_NAME, WEAPON_NAME, AVATAR_NAME, PLATINUM_AVATAR_NAME
+                    CHARACTER_INFORMATION_NAME, STATUS_NAME, EQUIPMENT_LIST, AVATAR_LIST, PLATINUM_AVATAR_LIST, \
+                    BASE_EQUIPMENT_NAME, EQUIPMENT_NAME, WEAPON_NAME, AVATAR_NAME, PLATINUM_AVATAR_NAME, GROWINFO_NAME
 
 __all__ = [
     "CharacterSearch",
     "CharacterInformation",
     "Timeline",
     "Status",
     "Equipments",
@@ -29,21 +30,36 @@
         """
         클래스 생성 시 Neople Open API key를 입력받는다
             Args :
                 arg_api_key(str) : Neople Open API key
         """        
         self._api_key = arg_api_key
 
-class CharacterSearch(PyNeople):
+class PyNeopleAttributeSetter(PyNeople):
     """
-    Neople Open API 02. 캐릭터 검색
+    하위 Attribute를 설정 할 수 있는 PyNeople Class 의 부모 Class
     """
 
-    def __init__(self, arg_api_key : str):
-        super().__init__(arg_api_key)
+    @classmethod
+    def set_sub_attributes(cls, arg_new_attribute_list : list[str]):
+        for new_attribute_name in arg_new_attribute_list:
+            if not new_attribute_name in cls.default_sub_attribute_list:
+                raise ValueError("사용할 수 없는 attribute 입니다.")
+        cls.sub_attribute_list = arg_new_attribute_list
+
+    @classmethod        
+    def init_sub_attributes(cls):
+        cls.sub_attribute_list = cls.default_sub_attribute_list
+
+class CharacterSearch(PyNeopleAttributeSetter):
+    """
+    Neople Open API 02. 캐릭터 검색
+    """
+    default_sub_attribute_list = CHARACTER_SEARCH_NAME.keys()
+    sub_attribute_list = default_sub_attribute_list
 
     def get_data(self, arg_server_name : str, arg_character_name : str):
         """
         서버 이름과 캐릭터 이름을 검색하면 기본 정보를 반환
             Args : 
                 arg_server_name(str) : 서버 이름  ex) 디레지에, diregie
                 
@@ -61,56 +77,44 @@
         url = f"https://api.neople.co.kr/df/servers/{arg_server_name}/characters?characterName={urllib.parse.quote(arg_character_name)}&limit=1&apikey={self._api_key}"
         
         # parse_data에 매개변수로 사용 될 것을 생각해서 dict를 받을 수 있도록 정보 다듬어서 제공
         try:
             return get_request(url).get("rows")[0]
         except IndexError:
             return dict()
-    sub_attribute_list = CHARACTER_SEARCH_NAME.keys()
-    
-    @classmethod
-    def set_sub_attributes(cls, new_attribute_list : list[str]):
-        cls.sub_attribute_list = new_attribute_list
 
     def parse_data(self, arg_data : dict):
         """
         데이터를 정리해서 하위 속성에 저장
             Args :
                 arg_data(dict) : Neople Open API 를 통해 받은 data
                 attribute_list(iterable of str) : 원하는 하위 속성 명
         """
         # 하위 속성에 데이터 할당
         for attribute_name in CharacterSearch.sub_attribute_list:            
             setattr(self, attribute_name, arg_data.get(CHARACTER_SEARCH_NAME[attribute_name]))
 
 
-class CharacterInformation(PyNeople):
+class CharacterInformation(PyNeopleAttributeSetter):
     """
     Neople Open API 03. 캐릭터 '기본정보' 조회
     """
-    def __init__(self, arg_api_key : str):
-        super().__init__(arg_api_key)
-    
+    default_sub_attribute_list = CHARACTER_INFORMATION_NAME.keys()
+    sub_attribute_list = default_sub_attribute_list
     def get_data(self, arg_server_id : str, arg_character_id : str):
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 기본 정보를 반환
             Args : 
                 arg_server_id(str) : 영문 서버 이름  ex) diregie
                 
                 arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
         """    
-        self._server_id = arg_server_id
+        self._total_id = f"{arg_server_id} {arg_character_id}"
         url = f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}?apikey={self._api_key}"
         return get_request(url)
-    
-    sub_attribute_list = CHARACTER_INFORMATION_NAME.keys()
-    
-    @classmethod
-    def set_sub_attributes(cls, new_attribute_list : list[str]):
-        cls.sub_attribute_list = new_attribute_list
 
     def parse_data(self, arg_data : dict):
 
         """
         데이터를 정리해서 하위 속성에 저장
             Args :
                 arg_data(dict) : Neople Open API 를 통해 받은 data
@@ -120,19 +124,15 @@
         for attribute_name in CharacterInformation.sub_attribute_list:
             setattr(self, attribute_name, arg_data.get(CHARACTER_INFORMATION_NAME[attribute_name]))
 
 
 class Timeline(PyNeople):
     """
     Neople Open API 04. 캐릭터 '타임라인 정보' 조회
-    """    
-
-    def __init__(self, arg_api_key : str):
-        super().__init__(arg_api_key)
-    
+    """  
     def get_data(self, 
                  arg_server_id : str, 
                  arg_character_id : str, 
                  arg_end_date : str, 
                  arg_last_end_date : str = "2017-09-21 00:00", 
                  arg_last_end_data : Union[dict, None] = None, 
                  arg_limit : int = 100, 
@@ -151,17 +151,17 @@
                 
                 arg_last_end_data(dict) : 지금까지 수집한 해당 캐릭터의 마지막 타임라인 데이터
                 
                 arg_limit(int) : 한번 request할 때 수집 할 타임라인 데이터의 개수
                 
                 arg_code(int) : 수집하고 싶은 타임라인 코드 ex)201, 202 참조) https://developers.neople.co.kr/contents/guide/pages/all 
                 
-                arg_print_log(boolean) : 데이터 수집의 과정의 print 여부   
+                arg_print_log(boolean) : 데이터 수집의 과정의 print 여부
         """
-        self._server_id = arg_server_id
+        self._total_id = f"{arg_server_id} {arg_character_id}"
         timeline = []
         
         end_date = datetime.datetime.strptime(arg_end_date, '%Y-%m-%d %H:%M')
         start_date = end_date - datetime.timedelta(days=90)
         if start_date < datetime.datetime.strptime(arg_last_end_date, '%Y-%m-%d %H:%M'):
             start_date = datetime.datetime.strptime(arg_last_end_date, '%Y-%m-%d %H:%M')
         next = ""
@@ -197,43 +197,35 @@
             else:
                 end_date = start_date
                 start_date = end_date - datetime.timedelta(days=90)
                 if start_date < datetime.datetime.strptime(arg_last_end_date, '%Y-%m-%d %H:%M'):
                     start_date = datetime.datetime.strptime(arg_last_end_date, '%Y-%m-%d %H:%M')
                 next = ""    
                 continue
-        return timeline
+        return {'timeline' : timeline} 
 
-class Status(PyNeople):
+class Status(PyNeopleAttributeSetter):
     """
     Neople Open API 05. 캐릭터 '능력치 정보' 조회
     """    
-
-    def __init__(self, arg_api_key : str):
-        super().__init__(arg_api_key)
-
+    default_sub_attribute_list = STATUS_NAME.keys()
+    sub_attribute_list = default_sub_attribute_list    
+    
     def get_data(self, arg_server_id : str, arg_character_id : str):
         """
         캐릭터의 모험단명부터 명성 등 정보를 반환한다
             Args:
                 arg_server_id(str) :  서버 ID
                 
                 arg_character_id(str) : 캐릭터 ID
         """
-        self._server_id = arg_server_id
+        self._total_id = f"{arg_server_id} {arg_character_id}"
         url = f'https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/status?apikey={self._api_key}'
         return get_request(url)
 
-    sub_attribute_list = STATUS_NAME.keys()
-    
-    @classmethod
-    def set_sub_attributes(cls, new_attribute_list : list[str]):
-        cls.sub_attribute_list = new_attribute_list
-
-
     def parse_data(self, arg_data : dict):
         """
         데이터를 정리해서 하위 attribute에 저장
             Args :
                 arg_data(dict) : Neople Open API 를 통해 받은 data
                 attribute_list(iterable of str) : 원하는 하위 속성 명
         """
@@ -253,95 +245,77 @@
         # 상세 스탯 정리
         if arg_data.get('status'):
             for item in arg_data['status']:
                 arg_data[item['name']] = item['value']   
         
         # 하위 속성에 데이터 할당
         for attribute_name in Status.sub_attribute_list:
-            setattr(self, attribute_name, arg_data.get(STATUS_NAME[attribute_name]))
+            setattr(self, attribute_name, arg_data.get(STATUS_NAME[attribute_name])) 
 
-class OptionInfo():
+class GrowInfo(PyNeopleAttributeSetter):
     """
     Equipments를 위해 사용되는 Class
     """
-
-    def __init__(self):
-        self.explain = None
+    default_sub_attribute_list = GROWINFO_NAME.keys()
+    sub_attribute_list = default_sub_attribute_list    
     
-    def get_option_info_data(self, arg_option_info_dict : dict):
-        self.explain = arg_option_info_dict.get('explain').replace("'", "") # 얼음 땡 옵션 예외처리를 위한 replace    
-
-class GrowInfo():
-    """
-    Equipments를 위해 사용되는 Class
-    """    
-
     def __init__(self):
-        self.level = None       # 장비 성장 레벨
-        self.exp_rate = None    # 장비 성장 경험치
-        self.transfer = None    # 전송 받은 옵션
-        self.option_1 = None    # 1옵션
-        self.option_2 = None    # 2옵션
-        self.option_3 = None    # 3옵션
-        self.option_4 = None    # 4옵션
+        for sub_attribute_name in GrowInfo.sub_attribute_list:
+            if sub_attribute_name == "option":
+                setattr(self, "transfer", None)
+                for i in range(1,5):
+                    setattr(self, f"{sub_attribute_name}_{i}", None)
+            else:
+                setattr(self, sub_attribute_name, None)
 
     def get_grow_info_data(self, arg_grow_info_dict : dict):
-        self.level = arg_grow_info_dict.get('level')
-        self.exp_rate = arg_grow_info_dict.get('expRate', 0)
-        if arg_grow_info_dict.get('options'):
-            for i, option in enumerate(arg_grow_info_dict.get('options')):
-                if option.get('transfer') == True:
-                    setattr(self, 'transfer', i+1)
-                else:
-                    pass    
-                setattr(self, f'option_{i+1}', option.get('explain')) 
+        for sub_attribute_name in GrowInfo.sub_attribute_list:
+            if sub_attribute_name == "option":
+                if arg_grow_info_dict.get(GROWINFO_NAME[sub_attribute_name]):
+                    for i, option in enumerate(arg_grow_info_dict.get(GROWINFO_NAME[sub_attribute_name])):
+                        setattr(self, f'option_{i+1}', option.get('explain'))                            
+                        if option.get('transfer'):
+                            setattr(self, 'transfer', i+1)
+            else:   
+                setattr(self, sub_attribute_name, arg_grow_info_dict.get(GROWINFO_NAME[sub_attribute_name])) 
 
-class BaseEquipment():
+class BaseEquipment(PyNeopleAttributeSetter):
     """
     Equipments를 위해 사용되는 Class
     가장 기초적인 장비 정보를 담으며 다른 장비에 부모클래스로 이용된다.
     """    
-    sub_attribute_list = BASE_EQUIPMENT_NAME.keys()
+    default_sub_attribute_list = BASE_EQUIPMENT_NAME.keys()
+    sub_attribute_list = default_sub_attribute_list
+    
     def __init__(self):
         for sub_attribute in BaseEquipment.sub_attribute_list:
             setattr(self, sub_attribute, None)
-    
-    @classmethod
-    def set_sub_attributes(cls, new_attribute_list : list[str]):
-        for new_attribute in new_attribute_list:
-            assert new_attribute in cls.sub_attribute_list
-        cls.sub_attribute_list = new_attribute_list
 
     def get_equipment_data(self, arg_equipment_dict : dict):
         
         for sub_attribute in BaseEquipment.sub_attribute_list:
             if sub_attribute == 'enchant':
                 setattr(self, sub_attribute, explain_enchant(arg_equipment_dict.get('enchant')))
-                pass
             else:    
                 setattr(self, sub_attribute, arg_equipment_dict.get(BASE_EQUIPMENT_NAME[sub_attribute]))
 
 class Equipment(BaseEquipment):
     """
     Equipments를 위해 사용되는 Class
-    """
-    sub_attribute_list = EQUIPMENT_NAME.keys()
+    """ 
+    default_sub_attribute_list = EQUIPMENT_NAME.keys()
+    sub_attribute_list = default_sub_attribute_list
     def __init__(self):
         super().__init__()
-        print(Equipment.sub_attribute_list)
         for sub_attribute in Equipment.sub_attribute_list:
             if sub_attribute == 'grow_info':
                 setattr(self, sub_attribute, GrowInfo())
             else:
                 setattr(self, sub_attribute, None)
 
-    # @classmethod
-    # def set_sub_attributes(cls, new_attribute_list : list[str]):
-    #     cls.sub_attribute_list = new_attribute_list
-
     def get_equipment_data(self, arg_equipment_dict):
         super().get_equipment_data(arg_equipment_dict)
         
         for sub_attribute in Equipment.sub_attribute_list:
             if sub_attribute == 'upgrade_info':
                 setattr(self, sub_attribute, arg_equipment_dict.get("upgradeInfo", dict()).get('itemName'))
             elif sub_attribute == 'mist_gear':
@@ -358,135 +332,89 @@
                     getattr(self, sub_attribute).get_grow_info_data(arg_equipment_dict.get('customOption'))
                 elif arg_equipment_dict.get("fixedOption"):
                     getattr(self, sub_attribute).get_grow_info_data(arg_equipment_dict.get("fixedOption"))
                 else :
                     pass
             else:
                 pass    
-    # def __init__(self):
-    #     self.item_name = None
-    #     self.item_available_level = None
-    #     self.item_rarity = None
-    #     self.reinforce = None
-    #     self.item_grade_name = None
-    #     self.enchant = None
-    #     self.amplification_name = None
-    #     self.refine = None
-    #     self.upgrade_info = None
-    #     self.mist_gear = None
-    #     self.grow_info = GrowInfo()
-    
-    # def get_equipment_data(self, arg_equipment_dict : dict):
-    #     self.item_name = arg_equipment_dict.get('itemName') # 이름
-    #     self.item_available_level = arg_equipment_dict.get('itemAvailableLevel') # 레벨 제한
-    #     self.item_rarity = arg_equipment_dict.get('itemRarity') # 레어도
-    #     self.reinforce = arg_equipment_dict.get('reinforce') # 강화수치             
-    #     self.amplification_name = arg_equipment_dict.get('amplificationName') # 차원의 기운 여부 ex 차원의 힘, 차원의 지능, None
-    #     self.refine = arg_equipment_dict.get('refine') # 제련   
-    #     self.item_grade_name = arg_equipment_dict.get('itemGradeName') # 등급(최상~최하)
-    #     self.enchant = explain_enchant(arg_equipment_dict.get('enchant')) # 마법부여
-
-    #     # 미스트 기어 정보
-    #     if arg_equipment_dict.get('mistGear'):
-    #         self.mist_gear = 'mist_gear'
-    #     elif arg_equipment_dict.get('pureMistGear'):
-    #         self.mist_gear = 'pure_mist_gear'   
-    #     elif arg_equipment_dict.get('refinedMistGear'):
-    #         self.mist_gear = 'refined_mistgear'                   
-    #     else :
-    #         pass    
-
-
-    #     if arg_equipment_dict.get("upgradeInfo"):
-    #         self.upgrade_info = arg_equipment_dict.get("upgradeInfo").get('itemName') # 융합장비
-        
-    #     # 105제 성장 장비 정보
-    #     if arg_equipment_dict.get("customOption"):
-    #         self.grow_info.get_grow_info_data(arg_equipment_dict.get('customOption'))
-    #     elif arg_equipment_dict.get("fixedOption"):
-    #         self.grow_info.get_grow_info_data(arg_equipment_dict.get("fixedOption"))
-    #     else :
-    #         pass
+    
 
 class BakalInfo():
     """
     Equipments를 위해 사용되는 Class
     """
 
     def __init__(self):
         self.option_1 = None
         self.option_2 = None
         self.option_3 = None
 
-    def get_bakal_info_data(self, arg_bakal_info_dict):
+    def get_info_data(self, arg_bakal_info_dict):
         if arg_bakal_info_dict.get('options'):
             for i, option in enumerate(arg_bakal_info_dict.get('options')):
                 setattr(self, f'option_{i+1}',option.get('explain'))                
 
 class Asrahan_Info():
     """
     Equipments를 위해 사용되는 Class
     """
     def __init__(self):
         self.memory_cluster = None
         self.memory_destination = None
 
-    def get_asrahan_info_data(self, arg_asrahan_info_dict):
-        for asrahan_info in arg_asrahan_info_dict.get('options'):
+    def get_info_data(self, arg_asrahan_info_dict):
+        for asrahan_info in arg_asrahan_info_dict.get('options', list()):
             if asrahan_info.get('name') == '기억의 종착지':
-                self.memory_destination = asrahan_info.get('step')     
+                self.memory_destination = asrahan_info.get('step')
             else:
-                self.memory_cluster = asrahan_info.get('step')     
+                self.memory_cluster = asrahan_info.get('step')
 
 class Weapon(Equipment):
     """
     Equipments를 위해 사용되는 Class
     """
-    sub_attribute_list = WEAPON_NAME.keys()
+    default_sub_attribute_list = WEAPON_NAME.keys()
+    sub_attribute_list = default_sub_attribute_list
     def __init__(self):
         super().__init__()
         for sub_attribute in Weapon.sub_attribute_list:
             if sub_attribute == 'bakal_info':
                 self.bakal_info = BakalInfo()
             elif sub_attribute == 'asrahan_info':
                 self.asrahan_info = Asrahan_Info()
             else:
                 pass    
 
     def get_equipment_data(self, arg_equipment_dict):
         super().get_equipment_data(arg_equipment_dict)
         for sub_attribute in Weapon.sub_attribute_list:
-            if sub_attribute == 'bakal_info':
-                self.bakal_info.get_bakal_info_data(arg_equipment_dict.get("bakalInfo", dict())) # 바칼 무기 융합
-            elif sub_attribute == 'asrahan_info':
-                self.asrahan_info.get_asrahan_info_data(arg_equipment_dict.get("asrahanOption", dict()))
-            else:
-                pass    
+            getattr(self, sub_attribute).get_info_data(arg_equipment_dict.get(WEAPON_NAME[sub_attribute], dict()))
+            # if sub_attribute == 'bakal_info':
+            #     self.bakal_info.get_bakal_info_data(arg_equipment_dict.get(WEAPON_NAME[sub_attribute], dict())) # 바칼 무기 융합
+            # elif sub_attribute == 'asrahan_info':
+            #     self.asrahan_info.get_asrahan_info_data(arg_equipment_dict.get("asrahanOption", dict()))
+            # else:
+            #     pass    
 
-class Equipments(PyNeople):
+class Equipments(PyNeopleAttributeSetter):
     """
     Neople Open API 06. 캐릭터 '장착 장비' 조회
     """    
-    sub_attribute_list = EQUIPMENT_LIST
-    def __init__(self, arg_api_key : str):
-        super().__init__(arg_api_key)
-    
-    @classmethod
-    def set_sub_attributes(cls, new_attribute_list : list[str]):
-        cls.sub_attribute_list = new_attribute_list
+    default_sub_attribute_list = EQUIPMENT_LIST
+    sub_attribute_list = default_sub_attribute_list
     
     def get_data(self, arg_server_id : str, arg_character_id : str):
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 장착 장비 정보를 반환
             Args : 
                 arg_server_id(str) : 영문 서버 이름  ex) diregie
                 
                 arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
         """        
-        self._server_id = arg_server_id
+        self._total_id = f"{arg_server_id} {arg_character_id}"
         url = f'https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/equipment?apikey={self._api_key}'
         return get_request(url)
     
     def parse_data(self, arg_data : dict):
         """
         데이터를 정리해서 하위 attribute에 저장
             Args :
@@ -519,39 +447,34 @@
                         set_item_info_list.append(" ".join(set_item_name_list))
                     setattr(self, 'set_item_info', ", ".join(set_item_info_list))
                 else:
                     pass
             else:
                 pass        
 
-class Avatar():
+class Avatar(PyNeopleAttributeSetter):
     """
     Avatars를 위해 사용되는 Class
     """
-    sub_attribute_list = AVATAR_NAME.keys()
+    default_sub_attribute_list = AVATAR_NAME.keys()
+    sub_attribute_list = default_sub_attribute_list
     
     def __init__(self):
         for sub_attribute in Avatar.sub_attribute_list:
             if sub_attribute == "emblems":
                 for i in range(1,3):
                     setattr(self, f"{sub_attribute}_{i}", None)
             else:
                 setattr(self, sub_attribute, None)
 
         # self.item_name = None       # 아바타 이름
         # self.item_rarity = None     # 아바타 레어도
         # self.option_ability = None  # 아바타 옵션
         # self.emblem_1 = None        # 엠블렘1 옵션
         # self.emblem_2 = None        # 엠블렘2 옵션
-    @classmethod
-    def set_sub_attributes(cls, new_attribute_list : list[str]):
-        for new_attribute in new_attribute_list:
-            if not new_attribute in cls.sub_attribute_list:
-                raise ValueError("사용할 수 없는 하위 속성입니다.")         
-        cls.sub_attribute_list = new_attribute_list
 
     def get_avatar_data(self, arg_avatar_dict):
         for sub_attribute in Avatar.sub_attribute_list:
             if sub_attribute == 'emblems':
                 for emblem in arg_avatar_dict.get('emblems', dict()):
                     setattr(self, f"{sub_attribute}_{emblem.get('slotNo')}", emblem.get('itemName'))
             else:    
@@ -592,19 +515,20 @@
             elif sub_attribute == "platinum_emblem":
                 for emblem in arg_avatar_dict.get(PLATINUM_AVATAR_NAME[sub_attribute], dict()):
                     if emblem.get('slotColor') == '플래티넘':
                         setattr(self, sub_attribute, emblem.get('itemName'))
             else:    
                 setattr(self, sub_attribute, arg_avatar_dict.get(AVATAR_NAME[sub_attribute]))
 
-class Avatars(PyNeople):
+class Avatars(PyNeopleAttributeSetter):
     """
     Neople Open API 07. 캐릭터 '장착 아바타' 조회
     """       
-    sub_attribute_list = AVATAR_LIST
+    default_sub_attribute_list = AVATAR_LIST
+    sub_attribute_list = default_sub_attribute_list
     def __init__(self, arg_api_key: str):
         super().__init__(arg_api_key)
     
     @classmethod
     def set_sub_attributes(cls, new_attribute_list : list[str]):
         cls.sub_attribute_list = new_attribute_list
 
@@ -612,15 +536,15 @@
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 장착 아바타 정보를 반환
             Args : 
                 arg_server_id(str) : 영문 서버 이름  ex) diregie
                 
                 arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
         """        
-        self._server_id = arg_server_id
+        self._total_id = f"{arg_server_id} {arg_character_id}"
         url = f'https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/avatar?apikey={self._api_key}'
         return get_request(url)
 
     def parse_data(self, arg_data : dict):
         """
         데이터를 정리해서 하위 attribute에 저장
             Args :
@@ -651,15 +575,15 @@
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 장착 크리쳐 정보를 반환
             Args : 
                 arg_server_id(str) : 영문 서버 이름  ex) diregie
                 
                 arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
         """
-        self._server_id = arg_server_id
+        self._total_id = f"{arg_server_id} {arg_character_id}"
         url = f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/creature?apikey={self._api_key}"
         return get_request(url)
     
     def parse_data(self, arg_data : dict):
         """
         데이터를 정리해서 하위 attribute에 저장
             Args :
@@ -679,15 +603,15 @@
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 장착 휘장 정보를 반환
             Args : 
                 arg_server_id(str) : 영문 서버 이름  ex) diregie
                 
                 arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
         """        
-        self._server_id = arg_server_id
+        self._total_id = f"{arg_server_id} {arg_character_id}"
         url = f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/flag?apikey={self._api_key}"
         return get_request(url)
     
     def parse_data(self, arg_data):
         """
         데이터를 정리해서 하위 attribute에 저장
             Args :
@@ -728,15 +652,15 @@
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 장착 탈리스만 정보를 반환
             Args : 
                 arg_server_id(str) : 영문 서버 이름  ex) diregie
                 
                 arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
         """                
-        self._server_id = arg_server_id
+        self._total_id = f"{arg_server_id} {arg_character_id}"
         url = f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/talisman?apikey={self._api_key}"         
         return get_request(url)
     
     def parse_data(self, arg_data : dict):
         """
         데이터를 정리해서 하위 attribute에 저장
             Args :
@@ -759,15 +683,15 @@
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 장비 특성 정보를 반환
             Args : 
                 arg_server_id(str) : 영문 서버 이름  ex) diregie
                 
                 arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
         """                
-        self._server_id = arg_server_id
+        self._total_id = f"{arg_server_id} {arg_character_id}"
         url = f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/equip/equipment-trait?apikey={self._api_key}"
         return get_request(url)
     
     def parse_data(self, arg_data : dict):
         """
         데이터를 정리해서 하위 attribute에 저장
         강력한 일격과 명상의 레벨만 확인
@@ -800,15 +724,15 @@
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 스킬 스타일 정보를 반환
             Args : 
                 arg_server_id(str) : 영문 서버 이름  ex) diregie
                 
                 arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
         """                
-        self._server_id = arg_server_id
+        self._total_id = f"{arg_server_id} {arg_character_id}"
         url = f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/skill/style?apikey={self._api_key}"
         return get_request(url)
 
     def parse_data(self, arg_data : dict):
         """
         데이터를 정리해서 하위 attribute에 저장
         스킬 코드만 구현 완료 나머지 추후 개발
@@ -862,15 +786,15 @@
         """
         영문 서버 이름과 캐릭터 ID 를 검색하면 버프 강화(장비, 아바타, 크리쳐) 정보를 반환
             Args : 
                 arg_server_id(str) : 영문 서버 이름  ex) diregie
                 
                 arg_character_name(str) : 캐릭터 ID ex) 80d9189c86147ab9a7b8c1481be85d95
         """   
-        self._server_id = arg_server_id
+        self._total_id = f"{arg_server_id} {arg_character_id}"
         buff_info_dict = {}     
         buff_equipment_data = get_request(f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/skill/buff/equip/equipment?apikey={self._api_key}")
         buff_avatar_data = get_request(f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/skill/buff/equip/avatar?apikey={self._api_key}")
         buff_creature_data = get_request(f"https://api.neople.co.kr/df/servers/{arg_server_id}/characters/{arg_character_id}/skill/buff/equip/creature?apikey={self._api_key}")
         buff_info_dict["equipment"] = buff_equipment_data
         buff_info_dict["avatar"] = buff_avatar_data
         buff_info_dict["creature"] = buff_creature_data
```

### Comparing `pyneople-0.2.9/src/pyneople/functions.py` & `pyneople-0.3.0/src/pyneople/functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 import time
 import json
 import requests
 from .METADATA import JOBCLASS
 from .METADATA import SETTINGS
 
-__all__ = ['change_settings', 'get_request', 'jobname_equalize', 'get_job_info', 'system_maintenance']
+__all__ = ['change_settings', 'get_request', 'jobname_equalize', 'get_job_info', 'system_maintenance', 'NeopleOpenAPIError', 'ServerMaintenanceError', 'value_flatten', 'attr_flatten']
 
-class PyneopleError(Exception):
+class NeopleOpenAPIError(Exception):
+    """
+    Error 핸들링을 위한 Class
+    """
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
 class ServerMaintenanceError(Exception):
+    """
+    Error 핸들링을 위한 Class
+    """    
     def __init__(self, *args: object) -> None:
         super().__init__(*args)
 
 def change_settings(arg_time_out : int = 5, arg_time_sleep : float = 0.0015):
     """
     request에 필요한 설정 값을 바꾸는 함수
 
@@ -38,15 +44,15 @@
     data = requests.get(arg_url, timeout = SETTINGS['request_time_out'])
     data = json.loads(data.text)
     # Neople Open API 상에서 규정된 에러가 발생할 경우 에러를 발생시킨다.
     if data.get("error"):
         if data.get("error").get('status') == 503:
             raise ServerMaintenanceError
         else:
-            raise PyneopleError(data.get("error"))
+            raise NeopleOpenAPIError(data.get("error"))
     elapsed_time = time.time() - start_time
     if elapsed_time < SETTINGS['request_time_sleep']:
         time.sleep(SETTINGS['request_time_sleep'] - elapsed_time)
     return data
 
 def _next(arg_dict : dict, arg_list : list):
     """
@@ -62,14 +68,16 @@
 
 def get_job_info(arg_api_key : str):
     """
     직업 정보를 받아오는 함수
     전직명(각성명)을 1차 전직명으로 통일시키는 jobname_equalize 함수에 매개변수로 사용되는 객체를 반환함
         Args :
             arg_api_key(str) : Neople Open API key
+        Retruns :
+            jobname_equalize 함수에 매개변수로 사용되는 객체
     """
     data = get_request(f"https://api.neople.co.kr/df/jobs?apikey={arg_api_key}")
     job_list = []
     jobGroW_total_list = []
     for job in data['rows']:
         job_list.append(job['jobName'])
         jobGroW_list = []
@@ -135,84 +143,67 @@
         output = ", ".join([f"{s['name']} {s['value']}" for s in arg_enchant_dict['status']])
     if "reinforceSkill" in arg_enchant_dict.keys():
         output = ", ".join([f"{s['name']} {s['value']}" for r in arg_enchant_dict['reinforceSkill'] for s in r['skills']]) + ", " + output 
     if "explain" in arg_enchant_dict.keys():
         output = arg_enchant_dict['explain'] + ", " + output
     return output
 
-def is_attr(arg_object):
+def _is_attr(arg_object):
     """
     하위 속성이 있는지 확인하는 함수
     """
     try:
         arg_object.__dict__.keys()
         return True
     except:
         return False
 
-def get_attr(arg_object, te = ""):
+def _get_attr(arg_object, te = ""):
     """
     객체의 하위 속성명을 list로 만들어주는 함수
     """
     st = []
     for sub in list(arg_object.__dict__.keys()):
-        if is_attr(getattr(arg_object, sub)) == False:
+        if _is_attr(getattr(arg_object, sub)) == False:
             if sub[0] != "_":
                 st.append(te + sub)
         else :     
-            st.append(get_attr(getattr(arg_object, sub), te + sub + "."))    
+            st.append(_get_attr(getattr(arg_object, sub), te + sub + "."))    
     return st    
 
-def get_values(arg_object):
+def _get_values(arg_object):
     """
     객체의 하위 속성값을 list로 만들어주는 함수
     """
     st = []
     for sub in list(arg_object.__dict__.keys()):
-        if is_attr(getattr(arg_object, sub)) == False:
+        if _is_attr(getattr(arg_object, sub)) == False:
             if sub[0] != "_":
                 st.append(getattr(arg_object, sub))
         else:
-            st.append(get_values(getattr(arg_object, sub)))    
+            st.append(_get_values(getattr(arg_object, sub)))    
     return st    
 
-def flatten(arg_list):
+def _flatten(arg_list):
     result = []
     for item in arg_list:
         if isinstance(item, list):
-            result += flatten(item)
+            result += _flatten(item)
         else:
             result.append(item)
     return result
 
 def attr_flatten(arg_object):
     """
     객체를 입력받으면 모든 하위속성의 이름을 문자열 list로 반환한다
     """
-    arg_object = get_attr(arg_object)
-    arg_object = flatten(arg_object)
+    arg_object = _get_attr(arg_object)
+    arg_object = _flatten(arg_object)
     return arg_object
 
 def value_flatten(arg_object):
     """
     객체를 입력받으면 모든 하위속성의 값을 list로 반환한다
     """
-    arg_object = get_values(arg_object)
-    arg_object = flatten(arg_object)
-    return arg_object
-
-# def one_slot(arg_equipment_list : list, arg_slot_name : str):
-#     """
-#     해당 부위의 정보만 반환하는 함수
-#         Args:
-#             arg_equipment_list(list) : 캐릭터 장비 데이터(dict)로 이루어진 list
-            
-#             arg_slot_name(str) : 해당 장비의 이름
-#         Returns:
-#             해당 장비의 dict            
-#     """
-#     if arg_equipment_list == []:
-#         return None
-#     for equipment in arg_equipment_list:
-#         if equipment['slotId'] == arg_slot_name :
-#             return equipment
-#     return None
+    arg_object = _get_values(arg_object)
+    arg_object = _flatten(arg_object)
+    return arg_object
```

### Comparing `pyneople-0.2.9/src/pyneople.egg-info/PKG-INFO` & `pyneople-0.3.0/src/pyneople.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pyneople
-Version: 0.2.9
+Version: 0.3.0
 Summary: Neople Open API wrapper for data analyst
 Home-page: https://github.com/ippo252525/pyneople
 Author: ippo252525
 Author-email: ippo252525@gmail.com
 Project-URL: Bug Tracker, https://github.com/ippo252525/pyneople/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyneople
 Neople Open API wrapper for data analyst
 
 ## Getting Started
```

