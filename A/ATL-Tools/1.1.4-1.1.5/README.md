# Comparing `tmp/atl_tools-1.1.4.tar.gz` & `tmp/atl_tools-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atl_tools-1.1.4.tar", last modified: Wed Apr 24 06:59:00 2024, max compression
+gzip compressed data, was "atl_tools-1.1.5.tar", last modified: Mon May  6 03:17:50 2024, max compression
```

## Comparing `atl_tools-1.1.4.tar` & `atl_tools-1.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-24 06:59:00.921746 atl_tools-1.1.4/
-drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-24 06:59:00.921746 atl_tools-1.1.4/ATL_Tools/
--rw-rw-r--   0 atl       (1002) atl       (1002)    30179 2024-04-24 06:51:21.000000 atl_tools-1.1.4/ATL_Tools/ATL_gdal.py
--rw-rw-r--   0 atl       (1002) atl       (1002)     4295 2024-04-16 11:35:05.000000 atl_tools-1.1.4/ATL_Tools/ATL_path.py
--rw-rw-r--   0 atl       (1002) atl       (1002)     2695 2024-04-16 11:17:35.000000 atl_tools-1.1.4/ATL_Tools/__init__.py
-drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-24 06:59:00.921746 atl_tools-1.1.4/ATL_Tools.egg-info/
--rw-r--r--   0 atl       (1002) atl       (1002)     4715 2024-04-24 06:59:00.000000 atl_tools-1.1.4/ATL_Tools.egg-info/PKG-INFO
--rw-rw-r--   0 atl       (1002) atl       (1002)      222 2024-04-24 06:59:00.000000 atl_tools-1.1.4/ATL_Tools.egg-info/SOURCES.txt
--rw-rw-r--   0 atl       (1002) atl       (1002)        1 2024-04-24 06:59:00.000000 atl_tools-1.1.4/ATL_Tools.egg-info/dependency_links.txt
--rw-rw-r--   0 atl       (1002) atl       (1002)       10 2024-04-24 06:59:00.000000 atl_tools-1.1.4/ATL_Tools.egg-info/top_level.txt
--rw-r--r--   0 atl       (1002) atl       (1002)     4715 2024-04-24 06:59:00.921746 atl_tools-1.1.4/PKG-INFO
--rw-rw-r--   0 atl       (1002) atl       (1002)     4417 2024-04-24 06:58:56.000000 atl_tools-1.1.4/README.md
--rw-rw-r--   0 atl       (1002) atl       (1002)      448 2024-04-24 06:58:55.000000 atl_tools-1.1.4/pyproject.toml
--rw-rw-r--   0 atl       (1002) atl       (1002)       38 2024-04-24 06:59:00.921746 atl_tools-1.1.4/setup.cfg
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-05-06 03:17:50.219870 atl_tools-1.1.5/
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-05-06 03:17:50.219870 atl_tools-1.1.5/ATL_Tools/
+-rw-rw-r--   0 atl       (1002) atl       (1002)    30727 2024-05-06 02:59:37.000000 atl_tools-1.1.5/ATL_Tools/ATL_gdal.py
+-rw-rw-r--   0 atl       (1002) atl       (1002)     4295 2024-04-16 11:35:05.000000 atl_tools-1.1.5/ATL_Tools/ATL_path.py
+-rw-rw-r--   0 atl       (1002) atl       (1002)     2695 2024-04-16 11:17:35.000000 atl_tools-1.1.5/ATL_Tools/__init__.py
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-05-06 03:17:50.219870 atl_tools-1.1.5/ATL_Tools.egg-info/
+-rw-r--r--   0 atl       (1002) atl       (1002)     5049 2024-05-06 03:17:50.000000 atl_tools-1.1.5/ATL_Tools.egg-info/PKG-INFO
+-rw-rw-r--   0 atl       (1002) atl       (1002)      222 2024-05-06 03:17:50.000000 atl_tools-1.1.5/ATL_Tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 atl       (1002) atl       (1002)        1 2024-05-06 03:17:50.000000 atl_tools-1.1.5/ATL_Tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 atl       (1002) atl       (1002)       10 2024-05-06 03:17:50.000000 atl_tools-1.1.5/ATL_Tools.egg-info/top_level.txt
+-rw-r--r--   0 atl       (1002) atl       (1002)     5049 2024-05-06 03:17:50.219870 atl_tools-1.1.5/PKG-INFO
+-rw-rw-r--   0 atl       (1002) atl       (1002)     4750 2024-05-06 03:07:18.000000 atl_tools-1.1.5/README.md
+-rw-rw-r--   0 atl       (1002) atl       (1002)      448 2024-05-06 03:02:11.000000 atl_tools-1.1.5/pyproject.toml
+-rw-rw-r--   0 atl       (1002) atl       (1002)       38 2024-05-06 03:17:50.219870 atl_tools-1.1.5/setup.cfg
```

### Comparing `atl_tools-1.1.4/ATL_Tools/ATL_gdal.py` & `atl_tools-1.1.5/ATL_Tools/ATL_gdal.py`

 * *Files 2% similar despite different names*

```diff
@@ -310,72 +310,75 @@
     elif img_list != None:
         print("  【ATL-LOG】指定img_list, 寻找指定的tif文件...")
         all_files = img_list
     assert all_files!=None, 'No tif files found in the path'
     print(f"  【ATL-LOG】本次镶嵌的影像有{len(all_files)}张")
 
     #获取待镶嵌栅格的最大最小的坐标值
