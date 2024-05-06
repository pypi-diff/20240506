# Comparing `tmp/dsplus-0.4.4.tar.gz` & `tmp/dsplus-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsplus-0.4.4.tar", last modified: Sun May  5 18:15:46 2024, max compression
+gzip compressed data, was "dsplus-0.4.5.tar", last modified: Mon May  6 02:20:33 2024, max compression
```

## Comparing `dsplus-0.4.4.tar` & `dsplus-0.4.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 18:15:46.569019 dsplus-0.4.4/
--rw-rw-rw-   0        0        0     1083 2024-03-15 02:57:42.000000 dsplus-0.4.4/LICENSE
--rw-rw-rw-   0        0        0      690 2024-05-05 18:15:46.563417 dsplus-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0       99 2024-02-24 21:14:11.000000 dsplus-0.4.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 18:15:46.545257 dsplus-0.4.4/dsplus/
--rw-rw-rw-   0        0        0      171 2024-05-05 18:15:24.000000 dsplus-0.4.4/dsplus/__init__.py
--rw-rw-rw-   0        0        0    24324 2024-05-02 23:18:42.000000 dsplus-0.4.4/dsplus/pb_functions_general.py
--rw-rw-rw-   0        0        0    42785 2024-05-02 23:18:42.000000 dsplus-0.4.4/dsplus/pb_functions_pandas.py
--rw-rw-rw-   0        0        0    56894 2024-04-02 22:58:04.000000 dsplus-0.4.4/dsplus/pb_functions_plotly.py
--rw-rw-rw-   0        0        0    58862 2024-05-05 17:55:16.000000 dsplus-0.4.4/dsplus/pb_functions_spatial.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:15:46.557330 dsplus-0.4.4/dsplus.egg-info/
--rw-rw-rw-   0        0        0      690 2024-05-05 18:15:46.000000 dsplus-0.4.4/dsplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-05-05 18:15:46.000000 dsplus-0.4.4/dsplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 18:15:46.000000 dsplus-0.4.4/dsplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-05 18:15:46.000000 dsplus-0.4.4/dsplus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 18:15:46.569019 dsplus-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0     1650 2024-03-29 02:13:48.000000 dsplus-0.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 18:15:46.557330 dsplus-0.4.4/tests/
--rw-rw-rw-   0        0        0    12530 2024-04-17 03:55:44.000000 dsplus-0.4.4/tests/Test_pandas.py
+drwxrwxrwx   0        0        0        0 2024-05-06 02:20:33.500525 dsplus-0.4.5/
+-rw-rw-rw-   0        0        0     1083 2024-03-15 02:57:42.000000 dsplus-0.4.5/LICENSE
+-rw-rw-rw-   0        0        0      690 2024-05-06 02:20:33.497803 dsplus-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0       99 2024-02-24 21:14:11.000000 dsplus-0.4.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 02:20:33.478319 dsplus-0.4.5/dsplus/
+-rw-rw-rw-   0        0        0      171 2024-05-06 02:20:02.000000 dsplus-0.4.5/dsplus/__init__.py
+-rw-rw-rw-   0        0        0    24324 2024-05-06 02:08:36.000000 dsplus-0.4.5/dsplus/pb_functions_general.py
+-rw-rw-rw-   0        0        0    42785 2024-05-02 23:18:42.000000 dsplus-0.4.5/dsplus/pb_functions_pandas.py
+-rw-rw-rw-   0        0        0    56900 2024-05-06 00:51:26.000000 dsplus-0.4.5/dsplus/pb_functions_plotly.py
+-rw-rw-rw-   0        0        0    59604 2024-05-06 02:18:16.000000 dsplus-0.4.5/dsplus/pb_functions_spatial.py
+drwxrwxrwx   0        0        0        0 2024-05-06 02:20:33.490027 dsplus-0.4.5/dsplus.egg-info/
+-rw-rw-rw-   0        0        0      690 2024-05-06 02:20:33.000000 dsplus-0.4.5/dsplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-05-06 02:20:33.000000 dsplus-0.4.5/dsplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 02:20:33.000000 dsplus-0.4.5/dsplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-06 02:20:33.000000 dsplus-0.4.5/dsplus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 02:20:33.501532 dsplus-0.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     1650 2024-03-29 02:13:48.000000 dsplus-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 02:20:33.492812 dsplus-0.4.5/tests/
+-rw-rw-rw-   0        0        0    12530 2024-04-17 03:55:44.000000 dsplus-0.4.5/tests/Test_pandas.py
```

### Comparing `dsplus-0.4.4/LICENSE` & `dsplus-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.4/PKG-INFO` & `dsplus-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsplus
-Version: 0.4.4
+Version: 0.4.5
 Summary: Helper functions for data science applications.
 Author: Prashana Bajracharya
 Author-email: pajracharya713@gmail.com
 Keywords: data science,pandas
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dsplus-0.4.4/dsplus/pb_functions_general.py` & `dsplus-0.4.5/dsplus/pb_functions_general.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.4/dsplus/pb_functions_pandas.py` & `dsplus-0.4.5/dsplus/pb_functions_pandas.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.4/dsplus/pb_functions_plotly.py` & `dsplus-0.4.5/dsplus/pb_functions_plotly.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,15 @@
 
     def _update_legend_show(self, trace, legend_show, legend_name):
         if legend_show is not None:
             trace.update_traces(showlegend=legend_show)
         if legend_name is not None:
             trace.update_traces(name=legend_name)
 
