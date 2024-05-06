# Comparing `tmp/erp_apis-1.0.1-py3-none-any.whl.zip` & `tmp/erp_apis-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 7616 bytes, number of entries: 12
--rw-rw-rw-  2.0 fat      315 b- defN 24-Apr-29 03:02 erp_apis/config.py
--rw-rw-rw-  2.0 fat     2902 b- defN 24-Apr-30 05:55 erp_apis/request.py
--rw-rw-rw-  2.0 fat     1097 b- defN 24-Apr-30 05:51 erp_apis/util.py
+Zip file size: 8666 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat      403 b- defN 24-May-06 06:32 erp_apis/config.py
+-rw-rw-rw-  2.0 fat     3486 b- defN 24-May-06 05:56 erp_apis/request.py
 -rw-rw-rw-  2.0 fat      141 b- defN 24-Apr-29 06:37 erp_apis/apis/__init__.py
--rw-rw-rw-  2.0 fat     1000 b- defN 24-Apr-30 05:51 erp_apis/apis/inventory.py
--rw-rw-rw-  2.0 fat     4032 b- defN 24-Apr-30 08:44 erp_apis/apis/order.py
--rw-rw-rw-  2.0 fat      380 b- defN 24-Apr-30 05:55 erp_apis/apis/test.py
--rw-rw-rw-  2.0 fat      749 b- defN 24-Apr-29 08:31 erp_apis/apis/user.py
--rw-rw-rw-  2.0 fat     1580 b- defN 24-Apr-30 08:48 erp_apis-1.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-30 08:48 erp_apis-1.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 24-Apr-30 08:48 erp_apis-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      922 b- defN 24-Apr-30 08:48 erp_apis-1.0.1.dist-info/RECORD
-12 files, 13233 bytes uncompressed, 6082 bytes compressed:  54.0%
+-rw-rw-rw-  2.0 fat     2550 b- defN 24-May-06 06:31 erp_apis/apis/afterSales.py
+-rw-rw-rw-  2.0 fat     1010 b- defN 24-Apr-30 10:14 erp_apis/apis/inventory.py
+-rw-rw-rw-  2.0 fat     3680 b- defN 24-May-05 08:01 erp_apis/apis/order.py
+-rw-rw-rw-  2.0 fat     1817 b- defN 24-May-06 06:32 erp_apis/apis/test.py
+-rw-rw-rw-  2.0 fat      777 b- defN 24-Apr-30 11:33 erp_apis/apis/user.py
+-rw-rw-rw-  2.0 fat     1580 b- defN 24-May-06 06:33 erp_apis-1.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-06 06:33 erp_apis-1.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       23 b- defN 24-May-06 06:33 erp_apis-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      934 b- defN 24-May-06 06:33 erp_apis-1.0.2.dist-info/RECORD
+12 files, 16493 bytes uncompressed, 7110 bytes compressed:  56.9%
```

## zipnote {}

```diff
@@ -1,37 +1,37 @@
 Filename: erp_apis/config.py
 Comment: 
 
 Filename: erp_apis/request.py
 Comment: 
 
-Filename: erp_apis/util.py
+Filename: erp_apis/apis/__init__.py
 Comment: 
 
-Filename: erp_apis/apis/__init__.py
+Filename: erp_apis/apis/afterSales.py
 Comment: 
 
 Filename: erp_apis/apis/inventory.py
 Comment: 
 
 Filename: erp_apis/apis/order.py
 Comment: 
 
 Filename: erp_apis/apis/test.py
 Comment: 
 
 Filename: erp_apis/apis/user.py
 Comment: 
 
-Filename: erp_apis-1.0.1.dist-info/METADATA
+Filename: erp_apis-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: erp_apis-1.0.1.dist-info/WHEEL
+Filename: erp_apis-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: erp_apis-1.0.1.dist-info/top_level.txt
+Filename: erp_apis-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: erp_apis-1.0.1.dist-info/RECORD
+Filename: erp_apis-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## erp_apis/config.py

```diff
@@ -1,11 +1,15 @@
 # coding: utf-8
 # Project：erp_out_of_stock
 # File：config.py
 # Author：李福成
 # Date ：2024-04-29 10:04
 # IDE：PyCharm
 
+Erp321BaseUrl = 'https://www.erp321.com'
+ErpApiBaseUrl = 'https://api.erp321.com'
+
+
 
 DEFAULT_HEADERS = {
     'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/237.84.2.178 Safari/537.36 Edg/109.0.1518.78',
 }
```

## erp_apis/request.py

