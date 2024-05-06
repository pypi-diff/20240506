# Comparing `tmp/JayttleProcess-0.2.8-py3-none-any.whl.zip` & `tmp/JayttleProcess-0.2.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 61159 bytes, number of entries: 15
+Zip file size: 62341 bytes, number of entries: 15
 -rw-rw-rw-  2.0 fat     2978 b- defN 24-Apr-29 13:43 JayttleProcess/CommonDecorator.py
 -rw-rw-rw-  2.0 fat    10785 b- defN 24-Apr-26 14:47 JayttleProcess/ComputerControl.py
 -rw-rw-rw-  2.0 fat      613 b- defN 24-Apr-08 05:57 JayttleProcess/EntertainmentCode.py
 -rw-rw-rw-  2.0 fat     6834 b- defN 24-Apr-29 06:01 JayttleProcess/FTPCommonUse.py
 -rw-rw-rw-  2.0 fat     5650 b- defN 24-Apr-24 02:33 JayttleProcess/JsonCommonManage.py
 -rw-rw-rw-  2.0 fat     3461 b- defN 24-Apr-28 07:21 JayttleProcess/MachineLearning.py
 -rw-rw-rw-  2.0 fat    39584 b- defN 24-Apr-24 13:25 JayttleProcess/RinexCommonManage.py
 -rw-rw-rw-  2.0 fat    34687 b- defN 24-Apr-29 13:43 JayttleProcess/SQLCommonUse.py
--rw-rw-rw-  2.0 fat    15081 b- defN 24-Apr-29 15:10 JayttleProcess/TBCProcessCsv.py
--rw-rw-rw-  2.0 fat   121805 b- defN 24-Apr-29 15:10 JayttleProcess/TimeSeriesDataMethod.py
+-rw-rw-rw-  2.0 fat    16485 b- defN 24-May-06 10:36 JayttleProcess/TBCProcessCsv.py
+-rw-rw-rw-  2.0 fat   124974 b- defN 24-May-06 10:35 JayttleProcess/TimeSeriesDataMethod.py
 -rw-rw-rw-  2.0 fat        0 b- defN 24-Mar-14 14:39 JayttleProcess/__init__.py
--rw-rw-rw-  2.0 fat      601 b- defN 24-Apr-29 15:11 JayttleProcess-0.2.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-29 15:11 JayttleProcess-0.2.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 24-Apr-29 15:11 JayttleProcess-0.2.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1312 b- defN 24-Apr-29 15:11 JayttleProcess-0.2.8.dist-info/RECORD
-15 files, 243498 bytes uncompressed, 58969 bytes compressed:  75.8%
+-rw-rw-rw-  2.0 fat      601 b- defN 24-May-06 10:36 JayttleProcess-0.2.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-06 10:36 JayttleProcess-0.2.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 24-May-06 10:36 JayttleProcess-0.2.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1312 b- defN 24-May-06 10:36 JayttleProcess-0.2.9.dist-info/RECORD
+15 files, 248071 bytes uncompressed, 60151 bytes compressed:  75.8%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: JayttleProcess/TimeSeriesDataMethod.py
 Comment: 
 
 Filename: JayttleProcess/__init__.py
 Comment: 
 
-Filename: JayttleProcess-0.2.8.dist-info/METADATA
+Filename: JayttleProcess-0.2.9.dist-info/METADATA
 Comment: 
 
-Filename: JayttleProcess-0.2.8.dist-info/WHEEL
+Filename: JayttleProcess-0.2.9.dist-info/WHEEL
 Comment: 
 
-Filename: JayttleProcess-0.2.8.dist-info/top_level.txt
+Filename: JayttleProcess-0.2.9.dist-info/top_level.txt
 Comment: 
 
-Filename: JayttleProcess-0.2.8.dist-info/RECORD
+Filename: JayttleProcess-0.2.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## JayttleProcess/TBCProcessCsv.py