-    min_x,max_y,max_x,min_y=read_img_get_geo(all_files[0]) 
+    min_x, max_y, max_x, min_y = read_img_get_geo(all_files[0]) 
     for in_fn in all_files:
-        minx, maxy, maxx, miny=read_img_get_geo(in_fn)
+        minx, maxy, maxx, miny = read_img_get_geo(in_fn)
         min_x = min(min_x, minx)
         min_y = min(min_y, miny)
         max_x = max(max_x, maxx)
         max_y = max(max_y, maxy)
 
+
     #计算镶嵌后影像的行列号
     in_ds=gdal.Open(all_files[0])
     geotrans=list(in_ds.GetGeoTransform())
     
     # 这一行代码获取了数据集的地理转换信息，包括地理坐标系的变换参数。
     # in_ds.GetGeoTransform() 返回一个包含六个浮点数的元组，
     # 分别表示左上角的X坐标、水平像素分辨率、X方向的旋转（通常为0）、
     # 左上角的Y坐标、Y方向的旋转（通常为0）、垂直像素分辨率。
     # 这一行代码将获取的元组转换为列表形式，并赋值给 geotrans。
 
-    width_geo_resolution=geotrans[1]
-    heigh_geo_resolution=geotrans[5]
+    width_geo_resolution = geotrans[1]
+    heigh_geo_resolution = geotrans[5]
     # print(f'width_geo_resolution:{width_geo_resolution}, heigh_geo_resolution:{heigh_geo_resolution}')
 
-    columns=math.ceil((max_x-min_x)/width_geo_resolution) 
-    rows=math.ceil((max_y-min_y)/(-heigh_geo_resolution))
-    
+    columns = math.ceil((max_x-min_x) / width_geo_resolution) + 50 # 有几个像素的偏差，所以会导致小图超出大图范围！！！ 
+    rows = math.ceil((max_y-min_y) / (-heigh_geo_resolution)) + 50 # 有几个像素的偏差，所以会导致小图超出大图范围！！！ 
+
     bands = in_ds.RasterCount  # 读进来的bands
     if not output_band_chan==None:
         bands = output_band_chan
         print("  【ATL-LOG】人为指定输出波段数为:", bands)
-    print(f'  【ATL-LOG】新合并图像的尺寸: {rows, columns, bands}')
+    print(f'  【ATL-LOG】新合并图像的尺寸: {rows, columns, bands} (高，宽，波段)')
 
     in_band_DataType = in_ds.GetRasterBand(1).DataType
 
-    driver=gdal.GetDriverByName('GTiff')
-    out_ds=driver.Create(output_path, columns, rows, bands, in_band_DataType)
+    driver = gdal.GetDriverByName('GTiff')
+    out_ds = driver.Create(output_path, columns, rows, bands, in_band_DataType)
     out_ds.SetProjection(in_ds.GetProjection())
     geotrans[0] = min_x
     geotrans[3] = max_y
     out_ds.SetGeoTransform(geotrans)
 
 
     #定义仿射逆变换
-    inv_geotrans=gdal.InvGeoTransform(geotrans)
+    inv_geotrans = gdal.InvGeoTransform(geotrans)
 
     #开始逐渐写入
-    for in_fn in tqdm(all_files, desc='正在镶嵌图像ing...'):
+    for in_fn in tqdm(all_files, desc='正在镶嵌图像ing...', colour='GREEN'):
         print('正在镶嵌:', os.path.abspath(in_fn))
         in_ds = gdal.Open(in_fn)
         in_gt = in_ds.GetGeoTransform()