```diff
@@ -1,20 +1,22 @@
 # coding: utf-8
 # Project：invoices
 # File：request.py
 # Author：李福成
 # Date ：2024-04-09 11:20
 # IDE：PyCharm
+import os
 from dataclasses import dataclass
 from typing import Optional
+from urllib.parse import urljoin
 
 from lxml import etree
 from requests import Session as S, Request as R
 import time, json as j
-from config import DEFAULT_HEADERS
+from config import DEFAULT_HEADERS, Erp321BaseUrl, ErpApiBaseUrl
 
 
 @dataclass
 class UserInfoType:
     u_cid: Optional[str]
     u_co_id: Optional[str]
     u_co_name: Optional[str]
@@ -30,35 +32,46 @@
         super().__init__()
         self.headers.update(DEFAULT_HEADERS)
         self.proxies = {'http': "", 'https': ""}
         self.viewstateItems = dict()
         self.userInfo : Optional[UserInfoType]
 
 
-    def erpSend(self, request,  **kwargs):
+
+    def erpSend(self, request:R, **kwargs):
         if not request.headers: request.headers = self.headers
+        hostType = getattr(request, 'hostType', None)
+        if hostType:
+            resp = getattr(self, hostType + "Send", None)(request, **kwargs)
+            if resp is None:
+                raise Exception(f"{hostType}没有这个域的send方法")
+            return resp
+        raise Exception('hostType is None')
+
+
+    def erp321Send(self, request, **kwargs):
+        request.url = urljoin(Erp321BaseUrl, request.url)
         if request.method == 'POST':
-            self.post_format(request, **kwargs)
+            request.headers.update({'Content-Type': 'application/x-www-form-urlencoded; charset=UTF-8'})
+            request.data.update({k: v for k, v in self.get_viewstate(request.url).items() if k and k != "updateTime"})
+        res = super().send(self.prepare_request(request), **kwargs)
+        if request.callback:
+            return request.callback(res)
+        return res
+
+    def erpApiSend(self, request, **kwargs):
+        request.url = urljoin(ErpApiBaseUrl, request.url)
         res = super().send(self.prepare_request(request), **kwargs)
         if request.callback:
             if request.callback == 'login':
                 self.userInfo = UserInfoType(**res.json().get('cookie'))
             else:
                 return request.callback(res)
         return res
 
-
-    def post_format(self, request, **kwargs):
-        if getattr(request, 'data', None):
-            request.headers.update({'Content-Type': 'application/x-www-form-urlencoded; charset=UTF-8'})
-            request.data.update({k: v for k, v in self.get_viewstate(request.url).items() if k and k != "updateTime"})
-        elif getattr(request, 'json', None):
-            request.headers.update({'Content-Type': 'application/json; charset=UTF-8'})
-
-
     def get_viewstate(self, url):
         if self.viewstateItems.get(url) and self.viewstateItems.get(url).get("updateTime") > time.time() - 60 * 5:
             return self.viewstateItems.get(url)
         if not self.viewstateItems.get(url):
             self.viewstateItems.update({url: {"updateTime": time.time()}})
         res = self.get(url)
         etree_xpath = etree.HTML(res.text)
@@ -67,21 +80,23 @@
             r = etree_xpath.xpath(xpath)
             return r[0] if r else None
 
         self.viewstateItems.get(url).update(
             {
                 "__VIEWSTATE": extract_first("//*[@id='__VIEWSTATE']/@value"),
                 "__VIEWSTATEGENERATOR": extract_first("//*[@id='__VIEWSTATEGENERATOR']/@value"),
-                "__EVENTVALIDATION": extract_first("//*[@id='__EVENTVALIDATION']/@value")
+                "__EVENTVALIDATION": extract_first("//*[@id='__EVENTVALIDATION']/@value"),
             }
         )
         return self.viewstateItems.get(url)
 
 
 class Request(R):
 
     def __init__(self,
+                 hostType: str = 'erp321',
                  callback: callable=None,
                  **kwargs
         ):
+        self.hostType = hostType
         self.callback = callback
         super().__init__(**kwargs)
```

## erp_apis/apis/inventory.py

