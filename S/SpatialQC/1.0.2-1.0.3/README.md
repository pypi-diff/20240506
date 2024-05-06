# Comparing `tmp/SpatialQC-1.0.2.tar.gz` & `tmp/SpatialQC-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpatialQC-1.0.2.tar", last modified: Fri Feb 16 13:18:11 2024, max compression
+gzip compressed data, was "SpatialQC-1.0.3.tar", last modified: Mon May  6 04:26:18 2024, max compression
```

## Comparing `SpatialQC-1.0.2.tar` & `SpatialQC-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,23 @@
-drwxr-xr-x   0 mgy       (1000) mgy       (1000)        0 2024-02-16 13:18:11.264232 SpatialQC-1.0.2/
--rw-r--r--   0 mgy       (1000) mgy       (1000)      363 2024-02-16 13:18:11.264232 SpatialQC-1.0.2/PKG-INFO
-drwxr-xr-x   0 mgy       (1000) mgy       (1000)        0 2024-02-16 13:18:11.254232 SpatialQC-1.0.2/SpatialQC/
--rw-r--r--   0 mgy       (1000) mgy       (1000)        0 2024-02-16 12:16:59.000000 SpatialQC-1.0.2/SpatialQC/__init__.py
--rw-r--r--   0 mgy       (1000) mgy       (1000)    24150 2024-02-16 12:11:43.000000 SpatialQC-1.0.2/SpatialQC/__main__.py
--rw-r--r--   0 mgy       (1000) mgy       (1000)     6748 2024-02-16 12:11:43.000000 SpatialQC-1.0.2/SpatialQC/base_qc_plot.py
--rw-r--r--   0 mgy       (1000) mgy       (1000)     2823 2024-02-16 12:11:43.000000 SpatialQC-1.0.2/SpatialQC/basic_statistics.py
-drwxr-xr-x   0 mgy       (1000) mgy       (1000)        0 2024-02-16 13:18:11.254232 SpatialQC-1.0.2/SpatialQC/data/
--rw-r--r--   0 mgy       (1000) mgy       (1000)  8257536 2024-02-16 12:11:43.000000 SpatialQC-1.0.2/SpatialQC/data/cell_marker.db
--rw-r--r--   0 mgy       (1000) mgy       (1000)     2680 2024-02-16 12:11:43.000000 SpatialQC-1.0.2/SpatialQC/get_markers.py
--rw-r--r--   0 mgy       (1000) mgy       (1000)     2581 2024-02-16 12:11:43.000000 SpatialQC-1.0.2/SpatialQC/markers_detected_by_filter_cells_genes.py
--rw-r--r--   0 mgy       (1000) mgy       (1000)     2585 2024-02-16 12:11:43.000000 SpatialQC-1.0.2/SpatialQC/markers_detected_by_filter_cells_genes2.py
--rw-r--r--   0 mgy       (1000) mgy       (1000)     1939 2024-02-16 12:11:43.000000 SpatialQC-1.0.2/SpatialQC/markers_detected_by_ngenes_cellbin.py
--rw-r--r--   0 mgy       (1000) mgy       (1000)     8380 2024-02-16 12:11:43.000000 SpatialQC-1.0.2/SpatialQC/slice_score.py
-drwxr-xr-x   0 mgy       (1000) mgy       (1000)        0 2024-02-16 13:18:11.264232 SpatialQC-1.0.2/SpatialQC/templates/
--rw-r--r--   0 mgy       (1000) mgy       (1000)     7827 2024-02-16 12:11:43.000000 SpatialQC-1.0.2/SpatialQC/templates/report_template.html
--rw-r--r--   0 mgy       (1000) mgy       (1000)     4661 2024-02-16 12:11:43.000000 SpatialQC-1.0.2/SpatialQC/valid_cells.py
-drwxr-xr-x   0 mgy       (1000) mgy       (1000)        0 2024-02-16 13:18:11.254232 SpatialQC-1.0.2/SpatialQC.egg-info/
--rw-r--r--   0 mgy       (1000) mgy       (1000)      363 2024-02-16 13:18:11.000000 SpatialQC-1.0.2/SpatialQC.egg-info/PKG-INFO
--rw-r--r--   0 mgy       (1000) mgy       (1000)      607 2024-02-16 13:18:11.000000 SpatialQC-1.0.2/SpatialQC.egg-info/SOURCES.txt
--rw-r--r--   0 mgy       (1000) mgy       (1000)        1 2024-02-16 13:18:11.000000 SpatialQC-1.0.2/SpatialQC.egg-info/dependency_links.txt
--rw-r--r--   0 mgy       (1000) mgy       (1000)       54 2024-02-16 13:18:11.000000 SpatialQC-1.0.2/SpatialQC.egg-info/entry_points.txt
--rw-r--r--   0 mgy       (1000) mgy       (1000)       59 2024-02-16 13:18:11.000000 SpatialQC-1.0.2/SpatialQC.egg-info/requires.txt
--rw-r--r--   0 mgy       (1000) mgy       (1000)       10 2024-02-16 13:18:11.000000 SpatialQC-1.0.2/SpatialQC.egg-info/top_level.txt
--rw-r--r--   0 mgy       (1000) mgy       (1000)       38 2024-02-16 13:18:11.264232 SpatialQC-1.0.2/setup.cfg
--rw-r--r--   0 mgy       (1000) mgy       (1000)      741 2024-02-16 13:18:01.000000 SpatialQC-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:26:18.308769 SpatialQC-1.0.3/
+-rw-rw-rw-   0        0        0      408 2024-05-06 04:26:18.308769 SpatialQC-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-06 04:26:18.278799 SpatialQC-1.0.3/SpatialQC/
+-rw-rw-rw-   0        0        0        0 2024-05-05 16:49:48.000000 SpatialQC-1.0.3/SpatialQC/__init__.py
+-rw-rw-rw-   0        0        0    28498 2024-05-05 16:49:48.000000 SpatialQC-1.0.3/SpatialQC/__main__.py
+-rw-rw-rw-   0        0        0     6877 2024-05-05 16:49:48.000000 SpatialQC-1.0.3/SpatialQC/base_qc_plot.py
+-rw-rw-rw-   0        0        0     3071 2024-05-05 16:49:48.000000 SpatialQC-1.0.3/SpatialQC/basic_statistics.py
+-rw-rw-rw-   0        0        0      946 2024-05-05 16:49:48.000000 SpatialQC-1.0.3/SpatialQC/get_input.py
+-rw-rw-rw-   0        0        0     2680 2024-05-05 16:49:48.000000 SpatialQC-1.0.3/SpatialQC/get_markers.py
+-rw-rw-rw-   0        0        0     2673 2024-05-05 16:49:48.000000 SpatialQC-1.0.3/SpatialQC/markers_detected_by_filter_cells_genes.py
+-rw-rw-rw-   0        0        0     2585 2024-05-05 16:49:48.000000 SpatialQC-1.0.3/SpatialQC/markers_detected_by_filter_cells_genes2.py
+-rw-rw-rw-   0        0        0     1939 2024-05-05 16:49:48.000000 SpatialQC-1.0.3/SpatialQC/markers_detected_by_ngenes_cellbin.py
+-rw-rw-rw-   0        0        0     8443 2024-05-05 16:49:49.000000 SpatialQC-1.0.3/SpatialQC/slice_score.py
+-rw-rw-rw-   0        0        0     4661 2024-05-05 16:49:49.000000 SpatialQC-1.0.3/SpatialQC/valid_cells.py
+drwxrwxrwx   0        0        0        0 2024-05-06 04:26:18.308769 SpatialQC-1.0.3/SpatialQC.egg-info/
+-rw-rw-rw-   0        0        0      408 2024-05-06 04:26:17.000000 SpatialQC-1.0.3/SpatialQC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      559 2024-05-06 04:26:17.000000 SpatialQC-1.0.3/SpatialQC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 04:26:17.000000 SpatialQC-1.0.3/SpatialQC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-06 04:26:17.000000 SpatialQC-1.0.3/SpatialQC.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       77 2024-05-06 04:26:17.000000 SpatialQC-1.0.3/SpatialQC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-06 04:26:17.000000 SpatialQC-1.0.3/SpatialQC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 04:26:18.308769 SpatialQC-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      812 2024-05-06 04:25:48.000000 SpatialQC-1.0.3/setup.py
```

### Comparing `SpatialQC-1.0.2/SpatialQC/__main__.py` & `SpatialQC-1.0.3/SpatialQC/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,21 +14,22 @@
 
 
     def mround(match):
         return "{:.4f}".format(float(match.group()))
 
     parser = argparse.ArgumentParser(formatter_class=argparse.RawTextHelpFormatter)
     group0 = parser.add_argument_group('Required parameters')