+        # print(f'  【ATL-LOG】读入图像的尺寸：{in_ds.RasterYSize, in_ds.RasterXSize} (高，宽)')
+
         #仿射逆变换
         offset = gdal.ApplyGeoTransform(inv_geotrans, in_gt[0], in_gt[3])
         x, y = map(int, offset)
         # print(f'逆变换后的像素：x:{x}, y:{y}')
         # 该函数返回一个转换器对象 trans，可以使用这个对象执行从输入数据集到输出数据集的坐标转换
         trans = gdal.Transformer(in_ds, out_ds, [])       # in_ds是源栅格，out_ds是目标栅格
         success, xyz = trans.TransformPoint(False, 0, 0)  # 计算in_ds中左上角像元对应out_ds中的行列号
         x, y, z = map(int, xyz)
-        # print(f'小图(0, 0)变换到大图的像素：(x:{x}, y:{y}, z:{z})')
+        # print(f'  【ATL-LOG】小图(0, 0)变换到大图的像素：(({y},{x}), ({y+in_ds.RasterYSize},{x+in_ds.RasterXSize}))')
 
         for band_num in range(bands):
             # 小图的单通道，(h,w),无数据全是nan
             in_ds_array = in_ds.GetRasterBand(band_num + 1).ReadAsArray() #(h,w)
             # 无效数据的地方全是nan,这也符合下载下来的图，空缺的地方是nan、
             # 把nan的地方，用0替代
             in_ds_array = np.nan_to_num(in_ds_array, nan=0.)
@@ -388,26 +391,29 @@
             # 最后要写入大图的数据：如果是根据矢量裁切完的应该不会有重合，直接相加就行
             # 但是如果是矩形大图的话，有重叠的话，则需要舍弃小图的重叠部分。
             # 第一步：找到大图中有数据的区域：即大图不为零的地方
             # 第二步：利用大图中不为零的地方，把小图中的值设置为0 
             # 第三部：把两个图相加，得到最后的结果
             zero_mask_in_tiny_of_big = Tiny_in_BigOut_data!=0.
             in_ds_array[zero_mask_in_tiny_of_big] = 0.
+            # print(f'小图的尺寸{in_ds_array.shape}')
+            # print(f'大图中小图尺寸：{Tiny_in_BigOut_data.shape}')
+            
             in_ds_array = Tiny_in_BigOut_data + in_ds_array
 
             # 写入大图
             big_out_band.WriteArray(in_ds_array, x, y)
     del in_ds, out_ds # 必须要有这个
 
-    if nan_or_zero=='zero' and add_alpha_chan==False:
+    if nan_or_zero == 'zero' and add_alpha_chan == False:
         print(f"  【ATL-LOG】空缺部分为'zero', 不添加alpha通道, 支持float32-img、uint8-label")
         pass
     # 最后把所有为0.的地方都变成nan
     # 如果是float32图像的话,nan是可以work的,则会让无数据的地方变成nan,显示的时候就是透明的
-    elif nan_or_zero=='nan' and add_alpha_chan==False:
+    elif nan_or_zero == 'nan' and add_alpha_chan ==  False:
         print(f"  【ATL-LOG】空缺部分为'nan', 不添加alpha通道,支持-float32img")
         output_img_ds = gdal.Open(output_path)
         Transform = output_img_ds.GetGeoTransform()
         Projection = output_img_ds.GetProjection()
         
         img_nan = output_img_ds.ReadAsArray()
         img_nan = img_nan.transpose(1,2,0)
@@ -417,15 +423,15 @@
                           out_path = output_path, # 覆盖图像
                           Transform = Transform,
                           Projection = Projection,
                           Datatype = output_img_ds.GetRasterBand(1).DataType,
                           Band = bands)
 
     # 如果创建的图像是uint8的话，nan是不行的，只能用0,添加alpha通道
-    elif add_alpha_chan==True:
+    elif add_alpha_chan == True:
         print(f"  【ATL-LOG】添加alpha通道,支持uint8-rgb-img uint8-RGB-label")
         output_img_ds = gdal.Open(output_path)
         Transform = output_img_ds.GetGeoTransform()
         Projection = output_img_ds.GetProjection()
 
         output_img = output_img_ds.ReadAsArray()
         output_img = np.transpose(output_img, (1, 2, 0))