```diff
@@ -3,26 +3,28 @@
 # File：inventory.py
 # Author：李福成
 # Date ：2024-04-28 18:27
 # IDE：PyCharm
 # 库存
 from typing import Optional
 from request import Request
-from util import getDefaultParams, dumps, JTable1
+from utils.util import getDefaultParams, dumps, JTable1
 
 
 # 查询库存
 def WmsSkuStock(queryData: Optional[list] = None, page_num: int = 1, page_size: int = 500):
     '''
     查询库存(分仓)
     :param page_num:  页数
     :param page_size:  每页条数
     :param queryData:  查询条件
     :return: 查询结果
     '''
+
+
     return Request(
         method='POST',
         url='https://www.erp321.com/app/item/SkuStock/WmsSkuStock.aspx',
         params=getDefaultParams({'defaultParams': ["ts___", "_c",'am___']}),
         data={
             '_jt_page_size': page_size,
             '__CALLBACKID': 'JTable1',
```

## erp_apis/apis/order.py

```diff
@@ -3,29 +3,25 @@
 # File：order.py
 # Author：李福成
 # Date ：2024-04-28 18:23
 # IDE：PyCharm
 # 订单API
 from typing import Optional, Union
 from request import Request
-from util import dumps, getDefaultParams, JTable1
-
-url = 'https://www.erp321.com/app/order/order/list.aspx'
-
-
-def OrderRequest(data: dict, url: str = url, method: str = 'LoadDataToJSON') -> Request:
+from utils.util import dumps, getDefaultParams, JTable1, generateChangeBatchItems
+def OrderRequest(data: dict, method: str = 'LoadDataToJSON') -> Request:
     return Request(
         method='POST',
-        url=url,
+        url='/app/order/order/list.aspx',
         params=getDefaultParams({'defaultParams': ["ts___", "_c"], 'am___': method}),
         data={
             '__CALLBACKID': 'JTable1',
             **data
         },
-        callback = JTable1
+        callback=JTable1
     )
 
 
 # 获取订单
 def OrderList(queryData: Optional[list] = None, page_num: int = 1, page_size: int = 500):
     '''
     获取订单
@@ -43,15 +39,15 @@
                 "Args": [
                     page_num,
                     dumps(queryData),
                     "{}"
                 ]
             }
         ),
-    },method='LoadDataToJSON')
+    }, method='LoadDataToJSON')
 
 
 # 修改订单异常类型
 def Questions(questionName: str, questionMsg: str, oid: Union[str, int]):
     '''
     修改订单异常类型
     :param questionName: 异常分类名称
@@ -60,49 +56,66 @@
     :return: 执行结果
     '''
     return OrderRequest({
         '__CALLBACKPARAM': dumps(
             {"Method": "Questions", "Args": [questionName, questionMsg, str(oid)], "CallControl": "{page}"}
         ),
     },
-    method='Questions')
+        method='Questions')
+
+
+# 转正常
+def UnQuestions(oid: Union[str, int]):
+    '''
+    修改订单异常类型
+    :param questionName: 异常分类名称
+    :param questionMsg:  异常信息
+    :param oid:  内部订单号
+    :return: 执行结果
+    '''
+    return OrderRequest({
+        '__CALLBACKPARAM': dumps(
+            {"Method": "UnQuestions", "Args": [str(oid)], "CallControl": "{page}"}
+        ),
+    },
+        method='UnQuestions')
 
 
 # 修改备注
 def Remarks(oid: Union[str, int], remarksMsg: str = '', isAppendRemarks: bool = True, flag: str = None):
     '''
     修改备注
     :param oid:  内部订单号
     :param remarksMsg:  备注信息
     :param isAppendRemarks:  是否追加备注
     :param flag:  旗帜类型： 1:红  2:黄  3:绿  4:蓝   5:紫
     :return: 执行结果
     '''
     return OrderRequest({
-        '__CALLBACKID': 'JTable1',
         '__CALLBACKPARAM': dumps({
             "Method": "SaveAppendRemarks",
             "Args": [
                 'null' if flag is None else str(flag),
                 remarksMsg,
                 str(oid),
-                'true' if isAppendRemarks else 'false'
+                'True' if isAppendRemarks else 'False'
             ],
             "CallControl": "{page}"
         }),
     },
-    method='SaveAppendRemarks')
+        method='SaveAppendRemarks')
 
 
 # 换商品
-def ChangeBatchItems(oid: Union[str, int], oldBatchItems: list, newBatchItems: list):
+def ChangeBatchItems(oid: Union[str, int], items: list, newBatchItems: list[dict]):
     '''
     换商品
     :param oid:  内部订单号
     :param oldBatchItems:  旧商品
     :param newBatchItems:  新商品
     :return: 执行结果
     '''
     return OrderRequest({
-        '__CALLBACKID': 'JTable1',
-        '__CALLBACKPARAM': '{"Method":"ChangeBatchItem","Args":["39044577","{"items":[{"sku_id":"M-男女宽松T-白色-光合作用-CP","qty":1,"price":0,"amount":"0.00","is_gift":false,"oi_id":56037011,"is_del":true,"sku_type":"normal","is_new":false},{"sku_id":"M-男女宽松T-福袋","qty":1,"price":-99999,"amount":"-99999.00","is_gift":false,"oi_id":0,"is_del":false,"is_new":true},{"sku_id":"M-女宽松背心-米色-宇宙恒星-CP","qty":1,"price":39.9,"amount":"39.90","is_gift":false,"oi_id":55970466,"is_del":false,"sku_type":"no_deliver","is_new":false},{"sku_id":"M-女宽松背心-米色-樱桃碎-CP","qty":1,"price":39.9,"amount":"39.90","is_gift":false,"oi_id":55970467,"is_del":false,"sku_type":"no_deliver","is_new":false},{"sku_id":"M-女宽松背心-黑色-复古故事书-CP","qty":1,"price":39.9,"amount":"39.90","is_gift":false,"oi_id":55970468,"is_del":false,"sku_type":"no_deliver","is_new":false}]}"],"CallControl":"{page}"}',
-    },method='ChangeBatchItem')
+        '__CALLBACKPARAM': dumps({"Method": "ChangeBatchItem",
+                                  "Args": [str(oid), dumps({"items": generateChangeBatchItems(items, newBatchItems)})],
+                                  "CallControl": "{page}"}),
+    }, method='ChangeBatchItem')
```

