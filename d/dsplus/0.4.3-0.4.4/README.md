# Comparing `tmp/dsplus-0.4.3.tar.gz` & `tmp/dsplus-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsplus-0.4.3.tar", last modified: Fri May  3 00:22:43 2024, max compression
+gzip compressed data, was "dsplus-0.4.4.tar", last modified: Sun May  5 18:15:46 2024, max compression
```

## Comparing `dsplus-0.4.3.tar` & `dsplus-0.4.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 00:22:43.069855 dsplus-0.4.3/
--rw-rw-rw-   0        0        0     1083 2024-03-15 02:57:42.000000 dsplus-0.4.3/LICENSE
--rw-rw-rw-   0        0        0      690 2024-05-03 00:22:43.066053 dsplus-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0       99 2024-02-24 21:14:11.000000 dsplus-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-03 00:22:43.035422 dsplus-0.4.3/dsplus/
--rw-rw-rw-   0        0        0      171 2024-05-03 00:09:20.000000 dsplus-0.4.3/dsplus/__init__.py
--rw-rw-rw-   0        0        0    24324 2024-05-02 23:18:42.000000 dsplus-0.4.3/dsplus/pb_functions_general.py
--rw-rw-rw-   0        0        0    42785 2024-05-02 23:18:42.000000 dsplus-0.4.3/dsplus/pb_functions_pandas.py
--rw-rw-rw-   0        0        0    56894 2024-04-02 22:58:04.000000 dsplus-0.4.3/dsplus/pb_functions_plotly.py
--rw-rw-rw-   0        0        0    48825 2024-05-02 23:18:42.000000 dsplus-0.4.3/dsplus/pb_functions_spatial.py
-drwxrwxrwx   0        0        0        0 2024-05-03 00:22:43.053322 dsplus-0.4.3/dsplus.egg-info/
--rw-rw-rw-   0        0        0      690 2024-05-03 00:22:42.000000 dsplus-0.4.3/dsplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-05-03 00:22:42.000000 dsplus-0.4.3/dsplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 00:22:42.000000 dsplus-0.4.3/dsplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-03 00:22:42.000000 dsplus-0.4.3/dsplus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-03 00:22:43.069855 dsplus-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1650 2024-03-29 02:13:48.000000 dsplus-0.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 00:22:43.057687 dsplus-0.4.3/tests/
--rw-rw-rw-   0        0        0    12530 2024-04-17 03:55:44.000000 dsplus-0.4.3/tests/Test_pandas.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:15:46.569019 dsplus-0.4.4/
+-rw-rw-rw-   0        0        0     1083 2024-03-15 02:57:42.000000 dsplus-0.4.4/LICENSE
+-rw-rw-rw-   0        0        0      690 2024-05-05 18:15:46.563417 dsplus-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0       99 2024-02-24 21:14:11.000000 dsplus-0.4.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-05 18:15:46.545257 dsplus-0.4.4/dsplus/
+-rw-rw-rw-   0        0        0      171 2024-05-05 18:15:24.000000 dsplus-0.4.4/dsplus/__init__.py
+-rw-rw-rw-   0        0        0    24324 2024-05-02 23:18:42.000000 dsplus-0.4.4/dsplus/pb_functions_general.py
+-rw-rw-rw-   0        0        0    42785 2024-05-02 23:18:42.000000 dsplus-0.4.4/dsplus/pb_functions_pandas.py
+-rw-rw-rw-   0        0        0    56894 2024-04-02 22:58:04.000000 dsplus-0.4.4/dsplus/pb_functions_plotly.py
+-rw-rw-rw-   0        0        0    58862 2024-05-05 17:55:16.000000 dsplus-0.4.4/dsplus/pb_functions_spatial.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:15:46.557330 dsplus-0.4.4/dsplus.egg-info/
+-rw-rw-rw-   0        0        0      690 2024-05-05 18:15:46.000000 dsplus-0.4.4/dsplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-05-05 18:15:46.000000 dsplus-0.4.4/dsplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-05 18:15:46.000000 dsplus-0.4.4/dsplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-05 18:15:46.000000 dsplus-0.4.4/dsplus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-05 18:15:46.569019 dsplus-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1650 2024-03-29 02:13:48.000000 dsplus-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-05 18:15:46.557330 dsplus-0.4.4/tests/
+-rw-rw-rw-   0        0        0    12530 2024-04-17 03:55:44.000000 dsplus-0.4.4/tests/Test_pandas.py
```

### Comparing `dsplus-0.4.3/LICENSE` & `dsplus-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.3/PKG-INFO` & `dsplus-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsplus
-Version: 0.4.3
+Version: 0.4.4
 Summary: Helper functions for data science applications.
 Author: Prashana Bajracharya
 Author-email: pajracharya713@gmail.com
 Keywords: data science,pandas
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dsplus-0.4.3/dsplus/pb_functions_general.py` & `dsplus-0.4.4/dsplus/pb_functions_general.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.3/dsplus/pb_functions_pandas.py` & `dsplus-0.4.4/dsplus/pb_functions_pandas.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.3/dsplus/pb_functions_plotly.py` & `dsplus-0.4.4/dsplus/pb_functions_plotly.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.3/dsplus/pb_functions_spatial.py` & `dsplus-0.4.4/dsplus/pb_functions_spatial.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import rasterio
 import rasterstats as rs
 
 import plotly.express as px
 
 from .pb_functions_general import *
 from .pb_functions_pandas import *
