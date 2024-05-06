# Comparing `tmp/datamapplot-0.2.2.tar.gz` & `tmp/datamapplot-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamapplot-0.2.2.tar", last modified: Sat Mar  2 01:34:38 2024, max compression
+gzip compressed data, was "datamapplot-0.3.0.tar", last modified: Mon May  6 02:41:10 2024, max compression
```

## Comparing `datamapplot-0.2.2.tar` & `datamapplot-0.3.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-02 01:34:38.134578 datamapplot-0.2.2/
--rw-r--r--   0 vsts      (1001) docker     (127)     1102 2024-03-02 01:33:42.000000 datamapplot-0.2.2/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)     5414 2024-03-02 01:34:38.134578 datamapplot-0.2.2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     4716 2024-03-02 01:33:42.000000 datamapplot-0.2.2/README.rst
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-02 01:34:38.130577 datamapplot-0.2.2/datamapplot/
--rw-r--r--   0 vsts      (1001) docker     (127)      432 2024-03-02 01:33:42.000000 datamapplot-0.2.2/datamapplot/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2753 2024-03-02 01:33:42.000000 datamapplot-0.2.2/datamapplot/alpha_shapes.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23480 2024-03-02 01:33:42.000000 datamapplot-0.2.2/datamapplot/create_plots.py
--rw-r--r--   0 vsts      (1001) docker     (127)    36111 2024-03-02 01:33:42.000000 datamapplot-0.2.2/datamapplot/interactive_rendering.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3069 2024-03-02 01:33:42.000000 datamapplot-0.2.2/datamapplot/medoids.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5189 2024-03-02 01:33:42.000000 datamapplot-0.2.2/datamapplot/overlap_computations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9263 2024-03-02 01:33:42.000000 datamapplot-0.2.2/datamapplot/palette_handling.py
--rw-r--r--   0 vsts      (1001) docker     (127)    23030 2024-03-02 01:33:42.000000 datamapplot-0.2.2/datamapplot/plot_rendering.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11856 2024-03-02 01:33:42.000000 datamapplot-0.2.2/datamapplot/text_placement.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-02 01:34:38.130577 datamapplot-0.2.2/datamapplot.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     5414 2024-03-02 01:34:38.000000 datamapplot-0.2.2/datamapplot.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      513 2024-03-02 01:34:38.000000 datamapplot-0.2.2/datamapplot.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-02 01:34:38.000000 datamapplot-0.2.2/datamapplot.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-02 01:34:35.000000 datamapplot-0.2.2/datamapplot.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      141 2024-03-02 01:34:38.000000 datamapplot-0.2.2/datamapplot.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       12 2024-03-02 01:34:38.000000 datamapplot-0.2.2/datamapplot.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      958 2024-03-02 01:34:38.134578 datamapplot-0.2.2/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)       69 2024-03-02 01:33:44.000000 datamapplot-0.2.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 02:41:10.810577 datamapplot-0.3.0/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1102 2024-05-06 02:40:16.000000 datamapplot-0.3.0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)     5612 2024-05-06 02:41:10.810577 datamapplot-0.3.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     4914 2024-05-06 02:40:16.000000 datamapplot-0.3.0/README.rst
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 02:41:10.810577 datamapplot-0.3.0/datamapplot/
+-rw-r--r--   0 vsts      (1001) docker     (127)      432 2024-05-06 02:40:16.000000 datamapplot-0.3.0/datamapplot/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2753 2024-05-06 02:40:16.000000 datamapplot-0.3.0/datamapplot/alpha_shapes.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    23591 2024-05-06 02:40:16.000000 datamapplot-0.3.0/datamapplot/create_plots.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    37970 2024-05-06 02:40:16.000000 datamapplot-0.3.0/datamapplot/interactive_rendering.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3069 2024-05-06 02:40:16.000000 datamapplot-0.3.0/datamapplot/medoids.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5189 2024-05-06 02:40:16.000000 datamapplot-0.3.0/datamapplot/overlap_computations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9343 2024-05-06 02:40:16.000000 datamapplot-0.3.0/datamapplot/palette_handling.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    31940 2024-05-06 02:40:16.000000 datamapplot-0.3.0/datamapplot/plot_rendering.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16185 2024-05-06 02:40:16.000000 datamapplot-0.3.0/datamapplot/text_placement.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-06 02:41:10.810577 datamapplot-0.3.0/datamapplot.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5612 2024-05-06 02:41:10.000000 datamapplot-0.3.0/datamapplot.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      513 2024-05-06 02:41:10.000000 datamapplot-0.3.0/datamapplot.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-06 02:41:10.000000 datamapplot-0.3.0/datamapplot.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-06 02:41:08.000000 datamapplot-0.3.0/datamapplot.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      155 2024-05-06 02:41:10.000000 datamapplot-0.3.0/datamapplot.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       12 2024-05-06 02:41:10.000000 datamapplot-0.3.0/datamapplot.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      973 2024-05-06 02:41:10.810577 datamapplot-0.3.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)       69 2024-05-06 02:40:18.000000 datamapplot-0.3.0/setup.py
```

### Comparing `datamapplot-0.2.2/LICENSE` & `datamapplot-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datamapplot-0.2.2/PKG-INFO` & `datamapplot-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamapplot
-Version: 0.2.2
+Version: 0.3.0
 Summary: A library for presentation and publication ready plots of data maps
 Home-page: https://github.com/TutteInstitute/datamapplot
 Author: Leland McInnes
 Author-email: leland.mcinnes@gmail.com
 Maintainer: Leland McInnes
 Maintainer-email: leland.mcinnes@gmail.com
 License: MIT License
@@ -51,14 +51,21 @@
 Using darkmode and some custom font choices:
 
 .. image:: examples/plot_arxiv_ml.png
    :width: 1024
    :alt: A data map plot of papers from ArXiv ML
    :align: center
 
+With labels over points in a word-cloud style:
+
+.. image:: examples/plot_arxiv_ml_word_cloud.png
+   :width: 1024
+   :alt: A word cloud style data map plot of papers from ArXiv ML
+   :align: center
+
 Alternative custom styling:
 
 .. image:: examples/plot_wikipedia.png
    :width: 1024
    :alt: A data map plot of Simple Wikipedia
    :align: center
```

### Comparing `datamapplot-0.2.2/README.rst` & `datamapplot-0.3.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,21 @@
 Using darkmode and some custom font choices:
 
 .. image:: examples/plot_arxiv_ml.png
    :width: 1024
    :alt: A data map plot of papers from ArXiv ML
    :align: center
 
+With labels over points in a word-cloud style:
+
+.. image:: examples/plot_arxiv_ml_word_cloud.png
+   :width: 1024
+   :alt: A word cloud style data map plot of papers from ArXiv ML
+   :align: center
+
 Alternative custom styling:
 
 .. image:: examples/plot_wikipedia.png
    :width: 1024
    :alt: A data map plot of Simple Wikipedia
    :align: center
```

### Comparing `datamapplot-0.2.2/datamapplot/alpha_shapes.py` & `datamapplot-0.3.0/datamapplot/alpha_shapes.py`

 * *Files identical despite different names*

### Comparing `datamapplot-0.2.2/datamapplot/create_plots.py` & `datamapplot-0.3.0/datamapplot/create_plots.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     dynamic_label_size=False,
     dpi=plt.rcParams["figure.dpi"],
     force_matplotlib=False,
     darkmode=False,
     highlight_labels=None,
     palette_hue_shift=0.0,
     palette_hue_radius_dependence=1.0,