```diff
@@ -1,13 +1,14 @@
 import os
 import csv
 import pandas as pd
 import json
 import chardet
 import pyproj
+import numpy as np
 from datetime import datetime
 from collections import defaultdict
 from dataclasses import dataclass
 from typing import TypedDict, List, Dict, Optional
 from JayttleProcess import CommonDecorator
 from JayttleProcess import TimeSeriesDataMethod as TSD
 from JayttleProcess.TimeSeriesDataMethod import TimeSeriesData
@@ -186,15 +187,15 @@
     if selected_value is None:
         return None
     
     # 提取 Time 属性
     time_value = datapoint.Time
     
     # 创建 TimeSeriesData 对象并返回
-    return TimeSeriesData(selected_value, time_value)
+    return TimeSeriesData(selected_value, time_value.strftime("%Y-%m-%d %H:%M:%S.%f"))
 
 
 def export_list_to_excel(datapoints: list[DataPoint]) -> None:
     # 将 DataPoint 对象列表转换为 Pandas DataFrame
     datapoints_df = pd.DataFrame([vars(dp) for dp in datapoints])
 
     # 将 start_time 转换为日期并设置为索引
@@ -292,16 +293,16 @@
     converted_lon_tsd = []
     
     for lat, lon in zip(lat_tsd, lon_tsd):
         # 对纬度和经度进行坐标转换
         converted_lat, converted_lon = convert_coordinates(lat.value, lon.value)
         
         # 创建新的 TimeSeriesData 对象并添加到列表中
-        converted_lat_tsd.append(TimeSeriesData(converted_lat, lat.datetime))
-        converted_lon_tsd.append(TimeSeriesData(converted_lon, lon.datetime))
+        converted_lat_tsd.append(TimeSeriesData(converted_lat, lat.datetime.strftime("%Y-%m-%d %H:%M:%S.%f")))
+        converted_lon_tsd.append(TimeSeriesData(converted_lon, lon.datetime.strftime("%Y-%m-%d %H:%M:%S.%f")))
     
     return converted_lat_tsd, converted_lon_tsd
 
 @CommonDecorator.log_function_call
 def do_porj1() -> None:
     # 读取数据
     read_data(r"D:\Program Files (x86)\Software\OneDrive\PyPackages\R081_data.txt")
@@ -310,14 +311,36 @@
     value_key = "Lon"
     lon_tsd = [ggkxDto_create_timeseries_data(datapoint, value_key) for datapoint in data_dict['81']]
     converted_lat_tsd, converted_lon_tsd = convert_latlon_coordinates(lat_tsd, lon_tsd)
     TSD.remove_average(converted_lat_tsd)
     TSD.remove_average(converted_lon_tsd)
     print(f'converted_lon_tsd:{len(converted_lon_tsd)}')
 
+    converted_lat_tsd = np.array(converted_lat_tsd)  # 将列表转换为NumPy数组
+    converted_lon_tsd = np.array(converted_lon_tsd)  # 将列表转换为NumPy数组
+
+    # 对北坐标执行傅里叶变换，只保留正频率
+    north_fft = np.fft.fft(converted_lat_tsd)
+    north_freq = np.fft.fftfreq(len(converted_lat_tsd))
+    north_positive_mask = north_freq > 0
+    north_fft = north_fft[north_positive_mask]
+    north_freq = north_freq[north_positive_mask]
+    
+    # 对东坐标执行傅里叶变换，只保留正频率
+    east_fft = np.fft.fft(converted_lon_tsd)
+    east_freq = np.fft.fftfreq(len(converted_lon_tsd))
+    east_positive_mask = east_freq > 0
+    east_fft = east_fft[east_positive_mask]
+    east_freq = east_freq[east_positive_mask]
+
+    TSD.analyze_fourier_transform_results_version2(north_freq,north_fft,east_freq,east_fft)
+
+
+
+
 
 @CommonDecorator.log_function_call
 def before_process_proj() -> None:
     json_file_path = r'D:\Program Files (x86)\Software\OneDrive\PyPackages\config.json'
     json_data: Data = read_json_file(json_file_path)
 
     
@@ -335,16 +358,21 @@
     csv_folder_path = r'D:\Ropeway\FTPCsv3'
     # Iterate through each CSV file in the folder
     for filename in os.listdir(csv_folder_path):
         if filename.endswith('.csv'):
             csv_file_path = os.path.join(csv_folder_path, filename)
             datapoints_csv.extend(read_csv_to_datapoints(csv_file_path))
 
-    export_list_to_excel(datapoints_csv)
-
     # 定义要提取的属性键
     value_key = "north_coordinate"
     # 使用列表推导式创建 TimeSeriesData 对象列表
     my_tsd: list[TimeSeriesData] = [dataPoint_create_timeseries_data(datapoint, value_key) for datapoint in datapoints_csv]
     TSD.remove_average(my_tsd)
     # TSD.plot_TimeSeriesData_threshold(my_tsd, True, threshold = 100)
+#TODO：再把晚上8点的~12点的 tbc处理
+#TODO：把东坐标 北坐标放入一个坐标系里看角度与分布  是否与风向有关
+#TODO：计算另一个天线进行对比比较 
+#TODO：找出突变的原因 可以先计算他的前后差值如果大则查看他的计算精度
+#TODO：按照季节分化 春夏秋冬看是否有差距
+#TODO：10hz数据的处理和查看
+#TODO：数据库里的环境数据是否可用hw
```