+from .pb_functions_plotly import *
 
 #endregion -----------------------------------------------------------------------------------------
 #region Variables
 
 #%%
 class Options_epsg(Enum):
     wgs84 = 4326
@@ -819,14 +820,265 @@
                 fig.data[i].showlegend = False
     if hover_skip:
         fig = fig\
             .update_traces(hoverinfo='skip',
                            hovertemplate=None)
     return fig
 
+#%%
+class px_Map(px_Plot):
+    fig = None
+
+    def __init__(self,
+                 sp=None,
+                 center_lon=-95.7129, 
+                 center_lat=37.0902, 
+                 zoom=2.5, 
+                 **kwargs) -> None:
+        if sp is not None:
+            if sp.crs.to_epsg() != Options_epsg.wgs84.value:
+                sp = sp.to_crs(Options_epsg.wgs84.value)
+        
+            temp_centroid = gpd.GeoDataFrame(geometry=sp.centroid)
+            center_lon = temp_centroid.geometry.x.mean()
+            center_lat = temp_centroid.geometry.y.mean()
+        fig = px.choropleth_mapbox(center=dict(lon=center_lon,
+                                               lat=center_lat),
+                                   zoom=zoom,
+                                   **kwargs)
+        
+        self.fig = fig
+
+        self.add_sp_basemap(Options_px_basemap.none.value)
+        
+    def add_sp_basemap(self, basemap):
+        fig = self.fig
+        
+        if pd.Series(dir(Options_px_tiles)).str.contains(basemap).any():
+            fig.update_layout(
+                mapbox_style="white-bg",
+                mapbox_layers=[
+                    {
+                        "below": "traces",
+                        "sourcetype": "raster",
+                        # "sourceattribution": "United States Geological Survey",
+                        "source": [Options_px_tiles[basemap].value],
+                    }
+                ],
+            )
+        else:
+            fig.update_layout(mapbox_style=basemap)
+
+        return self
+        
+    def add_sp_points(self,
+                      sp_points,
+                      color_value = None,
+                      size_value = None,
+                      symbol_value = None,
+                      legend_name = None,
+                      hover_skip = False,
+                      update_crs = True,
+                      **kwargs):
+        fig = self.fig
+
+        if update_crs:
+            if sp_points.crs.to_epsg() != Options_epsg.wgs84.value:
+                sp_points = sp_points.to_crs(Options_epsg.wgs84.value)
+        trace = px.scatter_mapbox(sp_points,
+                                lon=sp_points.geometry.x,
+                                lat=sp_points.geometry.y,
+                                **kwargs)
+        if color_value is not None:
+            trace = trace\
+                .update_traces(marker=dict(color=color_value))
+        if size_value is not None:
+            trace = trace\
+                .update_traces(marker=dict(size=size_value))
+        if symbol_value is not None:
+            trace = trace\
+                .update_traces(marker=dict(symbol=symbol_value))
+        if legend_name is not None:
+            if ('color' not in kwargs) and ('size' not in kwargs):
+                trace = trace\
+                    .update_traces(name=legend_name,
+                                   showlegend=True)
+            else:
+                trace = trace\
+                    .update_traces(legendgroup=legend_name,
+                                   legendgrouptitle_text=legend_name,
+                                   showlegend=True)
+        if hover_skip:
+            trace = trace\
+                .update_traces(hoverinfo='skip',
+                               hovertemplate=None)
+            
+        px_add_trace_data(fig, trace)
+
+        return self
+    
+    def add_sp_polylines(self,
+                        sp_lines,
+                        color_value = None,
+                        width_value = None,
+                        dash_value = None,
+                        legend_name = None,
+                        hover_skip = False,
+                        update_crs = True,
+                        **kwargs):
+        fig = self.fig
+
+        if update_crs:
+            if sp_lines.crs.to_epsg() != Options_epsg.wgs84.value:
+                sp_lines = sp_lines.to_crs(Options_epsg.wgs84.value)
+        df_lines_xy = sp_to_df_xy(sp_lines, cols_keep_all=True)
+        trace = px.line_mapbox(df_lines_xy,
+                            lon=df_lines_xy['x'],
+                            lat=df_lines_xy['y'],
+                            line_group=df_lines_xy['id_geom'],
+                            **kwargs)
+        if color_value is not None:
+            trace = trace\
+                .update_traces(line=dict(color=color_value))
+        if width_value is not None:
+            trace = trace\
+                .update_traces(line=dict(width=width_value))
+        if dash_value is not None:
+            trace = trace\
+                .update_traces(line=dict(dash=dash_value))
+        if legend_name is not None:
+            if 'color' not in kwargs:
+                trace = trace\
+                    .update_traces(name=legend_name,
+                                legendgroup=legend_name,
+                                showlegend=True)
+            else:
+                trace = trace\
+                    .update_traces(legendgroup=legend_name,
+                                legendgrouptitle_text=legend_name,
+                                showlegend=True)
+        if 'color' not in kwargs:
+            for i in range(len(trace.data)):
+                if i == 0:
+                    trace.data[i].showlegend = True
+                else:
+                    trace.data[i].showlegend = False
+        if hover_skip:
+            trace = trace\
+                .update_traces(hoverinfo='skip',
+                            hovertemplate=None)
+            
+        px_add_trace_data(fig, trace)
+
+        return self
+
+    def add_sp_polygons(self,
+                       sp_polygons,
+                       color_value = None,
+                       line_color = None,
+                       line_width = None,
+                       line_dash = None,
+                       legend_name = None,
+                       hover_skip = False,
+                       update_crs = True,
+                       **kwargs):
+        fig = self.fig
+
+        if update_crs:
+            if sp_polygons.crs.to_epsg() != Options_epsg.wgs84.value:
+                sp_polygons = sp_polygons.to_crs(Options_epsg.wgs84.value)
+        if color_value is not None:
+            kwargs['color_discrete_sequence'] = [color_value, color_value]
+        trace = px.choropleth_mapbox(sp_polygons,
+                                locations=sp_polygons.index,
+                                geojson=sp_polygons.geometry,
+                                **kwargs)
+        if line_color is not None:
+            trace = trace\
+                .update_traces(marker=dict(line=dict(color=line_color)))
+        if line_width is not None:
+            trace = trace\
+                .update_traces(marker=dict(line=dict(width=line_width)))
+        if line_dash is not None:
+            trace = trace\
+                .update_traces(marker=dict(line=dict(dash=line_dash)))
+        if legend_name is not None:
+            if 'color' not in kwargs:
+                trace = trace\
+                    .update_traces(name=legend_name,
+                                legendgroup=legend_name,
+                                showlegend=True)
+            else:
+                trace = trace\
+                    .update_traces(legendgroup=legend_name,
+                                legendgrouptitle_text=legend_name,
+                                showlegend=True)
+        if hover_skip:
+            trace = trace\
+                .update_traces(hoverinfo='skip',
+                            hovertemplate=None)
+            
+        px_add_trace_data(fig, trace)
+
+        return self
+
+    def add_sp_polygon_borders(self,
+                              sp_polygons,
+                              line_color = None,
+                              line_width = None,
+                              line_dash = None,
+                              legend_name = None,
+                              hover_skip = True,
+                              update_crs = True,
+                              **kwargs):
+        fig = self.fig
+
+        if update_crs:
+            if sp_polygons.crs.to_epsg() != Options_epsg.wgs84.value:
+                sp_polygons = sp_polygons.to_crs(Options_epsg.wgs84.value)
+        df_polygons_xy = sp_to_df_xy(sp_polygons, cols_keep_all=True)
+        trace = px.line_mapbox(df_polygons_xy,
+                            lon=df_polygons_xy['x'],
+                            lat=df_polygons_xy['y'],
+                            line_group=df_polygons_xy['id_geom'])
+        if line_color is not None:
+            trace = trace\
+                .update_traces(line=dict(color=line_color))
+        if line_width is not None:
+            trace = trace\
+                .update_traces(line=dict(width=line_width))
+        if line_dash is not None:
+            trace = trace\
+                .update_traces(line=dict(dash=line_dash))
+        if legend_name is not None:
+            if 'color' not in kwargs:
+                trace = trace\
+                    .update_traces(name=legend_name,
+                                legendgroup=legend_name,
+                                showlegend=True)
+            else:
+                trace = trace\
+                    .update_traces(legendgroup=legend_name,
+                                legendgrouptitle_text=legend_name,
+                                showlegend=True)
+        if 'color' not in kwargs:
+            for i in range(len(trace.data)):
+                if i == 0:
+                    trace.data[i].showlegend = True
+                else:
+                    trace.data[i].showlegend = False
+        if hover_skip:
+            trace = trace\
+                .update_traces(hoverinfo='skip',
+                            hovertemplate=None)
+            
+        px_add_trace_data(fig, trace)
+
+        return self
+
 #endregion -----------------------------------------------------------------------------------------
 #region Functions: Others
 
 #%%
 def sp_explode(sp: gpd.GeoDataFrame) -> gpd.GeoDataFrame:
     '''Explodes geodataframe.
```

### Comparing `dsplus-0.4.3/dsplus.egg-info/PKG-INFO` & `dsplus-0.4.4/dsplus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsplus
-Version: 0.4.3
+Version: 0.4.4
 Summary: Helper functions for data science applications.
 Author: Prashana Bajracharya
 Author-email: pajracharya713@gmail.com
 Keywords: data science,pandas
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dsplus-0.4.3/setup.py` & `dsplus-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.3/tests/Test_pandas.py` & `dsplus-0.4.4/tests/Test_pandas.py`

 * *Files identical despite different names*