+    palette_min_lightness=10,
     use_medoids=False,
     cmap=None,
     marker_color_array=None,
     **render_plot_kwds,
 ):
     """Create a static plot from ``data_map_coords`` with text labels provided by ``labels``.
     This is the primary function for DataMapPlot and provides the easiest interface to the
@@ -76,21 +77,25 @@
         The string used in the ``labels`` array to identify the unlabelled or noise points
         in the dataset.
 
     noise_color: str (optional, default="#999999")
         The colour to use for unlabelled or noise points in the data map. This should usually
         be a muted or neutral colour to distinguish background points from the labelled clusters.
 
-    color_label_text: bool (optional, default=True)
+    color_label_text: str or bool (optional, default=True)
         Whether to use colours for the text labels generated in the plot. If ``False`` then
         the text labels will default to either black or white depending on ``darkmode``.
+        If a string is provided it should be a valid matplotlib colour specification and all
+        text labels will be this colour.
 
-    color_label_arrows: bool (optional, default=True)
+    color_label_arrows: str or bool (optional, default=True)
         Whether to use colours for the arrows between the text labels and clusters. If ``False``
-        then the arrows will default to either black or white depending on ``darkmode``.
+        then the arrows will default to either black or white depending on ``darkmode``. If a 
+        string is provided it should eb a valid matplotlib colour specification and all arrows
+        will be this colour.
 
     label_wrap_width: int (optional, default=16)
         The number of characters to apply text-wrapping at when creating text labels for
         display in the plot. Note that long words will not be broken, so you can choose
         relatively small values if you want tight text-wrapping.
 
     label_color_map: dict or None (optional, default=None)
@@ -193,21 +198,23 @@
     if label_color_map is None:
         if cmap is None:
             palette = palette_from_datamap(
                 data_map_coords,
                 label_locations,
                 hue_shift=palette_hue_shift,
                 radius_weight_power=palette_hue_radius_dependence,
+                min_lightness=palette_min_lightness,
             )
         else:
             palette = palette_from_cmap_and_datamap(
                 cmap,
                 data_map_coords,
                 label_locations,
                 radius_weight_power=palette_hue_radius_dependence,
+                lightness_bounds=(palette_min_lightness, 80),
             )
         label_to_index_map = {
             name: index for index, name in enumerate(unique_non_noise_labels)
         }
         color_list = [
             palette[label_to_index_map[x]] if x in label_to_index_map else noise_color
             for x in cluster_label_vector
@@ -227,42 +234,36 @@
         ]
 
     if marker_color_array is not None:
         color_list = list(marker_color_array)
 
     label_colors = [label_color_map[x] for x in unique_non_noise_labels]
 
-    if color_label_text and len(label_colors) > 0:
+    if type(color_label_text) == str:
+        label_text_colors = color_label_text
+    elif color_label_text and len(label_colors) > 0:
         # Darken and reduce chroma of label colors to get text labels
         if darkmode:
             label_text_colors = pastel_palette(label_colors)
         else:
             label_text_colors = deep_palette(label_colors)
     else:
         label_text_colors = None
 
-    if color_label_arrows:
+    if type(color_label_arrows) == str:
+        label_arrow_colors = color_label_arrows
+    elif color_label_arrows:
         label_arrow_colors = label_colors
     else:
         label_arrow_colors = None
 
-    if dynamic_label_size:
-        font_scale_factor = np.sqrt(figsize[0] * figsize[1])
-        cluster_sizes = np.sqrt(pd.Series(cluster_label_vector).value_counts())
-        label_size_adjustments = cluster_sizes - cluster_sizes.min()
-        label_size_adjustments /= label_size_adjustments.max()
-        label_size_adjustments *= (
-            render_plot_kwds.get("label_font_size", font_scale_factor) + 2
-        )
-        label_size_adjustments = dict(label_size_adjustments - 2)
-        label_size_adjustments = [
-            label_size_adjustments[x] for x in unique_non_noise_labels
-        ]
-    else:
-        label_size_adjustments = [0.0] * len(unique_non_noise_labels)
+    cluster_sizes = pd.Series(cluster_label_vector).value_counts()
+    label_cluster_sizes = np.asarray([
+            cluster_sizes[x] for x in unique_non_noise_labels
+    ])
 
     # Heuristics for point size and alpha values
     n_points = data_map_coords.shape[0]
     if data_map_coords.shape[0] < 100_000 or force_matplotlib:
         magic_number = np.clip(128 * 4 ** (-np.log10(n_points)), 0.05, 64)
         point_scale_factor = np.sqrt(figsize[0] * figsize[1])
         point_size = magic_number * (point_scale_factor / 2)
@@ -278,24 +279,25 @@
         alpha = render_plot_kwds.pop("alpha")
 
     fig, ax = render_plot(
         data_map_coords,
         color_list,
         label_text,
         label_locations,
+        label_cluster_sizes,
         title=title,
         sub_title=sub_title,
         point_size=point_size,
         alpha=alpha,
         label_text_colors=None if not color_label_text else label_text_colors,
         label_arrow_colors=None if not color_label_arrows else label_arrow_colors,
         highlight_colors=[label_color_map[x] for x in unique_non_noise_labels],
         figsize=figsize,
         noise_color=noise_color,
-        label_size_adjustments=label_size_adjustments,
+        dynamic_label_size=dynamic_label_size,
         dpi=dpi,
         force_matplotlib=force_matplotlib,
         darkmode=darkmode,
         highlight_labels=highlight_labels,
         **render_plot_kwds,
     )
```

### Comparing `datamapplot-0.2.2/datamapplot/interactive_rendering.py` & `datamapplot-0.3.0/datamapplot/interactive_rendering.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,17 @@
   <head>
     <meta http-equiv="content-type" content="text/html; charset=UTF-8" />
     <title>{{title}}</title>
     {% if google_font %}
     <link rel="preconnect" href="https://fonts.googleapis.com">
     <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
     <link href="https://fonts.googleapis.com/css2?family={{google_font}}&display=swap" rel="stylesheet">
+    {% if google_tooltip_font %}
+    <link href="https://fonts.googleapis.com/css2?family={{google_tooltip_font}}&display=swap" rel="stylesheet">
+    {% endif %}
     {% endif %}
        
     <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.2.0/css/bootstrap-theme.min.css" />
     <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/font-awesome/4.6.3/css/font-awesome.min.css" />
     <script src="https://unpkg.com/deck.gl@latest/dist.min.js"></script>
     {% if inline_data %}
     <script src="https://unpkg.com/fflate@0.8.0"></script>
@@ -260,14 +263,15 @@
         outlineWidth: {{text_outline_width}},
         outlineColor: {{text_outline_color}},
         getBackgroundColor: {{text_background_color}},
         getBackgroundPadding: [15, 15, 15, 15],
         background: true,
         characterSet: "auto",
         fontFamily: "{{font_family}}",
+        fontWeight: {{font_weight}},
         lineHeight: {{line_spacing}},
         fontSettings: {"sdf": true},
         getTextAnchor: "middle",
         getAlignmentBaseline: "center",
         lineHeight: 0.95,
         elevation: 100,
         // CollideExtension options
@@ -364,14 +368,15 @@
     </script>
 </html>
 """
 
 _TOOL_TIP_CSS = """
             font-size: 0.8em;
             font-family: {{title_font_family}};
+            font-weight: {{title_font_weight}};
             color: {{title_font_color}} !important;
             background-color: {{title_background}} !important;
             border-radius: 12px;
             box-shadow: 2px 3px 10px {{shadow_color}};
             max-width: 25%;
 """
 
@@ -494,23 +499,26 @@
     label_dataframe,
     inline_data=True,
     title=None,
     sub_title=None,
     title_font_size=36,
     sub_title_font_size=18,
     text_collision_size_scale=3,
-    text_min_pixel_size=12,
+    text_min_pixel_size=18,
     text_max_pixel_size=36,
-    font_family="arial",
+    font_family="Roboto",
+    font_weight=900,
+    tooltip_font_family=None,
+    tooltip_font_weight=300,
     logo=None,
     logo_width=256,
     color_label_text=True,
     line_spacing=0.95,
-    min_fontsize=12,
-    max_fontsize=24,
+    min_fontsize=18,
+    max_fontsize=28,
     text_outline_width=8,
     text_outline_color="#eeeeeedd",
     point_hover_color="#aa0000bb",
     point_radius_min_pixels=0.01,
     point_radius_max_pixels=24,
     point_line_width_min_pixels=0.1,
     point_line_width_max_pixels=8,
@@ -577,19 +585,34 @@
         The minimum pixel size of label text. If text would be smaller than this in size
         then render the text to be at least this size.
 
     text_max_pixel_size: float (optional, default=36.0)
         The maximum pixel size of label text. If text would be larger than this in size
         then render the text to be at most this size.
 
-    font_family: str (optional, default="arial")
+    font_family: str (optional, default="Roboto")
         The font family to use for label text and titles. If the font family is a
         google font then the required google font api handling will automatically
         make the font available, so any google font family is acceptable.
 
+    font_weight: str or int (optional, default=900)
+        The font weight to use for the text labels within the plot. Either weight
+        specification such as "thin", "normal", or "bold" or an integer value
+        between 0 (ultra-thin) and 1000 (ultra-black).
+
+    tooltip_font_family: str (optional default="Roboto")
+        The font family to use in tooltips/hover text. If the font family is a
+        google font then the required google font api handling will automatically
+        make the font available, so any google font family is acceptable.
+
+    tooltip_font_weight: str or int (optional, default=400)
+        The font weight to use for the tooltip /hover text within the plot. Either weight
+        specification such as "thin", "normal", or "bold" or an integer value
+        between 0 (ultra-thin) and 1000 (ultra-black).
+
     logo: str or None (optional, default=None)
         A logo image to include in the bottom right corner of the map. This should be
         a URL to the image.
 
     logo_width: int (optional, default=256)
         The width, in pixels, of the logo to be included in the bottom right corner.
         The logo will retain it's aspect ratio, so choose the width accordingly.