## JayttleProcess/TimeSeriesDataMethod.py

```diff
@@ -42,22 +42,28 @@
 # 禁用特定警告
 warnings.filterwarnings('ignore', category=UserWarning, append=True)
 # 或者关闭所有警告
 warnings.filterwarnings("ignore")
 # endregion
 
 class TimeSeriesData:
-    def __init__(self, value: float, date_time_str: str):
-        self.value: float = value
-        self.datetime: datetime = datetime.strptime(date_time_str, "%Y-%m-%d %H:%M:%S")
+    def __init__(self, value: float, datetime_input):
+        self.value = value
+        # Check if the input is a datetime object or a string
+        if isinstance(datetime_input, datetime):
+            self.datetime = datetime_input
+        elif isinstance(datetime_input, str):
+            # Parse the datetime string
+            self.datetime = datetime.strptime(datetime_input, "%Y-%m-%d %H:%M:%S.%f")
+        else:
+            raise TypeError("datetime_input must be a datetime object or a datetime string in the format '%Y-%m-%d %H:%M:%S.%f'")
 
-    def __str__(self) -> str:
+    def __str__(self):
         return f"Value: {self.value}, Datetime: {self.datetime}"
 
-
 # region 无关功能
 def check_data_type(data: np.ndarray) ->None:
     print("数据类型:", type(data))
     print("形状:", data.shape)
 
 
 # endregion
@@ -1547,14 +1553,63 @@
     if SaveFilePath is not None:
         plt.savefig(SaveFilePath)
     else: 
         plt.show()
     plt.close()
 
 
+def analyze_fourier_fft_freq(north_freq: np.ndarray, 
+                             north_fft: np.ndarray, 
+                             east_freq: np.ndarray, 
+                             east_fft: np.ndarray) -> None:
+    """
+    函数“analyze_fourier_transform_results”用于计算和可视化北坐标和东坐标的振幅谱，并识别数据中的主要周期分量。
+
+    :param north_freq: 北坐标数据的频率值，与傅立叶变换结果相关联。
+    :type north_freq: numpy.ndarray
+    :param north_fft: 北坐标数据的傅里叶变换结果，包含有关不同频率分量的幅度和相位信息。
+    :type north_fft: numpy.ndarray
+    :param east_freq: 东坐标数据的频率值，与傅立叶变换结果相关联。
+    :type east_freq: numpy.ndarray
+    :param east_fft: 东坐标数据的傅里叶变换结果，包含有关不同频率分量的幅度和相位信息。
+    :type east_fft: numpy.ndarray
+    
+    该函数排除了零频率，并绘制了北坐标和东坐标的振幅谱图。然后，它识别出每个坐标系中的主要周期成分，并将其打印出来。
+    """
+    # 排除零频率
+    north_amplitude_spectrum: np.ndarray = np.abs(north_fft[1:])
+    east_amplitude_spectrum: np.ndarray = np.abs(east_fft[1:])
+    non_zero_north_freq: np.ndarray = north_freq[1:]
+    non_zero_east_freq: np.ndarray = east_freq[1:]
+    
+    # 计算主周期频率
+    north_main_period_index: int = np.argmax(north_amplitude_spectrum)
+    east_main_period_index: int = np.argmax(east_amplitude_spectrum)
+    north_main_period_frequency: float = non_zero_north_freq[north_main_period_index]
+    east_main_period_frequency: float = non_zero_east_freq[east_main_period_index]
+    
+    # 绘制频谱图
+    plt.figure(figsize=(12, 6))
+    plt.subplot(2, 1, 1)
+    plt.plot(non_zero_north_freq, north_amplitude_spectrum, color='black', linestyle='-', linewidth=1)  # 使用灰色线条
+    plt.scatter(north_main_period_frequency, north_amplitude_spectrum[north_main_period_index], color='red', marker='o', s=10)  # 添加红色标记，并设置大小为10
+    plt.title(f'北坐标幅度谱 (主周期: {1 / north_main_period_frequency:.2f})')
+    plt.xlabel('频率')
+    plt.ylabel('幅度')
+    
+    plt.subplot(2, 1, 2)
+    plt.plot(non_zero_east_freq, east_amplitude_spectrum, color='black', linestyle='-', linewidth=1)  # 使用灰色线条
+    plt.scatter(east_main_period_frequency, east_amplitude_spectrum[east_main_period_index], color='red', marker='o', s=10)  # 添加红色标记，并设置大小为10
+    plt.title(f'东坐标幅度谱 (主周期: {1 / east_main_period_frequency:.2f})')
+    plt.xlabel('频率')
+    plt.ylabel('幅度')
+    
+    plt.tight_layout()
+    
+    plt.show()
 # endregion
 # region statsmodels的运用
 def plot_time_series_decomposition(time_series: List[TimeSeriesData], SaveFilePath: str = None) -> None:
     """进行季节性分解"""
     # 将 TimeSeriesData 转换为 Pandas 的 Series 对象
     values = [data.value for data in time_series]
     datetimes = [data.datetime for data in time_series]
```