-    group4 = parser.add_argument_group('Markers input options (From CellMarker2.0)')
-    group5 = parser.add_argument_group('Other parameters related to images in html reports')
     group1 = parser.add_argument_group('Modify the scoring rules for Slice Scores')
     group2 = parser.add_argument_group('Filter related parameters')
     group3 = parser.add_argument_group('Other options')
+    group4 = parser.add_argument_group('Markers input options (From CellMarker2.0)')
+    group5 = parser.add_argument_group('Other parameters related to images in html reports')
 
-    group0.add_argument('--adata', metavar='', help='The path to your adata file.')
+    group3.add_argument('--platform', metavar='', help = 'ST platform')
+    group0.add_argument('--input', metavar='', help='The path to your adata file.')
     group0.add_argument('--markers', metavar='', help='The path to your markers csv file. Prior knowledge,'
                         ' or scRNA-seq of the same tissue to find differential genes, or you may be able to find the '
                                                       'appropriate ones from the Markers input options below')
     group4.add_argument('--species', metavar='', help='The species of your sample.')
     group4.add_argument('--tissue_class', metavar='', help='The tissue class of your sample.')
     group4.add_argument('--tissue_type', metavar='', help='The tissue type of your sample.')
     group4.add_argument('--cancer_type', default='Normal', metavar='', help='The cancer type of your sample.'
@@ -110,126 +111,176 @@
     from . import basic_statistics
     from . import slice_score
     from . import markers_detected_by_ngenes_cellbin
     from . import markers_detected_by_filter_cells_genes
     from . import markers_detected_by_filter_cells_genes2
     from . import valid_cells
     from . import base_qc_plot
+    from . import get_input
 
+    #platform
+    if args.platform in ['Visium', 'Slide-seq', 'ST', 'DBiT-seq']:
+        args.doublet = args.doublet if args.doublet else False
+        args.n = args.n if args.n else 0.95
+        args.l = args.l if args.l else 0.99
+        args.s = args.s if args.s else 4
+        args.min_genes_list = args.min_genes_list if args.min_genes_list else [0, 200, 400, 600, 800, 1000, 1200]
+        args.min_genes_list2 = args.min_genes_list2 if args.min_genes_list2 else [0, 200, 400, 600, 800, 1000, 1200]
+        args.min_cells_list = args.min_cells_list if args.min_genes_list else [1, 2, 3, 4, 5]
+    elif args.platform in ['MERFISH', 'Xenium', 'CosMx', 'HybISS']:
+        args.doublet = args.doublet if args.doublet else True
+        args.n = args.n if args.n else 0.9
+        args.min_cells = args.min_cells if args.min_cells else 1
+        args.s = args.s if args.s else 3
+        args.min_genes_list = args.min_genes_list if args.min_genes_list else [0, 10, 20, 30, 40, 50]
+        args.min_genes_list2 = args.min_genes_list2 if args.min_genes_list2 else [0, 10, 20, 30, 40, 50]
+        args.min_cells_list = args.min_cells_list if args.min_genes_list else [1]
+        args.s2 = args.s2 if args.s2 else [0, 0, 1]
+    elif args.platform in ['Stereo-seq', 'Seq-scope', 'Pixel-seq', 'HDST', 'Visium HD']:
+        args.doublet = args.doublet if args.doublet else True
+        args.n = args.n if args.n else 0.7
+        args.l = args.l if args.l else 0.99
+        args.s = args.s if args.s else 4
+        args.min_genes_list = args.min_genes_list if args.min_genes_list else [0, 200, 400, 600, 800, 1000, 1200]
+        args.min_genes_list2 = args.min_genes_list2 if args.min_genes_list2 else [0, 200, 400, 600, 800, 1000, 1200]
+        args.min_cells_list = args.min_cells_list if args.min_genes_list else [0, 10, 20, 30, 40]
+    else:
+        if args.platform is not None:
+            raise ValueError(f"Invalid platform: {args.platform}")   
+            
+    if args.min_cells is None or args.min_cells == "None":
+            if args.markers == 'False':
+                raise ValueError("If --markers is False, --min_cells must be supplied")
+    
+    import os
+    _, file_extension = os.path.splitext(args.input)
 
-    adata = sc.read_h5ad(args.adata)
+    if file_extension == '.h5ad':
+        adata = sc.read_h5ad(args.input)
+    elif file_extension == '.rds':
+        adata = get_input.convert_to_anndata(args.input)
+    else:
+        print(f"Unsupported file types: {file_extension}")
+        
     sc.pp.filter_cells(adata, min_genes=1)
     sc.pp.filter_cells(adata, min_counts=1)
     sc.pp.filter_genes(adata, min_cells=1)
     ribo_genes = adata.var_names.str.startswith(tuple(args.ribo.split(',')))
     hb_genes = adata.var_names.str.startswith(tuple(args.hemo.split(',')))
     import numpy as np
+    from joblib import Parallel, delayed
     adata.obs['percent_hb'] = np.sum(
         adata[:, hb_genes].X, axis=1) / np.sum(adata.X, axis=1)
     adata.obs['percent_ribo'] = np.sum(
         adata[:, ribo_genes].X, axis=1) / np.sum(adata.X, axis=1)
     markers = None
     import pandas as pd
-    if args.markers is not None:
+    if args.markers is not None and args.markers != 'False':
         markers = pd.read_csv(args.markers).squeeze("columns").tolist()
+    elif args.markers == 'False':
+        markers = []
 
+    if args.slice_number == '1':
+        adata.obs['slice1']='slice1'
+        args.slice = 'slice1'
     button_plots = []
     slice_score_fig_all, modified_adata = slice_score.create_plot(
         adata, markers, args.species, args.tissue_class, args.tissue_type, args.cancer_type, slice=args.slice,
         mito=args.mito, mito_p=args.mito_percent, doublet=args.doublet, s1=args.s1, s2=args.s2, s3=args.s3, s4=args.s4, s5=args.s5,
         s6=args.s6, s7=args.s7, s8=args.s8)
     del adata
-    if modified_adata.obs[args.slice].nunique() > 6:
-        valid_cell_fig_all = valid_cells.create_plot1(modified_adata, slice=args.slice, min_genes_list2=args.min_genes_list2)
-    else:
-        valid_cell_fig_all = valid_cells.create_plot2(modified_adata, slice=args.slice, min_genes_list2=args.min_genes_list2)
-    from joblib import Parallel, delayed
-    functions_and_params = [
-        (basic_statistics.create_plot,
-         (modified_adata, markers, args.species, args.tissue_class, args.tissue_type, args.cancer_type, args.slice)),
-        (base_qc_plot.kde_dis, (modified_adata, 'n_counts')),
-        (base_qc_plot.kde_dis, (modified_adata, 'n_genes')),
-        (base_qc_plot.kde_dis, (modified_adata, 'log10GenesPerUMI')),
-        (base_qc_plot.plot_distribution, (modified_adata, 'percent_mt')),
-        (base_qc_plot.mito_ratio, (modified_adata, args.mito_percent)),
-        (base_qc_plot.plot_distribution, (modified_adata, 'percent_ribo')),
-        (base_qc_plot.plot_distribution, (modified_adata, 'percent_hb')),
-        (markers_detected_by_ngenes_cellbin.create_plot, (
-        modified_adata, markers, args.species, args.tissue_class, args.tissue_type, args.cancer_type, args.bin_value)),
-        (basic_statistics.cell_numbers_by_min_genes, (modified_adata, args.min_genes_list)),
-        (markers_detected_by_filter_cells_genes2.create_plot, (
-        modified_adata, markers, args.species, args.tissue_class, args.tissue_type, args.cancer_type,
-        args.min_genes_list, args.min_cells_list)),
-        (markers_detected_by_filter_cells_genes.create_plot, (
-        modified_adata, markers, args.species, args.tissue_class, args.tissue_type, args.cancer_type,
-        args.min_genes_list, args.min_cells_list))
-    ]
-    results = Parallel(n_jobs=args.j)(delayed(func)(*params) for func, params in functions_and_params)
-    (basic_statistics_fig_all, n_counts_per_cell_fig_all, n_genes_per_cell_fig_all, log10_genes_per_umi_fig_all, mito_box_fig_all,
-     mito_ratio_fig_all, ribo_fig_all, hb_fig_all, marker_proportion_fig_all, cell_number_fig_all, marker_post_min_genes_fig_all,
-     marker_detected_post_filter_fig_all) = results
-
-    button_plots.append({
-        'basic_statistics_all': {
-            'data': basic_statistics_fig_all['data'],
-            'layout': basic_statistics_fig_all['layout']
-        },
-        'slice_score_all': {
-            'data': slice_score_fig_all['data'],
-            'layout': slice_score_fig_all['layout']
-        },
-        'n_counts_per_cell_all': {
-            'data': n_counts_per_cell_fig_all['data'],
-            'layout': n_counts_per_cell_fig_all['layout']
-        },
-        'n_genes_per_cell_all': {
-            'data': n_genes_per_cell_fig_all['data'],
-            'layout': n_genes_per_cell_fig_all['layout']
-        },
-        'log10GenesPerUMI_all': {
-            'data': log10_genes_per_umi_fig_all['data'],
-            'layout': log10_genes_per_umi_fig_all['layout']
-        },
-        'mito_box_all': {
-            'data': mito_box_fig_all['data'],
-            'layout': mito_box_fig_all['layout']
-        },
-        'mito_ratio_all': {
-            'data': mito_ratio_fig_all['data'],
-            'layout': mito_ratio_fig_all['layout']
-        },
-        'ribo_all': {
-            'data': ribo_fig_all['data'],
-            'layout': ribo_fig_all['layout']
-        },
-        'hb_all': {
-            'data': hb_fig_all['data'],
-            'layout': hb_fig_all['layout']
-        },
-        'marker_proportion_all': {
-            'data': marker_proportion_fig_all['data'],
-            'layout': marker_proportion_fig_all['layout']
-        },
-        'valid_cell_all': {
-            'data': valid_cell_fig_all['data'],
-            'layout': valid_cell_fig_all['layout']
-        },
-        'cell_number_all': {
-            'data': cell_number_fig_all['data'],
-            'layout': cell_number_fig_all['layout']
-        },
-        'marker_post_min_cells_all': {
-            'data': marker_post_min_genes_fig_all['data'],
-            'layout': marker_post_min_genes_fig_all['layout']
-        },
-        'marker_detected_post_filter_all': {
-            'data': marker_detected_post_filter_fig_all['data'],
-            'layout': marker_detected_post_filter_fig_all['layout']
-        }
-    })
+    if args.slice_number == 'multiple':
+        if modified_adata.obs[args.slice].nunique() > 6:
+            valid_cell_fig_all = valid_cells.create_plot1(modified_adata, slice=args.slice, min_genes_list2=args.min_genes_list2)
+        else:
+            valid_cell_fig_all = valid_cells.create_plot2(modified_adata, slice=args.slice, min_genes_list2=args.min_genes_list2)
+
+        functions_and_params = [
+            (basic_statistics.create_plot,
+             (modified_adata, markers, args.species, args.tissue_class, args.tissue_type, args.cancer_type, args.slice)),
+            (base_qc_plot.kde_dis, (modified_adata, 'n_counts')),
+            (base_qc_plot.kde_dis, (modified_adata, 'n_genes')),
+            (base_qc_plot.kde_dis, (modified_adata, 'log10GenesPerUMI')),
+            (base_qc_plot.plot_distribution, (modified_adata, 'percent_mt')),
+            (base_qc_plot.mito_ratio, (modified_adata, args.mito_percent)),
+            (base_qc_plot.plot_distribution, (modified_adata, 'percent_ribo')),
+            (base_qc_plot.plot_distribution, (modified_adata, 'percent_hb')),
+            (markers_detected_by_ngenes_cellbin.create_plot, (
+            modified_adata, markers, args.species, args.tissue_class, args.tissue_type, args.cancer_type, args.bin_value)),
+            (basic_statistics.cell_numbers_by_min_genes, (modified_adata, args.min_genes_list)),
+            (markers_detected_by_filter_cells_genes2.create_plot, (
+            modified_adata, markers, args.species, args.tissue_class, args.tissue_type, args.cancer_type,
+            args.min_genes_list, args.min_cells_list)),
+            (markers_detected_by_filter_cells_genes.create_plot, (
+            modified_adata, markers, args.species, args.tissue_class, args.tissue_type, args.cancer_type,
+            args.min_genes_list, args.min_cells_list))
+        ]
+        results = Parallel(n_jobs=args.j)(delayed(func)(*params) for func, params in functions_and_params)
+        (basic_statistics_fig_all, n_counts_per_cell_fig_all, n_genes_per_cell_fig_all, log10_genes_per_umi_fig_all, mito_box_fig_all,
+         mito_ratio_fig_all, ribo_fig_all, hb_fig_all, marker_proportion_fig_all, cell_number_fig_all, marker_post_min_genes_fig_all,
+         marker_detected_post_filter_fig_all) = results
+
+        button_plots.append({
+            'basic_statistics_all': {
+                'data': basic_statistics_fig_all['data'],
+                'layout': basic_statistics_fig_all['layout']
+            },
+            'slice_score_all': {
+                'data': slice_score_fig_all['data'],
+                'layout': slice_score_fig_all['layout']
+            },
+            'n_counts_per_cell_all': {
+                'data': n_counts_per_cell_fig_all['data'],
+                'layout': n_counts_per_cell_fig_all['layout']
+            },
+            'n_genes_per_cell_all': {
+                'data': n_genes_per_cell_fig_all['data'],
+                'layout': n_genes_per_cell_fig_all['layout']
+            },
+            'log10GenesPerUMI_all': {
+                'data': log10_genes_per_umi_fig_all['data'],
+                'layout': log10_genes_per_umi_fig_all['layout']
+            },
+            'mito_box_all': {
+                'data': mito_box_fig_all['data'],
+                'layout': mito_box_fig_all['layout']
+            },
+            'mito_ratio_all': {
+                'data': mito_ratio_fig_all['data'],
+                'layout': mito_ratio_fig_all['layout']
+            },
+            'ribo_all': {
+                'data': ribo_fig_all['data'],
+                'layout': ribo_fig_all['layout']
+            },
+            'hb_all': {
+                'data': hb_fig_all['data'],
+                'layout': hb_fig_all['layout']
+            },
+            'marker_proportion_all': {
+                'data': marker_proportion_fig_all['data'],
+                'layout': marker_proportion_fig_all['layout']
+            },
+            'valid_cell_all': {
+                'data': valid_cell_fig_all['data'],
+                'layout': valid_cell_fig_all['layout']
+            },
+            'cell_number_all': {
+                'data': cell_number_fig_all['data'],
+                'layout': cell_number_fig_all['layout']
+            },
+            'marker_post_min_cells_all': {
+                'data': marker_post_min_genes_fig_all['data'],
+                'layout': marker_post_min_genes_fig_all['layout']
+            },
+            'marker_detected_post_filter_all': {
+                'data': marker_detected_post_filter_fig_all['data'],
+                'layout': marker_detected_post_filter_fig_all['layout']
+            }
+        })
 
     # for slice
     def process_slice(slice_id):
         bdata = modified_adata[modified_adata.obs[args.slice] == slice_id].copy()
         sc.pp.filter_genes(bdata, min_cells=1)
         basic_statistics_fig_slice = basic_statistics.create_plot(
             bdata, markers, args.species, args.tissue_class, args.tissue_type, args.cancer_type, slice=args.slice)
@@ -342,34 +393,39 @@
                 'layout': marker_post_min_genes_fig_slice['layout']
             },
             'marker_detected_post_filter_' + slice_id: {
                 'data': marker_detected_post_filter_fig_slice['data'],
                 'layout': marker_detected_post_filter_fig_slice['layout']
             }
         }