@@ -715,15 +738,15 @@
     -------
     interactive_plot: InteractiveFigure
         An interactive figure with hover, pan, and zoom. This will display natively
         in a notebook, and can be saved to an HTML file via the `save` method.
     """
     # Compute point scaling
     n_points = point_dataframe.shape[0]
-    magic_number = np.clip(32 * 4 ** (-np.log10(n_points)), 0.005, 4)
+    magic_number = np.clip(32 * 4 ** (-np.log10(n_points)), 0.005, 0.1)
     if "size" not in point_dataframe.columns:
         point_size = magic_number
     else:
         point_dataframe["size"] = magic_number * (
             point_dataframe["size"] / point_dataframe["size"].median()
         )
         point_size = -1
@@ -791,28 +814,28 @@
                     + hover_text_html_template.format_map(replacements)
                     + "`} : null"
                 )
             else:
                 get_tooltip = "({index}) => hoverData.data.hover_text[index]"
 
             if on_click is not None:
-                on_click = "({index}, event) => " + on_click.format_map(replacements)
+                on_click = "({index, picked}, event) => { if (picked) {" + on_click.format_map(replacements) + " } }"
         else:
             hover_data = point_dataframe[["hover_text"]]
             get_tooltip = "({index}) => hoverData.data.hover_text[index]"
 
             replacements = FormattingDict(
                 **{
                     str(name): f"${{hoverData.data.{name}[index]}}"
                     for name in hover_data.columns
                 }
             )
 
             if on_click is not None:
-                on_click = "({index}, event) => " + on_click.format_map(replacements)
+                on_click = "({index, picked}, event) => { if (picked) {" + on_click.format_map(replacements) + " } }"
     elif extra_point_data is not None:
         hover_data = extra_point_data
         replacements = FormattingDict(
             **{
                 str(name): f"${{hoverData.data.{name}[index]}}"
                 for name in hover_data.columns
             }
@@ -821,14 +844,17 @@
             get_tooltip = (
                 '({index, picked}) => picked ? {"html": `'
                 + hover_text_html_template.format_map(replacements)
                 + "`} : null"
             )
         else:
             get_tooltip = "null"
+
+        if on_click is not None:
+            on_click = "({index, picked}, event) => { if (picked) {" + on_click.format_map(replacements) + " } }"
     else:
         hover_data = pd.DataFrame(columns=("hover_text",))
         get_tooltip = "null"
 
     if inline_data:
         buffer = io.BytesIO()
         point_data.to_feather(buffer, compression="uncompressed")
@@ -872,35 +898,44 @@
     shadow_color = "#aaaaaa44" if not darkmode else "#00000044"
     input_background = "#ffffffdd" if not darkmode else "#000000dd"
     input_border = "#ddddddff" if not darkmode else "222222ff"
 
     if tooltip_css is None:
         tooltip_css_template = jinja2.Template(_TOOL_TIP_CSS)
         tooltip_css = tooltip_css_template.render(
-            title_font_family=font_family,
+            title_font_family=tooltip_font_family or font_family,
             title_font_color=title_font_color,
+            title_font_weight=tooltip_font_weight,
             title_background=title_background,
             shadow_color=shadow_color,
         )
 
     if background_color is None:
         page_background_color = "#ffffff" if not darkmode else "#000000"
     else:
         page_background_color = background_color
 
     template = jinja2.Template(_DECKGL_TEMPLATE_STR)
     api_fontname = font_family.replace(" ", "+")
     resp = requests.get(f"https://fonts.googleapis.com/css?family={api_fontname}")
     if not resp.ok:
         api_fontname = None
+    if tooltip_font_family is not None:
+        api_tooltip_fontname = tooltip_font_family.replace(" ", "+")
+        resp = requests.get(f"https://fonts.googleapis.com/css?family={api_tooltip_fontname}")
+        if not resp.ok:
+            api_tooltip_fontname = None
+    else:
+        api_tooltip_fontname = None
 
     html_str = template.render(
         title=title if title is not None else "Interactive Data Map",
         sub_title=sub_title if sub_title is not None else "",
         google_font=api_fontname,
+        google_tooltip_font=api_tooltip_fontname,
         page_background_color=page_background_color,
         search=enable_search,
         title_font_family=font_family,
         title_font_color=title_font_color,
         title_background=title_background,
         tooltip_css=tooltip_css,
         shadow_color=shadow_color,
@@ -931,14 +966,15 @@
         line_spacing=line_spacing,
         text_min_pixel_size=text_min_pixel_size,
         text_max_pixel_size=text_max_pixel_size,
         text_outline_width=text_outline_width,
         text_outline_color=[int(c * 255) for c in to_rgba(text_outline_color)],
         text_background_color=text_background_color,
         font_family=font_family,
+        font_weight=font_weight,
         text_collision_size_scale=text_collision_size_scale,
         cluster_boundary_polygons="polygon" in label_dataframe.columns,
         cluster_boundary_line_width=cluster_boundary_line_width,
         zoom_level=zoom_level,
         data_center_x=data_center[0],
         data_center_y=data_center[1],
         on_click=on_click,
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
 import numpy as np import pandas as pd import jinja2 import requests import
 base64 import io import gzip import html import warnings import zipfile import
 os from scipy.spatial import Delaunay from matplotlib.colors import to_rgba
 from datamapplot.medoids import medoid from datamapplot.alpha_shapes import
 create_boundary_polygons, smooth_polygon _DECKGL_TEMPLATE_STR = """
 {% if google_font %}
-{% endif %}
+{% if google_tooltip_font %}
+{% endif %} {% endif %}
 {% if inline_data %}
 {% endif %}
 [Loading...]
 {% if use_title %}
 {{title}}
 {{sub_title}} {% if search %}
 [Unknown INPUT type]
@@ -16,30 +17,31 @@
 {% elif search %}
 [Unknown INPUT type]
 {% endif %} {% if logo %}
 [{{logo}}]
 {% endif %}
 {% if custom_html %} {{custom_html}} {% endif %}
 """ _TOOL_TIP_CSS = """ font-size: 0.8em; font-family: {{title_font_family}};