## Comparing `JayttleProcess-0.2.8.dist-info/METADATA` & `JayttleProcess-0.2.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JayttleProcess
-Version: 0.2.8
+Version: 0.2.9
 Summary: modifty time:2024-04-29 21:25
  en: Data Process;
  zh_CN:数据处理的方法
 Home-page: UNKNOWN
 Author: Jayttle
 Author-email: 294448068@qq.com
 License: UNKNOWN
```

## Comparing `JayttleProcess-0.2.8.dist-info/RECORD` & `JayttleProcess-0.2.9.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 JayttleProcess/ComputerControl.py,sha256=xm-Z3JxJNdZP86SPXvGcZ3-dOyL12Zs9wqmFatOR2iU,10785
 JayttleProcess/EntertainmentCode.py,sha256=KR-nFHjwIjfl8E_IMuRl44p2Xwkw6UMZYuvkdL9NFck,613
 JayttleProcess/FTPCommonUse.py,sha256=awsRf0Dm0faUCdI3dW8FNg2bZWGT1bRd3MNcPIfhttA,6834
 JayttleProcess/JsonCommonManage.py,sha256=KJtfAxPUGktFMocoFKFd8E_VtGW-vyhAMPPz--34mkA,5650
 JayttleProcess/MachineLearning.py,sha256=Xi3iI7woakrlusNqFhoVHznpuwntUt9YUeWIZTLP2MI,3461
 JayttleProcess/RinexCommonManage.py,sha256=bDOK6YLqXYSD4shuKzioDZxuNhgubfKYp8VLMVZFfZ4,39584
 JayttleProcess/SQLCommonUse.py,sha256=PZe1IgQ60ZQYDbCU-f_z_kt4uBDBXlJQboa-niiixV4,34687
-JayttleProcess/TBCProcessCsv.py,sha256=mlP0_Uzf0HOwpfjYe0z5G_BDpv1p-qPo2v3jpeK2Ul8,15081
-JayttleProcess/TimeSeriesDataMethod.py,sha256=f8LG2LBKRRDGStMaH3tSfaYX1V24vnQUXk1ziujByjE,121805
+JayttleProcess/TBCProcessCsv.py,sha256=R3jv-aOel69sbsOlR30waSqnhRXamQTGI8nOrxNCCIY,16485
+JayttleProcess/TimeSeriesDataMethod.py,sha256=Hhx8VzjiWCWYkyIxKDMNr2RSzrPvfNsn5yt5H_gnMS0,124974
 JayttleProcess/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-JayttleProcess-0.2.8.dist-info/METADATA,sha256=F-rxjAMX_uCNg82cVTihzdw9k_3gYUnAufbf4OYfuDc,601
-JayttleProcess-0.2.8.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-JayttleProcess-0.2.8.dist-info/top_level.txt,sha256=0wohZ9zSz5j0d_abN3JTtoTUIvlCsfp-LHIP_NcoOlw,15
-JayttleProcess-0.2.8.dist-info/RECORD,,
+JayttleProcess-0.2.9.dist-info/METADATA,sha256=s3ITNYwuIoktbz2lWi05Grjsd4eiMqquZ8UXzS2GbuM,601
+JayttleProcess-0.2.9.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+JayttleProcess-0.2.9.dist-info/top_level.txt,sha256=0wohZ9zSz5j0d_abN3JTtoTUIvlCsfp-LHIP_NcoOlw,15
+JayttleProcess-0.2.9.dist-info/RECORD,,
```