-    if args.slice_number == 'multiple':
-        slice_ids = modified_adata.obs[args.slice].unique()
-        results = Parallel(n_jobs=args.j)(
-            delayed(process_slice)(slice_id) for slice_id in modified_adata.obs[args.slice].unique())
-        button_plots.extend(results)
-        slice_names = list(slice_ids)
+
+    slice_ids = modified_adata.obs[args.slice].unique()
+    results = Parallel(n_jobs=args.j)(
+        delayed(process_slice)(slice_id) for slice_id in modified_adata.obs[args.slice].unique())
+    button_plots.extend(results)
+    slice_names = list(slice_ids)
+    if args.slice_number == '1':
+        for plot in button_plots:
+            if 'slice_score_all' in plot:
+                del plot['slice_score_all']
 
     # report
     import json
-    import os
     import plotly
     import re
     import gzip
     import base64
     js_data = json.dumps(button_plots, cls=plotly.utils.PlotlyJSONEncoder, separators=(',', ':'))
     js_data = re.sub(re.compile(r"\d+\.\d{8,}"), mround, js_data)
     js_data2 = gzip.compress(js_data.encode('utf-8'))
     js_data3 = base64.b64encode(js_data2).decode('utf-8')
-
-    slice_names_json = json.dumps(['all'] + slice_names)
+    if args.slice_number == 'multiple':
+        slice_names_json = json.dumps(['all'] + slice_names)
+    else:
+        slice_names_json = json.dumps(slice_names)
     dir1 = os.path.dirname(os.path.realpath(__file__))
     html_path = os.path.join(dir1, 'templates', 'report_template.html')
 
     with open(html_path, 'r') as f:
         template = f.read()
     html = template.replace('{{data}}', js_data3)
     html = html.replace('{{slice_names}}', f'{slice_names_json}')