## erp_apis/apis/test.py

```diff
@@ -1,16 +1,42 @@
 # coding: utf-8
 # Project：erp_out_of_stock
 # File：test.py
 # Author：李福成
 # Date ：2024-04-28 18:24
 # IDE：PyCharm
 from apis.inventory import WmsSkuStock
-from apis.order import OrderList
+from apis.order import OrderList, ChangeBatchItems
+from apis.user import login
+from apis.afterSales import aftersaleList, aftersaleCommon, clearException
 
 from request import Session
 
 if __name__ == '__main__':
     session = Session()
-
+    session.erpSend(login(
+        username="",
+        password=""
+    ))
     # 获取分仓库存
-    print(session.erpSend(OrderList(queryData=[])).json())
+    # order = session.erpSend(OrderList(queryData=[{"k": "o_id", "v": "39104496", "c": "@="}])).json()['ReturnValue']['datas'][0]
+    # print(order)
+    # res = session.erpSend(ChangeBatchItems(
+    #     oid = order['o_id'],
+    #     items = order['items'],
+    #     newBatchItems = [
+    #         {
+    #             "sku_id": "M-男女宽松T-福袋",
+    #             "oi_id": order['items'][0]['oi_id'],
+    #         }
+    #     ]
+    # ))
+    # res = session.erpSend(aftersaleList([{
+    #     "k": "shop_id",
+    #     "v": "15429635,14421166,14129300,14409794,13077664,11288284,12151690,12391281,11288291,10341596,15581347,13116222,14242518,14163461,14163558,15517378,15297892,15513593,14420990,14699171,15982786,15748932,14699049,13530518,13445299,14421297,11700009,11725757,14484991,13168313,14418703,13168328",
+    #     "c": "@="}, {"k": "status", "v": "waitconfirm", "c": "@="}, {"k": "type", "v": "换货", "c": "@="},
+    #     {"k": "shop_type", "v": "换货", "c": "@="}, {"k": "as_date", "v": "30天前", "c": ">=", "t": "date"},
+    #     {"k": "as_date", "v": "今天 23:59:59.999", "c": "<=", "t": "date"}])
+    # )
+    # res = session.erpSend(aftersaleCommon(1452451077))
+    res = session.erpSend(clearException(1452451077))
+    print(res.json())
```

## erp_apis/apis/user.py

```diff
@@ -24,12 +24,13 @@
                 "password": password,
                 "j_d_3": "",
                 "v_d_144": "",
                 "isApp": False
             },
             "ipAddress": ""
         },
-        callback='login'
+        callback='login',
+        hostType='erpApi'
     )
```

## Comparing `erp_apis-1.0.1.dist-info/METADATA` & `erp_apis-1.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erp-apis
-Version: 1.0.1
+Version: 1.0.2
 Summary: erp_apis
 Home-page: https://gitee.com/li_fucheng/erp_sdk_python
 Author: 李福成
 Author-email: lfct@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://gitee.com/li_fucheng/erp_sdk_python/issues
 Project-URL: Documentation, https://gitee.com/li_fucheng/erp_sdk_python
```