-    def dec_add(marginal='xy'):
+    def _dec_add(marginal='xy'):
         '''Decorator to make the following updates:
             - Dataframe, x, and y arguments
             - Log scale arguments
             - Category order arguments
             - Facet arguments
             - Marginal arguemnts
             - Hover arguemnts
@@ -345,15 +345,15 @@
         fig = self.fig
 
         fig = px_add_trace_data(fig, trace)
 
         self.fig=fig
         return self
 
-    @dec_add(marginal='xy')
+    @_dec_add(marginal='xy')
     def add_scatter(self,
                     df: pd.DataFrame = None,
                     x = None,
                     y = None,
                     color = None,
                     size = None,
                     symbol = None,
@@ -410,15 +410,15 @@
         if opacity_value is not None:
             trace.update_traces(marker_opacity=opacity_value)
         if hover_template is not None:
             trace.update_traces(hovertemplate=hover_template)
 
         return trace
 
-    @dec_add(marginal='')
+    @_dec_add(marginal='')
     def add_line(self,
                  df: pd.DataFrame = None,
                  x = None,
                  y = None,
                  color = None,
                  dash = None,
                  color_value = None,
@@ -464,15 +464,15 @@
         if dash_value is not None:
             trace.update_traces(line_dash=dash_value)
         if hover_template is not None:
             trace.update_traces(hovertemplate=hover_template)
 
         return trace
 
-    @dec_add(marginal='')
+    @_dec_add(marginal='')
     def add_bar(self,
                  df: pd.DataFrame = None,
                  x = None,
                  y = None,
                  color = None,
                  pattern = None,
                  color_value = None,
@@ -527,15 +527,15 @@
         if opacity_value is not None:
             trace.update_traces(marker_opacity=opacity_value)
         if hover_template is not None:
             trace.update_traces(hovertemplate=hover_template)
 
         return trace
 
-    @dec_add(marginal='x')
+    @_dec_add(marginal='x')
     def add_histogram(self,
                       df: pd.DataFrame = None,
                       x = None,
                       y = None,
                       color = None,
                       shape = None,
                       color_value = None,
@@ -598,15 +598,15 @@
         if opacity_value is not None:
             trace.update_traces(marker_opacity=opacity_value)
         if hover_template is not None:
             trace.update_traces(hovertemplate=hover_template)
 
         return trace
 
-    @dec_add(marginal='xy')
+    @_dec_add(marginal='xy')
     def add_heatmap(self,
                     df: pd.DataFrame = None,
                     x = None,
                     y = None,
                     z = None,
                     opacity_value = None,
                     aes_color_continuous_scale = None,
```

### Comparing `dsplus-0.4.4/dsplus/pb_functions_spatial.py` & `dsplus-0.4.5/dsplus/pb_functions_spatial.py`

 * *Files 5% similar despite different names*

```diff
@@ -866,218 +866,262 @@
                 ],
             )
         else:
             fig.update_layout(mapbox_style=basemap)
 
         return self
         
+    def _dec_add_sp(hover_skip=False):
+        def inner(func):
+            def wrapper(self, *args, **kwargs):
+                if 'update_crs' in kwargs:
+                    update_crs = kwargs['update_crs']
+                else:
+                    update_crs = True
+                
+                if update_crs:
+                    if 'sp' in kwargs:
+                        sp = kwargs['sp']
+                    elif len(args) > 0:
+                        sp = args[0]
+
+                    if sp.crs.to_epsg() != Options_epsg.wgs84.value:
+                        sp = sp.to_crs(Options_epsg.wgs84.value)
+
+                    args = ()
+                    kwargs['sp'] = sp
+                
+                trace = func(self, *args, **kwargs)
+
+                if 'hover_skip' in kwargs:
+                    hover_skip_check = kwargs['hover_skip']
+                else:
+                    hover_skip_check = hover_skip
+
+                if hover_skip_check:
+                    trace = \
+                    (trace
+                        .update_traces(hoverinfo='skip',
+                                       hovertemplate=None)
+                    )                
+
+                self.add(trace)
+
+                return self
+            return wrapper
+        return inner
+    
+    @_dec_add_sp(hover_skip=False)
     def add_sp_points(self,
-                      sp_points,
+                      sp,
                       color_value = None,
                       size_value = None,
                       symbol_value = None,
+                      *,
                       legend_name = None,
                       hover_skip = False,
                       update_crs = True,
-                      **kwargs):
-        fig = self.fig
-
-        if update_crs:
-            if sp_points.crs.to_epsg() != Options_epsg.wgs84.value:
-                sp_points = sp_points.to_crs(Options_epsg.wgs84.value)
-        trace = px.scatter_mapbox(sp_points,
-                                lon=sp_points.geometry.x,
-                                lat=sp_points.geometry.y,
-                                **kwargs)
+                      **kwargs) -> Self:
+        trace = px.scatter_mapbox(sp,
+                                  lon=sp.geometry.x,
+                                  lat=sp.geometry.y,
+                                  **kwargs)
         if color_value is not None:
-            trace = trace\
+            trace = \
+            (trace
                 .update_traces(marker=dict(color=color_value))
+            )
         if size_value is not None:
-            trace = trace\
+            trace = \
+            (trace
                 .update_traces(marker=dict(size=size_value))
+            )
         if symbol_value is not None:
-            trace = trace\
+            trace = \
+            (trace
                 .update_traces(marker=dict(symbol=symbol_value))
+            )
         if legend_name is not None:
             if ('color' not in kwargs) and ('size' not in kwargs):
-                trace = trace\
+                trace = \
+                (trace
                     .update_traces(name=legend_name,
                                    showlegend=True)
+                )
             else:
-                trace = trace\
+                trace = \
+                (trace
                     .update_traces(legendgroup=legend_name,
                                    legendgrouptitle_text=legend_name,
                                    showlegend=True)
-        if hover_skip:
-            trace = trace\
-                .update_traces(hoverinfo='skip',
-                               hovertemplate=None)
+                )
             
-        px_add_trace_data(fig, trace)
-
-        return self
+        return trace
     
+    @_dec_add_sp(hover_skip=False)
     def add_sp_polylines(self,
-                        sp_lines,
-                        color_value = None,
-                        width_value = None,
-                        dash_value = None,
-                        legend_name = None,
-                        hover_skip = False,
-                        update_crs = True,
-                        **kwargs):
-        fig = self.fig
-
-        if update_crs:
-            if sp_lines.crs.to_epsg() != Options_epsg.wgs84.value:
-                sp_lines = sp_lines.to_crs(Options_epsg.wgs84.value)
-        df_lines_xy = sp_to_df_xy(sp_lines, cols_keep_all=True)
+                         sp,
+                         color_value = None,
+                         width_value = None,
+                         dash_value = None,
+                         *,
+                         legend_name = None,
+                         hover_skip = False,
+                         update_crs = True,
+                         **kwargs) -> Self:
+        df_lines_xy = sp_to_df_xy(sp, cols_keep_all=True)
         trace = px.line_mapbox(df_lines_xy,
-                            lon=df_lines_xy['x'],
-                            lat=df_lines_xy['y'],
-                            line_group=df_lines_xy['id_geom'],
-                            **kwargs)
+                               lon=df_lines_xy['x'],
+                               lat=df_lines_xy['y'],
+                               line_group=df_lines_xy['id_geom'],
+                               **kwargs)
         if color_value is not None:
-            trace = trace\
+            trace = \
+            (trace
                 .update_traces(line=dict(color=color_value))
+            )
         if width_value is not None:
-            trace = trace\
+            trace = \
+            (trace
                 .update_traces(line=dict(width=width_value))
+            )
         if dash_value is not None:
-            trace = trace\
+            trace = \
+            (trace
                 .update_traces(line=dict(dash=dash_value))
+            )
         if legend_name is not None:
             if 'color' not in kwargs:
-                trace = trace\
+                trace = \
+                (trace
                     .update_traces(name=legend_name,
-                                legendgroup=legend_name,
-                                showlegend=True)
+                                   legendgroup=legend_name,
+                                   showlegend=True)
+                )
             else:
-                trace = trace\
+                trace = \
+                (trace
                     .update_traces(legendgroup=legend_name,
-                                legendgrouptitle_text=legend_name,
-                                showlegend=True)
+                                   legendgrouptitle_text=legend_name,
+                                   showlegend=True)
+                )
         if 'color' not in kwargs:
             for i in range(len(trace.data)):
                 if i == 0:
                     trace.data[i].showlegend = True
                 else:
                     trace.data[i].showlegend = False
-        if hover_skip:
-            trace = trace\
-                .update_traces(hoverinfo='skip',
-                            hovertemplate=None)
             
-        px_add_trace_data(fig, trace)
-
-        return self
+        return trace
 
+    @_dec_add_sp(hover_skip=False)
     def add_sp_polygons(self,
-                       sp_polygons,
-                       color_value = None,
-                       line_color = None,
-                       line_width = None,
-                       line_dash = None,
-                       legend_name = None,
-                       hover_skip = False,
-                       update_crs = True,
-                       **kwargs):
-        fig = self.fig
-
-        if update_crs:
-            if sp_polygons.crs.to_epsg() != Options_epsg.wgs84.value:
-                sp_polygons = sp_polygons.to_crs(Options_epsg.wgs84.value)
+                        sp,
+                        color_value = None,
+                        line_color = None,
+                        line_width = None,
+                        line_dash = None,
+                        *,
+                        legend_name = None,
+                        hover_skip = False,
+                        update_crs = True,
+                        **kwargs) -> Self:
         if color_value is not None:
             kwargs['color_discrete_sequence'] = [color_value, color_value]
-        trace = px.choropleth_mapbox(sp_polygons,
-                                locations=sp_polygons.index,
-                                geojson=sp_polygons.geometry,
-                                **kwargs)
+        trace = px.choropleth_mapbox(sp,
+                                     locations=sp.index,
+                                     geojson=sp.geometry,
+                                     **kwargs)
         if line_color is not None:
-            trace = trace\
+            trace = \
+            (trace
                 .update_traces(marker=dict(line=dict(color=line_color)))
+            )
         if line_width is not None:
-            trace = trace\
+            trace = \
+            (trace
                 .update_traces(marker=dict(line=dict(width=line_width)))
+            )
         if line_dash is not None:
-            trace = trace\
+            trace = \
+            (trace
                 .update_traces(marker=dict(line=dict(dash=line_dash)))
+            )
         if legend_name is not None:
             if 'color' not in kwargs:
-                trace = trace\
+                trace = \
+                (trace
                     .update_traces(name=legend_name,
-                                legendgroup=legend_name,
-                                showlegend=True)
+                                   legendgroup=legend_name,
+                                   showlegend=True)
+                )
             else:
-                trace = trace\
+                trace = \
+                (trace
                     .update_traces(legendgroup=legend_name,
-                                legendgrouptitle_text=legend_name,
-                                showlegend=True)
-        if hover_skip:
-            trace = trace\
-                .update_traces(hoverinfo='skip',
-                            hovertemplate=None)
+                                   legendgrouptitle_text=legend_name,
+                                   showlegend=True)
+                )
             
-        px_add_trace_data(fig, trace)
-
-        return self
+        return trace
 
+    @_dec_add_sp(hover_skip=True)
     def add_sp_polygon_borders(self,
-                              sp_polygons,
-                              line_color = None,
-                              line_width = None,
-                              line_dash = None,
-                              legend_name = None,
-                              hover_skip = True,
-                              update_crs = True,
-                              **kwargs):
-        fig = self.fig
-
-        if update_crs:
-            if sp_polygons.crs.to_epsg() != Options_epsg.wgs84.value:
-                sp_polygons = sp_polygons.to_crs(Options_epsg.wgs84.value)
-        df_polygons_xy = sp_to_df_xy(sp_polygons, cols_keep_all=True)
+                               sp,
+                               line_color = None,
+                               line_width = None,
+                               line_dash = None,
+                               *,
+                               legend_name = None,
+                               hover_skip = True,
+                               update_crs = True,
+                               **kwargs) -> Self:
+        df_polygons_xy = sp_to_df_xy(sp, cols_keep_all=True)
         trace = px.line_mapbox(df_polygons_xy,
-                            lon=df_polygons_xy['x'],
-                            lat=df_polygons_xy['y'],
-                            line_group=df_polygons_xy['id_geom'])
+                               lon=df_polygons_xy['x'],
+                               lat=df_polygons_xy['y'],
+                               line_group=df_polygons_xy['id_geom'])
         if line_color is not None:
-            trace = trace\
+            trace = \
+            (trace
                 .update_traces(line=dict(color=line_color))
+            )
         if line_width is not None:
-            trace = trace\
+            trace = \
+            (trace
                 .update_traces(line=dict(width=line_width))
+            )
         if line_dash is not None:
-            trace = trace\
+            trace = \
+            (trace
                 .update_traces(line=dict(dash=line_dash))
+            )
         if legend_name is not None:
             if 'color' not in kwargs:
-                trace = trace\
+                trace = \
+                (trace
                     .update_traces(name=legend_name,
-                                legendgroup=legend_name,
-                                showlegend=True)
+                                   legendgroup=legend_name,
+                                   showlegend=True)
+                )
             else:
-                trace = trace\
+                trace = \
+                (trace
                     .update_traces(legendgroup=legend_name,
-                                legendgrouptitle_text=legend_name,
-                                showlegend=True)
+                                   legendgrouptitle_text=legend_name,
+                                   showlegend=True)
+                )
         if 'color' not in kwargs:
             for i in range(len(trace.data)):
                 if i == 0:
                     trace.data[i].showlegend = True
                 else:
                     trace.data[i].showlegend = False
-        if hover_skip:
-            trace = trace\
-                .update_traces(hoverinfo='skip',
-                            hovertemplate=None)
-            
-        px_add_trace_data(fig, trace)
 
-        return self
+        return trace
 
 #endregion -----------------------------------------------------------------------------------------
 #region Functions: Others
 
 #%%
 def sp_explode(sp: gpd.GeoDataFrame) -> gpd.GeoDataFrame:
     '''Explodes geodataframe.
```

### Comparing `dsplus-0.4.4/dsplus.egg-info/PKG-INFO` & `dsplus-0.4.5/dsplus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsplus
-Version: 0.4.4
+Version: 0.4.5
 Summary: Helper functions for data science applications.
 Author: Prashana Bajracharya
 Author-email: pajracharya713@gmail.com
 Keywords: data science,pandas
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `dsplus-0.4.4/setup.py` & `dsplus-0.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `dsplus-0.4.4/tests/Test_pandas.py` & `dsplus-0.4.5/tests/Test_pandas.py`

 * *Files identical despite different names*