@@ -377,44 +433,65 @@
     os.makedirs(args.output, exist_ok=True)
     output_directory = args.output
     with open(os.path.join(output_directory, args.o1), 'w') as f:
         f.write(html)
 
     # filter
     if args.f:
-        selected_slices = modified_adata.obs.groupby(args.slice)['cell_score'].median() > args.s
+        selected_slices = modified_adata.obs.groupby(args.slice)['cell_score'].median() >= args.s
+        selected_slices2 = modified_adata.obs.groupby(args.slice)['cell_score'].median()
+        for slice_name, score in selected_slices2.items():
+            print(f"{slice_name} score: {score}")
+
         cdata = modified_adata[modified_adata.obs[args.slice].isin(selected_slices[selected_slices].index)].copy()
         if cdata.obs['predicted_doublets'].isnull().any():
             print("Warning: 'predicted_doublets' contains null values. Maybe you need to double-check doublet")
+        detected_doublets_count = len(cdata) - len(cdata[cdata.obs['predicted_doublets'].isin([False, None])])
+        print(f"Number of detected doublets: {detected_doublets_count}")
         cdata = cdata[cdata.obs['predicted_doublets'].isin([False, None])].copy()
         if args.min_genes is None or args.min_genes == "None":
-            thresholds = cdata.obs.groupby(args.slice).apply(lambda group: group['n_genes'].quantile(1 - args.n))
+            if len(cdata.obs[args.slice].unique()) > 1:
+                thresholds = cdata.obs.groupby(args.slice).apply(lambda group: group['n_genes'].quantile(1 - args.n))
+            else:
+                thresholds = cdata.obs['n_genes'].quantile(1 - args.n)
             final_threshold = int(thresholds.min() / 10) * 10