```

### Comparing `atl_tools-1.1.4/ATL_Tools/ATL_path.py` & `atl_tools-1.1.5/ATL_Tools/ATL_path.py`

 * *Files identical despite different names*

### Comparing `atl_tools-1.1.4/ATL_Tools/__init__.py` & `atl_tools-1.1.5/ATL_Tools/__init__.py`

 * *Files identical despite different names*

### Comparing `atl_tools-1.1.4/ATL_Tools.egg-info/PKG-INFO` & `atl_tools-1.1.5/ATL_Tools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ATL_Tools
-Version: 1.1.4
+Version: 1.1.5
 Summary: AI-Tianlong的Tools打包，开箱即用, 包含ATL_path和ATL_gdal,可用于文件夹创建、文件搜索、遥感图像处理
 License: MIT License
 Keywords: ATL_Tools,GDAL,AI-Tianlong,Chinese
 Description-Content-Type: text/markdown
 
 # ATL_Tools 使用指南
 ## 0. 简介
@@ -31,15 +31,16 @@
     geo_to_pix,         # 根据GDAL的仿射变换参数模型将给定的投影或地理坐标转为影像图上坐标（行列号）
     Mosaic_all_imgs,    # ✔将指定路径文件夹下的tif影像全部镶嵌到一张影像上
     Mosaic_2img_to_one, # 将两幅影像镶嵌至同一幅影像
     raster_overlap,     # 两个栅格数据集取重叠区或求交集（仅测试方形影像）
     crop_tif_with_json_zero, # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为0
     crop_tif_with_json_nan,  # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为nan
     Merge_multi_json,   # ✔将多个小的json合并为一个大的json,
-    resample_image      # ✔使用GDAL对图像进行重采样
+    resample_image,      # ✔使用GDAL对图像进行重采样
+    shp_to_geojson,      # ✔将shp文件转为geojson文件
                         )
 ```
 ## 3. 使用方法
 
 ### 3.1 ATL_path 文件夹工具
 
 使用程序示例:  
@@ -86,7 +87,8 @@
 - 2024-04-16 v1.0.8 修复 `ValueError: cannot convert float NaN to integer` in ATL_gdal Line 371
 - 2024-04-16 v1.0.9 修复 修复`Mosaic_all_images()`对于mosaic RGB uint8标签的支持，优化`find_data_list()`函数显示，优化`_init_.py`, 优化`Readme.md`显示
 - 2024-04-16 v1.1.0 pypi页面增加`ATL_Tools`Github贡献地址。
 - 2024-04-16 v1.1.1 `crop_tif_with_json_nan()`增加可选参数`add_alpha_chan: bool`控制是否为RGB标签增加 alpha 通道
 - 2024-04-16 v1.1.2 修复 ATL_gdal Line 397 变量使用错误
 - 2024-04-18 v1.1.3 修复 ATL_gdal Mosaic中对float32图像背景设置为nan的支持
 - 2024-04-24 v1.1.4 修复 ATL_gdal Mosaic中指定img_list功能的支持，可以指定Mosaic的图像，增加`shp`转换为`Geojson`的功能函数`shp_to_geojson()`
+- 2024-05-06 v1.1.5 修复 ATL_gdal 中 `Mosaic_all_imgs()`函数在某些情况下，可能导致计算出的合并后的大图尺寸要比嵌入的小图位置要小几个像素，在 line 340 代码中，给图像的高宽各+50像素，暂时避免了这个问题。
```

### Comparing `atl_tools-1.1.4/PKG-INFO` & `atl_tools-1.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ATL_Tools
-Version: 1.1.4
+Version: 1.1.5
 Summary: AI-Tianlong的Tools打包，开箱即用, 包含ATL_path和ATL_gdal,可用于文件夹创建、文件搜索、遥感图像处理
 License: MIT License
 Keywords: ATL_Tools,GDAL,AI-Tianlong,Chinese
 Description-Content-Type: text/markdown
 
 # ATL_Tools 使用指南
 ## 0. 简介
@@ -31,15 +31,16 @@
     geo_to_pix,         # 根据GDAL的仿射变换参数模型将给定的投影或地理坐标转为影像图上坐标（行列号）
     Mosaic_all_imgs,    # ✔将指定路径文件夹下的tif影像全部镶嵌到一张影像上
     Mosaic_2img_to_one, # 将两幅影像镶嵌至同一幅影像
     raster_overlap,     # 两个栅格数据集取重叠区或求交集（仅测试方形影像）
     crop_tif_with_json_zero, # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为0
     crop_tif_with_json_nan,  # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为nan
     Merge_multi_json,   # ✔将多个小的json合并为一个大的json,