-color: {{title_font_color}} !important; background-color: {{title_background}}
-!important; border-radius: 12px; box-shadow: 2px 3px 10px {{shadow_color}};
-max-width: 25%; """ class FormattingDict(dict): def __missing__(self, key):
-return f"{{{key}}}" class InteractiveFigure: """A simple class to hold
-interactive plot outputs. This allows for and object with a `_repr_html_` to
-display in notebooks. The actual content of the plot is HTML, and the `save`
-method can be used to save the results to an HTML file while can then be
-shared. """ def __init__(self, html_str, width="100%", height=800):
-self._html_str = html_str self.width = width self.height = height def __repr__
-(self): return f"" def __str__(self): return self._html_str def _repr_html_
-(self): src_doc = html.escape(self._html_str) iframe = f""" """ from
-IPython.display import HTML with warnings.catch_warnings(): msg = "Consider
-using IPython.display.IFrame instead" warnings.filterwarnings("ignore",
-message=msg) html_obj = HTML(iframe) return getattr(html_obj, "data", "") def
-save(self, filename): """Save an interactive firgure to the HTML file with name
-`filename`""" with open(filename, "w+") as f: f.write(self._html_str) def
+font-weight: {{title_font_weight}}; color: {{title_font_color}} !important;
+background-color: {{title_background}} !important; border-radius: 12px; box-
+shadow: 2px 3px 10px {{shadow_color}}; max-width: 25%; """ class FormattingDict
+(dict): def __missing__(self, key): return f"{{{key}}}" class
+InteractiveFigure: """A simple class to hold interactive plot outputs. This
+allows for and object with a `_repr_html_` to display in notebooks. The actual
+content of the plot is HTML, and the `save` method can be used to save the
+results to an HTML file while can then be shared. """ def __init__(self,
+html_str, width="100%", height=800): self._html_str = html_str self.width =
+width self.height = height def __repr__(self): return f"" def __str__(self):
+return self._html_str def _repr_html_(self): src_doc = html.escape
+(self._html_str) iframe = f""" """ from IPython.display import HTML with
+warnings.catch_warnings(): msg = "Consider using IPython.display.IFrame
+instead" warnings.filterwarnings("ignore", message=msg) html_obj = HTML(iframe)
+return getattr(html_obj, "data", "") def save(self, filename): """Save an
+interactive firgure to the HTML file with name `filename`""" with open
+(filename, "w+") as f: f.write(self._html_str) def
 label_text_and_polygon_dataframes( labels, data_map_coords,
 noise_label="Unlabelled", use_medoids=False, cluster_polygons=False,
 alpha=0.05, ): cluster_label_vector = np.asarray(labels)
 unique_non_noise_labels = [ label for label in np.unique(cluster_label_vector)
 if label != noise_label ] label_map = {n: i for i, n in enumerate
 (unique_non_noise_labels)} label_map[noise_label] = -1 label_unmap = {i: n for
 n, i in label_map.items()} cluster_idx_vector = np.asarray(pd.Series
@@ -54,17 +56,18 @@
 label_locations = np.asarray(label_locations) if cluster_polygons: return
 pd.DataFrame( { "x": label_locations.T[0], "y": label_locations.T[1], "label":
 unique_non_noise_labels, "size": cluster_sizes, "polygon": polygons, } ) else:
 return pd.DataFrame( { "x": label_locations.T[0], "y": label_locations.T[1],
 "label": unique_non_noise_labels, "size": cluster_sizes, } ) def render_html
 ( point_dataframe, label_dataframe, inline_data=True, title=None,
 sub_title=None, title_font_size=36, sub_title_font_size=18,
-text_collision_size_scale=3, text_min_pixel_size=12, text_max_pixel_size=36,
-font_family="arial", logo=None, logo_width=256, color_label_text=True,
-line_spacing=0.95, min_fontsize=12, max_fontsize=24, text_outline_width=8,
+text_collision_size_scale=3, text_min_pixel_size=18, text_max_pixel_size=36,
+font_family="Roboto", font_weight=900, tooltip_font_family=None,
+tooltip_font_weight=300, logo=None, logo_width=256, color_label_text=True,
+line_spacing=0.95, min_fontsize=18, max_fontsize=28, text_outline_width=8,
 text_outline_color="#eeeeeedd", point_hover_color="#aa0000bb",
 point_radius_min_pixels=0.01, point_radius_max_pixels=24,
 point_line_width_min_pixels=0.1, point_line_width_max_pixels=8,
 point_line_width=0.001, cluster_boundary_line_width=1,
 initial_zoom_fraction=1.0, background_color=None, darkmode=False,
 offline_data_prefix=None, tooltip_css=None, hover_text_html_template=None,
 extra_point_data=None, enable_search=False, search_field="hover_text",
@@ -93,18 +96,28 @@
 font-size of the sub-title in points. text_collision_size_scale: float
 (optional, default=3.0) How to scale text labels for the purpose of collision
 detection to determine which labels to display. text_min_pixel_size: float
 (optional, default=12.0) The minimum pixel size of label text. If text would be
 smaller than this in size then render the text to be at least this size.
 text_max_pixel_size: float (optional, default=36.0) The maximum pixel size of
 label text. If text would be larger than this in size then render the text to
-be at most this size. font_family: str (optional, default="arial") The font
+be at most this size. font_family: str (optional, default="Roboto") The font
 family to use for label text and titles. If the font family is a google font
 then the required google font api handling will automatically make the font
-available, so any google font family is acceptable. logo: str or None
+available, so any google font family is acceptable. font_weight: str or int
+(optional, default=900) The font weight to use for the text labels within the
+plot. Either weight specification such as "thin", "normal", or "bold" or an
+integer value between 0 (ultra-thin) and 1000 (ultra-black).
+tooltip_font_family: str (optional default="Roboto") The font family to use in
+tooltips/hover text. If the font family is a google font then the required
+google font api handling will automatically make the font available, so any
+google font family is acceptable. tooltip_font_weight: str or int (optional,
+default=400) The font weight to use for the tooltip /hover text within the
+plot. Either weight specification such as "thin", "normal", or "bold" or an
+integer value between 0 (ultra-thin) and 1000 (ultra-black). logo: str or None
 (optional, default=None) A logo image to include in the bottom right corner of
 the map. This should be a URL to the image. logo_width: int (optional,
 default=256) The width, in pixels, of the logo to be included in the bottom
 right corner. The logo will retain it's aspect ratio, so choose the width
 accordingly. color_label_text: bool (optional, default=True) Whether the text
 labels for clusters should be coloured or not. If set to False the labels will
 be either black or white depending on whether ``darkmode`` is set.
@@ -180,16 +193,16 @@
 ``on_click`` action for example. custom_js: str or None (optional,
 default=None) A string of custom Javascript code that is to be added after the
 code for rendering the scatterplot. This can include code to interact with the
 plot which is stored as ``deckgl``. Returns ------- interactive_plot:
 InteractiveFigure An interactive figure with hover, pan, and zoom. This will
 display natively in a notebook, and can be saved to an HTML file via the `save`
 method. """ # Compute point scaling n_points = point_dataframe.shape[0]
-magic_number = np.clip(32 * 4 ** (-np.log10(n_points)), 0.005, 4) if "size" not
-in point_dataframe.columns: point_size = magic_number else: point_dataframe
+magic_number = np.clip(32 * 4 ** (-np.log10(n_points)), 0.005, 0.1) if "size"
+not in point_dataframe.columns: point_size = magic_number else: point_dataframe
 ["size"] = magic_number * ( point_dataframe["size"] / point_dataframe
 ["size"].median() ) point_size = -1 # Compute zoom level and initial view
 location data_width = point_dataframe.x.max() - point_dataframe.x.min()
 data_height = point_dataframe.y.max() - point_dataframe.y.min() data_center =
 point_dataframe[["x", "y"]].values.mean(axis=0) spread = max(data_width,
 data_height) * initial_zoom_fraction if spread < (360.0 * np.power(2.0, -20)):
 zoom_level = 21 else: zoom_level = max(1, np.log2(360.0) - np.log2(spread)) if
@@ -212,60 +225,68 @@
 point_dataframe.columns: if extra_point_data is not None: hover_data =
 pd.concat( [point_dataframe[["hover_text"]], extra_point_data], axis=1, )
 replacements = FormattingDict( **{ str(name): f"${{hoverData.data.{name}
 [index]}}" for name in hover_data.columns } ) if hover_text_html_template is
 not None: get_tooltip = ( '({index, picked}) => picked ? {"html": `' +
 hover_text_html_template.format_map(replacements) + "`} : null" ) else:
 get_tooltip = "({index}) => hoverData.data.hover_text[index]" if on_click is
-not None: on_click = "({index}, event) => " + on_click.format_map(replacements)
-else: hover_data = point_dataframe[["hover_text"]] get_tooltip = "({index}) =>
-hoverData.data.hover_text[index]" replacements = FormattingDict( **{ str(name):
-f"${{hoverData.data.{name}[index]}}" for name in hover_data.columns } ) if
-on_click is not None: on_click = "({index}, event) => " + on_click.format_map
-(replacements) elif extra_point_data is not None: hover_data = extra_point_data
+not None: on_click = "({index, picked}, event) => { if (picked) {" +
+on_click.format_map(replacements) + " } }" else: hover_data = point_dataframe[
+["hover_text"]] get_tooltip = "({index}) => hoverData.data.hover_text[index]"
 replacements = FormattingDict( **{ str(name): f"${{hoverData.data.{name}
-[index]}}" for name in hover_data.columns } ) if hover_text_html_template is
-not None: get_tooltip = ( '({index, picked}) => picked ? {"html": `' +
-hover_text_html_template.format_map(replacements) + "`} : null" ) else:
-get_tooltip = "null" else: hover_data = pd.DataFrame(columns=("hover_text",))
-get_tooltip = "null" if inline_data: buffer = io.BytesIO()
-point_data.to_feather(buffer, compression="uncompressed") buffer.seek(0)
-base64_point_data = base64.b64encode(buffer.read()).decode() buffer =
-io.BytesIO() hover_data.to_feather(buffer, compression="uncompressed")
-buffer.seek(0) arrow_bytes = buffer.read() gzipped_bytes = gzip.compress
-(arrow_bytes) base64_hover_data = base64.b64encode(gzipped_bytes).decode()
-label_data_json = label_dataframe.to_json(orient="records") gzipped_label_data
-= gzip.compress(bytes(label_data_json, "utf-8")) base64_label_data =
-base64.b64encode(gzipped_label_data).decode() file_prefix = None else:
-base64_point_data = "" base64_hover_data = "" base64_label_data = ""
-file_prefix = offline_data_prefix if offline_data_prefix is not None else
-"datamapplot" point_data.to_feather(f"{file_prefix}_point_df.arrow",
-compression="uncompressed") hover_data.to_feather("point_hover_data.arrow",
-compression="uncompressed") with zipfile.ZipFile( f"
-{file_prefix}_point_hover_data.zip", "w", compression=zipfile.ZIP_DEFLATED,
-compresslevel=9, ) as f: f.write("point_hover_data.arrow") os.remove
-("point_hover_data.arrow") label_dataframe.to_json("label_data.json",
-orient="records") with zipfile.ZipFile( f"{file_prefix}_label_data.zip", "w",
+[index]}}" for name in hover_data.columns } ) if on_click is not None: on_click
+= "({index, picked}, event) => { if (picked) {" + on_click.format_map
+(replacements) + " } }" elif extra_point_data is not None: hover_data =
+extra_point_data replacements = FormattingDict( **{ str(name): f"${
+{hoverData.data.{name}[index]}}" for name in hover_data.columns } ) if
+hover_text_html_template is not None: get_tooltip = ( '({index, picked}) =>
+picked ? {"html": `' + hover_text_html_template.format_map(replacements) + "`}
+: null" ) else: get_tooltip = "null" if on_click is not None: on_click = "(
+{index, picked}, event) => { if (picked) {" + on_click.format_map(replacements)
++ " } }" else: hover_data = pd.DataFrame(columns=("hover_text",)) get_tooltip =
+"null" if inline_data: buffer = io.BytesIO() point_data.to_feather(buffer,
+compression="uncompressed") buffer.seek(0) base64_point_data = base64.b64encode
+(buffer.read()).decode() buffer = io.BytesIO() hover_data.to_feather(buffer,
+compression="uncompressed") buffer.seek(0) arrow_bytes = buffer.read()
+gzipped_bytes = gzip.compress(arrow_bytes) base64_hover_data = base64.b64encode
+(gzipped_bytes).decode() label_data_json = label_dataframe.to_json
+(orient="records") gzipped_label_data = gzip.compress(bytes(label_data_json,
+"utf-8")) base64_label_data = base64.b64encode(gzipped_label_data).decode()
+file_prefix = None else: base64_point_data = "" base64_hover_data = ""
+base64_label_data = "" file_prefix = offline_data_prefix if offline_data_prefix
+is not None else "datamapplot" point_data.to_feather(f"
+{file_prefix}_point_df.arrow", compression="uncompressed")
+hover_data.to_feather("point_hover_data.arrow", compression="uncompressed")
+with zipfile.ZipFile( f"{file_prefix}_point_hover_data.zip", "w",
+compression=zipfile.ZIP_DEFLATED, compresslevel=9, ) as f: f.write
+("point_hover_data.arrow") os.remove("point_hover_data.arrow")
+label_dataframe.to_json("label_data.json", orient="records") with
+zipfile.ZipFile( f"{file_prefix}_label_data.zip", "w",
 compression=zipfile.ZIP_DEFLATED, compresslevel=9 ) as f: f.write
 ("label_data.json") os.remove("label_data.json") title_font_color = "#000000"
 if not darkmode else "#ffffff" sub_title_font_color = "#777777"
 title_background = "#ffffffaa" if not darkmode else "#000000aa" shadow_color =
 "#aaaaaa44" if not darkmode else "#00000044" input_background = "#ffffffdd" if
 not darkmode else "#000000dd" input_border = "#ddddddff" if not darkmode else
 "222222ff" if tooltip_css is None: tooltip_css_template = jinja2.Template
 (_TOOL_TIP_CSS) tooltip_css = tooltip_css_template.render
-( title_font_family=font_family, title_font_color=title_font_color,
+( title_font_family=tooltip_font_family or font_family,
+title_font_color=title_font_color, title_font_weight=tooltip_font_weight,
 title_background=title_background, shadow_color=shadow_color, ) if
 background_color is None: page_background_color = "#ffffff" if not darkmode
 else "#000000" else: page_background_color = background_color template =
 jinja2.Template(_DECKGL_TEMPLATE_STR) api_fontname = font_family.replace(" ",
 "+") resp = requests.get(f"https://fonts.googleapis.com/css?family=
-{api_fontname}") if not resp.ok: api_fontname = None html_str = template.render
-( title=title if title is not None else "Interactive Data Map",
-sub_title=sub_title if sub_title is not None else "", google_font=api_fontname,
+{api_fontname}") if not resp.ok: api_fontname = None if tooltip_font_family is
+not None: api_tooltip_fontname = tooltip_font_family.replace(" ", "+") resp =
+requests.get(f"https://fonts.googleapis.com/css?family={api_tooltip_fontname}")
+if not resp.ok: api_tooltip_fontname = None else: api_tooltip_fontname = None
+html_str = template.render( title=title if title is not None else "Interactive
+Data Map", sub_title=sub_title if sub_title is not None else "",
+google_font=api_fontname, google_tooltip_font=api_tooltip_fontname,
 page_background_color=page_background_color, search=enable_search,
 title_font_family=font_family, title_font_color=title_font_color,
 title_background=title_background, tooltip_css=tooltip_css,
 shadow_color=shadow_color, input_background=input_background,
 input_border=input_border, custom_css=custom_css, use_title=title is not None,
 title_font_size=title_font_size, sub_title_font_size=sub_title_font_size,
 sub_title_font_color=sub_title_font_color, logo=logo, logo_width=logo_width,
@@ -280,13 +301,13 @@
 point_radius_max_pixels=point_radius_max_pixels,
 point_radius_min_pixels=point_radius_min_pixels,
 label_text_color=label_text_color, line_spacing=line_spacing,
 text_min_pixel_size=text_min_pixel_size,
 text_max_pixel_size=text_max_pixel_size, text_outline_width=text_outline_width,
 text_outline_color=[int(c * 255) for c in to_rgba(text_outline_color)],
 text_background_color=text_background_color, font_family=font_family,
-text_collision_size_scale=text_collision_size_scale,
+font_weight=font_weight, text_collision_size_scale=text_collision_size_scale,
 cluster_boundary_polygons="polygon" in label_dataframe.columns,
 cluster_boundary_line_width=cluster_boundary_line_width, zoom_level=zoom_level,
 data_center_x=data_center[0], data_center_y=data_center[1], on_click=on_click,
 get_tooltip=get_tooltip, search_field=search_field, custom_js=custom_js, )
 return html_str
```

### Comparing `datamapplot-0.2.2/datamapplot/medoids.py` & `datamapplot-0.3.0/datamapplot/medoids.py`

 * *Files identical despite different names*

### Comparing `datamapplot-0.2.2/datamapplot/overlap_computations.py` & `datamapplot-0.3.0/datamapplot/overlap_computations.py`

 * *Files identical despite different names*

### Comparing `datamapplot-0.2.2/datamapplot/palette_handling.py` & `datamapplot-0.3.0/datamapplot/palette_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 def palette_from_datamap(
     umap_coords,
     label_locations,
     hue_shift=0.0,
     theta_range=np.pi / 16,
     radius_weight_power=1.0,
+    min_lightness=10,
 ):
     if label_locations.shape[0] == 0:
         return []
 
     data_center = np.asarray(
         umap_coords.min(axis=0)
         + (umap_coords.max(axis=0) - umap_coords.min(axis=0)) / 2
@@ -55,15 +56,15 @@
 
             mask_size = np.sum(r_mask)
             chroma = (
                 np.argsort(np.argsort(data_map_radii[r_mask])) / mask_size
             ) * 80 + 20
             lightness = (
                 1.0 - (np.argsort(np.argsort(data_map_radii[r_mask])) / mask_size)
-            ) * 70 + 10
+            ) * (80 - min_lightness) + min_lightness
             location_lightness.append(
                 np.interp(
                     r,
                     np.sort(data_map_radii[r_mask]),
                     np.sort(lightness)[::-1],
                 )
             )
@@ -90,15 +91,15 @@
 
             mask_size = np.sum(r_mask)
             chroma = (
                 np.argsort(np.argsort(data_map_radii[r_mask])) / mask_size
             ) * 80 + 20
             lightness = (
                 1.0 - (np.argsort(np.argsort(data_map_radii[r_mask])) / mask_size)
-            ) * 70 + 10
+            ) * (80 - min_lightness) + min_lightness
             sorted_chroma.append(np.sort(chroma))
             sorted_lightness.append(np.sort(lightness)[::-1])
             sorted_radii.append(np.sort(data_map_radii[r_mask]))
 
         for r, theta in zip(label_location_radii, label_location_thetas):
             nearest_theta_idx = np.argmin(np.abs(uniform_thetas - theta))
             location_lightness.append(
```

### Comparing `datamapplot-0.2.2/datamapplot/plot_rendering.py` & `datamapplot-0.3.0/datamapplot/plot_rendering.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,43 +8,49 @@
 from functools import partial
 
 from sklearn.neighbors import KernelDensity
 from skimage.transform import rescale
 
 from matplotlib import pyplot as plt
 from matplotlib import font_manager
+from matplotlib import patheffects
 
 from datamapplot.overlap_computations import get_2d_coordinates
 from datamapplot.text_placement import (
+    estimate_dynamic_font_size,
     initial_text_location_placement,
     fix_crossings,
     adjust_text_locations,
     estimate_font_size,
+    pylabeladjust_text_locations,
 )
 
 from warnings import warn
 from tempfile import NamedTemporaryFile
 
 import requests
 import re
 
 
 def get_google_font(fontname):
-    api_fontname = fontname.replace(" ", "+")
-    api_response = requests.get(
-        f"https://fonts.googleapis.com/css?family={api_fontname}:black,bold,regular,light"
-    )
-    if api_response.ok:
-        font_urls = re.findall(r"(https?://[^\)]+)", str(api_response.content))
-        for font_url in font_urls:
-            font_data = requests.get(font_url)
-            f = NamedTemporaryFile(delete=False, suffix=".ttf")
-            f.write(font_data.content)
-            f.close()
-            font_manager.fontManager.addfont(f.name)
+    try:
+        api_fontname = fontname.replace(" ", "+")
+        api_response = requests.get(
+            f"https://fonts.googleapis.com/css?family={api_fontname}:black,bold,regular,light"
+        )
+        if api_response.ok:
+            font_urls = re.findall(r"(https?://[^\)]+)", str(api_response.content))
+            for font_url in font_urls:
+                font_data = requests.get(font_url)
+                f = NamedTemporaryFile(delete=False, suffix=".ttf")
+                f.write(font_data.content)
+                f.close()
+                font_manager.fontManager.addfont(f.name)
+    except:
+        warn(f"Failed in getting google-font {fontname}; using fallback ...")
 
 
 def datashader_scatterplot(
     data_map_coords,
     color_list,
     point_size,
     ax,
@@ -71,15 +77,15 @@
 
 def add_glow_to_scatterplot(
     data_map_coords,
     color_list,
     ax,
     noise_color="#999999",
     kernel_bandwidth=0.25,
-    approx_patch_size=64,
+    approx_patch_size=32,
     kernel="gaussian",
     n_levels=8,
     max_alpha=0.5,
 ):
     # we are assuming colors are hex strings!
     unique_colors = np.unique(color_list)
     color_array = np.asarray(color_list)
@@ -146,34 +152,42 @@
 
 
 def render_plot(
     data_map_coords,
     color_list,
     label_text,
     label_locations,
+    label_cluster_sizes,
     *,
     title=None,
     sub_title=None,
     figsize=(12, 12),
-    fontfamily="DejaVu Sans",
+    dynamic_label_size=False,
+    dynamic_label_size_scaling_factor=0.75,
+    font_family="Roboto",
+    font_weight=400,
     label_linespacing=0.95,
     label_font_size=None,
     label_text_colors=None,
     label_arrow_colors=None,
     highlight_colors=None,
     point_size=1,
     alpha=1.0,
     dpi=plt.rcParams["figure.dpi"],
+    label_over_points=False,
     label_base_radius=None,
     label_margin_factor=1.5,
+    min_font_size=4.0,
+    max_font_size=24.0,
+    min_font_weight=200,
+    max_font_weight=800,
     highlight_labels=None,
-    highlight_label_keywords={"fontweight": "bold"},
+    highlight_label_keywords={"fontweight": 1000},
     add_glow=True,
     noise_color="#999999",
-    label_size_adjustments=None,
     glow_keywords={
         "kernel": "gaussian",
         "kernel_bandwidth": 0.25,
         "approx_patch_size": 64,
     },
     darkmode=False,
     logo=None,
@@ -181,14 +195,20 @@
     force_matplotlib=False,
     label_direction_bias=None,
     marker_type="o",
     marker_size_array=None,
     arrowprops={},
     title_keywords=None,
     sub_title_keywords=None,
+    pylabeladjust_speed=None,
+    pylabeladjust_max_iterations=500,
+    pylabeladjust_adjust_by_size=True,
+    pylabeladjust_margin_percentage=7.5,
+    pylabeladjust_radius_scale=1.05,
+    verbose=False,
 ):
     """Render a static data map plot with given colours and label locations and text. This is
     a lower level function, and should usually not be used directly unless there are specific
     reasons for digging in. This usually involves things like getting direct control over label
     locations, altering label texts to suit specific needs, or direct control over point
     colouring in the scatterplot.
 
@@ -220,34 +240,42 @@
         A sub-title for the plot. If ``None`` then no sub-title is used for the plot.
         The sub-title can be significantly longer then the title and provide more information\
         about the plot and data sources.
 
     figsize: (int, int) (optional, default=(12,12))
         How big to make the figure in inches (actual pixel size will depend on ``dpi``).
 
-    fontfamily: str (optional, default="DejaVu Sans")
-        The fontfamily to use for the plot -- the labels and the title and sub-title
+    dynamic_label_size: bool (optional, default=False)
+        Whether to use dynamic label sizing based on the sizes of the clusters.
+
+    dynamic_label_size_scaling_factor: float (optional, default=0.75)
+        The scaling factor to use when using dynamic label sizing based on the sizes of the clusters.
+
+    font_family: str (optional, default="DejaVu Sans")
+        The font_family to use for the plot -- the labels and the title and sub-title
         unless explicitly over-ridden by title_keywords or sub_title_keywords.
 
     label_linespacing: float (optional, default=0.95)
         The line-spacing to use when rendering multi-line labels in the plot. The default
         of 0.95 keeps multi-line labels compact, but can be less than ideal for some fonts.
 
     label_font_size: float or None (optional, default=None)
         The font-size (in pts) to use for the text labels in the plot. If this is ``None``
         then a heuristic will be used to try to find the best font size that can fit all
         the labels in.
 
-    label_text_colors: list of str or None (optional, default=None)
+    label_text_colors: str or list of str or None (optional, default=None)
         The colours of the text labels, one per text label. If None then the text labels
-        will be either black or white depending on ``darkmode``.
+        will be either black or white depending on ``darkmode``. If just a single string
+        then it is assumed to be a fixed colour for all labels.
 
-    label_arrow_colors: list of str or None (optional, default=None)
+    label_arrow_colors: str or list of str or None (optional, default=None)
         The colours of the arrows between the text labels and clusters, one per text label.
         If None then the arrows will be either black or white depending on ``darkmode``.
+        If just a single string then it is assumed to be a fixed colour for all arrows.
 
     highlight_colors: list of str or None (optional default=None)
         The colours used if text labels are highlighted and a bounding box around the label is
         used. For example ``create_plot`` uses the cluster colours from the colour mapping that
         was passed or created.
 
     point_size: int or float (optional, default=1)
@@ -260,22 +288,41 @@
 
     alpha: float (optional, default=1.0)
         The alpha transparency value to use when rendering points.
 
     dpi: int (optional, default=plt.rcParams["figure.dpi"])
         The dots-per-inch to use when rendering the plot.
 
+    label_over_points: bool (optional, default=False)
+        Whether to attempt tom place text labels directly on top of the points in clusters. This
+        can result in severe over-packing, and this is remedied via pylabeladjust which can end up
+        moving labels some distance. For smaller numbers of labels this is likely a good choice, for
+        more than 20 labels this will require a small font. For larger numbers of labels still this
+        may be sub-optimal.
+
     label_base_radius: float or None (optional, default=None)
         Labels are placed in rings around the data map. This value can explicitly control the
         radius (in data coordinates) of the innermost such ring.
 
     label_margin_factor: float (optional, default=1.5)
         The expansion factor to use when creating a bounding box around the label text
         to compute whether overlaps are occurring during the label placement adjustment phase.
 
+    min_font_size: float (optional, default=4.0)
+        The minimum font size to use when estimating the font size for the labels.
+
+    max_font_size: float (optional, default=24.0)
+        The maximum font size to use when estimating the font size for the labels.
+
+    min_font_weight: int (optional, default=200)
+        The minimum font weight to use when using dynamic label sizing (font weights will vary as well).
+
+    max_font_weight: int (optional, default=800)
+        The maximum font weight to use when using dynamic label sizing (font weights will vary as well).
+
     highlight_labels: list of str or None (optional, default=None)
         A list of the labels to be highlighted.
 
     highlight_label_keywords: dict (optional, default={"fontweight": "bold"})
         Keywords for how to highlight the labels. This dict will be passed on as keyword
         arguments to the matplotlib ``annotate`` function. See the matplotlib documentation
         for more details on what can be done.
@@ -283,18 +330,14 @@
     add_glow: bool (optional, default=True)
         Whether to add a glow-effect using KDEs.
 
     noise_color: str (optional, default="#999999")
         The colour to use for unlabelled or noise points in the data map. This should usually
         be a muted or neutral colour to distinguish background points from the labelled clusters.
 
-    label_size_adjustments: ndarray of shape (n_labels,) or None (optional, default=None)
-        Size adjustments to be applied to each label; this should be an adjustment, in pts,
-        to the fontsize for each label.
-
     glow_keywords: dict (optional, default={"kernel": "gaussian","kernel_bandwidth": 0.25})
         Keyword arguments that will be passed along to the ``add_glow_to_scatterplot``
         function. See that function for more details.
 
     darkmode: bool (optional, default=False)
         Whether to render the plot in darkmode (with a dark background) or not.
 
@@ -336,29 +379,58 @@
         A dictionary of keyword arguments to pass through to matplotlib's ``suptitle`` fucntion.
         This includes things like fontfamily, fontsize, fontweight, color, etc.
 
     sub_title_keywords: dict or None (optional, default=None)
         A dictionary of keyword arguments to pass through to matplotlib's ``title`` fucntion.
         This includes things like fontfamily, fontsize, fontweight, color, etc.
 
+    pylabeladjust_speed: None or float (optional, default=None)
+        pylabeladjust speed for adjusting label positioning when doing labels over points. If
+        ``label_over_points`` is ``False`` then this will have no effect. If ``None`` then
+        a good choice of speed will be approximated from the data.
+
+    pylabeladjust_max_iterations: int (optional, default=500)
+        The maximum number of pylabeladjust iterations for adjusting label positioning when
+        doing labels over points. If ``label_over_points`` is ``False`` then this will have
+        no effect.
+
+    pylabeladjust_adjust_by_size: bool (optional, default=True)
+        Whether to adjust the labels based on the size of the rectangles for adjusting label
+        positioning when doing labels over points. If ``label_over_points`` is ``False`` then
+        this will have no effect.
+
+    pylabeladjust_margin_percentage: float (optional, default=7.5)
+        The margin percentage for the repulsion radius for adjusting label positioning when
+        doing labels over points. If ``label_over_points`` is ``False`` then this will have no effect.
+
+    pylabeladjust_radius_scale: float (optional, default=1.05)
+        The scale factor for the repulsion radius for adjusting label
+        positioning when doing labels over points. If ``label_over_points`` is ``False`` then
+        this will have no effect.
+
+    verbose: bool (optional, default=False)
+        Print progress as the plot is being created.
+
     Returns
     -------
     fig: matplotlib.Figure
         The figure that the resulting plot is rendered to.
 
     ax: matpolotlib.Axes
         The axes contained within the figure that the plot is rendered to.
 
     """
     # Create the figure
     fig, ax = plt.subplots(figsize=figsize, dpi=dpi, constrained_layout=True)
 
+    if verbose:
+        print("Getting any required fonts...")
     # Get any google fonts if required
-    get_google_font(fontfamily)
-    get_google_font(fontfamily.split()[0])
+    get_google_font(font_family)
+    get_google_font(font_family.split()[0])
     if title_keywords is not None and "fontfamily" in title_keywords:
         get_google_font(title_keywords["fontfamily"])
         get_google_font(title_keywords["fontfamily"].split()[0])
     if sub_title_keywords is not None and "fontfamily" in sub_title_keywords:
         get_google_font(sub_title_keywords["fontfamily"])
         get_google_font(sub_title_keywords["fontfamily"].split()[0])
 
@@ -380,14 +452,16 @@
                 "Adjusting marker type or size cannot be done with datashader; use force_matplotlib=True"
             )
         datashader_scatterplot(
             data_map_coords, color_list, point_size=point_size, ax=ax
         )
 
     # Create background glow
+    if verbose:
+        print("Adding glow to scatterplot...")
     if add_glow:
         add_glow_to_scatterplot(
             data_map_coords, color_list, ax, noise_color=noise_color, **glow_keywords
         )
 
     # Add a mark in the bottom right if provided
     if logo is not None:
@@ -397,65 +471,165 @@
         ax.imshow(
             logo,
             extent=(0.98 - logo_width, 0.98, 0.02, 0.02 + mark_height),
             transform=ax.transAxes,
         )
 
     # Find initial placements for text, fix any line crossings, then optimize placements
+    if verbose:
+        print("Placing labels...")
     ax.autoscale_view()
     if label_locations.shape[0] > 0:
-        label_text_locations = initial_text_location_placement(
-            label_locations,
-            base_radius=label_base_radius,
-            theta_stretch=label_direction_bias,
-        )
-        fix_crossings(label_text_locations, label_locations)
-
-        font_scale_factor = np.sqrt(figsize[0] * figsize[1])
-        if label_font_size is None:
-            font_size = estimate_font_size(
-                label_text_locations,
-                label_text,
-                0.9 * font_scale_factor,
-                fontfamily=fontfamily,
-                linespacing=label_linespacing,
-                ax=ax,
-            )
-        else:
-            font_size = label_font_size
 
         # Ensure we can look up labels for highlighting
         if highlight_labels is not None:
             highlight = set(highlight_labels)
         else:
             highlight = set([])
 
-        label_text_locations = adjust_text_locations(
-            label_text_locations,
-            label_locations,
-            label_text,
-            fontfamily=fontfamily,
-            font_size=font_size,
-            linespacing=label_linespacing,
-            highlight=highlight,
-            highlight_label_keywords=highlight_label_keywords,
-            ax=ax,
-            expand=(label_margin_factor, label_margin_factor),
-            label_size_adjustments=label_size_adjustments,
-        )
+        if label_over_points:
+            font_scale_factor = np.sqrt(figsize[0] * figsize[1])
+            if verbose:
+                print("Estimating font size...")
+            if label_font_size is None:
+                if dynamic_label_size:
+                    font_sizes, font_weights = estimate_dynamic_font_size(
+                        label_locations,
+                        label_text,
+                        fontfamily=font_family,
+                        linespacing=label_linespacing,
+                        expand=(1.0, 1.0),
+                        overlap_percentage_allowed=0.66,
+                        dynamic_size_array=label_cluster_sizes
+                        ** dynamic_label_size_scaling_factor,
+                        min_font_size=min_font_size,
+                        max_font_size=max_font_size,
+                        min_font_weight=min_font_weight,
+                        max_font_weight=max_font_weight,
+                        ax=ax,
+                    )
+                    font_size = None
+                else:
+                    font_size = estimate_font_size(
+                        label_locations,
+                        label_text,
+                        font_scale_factor,
+                        fontfamily=font_family,
+                        fontweight=font_weight,
+                        linespacing=label_linespacing,
+                        expand=(1.0, 1.0),
+                        overlap_percentage_allowed=0.66,
+                        min_font_size=min_font_size,
+                        max_font_size=max_font_size,
+                        ax=ax,
+                    )
+                    font_sizes = None
+                    font_weights = None
+            else:
+                font_size = label_font_size
+                font_sizes = None
+                font_weights = None
+
+            label_text_locations = pylabeladjust_text_locations(
+                label_locations,
+                label_text,
+                fontfamily=font_family,
+                font_size=font_size,
+                font_sizes=font_sizes,
+                font_weights=font_weights,
+                linespacing=label_linespacing,
+                highlight=highlight,
+                highlight_label_keywords=highlight_label_keywords,
+                ax=ax,
+                fig=fig,
+                speed=pylabeladjust_speed,
+                max_iterations=pylabeladjust_max_iterations,
+                adjust_by_size=pylabeladjust_adjust_by_size,
+                margin_percentage=pylabeladjust_margin_percentage,
+                radius_scale=pylabeladjust_radius_scale,
+            )
+        else:
+            if verbose:
+                print("Creating initial label placements...")
+            label_text_locations = initial_text_location_placement(
+                label_locations,
+                base_radius=label_base_radius,
+                theta_stretch=label_direction_bias,
+            )
+            fix_crossings(label_text_locations, label_locations)
+
+            if verbose:
+                print("Estimating font size...")
+            font_scale_factor = np.sqrt(figsize[0] * figsize[1])
+            if label_font_size is None:
+                if dynamic_label_size:
+                    font_sizes, font_weights = estimate_dynamic_font_size(
+                        label_locations,
+                        label_text,
+                        fontfamily=font_family,
+                        linespacing=label_linespacing,
+                        expand=(label_margin_factor, label_margin_factor),
+                        overlap_percentage_allowed=0.5,
+                        dynamic_size_array=label_cluster_sizes
+                        ** dynamic_label_size_scaling_factor,
+                        min_font_size=min_font_size,
+                        max_font_size=max_font_size,
+                        min_font_weight=min_font_weight,
+                        max_font_weight=max_font_weight,
+                        ax=ax,
+                    )
+                    font_size = None
+                else:
+                    font_size = estimate_font_size(
+                        label_text_locations,
+                        label_text,
+                        0.9 * font_scale_factor,
+                        fontfamily=font_family,
+                        fontweight=font_weight,
+                        linespacing=label_linespacing,
+                        min_font_size=min_font_size,
+                        max_font_size=max_font_size,
+                        ax=ax,
+                    )
+                    font_sizes = None
+                    font_weights = None
+            else:
+                font_size = label_font_size
+                font_sizes = None
+                font_weights = None
+
+            if verbose:
+                print("Adjusting label placements...")
+            label_text_locations = adjust_text_locations(
+                label_text_locations,
+                label_locations,
+                label_text,
+                fontfamily=font_family,
+                font_size=font_size,
+                fontweight=font_weight,
+                linespacing=label_linespacing,
+                highlight=highlight,
+                highlight_label_keywords=highlight_label_keywords,
+                ax=ax,
+                expand=(label_margin_factor, label_margin_factor),
+                font_sizes=font_sizes,
+                font_weights=font_weights,
+            )
 
         # Build highlight boxes
         if (
             "bbox" in highlight_label_keywords
             and highlight_label_keywords["bbox"] is not None
         ):
             base_bbox_keywords = highlight_label_keywords["bbox"]
         else:
             base_bbox_keywords = None
 
+        if verbose:
+            print("Adding labels to the plot...")
         # Add the annotations to the plot
         texts = []
         for i in range(label_locations.shape[0]):
             if base_bbox_keywords is not None:
                 bbox_keywords = dict(base_bbox_keywords.items())
                 if "fc" not in base_bbox_keywords:
                     if highlight_colors is not None:
@@ -463,22 +637,28 @@
                     else:
                         bbox_keywords["fc"] = "#cccccc33" if darkmode else "#33333333"
                 if "ec" not in base_bbox_keywords:
                     bbox_keywords["ec"] = "none"
             else:
                 bbox_keywords = None
 
-            if label_text_colors:
+            if type(label_text_colors) == str:
+                text_color = label_text_colors
+            elif label_text_colors:
                 text_color = label_text_colors[i]
             elif darkmode:
                 text_color = "white"
             else:
                 text_color = "black"
 
-            if label_arrow_colors:
+            outline_color = "#00000077" if darkmode else "#ffffff77"
+
+            if type(label_arrow_colors) == str:
+                arrow_color = label_arrow_colors
+            elif label_arrow_colors:
                 arrow_color = label_arrow_colors[i]
             elif darkmode:
                 arrow_color = "#dddddd"
             else:
                 arrow_color = "#333333"
 
             texts.append(
@@ -486,36 +666,47 @@
                     label_text[i],
                     label_locations[i],
                     xytext=label_text_locations[i],
                     ha="center",
                     ma="center",
                     va="center",
                     linespacing=label_linespacing,
-                    fontfamily=fontfamily,
-                    arrowprops={
-                        "arrowstyle": "-",
-                        "linewidth": 0.5,
-                        "color": arrow_color,
-                        **arrowprops,
-                    },
+                    fontfamily=font_family,
+                    arrowprops=(
+                        {
+                            "arrowstyle": "-",
+                            "linewidth": 0.5,
+                            "color": arrow_color,
+                            **arrowprops,
+                        }
+                        if not label_over_points
+                        else None
+                    ),
                     fontsize=(
                         highlight_label_keywords.get("fontsize", font_size)
                         if label_text[i] in highlight
                         else font_size
                     )
-                    + (
-                        label_size_adjustments[i]
-                        if label_size_adjustments is not None
-                        else 0.0
+                    if font_sizes is None
+                    else font_sizes[i],
+                    path_effects=(
+                        [
+                            patheffects.Stroke(linewidth=3, foreground=outline_color),
+                            patheffects.Normal(),
+                        ]
+                        if label_over_points
+                        else None
                     ),
                     bbox=bbox_keywords if label_text[i] in highlight else None,
                     color=text_color,
-                    fontweight=highlight_label_keywords.get("fontweight", "normal")
-                    if label_text[i] in highlight
-                    else "normal",
+                    fontweight=(
+                        highlight_label_keywords.get("fontweight", font_weight)
+                        if label_text[i] in highlight
+                        else (font_weights[i] if font_weights is not None else font_weight)
+                    ),
                 )
             )
 
         # Ensure we have plot bounds that meet the newly place annotations
         coords = get_2d_coordinates(texts)
         x_min, y_min = ax.transData.inverted().transform(
             (coords[:, [0, 2]].copy().min(axis=0))
@@ -536,30 +727,34 @@
         height = y_max - y_min
         x_min -= 0.05 * width
         x_max += 0.05 * width
         y_min -= 0.05 * height
         y_max += 0.05 * height
 
     # decorate the plot
+    if verbose:
+        print("Decorating plot...")
     ax.set(xticks=[], yticks=[])
     if sub_title is not None:
         if sub_title_keywords is not None:
             keyword_args = {
                 "fontweight": "light",
                 "color": "gray",
-                "fontsize": (1.2 * font_scale_factor),
-                "fontfamily": fontfamily,
+                "fontsize": (1.6 * font_scale_factor),
+                "fontfamily": font_family,
+                "fontweight": font_weight,
                 **sub_title_keywords,
             }
         else:
             keyword_args = {
                 "fontweight": "light",
                 "color": "gray",
-                "fontsize": (1.2 * font_scale_factor),
-                "fontfamily": fontfamily,
+                "fontsize": (1.6 * font_scale_factor),
+                "fontfamily": font_family,
+                "fontweight": font_weight,
             }
         axis_title = ax.set_title(
             sub_title,
             loc="left",
             va="baseline",
             fontdict=keyword_args,
         )
@@ -574,27 +769,27 @@
 
     if title is not None:
         if title_keywords is not None:
             keyword_args = {
                 "color": "white" if darkmode else "black",
                 "ha": "left",
                 "va": "bottom",
-                "fontweight": "bold",
-                "fontsize": int(1.6 * font_scale_factor),
-                "fontfamily": fontfamily,
+                "fontweight": 900,
+                "fontsize": int(3.2 * font_scale_factor),
+                "fontfamily": font_family,
                 **title_keywords,
             }
         else:
             keyword_args = {
                 "color": "white" if darkmode else "black",
                 "ha": "left",
                 "va": "bottom",
-                "fontweight": "bold",
-                "fontsize": int(1.6 * font_scale_factor),
-                "fontfamily": fontfamily,
+                "fontweight": 900,
+                "fontsize": int(3.2 * font_scale_factor),
+                "fontfamily": font_family,
             }
         fig.suptitle(
             title, x=0.0, y=sup_title_y_value, transform=ax.transAxes, **keyword_args
         )
 
     ax_x_min, ax_x_max = ax.get_xlim()
     ax_y_min, ax_y_max = ax.get_ylim()
```

### Comparing `datamapplot-0.2.2/datamapplot/text_placement.py` & `datamapplot-0.3.0/datamapplot/text_placement.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import numpy as np
 from sklearn.metrics import pairwise_distances
+from sklearn.preprocessing import MinMaxScaler
+from pylabeladjust import adjust_texts
 
 from datamapplot.overlap_computations import (
     get_2d_coordinates,
     overlap_intervals,
     text_line_overlaps,
     intersect,
 )
@@ -133,35 +135,40 @@
     return result
 
 
 def estimate_font_size(
     text_locations,
     label_text,
     initial_font_size,
-    fontfamily="DejaVu Sans",
+    fontfamily="Roboto",
+    fontweight=400,
     linespacing=0.95,
     expand=(1.5, 1.5),
+    overlap_percentage_allowed=0.5,
+    min_font_size=3.0,
+    max_font_size=16.0,
     ax=None,
 ):
     if ax is None:
         ax = plt.gca()
 
     font_size = initial_font_size
     overlap_percentage = 1.0
-    while overlap_percentage > 0.5 and font_size > 3.0:
+    while overlap_percentage > overlap_percentage_allowed and font_size > min_font_size:
         texts = [
             ax.text(
                 *text_locations[i],
                 label_text[i],
                 ha="center",
                 ma="center",
                 va="center",
                 linespacing=linespacing,
                 alpha=0.0,
                 fontfamily=fontfamily,
+                fontweight=fontweight,
                 fontsize=font_size,
             )
             for i in range(text_locations.shape[0])
         ]
         coords = get_2d_coordinates(texts, expand=expand)
         xoverlaps = overlap_intervals(
             coords[:, 0], coords[:, 1], coords[:, 0], coords[:, 1]
@@ -178,26 +185,94 @@
             t.remove()
 
         font_size = 0.9 * font_size
 
     return font_size
 
 
+def estimate_dynamic_font_size(
+    text_locations,
+    label_text,
+    fontfamily="DejaVu Sans",
+    linespacing=0.95,
+    expand=(1.5, 1.5),
+    overlap_percentage_allowed=0.5,
+    dynamic_size_array=None,
+    min_font_size=4.0,
+    max_font_size=24.0,
+    min_font_weight=200,
+    max_font_weight=500,
+    ax=None,
+):
+    if ax is None:
+        ax = plt.gca()
+
+    overlap_percentage = 1.0
+    current_max_font_size = max_font_size
+    weight_scaler = MinMaxScaler(feature_range=(min_font_weight, max_font_weight))
+    font_weights = np.squeeze(
+        weight_scaler.fit_transform(dynamic_size_array.reshape(-1, 1))
+    )
+    while (
+        overlap_percentage > overlap_percentage_allowed
+        and current_max_font_size > min_font_size
+    ):
+        size_scaler = MinMaxScaler(feature_range=(min_font_size, current_max_font_size))
+        font_sizes = np.squeeze(
+            size_scaler.fit_transform(dynamic_size_array.reshape(-1, 1))
+        )
+        texts = [
+            ax.text(
+                *text_locations[i],
+                label_text[i],
+                ha="center",
+                ma="center",
+                va="center",
+                linespacing=linespacing,
+                alpha=0.0,
+                fontfamily=fontfamily,
+                fontsize=font_sizes[i],
+                fontweight=font_weights[i],
+            )
+            for i in range(text_locations.shape[0])
+        ]
+        coords = get_2d_coordinates(texts, expand=expand)
+        xoverlaps = overlap_intervals(
+            coords[:, 0], coords[:, 1], coords[:, 0], coords[:, 1]
+        )
+        xoverlaps = xoverlaps[xoverlaps[:, 0] != xoverlaps[:, 1]]
+        yoverlaps = overlap_intervals(
+            coords[:, 2], coords[:, 3], coords[:, 2], coords[:, 3]
+        )
+        yoverlaps = yoverlaps[yoverlaps[:, 0] != yoverlaps[:, 1]]
+        overlaps = yoverlaps[(yoverlaps[:, None] == xoverlaps).all(-1).any(-1)]
+        overlap_percentage = len(overlaps) / (2 * text_locations.shape[0])
+        # remove texts
+        for t in texts:
+            t.remove()
+
+        current_max_font_size = 0.9 * current_max_font_size
+
+    return font_sizes, font_weights
+
+
 def adjust_text_locations(
     text_locations,
     label_locations,
     label_text,
     font_size=12,
     fontfamily="DejaVu Sans",
+    fontweight=400,
     linespacing=0.95,
     expand=(1.5, 1.5),
     max_iter=100,
-    label_size_adjustments=None,
     highlight=frozenset([]),
     highlight_label_keywords={},
+    font_sizes=None,
+    font_weights=None,
     ax=None,
 ):
     if ax is None:
         ax = plt.gca()
 
     # Add text to the axis and set up for optimization
     new_text_locations = text_locations.copy()
@@ -212,18 +287,21 @@
             alpha=0.0,
             fontfamily=fontfamily,
             fontsize=(
                 highlight_label_keywords.get("fontsize", font_size)
                 if label_text[i] in highlight
                 else font_size
             )
-            + (
-                label_size_adjustments[i] if label_size_adjustments is not None else 0.0
+            if font_sizes is None
+            else font_sizes[i],
+            fontweight=(
+                "bold"
+                if label_text[i] in highlight
+                else (font_weights[i] if font_weights is not None else fontweight)
             ),
-            fontweight="bold" if label_text[i] in highlight else "normal",
         )
         for i in range(label_locations.shape[0])
     ]
     coords = get_2d_coordinates(texts, expand=expand)
     xoverlaps = overlap_intervals(
         coords[:, 0], coords[:, 1], coords[:, 0], coords[:, 1]
     )
@@ -316,7 +394,75 @@
         fix_crossings(new_text_locations, label_locations)
         for i, text in enumerate(texts):
             text.set_position(new_text_locations[i])
 
         n_iter += 1
 
     return new_text_locations
+
+
+def pylabeladjust_text_locations(
+    label_locations,
+    label_text,
+    font_size=12,
+    font_sizes=None,
+    font_weights=None,
+    fontfamily="DejaVu Sans",
+    linespacing=0.95,
+    highlight=frozenset([]),
+    highlight_label_keywords={},
+    speed=None,
+    max_iterations=500,
+    adjust_by_size=True,
+    margin_percentage=7.5,
+    radius_scale=1.05,
+    ax=None,
+    fig=None,
+):
+    if ax is None:
+        ax = plt.gca()
+
+    if fig is None:
+        fig = plt.gcf()
+
+    if speed is None:
+        data_radius = np.max(row_norm(label_locations))
+        speed = data_radius / 125.0
+
+    # Add text to the axis and set up for optimization
+    new_text_locations = label_locations.copy()
+    texts = [
+        ax.text(
+            *new_text_locations[i],
+            label_text[i],
+            ha="center",
+            ma="center",
+            va="center",
+            linespacing=linespacing,
+            alpha=0.0,
+            fontfamily=fontfamily,
+            fontsize=(
+                highlight_label_keywords.get("fontsize", font_size)
+                if label_text[i] in highlight
+                else font_size
+            )
+            if font_sizes is None
+            else font_sizes[i],
+            fontweight=(
+                "bold"
+                if label_text[i] in highlight
+                else (font_weights[i] if font_weights is not None else "normal")
+            ),
+        )
+        for i in range(label_locations.shape[0])
+    ]
+    fig.canvas.draw()
+    rectangles_adjusted = adjust_texts(
+        texts,
+        speed=speed,
+        max_iterations=max_iterations,
+        adjust_by_size=adjust_by_size,
+        margin=margin_percentage,
+        margin_type="percentage",
+        radius_scale=radius_scale,
+    )
+    return rectangles_adjusted[["x_center", "y_center"]].values
```

### Comparing `datamapplot-0.2.2/datamapplot.egg-info/PKG-INFO` & `datamapplot-0.3.0/datamapplot.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datamapplot
-Version: 0.2.2
+Version: 0.3.0
 Summary: A library for presentation and publication ready plots of data maps
 Home-page: https://github.com/TutteInstitute/datamapplot
 Author: Leland McInnes
 Author-email: leland.mcinnes@gmail.com
 Maintainer: Leland McInnes
 Maintainer-email: leland.mcinnes@gmail.com
 License: MIT License
@@ -51,14 +51,21 @@
 Using darkmode and some custom font choices:
 
 .. image:: examples/plot_arxiv_ml.png
    :width: 1024
    :alt: A data map plot of papers from ArXiv ML
    :align: center
 
+With labels over points in a word-cloud style:
+
+.. image:: examples/plot_arxiv_ml_word_cloud.png
+   :width: 1024
+   :alt: A word cloud style data map plot of papers from ArXiv ML
+   :align: center
+
 Alternative custom styling:
 
 .. image:: examples/plot_wikipedia.png
    :width: 1024
    :alt: A data map plot of Simple Wikipedia
    :align: center
```

### Comparing `datamapplot-0.2.2/datamapplot.egg-info/SOURCES.txt` & `datamapplot-0.3.0/datamapplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datamapplot-0.2.2/setup.cfg` & `datamapplot-0.3.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = datamapplot
-version = 0.2.2
+version = 0.3.0
 author = Leland McInnes
 author_email = leland.mcinnes@gmail.com
 maintainer = Leland McInnes
 maintainer_email = leland.mcinnes@gmail.com
 description = A library for presentation and publication ready plots of data maps
 long_description = file: README.rst
 keywords = data map, visualization, topic modelling, cluster, clustering
@@ -27,14 +27,15 @@
 	matplotlib>=3.8
 	scikit-learn>=1.1
 	pandas>=1.0
 	datashader>=0.16
 	colorspacious>=1.1
 	scikit-image>=0.22
 	numba>=0.56
+	pylabeladjust
 	requests
 	jinja2
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