-            print(f"Automatic threshold for n_genes is: {final_threshold}")
+            print(f"Automatic threshold for min_genes is: {final_threshold}")
         else:
             final_threshold = int(args.min_genes)
             print(f"Using user-provided min_genes: {final_threshold}")
+
         sc.pp.filter_cells(cdata, min_genes=final_threshold)
+        total_cells_count = len(cdata)
+        satisfactory_cells_count = len(cdata[cdata.obs['percent_mt'] <= args.mito_percent])
+        unsatisfactory_cells_count = total_cells_count - satisfactory_cells_count
+        print(
+            f"Count of cells with mitochondrial gene percentage greater than {args.mito_percent}: {unsatisfactory_cells_count}")
         cdata = cdata[cdata.obs['percent_mt'] <= args.mito_percent].copy()
         sc.pp.filter_genes(cdata, min_cells=1)
+        
         if args.min_cells is None or args.min_cells == "None":
             from .get_markers import get_markers_from_db
             markers = get_markers_from_db(args.species, args.tissue_class, args.tissue_type,
                                           args.cancer_type) if args.markers is None else pd.read_csv(
                 args.markers).squeeze(
                 "columns").tolist()
             i = list(set(markers).intersection(cdata.var_names))
             selected = cdata.var.loc[i]
             threshold = int(selected['n_cells'].quantile(1 - args.l))