-    resample_image      # ✔使用GDAL对图像进行重采样
+    resample_image,      # ✔使用GDAL对图像进行重采样
+    shp_to_geojson,      # ✔将shp文件转为geojson文件
                         )
 ```
 ## 3. 使用方法
 
 ### 3.1 ATL_path 文件夹工具
 
 使用程序示例:  
@@ -86,7 +87,8 @@
 - 2024-04-16 v1.0.8 修复 `ValueError: cannot convert float NaN to integer` in ATL_gdal Line 371
 - 2024-04-16 v1.0.9 修复 修复`Mosaic_all_images()`对于mosaic RGB uint8标签的支持，优化`find_data_list()`函数显示，优化`_init_.py`, 优化`Readme.md`显示
 - 2024-04-16 v1.1.0 pypi页面增加`ATL_Tools`Github贡献地址。
 - 2024-04-16 v1.1.1 `crop_tif_with_json_nan()`增加可选参数`add_alpha_chan: bool`控制是否为RGB标签增加 alpha 通道
 - 2024-04-16 v1.1.2 修复 ATL_gdal Line 397 变量使用错误
 - 2024-04-18 v1.1.3 修复 ATL_gdal Mosaic中对float32图像背景设置为nan的支持
 - 2024-04-24 v1.1.4 修复 ATL_gdal Mosaic中指定img_list功能的支持，可以指定Mosaic的图像，增加`shp`转换为`Geojson`的功能函数`shp_to_geojson()`
+- 2024-05-06 v1.1.5 修复 ATL_gdal 中 `Mosaic_all_imgs()`函数在某些情况下，可能导致计算出的合并后的大图尺寸要比嵌入的小图位置要小几个像素，在 line 340 代码中，给图像的高宽各+50像素，暂时避免了这个问题。
```

### Comparing `atl_tools-1.1.4/README.md` & `atl_tools-1.1.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,16 @@
     geo_to_pix,         # 根据GDAL的仿射变换参数模型将给定的投影或地理坐标转为影像图上坐标（行列号）
     Mosaic_all_imgs,    # ✔将指定路径文件夹下的tif影像全部镶嵌到一张影像上
     Mosaic_2img_to_one, # 将两幅影像镶嵌至同一幅影像
     raster_overlap,     # 两个栅格数据集取重叠区或求交集（仅测试方形影像）
     crop_tif_with_json_zero, # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为0
     crop_tif_with_json_nan,  # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为nan
     Merge_multi_json,   # ✔将多个小的json合并为一个大的json,
-    resample_image      # ✔使用GDAL对图像进行重采样
+    resample_image,      # ✔使用GDAL对图像进行重采样
+    shp_to_geojson,      # ✔将shp文件转为geojson文件
                         )
 ```
 ## 3. 使用方法
 
 ### 3.1 ATL_path 文件夹工具
 
 使用程序示例:  
@@ -78,7 +79,8 @@
 - 2024-04-16 v1.0.8 修复 `ValueError: cannot convert float NaN to integer` in ATL_gdal Line 371
 - 2024-04-16 v1.0.9 修复 修复`Mosaic_all_images()`对于mosaic RGB uint8标签的支持，优化`find_data_list()`函数显示，优化`_init_.py`, 优化`Readme.md`显示
 - 2024-04-16 v1.1.0 pypi页面增加`ATL_Tools`Github贡献地址。
 - 2024-04-16 v1.1.1 `crop_tif_with_json_nan()`增加可选参数`add_alpha_chan: bool`控制是否为RGB标签增加 alpha 通道
 - 2024-04-16 v1.1.2 修复 ATL_gdal Line 397 变量使用错误
 - 2024-04-18 v1.1.3 修复 ATL_gdal Mosaic中对float32图像背景设置为nan的支持
 - 2024-04-24 v1.1.4 修复 ATL_gdal Mosaic中指定img_list功能的支持，可以指定Mosaic的图像，增加`shp`转换为`Geojson`的功能函数`shp_to_geojson()`
+- 2024-05-06 v1.1.5 修复 ATL_gdal 中 `Mosaic_all_imgs()`函数在某些情况下，可能导致计算出的合并后的大图尺寸要比嵌入的小图位置要小几个像素，在 line 340 代码中，给图像的高宽各+50像素，暂时避免了这个问题。
```