-            print(f"The suitable threshold for n_cells is: {threshold}")
+            print(f"The suitable threshold for min_cells is: {threshold}")
         else:
-            threshold = int(args.min_cells)
+            threshold = int(args.min_cells) 
             print(f"Using user-provided min_cells: {threshold}")
+            
         sc.pp.filter_genes(cdata, min_cells=threshold)
+        num_cells, num_genes = cdata.shape
+        print(f"Number of cells after filtered: {num_cells}")
+        print(f"Number of genes after filtered: {num_genes}")
+
         cdata.obs = cdata.obs.drop(['percent.mt_score', 'log10GenesPerUMI_score', 'n_genes_score', 'markerDetectionRatio_score',
-         'markerProportion_score', 'markerCountsRatio_score', 'doublet_score', 'n_counts_score', 'cell_score', 'remain_ratio',
+         'markerProportion_score', 'markerCountsRatio_score', 'doublet_score', 'n_counts_score', 'remain_ratio',
                                     'marker_ratio', 'marker_exp', 'predicted_doublets'], axis=1)
         cdata.write(filename=os.path.join(output_directory, args.o2))
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `SpatialQC-1.0.2/SpatialQC/base_qc_plot.py` & `SpatialQC-1.0.3/SpatialQC/base_qc_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,24 +127,28 @@
     return {'data': fig['data'], 'layout': fig['layout']}
 
 
 def mito_ratio(adata, mito_percent=0.1):
     n_counts = adata.obs['n_counts']
     n_genes = adata.obs['n_genes']
     percent_mt = adata.obs['percent_mt']
+    if percent_mt.min() == 0 and percent_mt.max() == 0:
+        point_color = 'blue'
+    else:
+        point_color = percent_mt
     fig = go.Figure()
 
     fig.add_trace(
         go.Scattergl(
             x=n_counts,
             y=n_genes,
             mode='markers',
             marker=dict(
                 size=4,
-                color=percent_mt,
+                color=point_color,
                 colorscale='Greys',
                 colorbar=dict(title='Percent mt'),
                 cmin=0,
                 cmax=mito_percent,
                 symbol='circle',
             ),
             text='Ratio:' + percent_mt.astype(str),
```

### Comparing `SpatialQC-1.0.2/SpatialQC/basic_statistics.py` & `SpatialQC-1.0.3/SpatialQC/basic_statistics.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,20 +6,26 @@
 @marker_decorator
 def basic_statistics(adata, markers, slice='id'):
     cell_count = adata.shape[0]
     gene_count = adata.shape[1]
     slice_count = adata.obs[slice].nunique()
     median_n_genes = adata.obs['n_genes'].median()
     mean_n_genes = adata.obs['n_genes'].mean()
-    median_n_UMIs = adata.obs['n_counts'].median()
-    mean_n_UMIs = adata.obs['n_counts'].mean()
-    provided_marker_counts = len(set(markers))
-    detected_marker_counts = len(set(markers).intersection(adata.var_names))
-    marker_detected_ratio = detected_marker_counts / len(set(markers))
-    marker_proportion = detected_marker_counts / gene_count
+    median_n_UMIs = adata.obs['n_counts'].copy().median()
+    mean_n_UMIs = adata.obs['n_counts'].copy().mean()
+    if len(set(markers)) > 0:
+        provided_marker_counts = len(set(markers))
+        detected_marker_counts = len(set(markers).intersection(adata.var_names))
+        marker_detected_ratio = detected_marker_counts / len(set(markers))
+        marker_proportion = detected_marker_counts / gene_count
+    else:
+        provided_marker_counts = float('NaN')
+        detected_marker_counts = float('NaN')
+        marker_detected_ratio = float('NaN')
+        marker_proportion = float('NaN')
     doublet_count = adata.obs['predicted_doublets'].sum()
 
     data = [['Measure', 'Value'],
             ['Slice counts', slice_count],
             ['Cell counts', cell_count],
             ['Gene counts', gene_count],
             ['Median n_genes', median_n_genes],
```

### Comparing `SpatialQC-1.0.2/SpatialQC/get_markers.py` & `SpatialQC-1.0.3/SpatialQC/get_markers.py`

 * *Files identical despite different names*

### Comparing `SpatialQC-1.0.2/SpatialQC/markers_detected_by_filter_cells_genes.py` & `SpatialQC-1.0.3/SpatialQC/markers_detected_by_filter_cells_genes.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,18 @@
             if issparse(adata.X):
                 new_n_cells = adata.X[adata.obs_names.isin(remaining_cells),].getnnz(axis=0)
             else:
                 new_n_cells = np.count_nonzero(adata.X[adata.obs_names.isin(remaining_cells),], axis=0)
             valid_genes = new_n_cells >= frac
             remaining_genes = adata.var_names[valid_genes].tolist()
             overlap_genes = set(remaining_genes).intersection(markers_set)
-            marker_overlap_percent = len(overlap_genes) / counts
+            if counts > 0:
+                marker_overlap_percent = len(overlap_genes) / counts
+            else:
+                marker_overlap_percent = 0
             marker_overlap[frac].append(marker_overlap_percent)
 
     fig = go.Figure()
     
     for frac in min_cells_list:
         fig.add_trace(go.Scatter(x=min_genes_list, y=marker_overlap[frac], mode='lines', name=f'min_cells={frac}'))
```

### Comparing `SpatialQC-1.0.2/SpatialQC/markers_detected_by_filter_cells_genes2.py` & `SpatialQC-1.0.3/SpatialQC/markers_detected_by_filter_cells_genes2.py`

 * *Files identical despite different names*

### Comparing `SpatialQC-1.0.2/SpatialQC/markers_detected_by_ngenes_cellbin.py` & `SpatialQC-1.0.3/SpatialQC/markers_detected_by_ngenes_cellbin.py`

 * *Files identical despite different names*

### Comparing `SpatialQC-1.0.2/SpatialQC/slice_score.py` & `SpatialQC-1.0.3/SpatialQC/slice_score.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
     if issparse(adata.X):
         adata.obs['marker_exp'] = np.sum(adata[:, common_genes].X, axis=1).A1 / adata.obs['n_counts']
     else:
         adata.obs['marker_exp'] = np.sum(adata[:, common_genes].X, axis=1) / adata.obs['n_counts']
 
     if doublet:
+        adata.obs[slice] = adata.obs[slice].astype('category')
         slice_list = adata.obs[slice].cat.categories.tolist()
         alldata = {}
         for i in slice_list:
             adata_filtered = adata[adata.obs[slice] == i,]
             scrub = scr.Scrublet(adata_filtered.X)
             out = scrub.scrub_doublets(verbose=False)
             alldata[i] = pd.DataFrame({'doublet_score': out[0], 'predicted_doublets': out[1]},
```

### Comparing `SpatialQC-1.0.2/SpatialQC/valid_cells.py` & `SpatialQC-1.0.3/SpatialQC/valid_cells.py`

 * *Files identical despite different names*

### Comparing `SpatialQC-1.0.2/SpatialQC.egg-info/SOURCES.txt` & `SpatialQC-1.0.3/SpatialQC.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 setup.py
 SpatialQC/__init__.py
 SpatialQC/__main__.py
 SpatialQC/base_qc_plot.py
 SpatialQC/basic_statistics.py
+SpatialQC/get_input.py
 SpatialQC/get_markers.py
 SpatialQC/markers_detected_by_filter_cells_genes.py
 SpatialQC/markers_detected_by_filter_cells_genes2.py
 SpatialQC/markers_detected_by_ngenes_cellbin.py
 SpatialQC/slice_score.py
 SpatialQC/valid_cells.py
 SpatialQC.egg-info/PKG-INFO
 SpatialQC.egg-info/SOURCES.txt
 SpatialQC.egg-info/dependency_links.txt
 SpatialQC.egg-info/entry_points.txt
 SpatialQC.egg-info/requires.txt
-SpatialQC.egg-info/top_level.txt
-SpatialQC/data/cell_marker.db
-SpatialQC/templates/report_template.html
+SpatialQC.egg-info/top_level.txt
```

### Comparing `SpatialQC-1.0.2/setup.py` & `SpatialQC-1.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 
 setup(
     name='SpatialQC',
-    version='1.0.2',
+    version='1.0.3',
     description=('Spatial transcriptome quality control, generate HTML QC report, obtain filtered clean data'
     ),
     author='Mao Guangyao',
     url='https://github.com/mgy520/SpatialQC',
     packages=find_packages(),
     include_package_data=True,
-    package_data={'SpatialQC': ['data/*.db', 'templates/*.html']},
+    package_data={
+        'SpatialQC.data': ['*.db'],
+        'SpatialQC.templates': ['*.html'],
+    },
     entry_points={
         'console_scripts': [
             'SpatialQC = SpatialQC.__main__:main',
         ]
     },
-    python_requires='>=3.8',
+    python_requires='==3.8',
     install_requires=[
-            'scanpy>=1.9.6',
-            'joblib>=1.2.0',
-            'plotly>=5.18.0',
-            'scrublet>=0.2.3'
+            'scanpy==1.9.8',
+            'joblib==1.4.2',
+            'plotly==5.22.0',
+            'scrublet==0.2.3',
+            'anndata2ri==1.3.1'
             ]
 )
```

