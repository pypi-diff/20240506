# Comparing `tmp/superqt-0.6.4.tar.gz` & `tmp/superqt-0.6.5.tar.gz`

## Comparing `superqt-0.6.4.tar` & `superqt-0.6.5.tar`

### file list

```diff
@@ -1,86 +1,86 @@
--rw-r--r--   0        0        0    23682 2020-02-02 00:00:00.000000 superqt-0.6.4/CHANGELOG.md
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/py.typed
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/cmap/__init__.py
--rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/cmap/_catalog_combo.py
--rw-r--r--   0        0        0     8144 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/cmap/_cmap_combo.py
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/cmap/_cmap_item_delegate.py
--rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/cmap/_cmap_line_edit.py
--rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/cmap/_cmap_utils.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/collapsible/__init__.py
--rw-r--r--   0        0        0     7923 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/collapsible/_collapsible.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/combobox/__init__.py
--rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/combobox/_color_combobox.py
--rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/combobox/_enum_combobox.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/combobox/_searchable_combo_box.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/elidable/__init__.py
--rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/elidable/_eliding.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/elidable/_eliding_label.py
--rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/elidable/_eliding_line_edit.py
--rw-r--r--   0        0        0     7883 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/fonticon/__init__.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/fonticon/_animations.py
--rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/fonticon/_iconfont.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/fonticon/_plugins.py
--rw-r--r--   0        0        0    20154 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/fonticon/_qfont_icon.py
--rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/iconify/__init__.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/qtcompat/__init__.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/selection/__init__.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/selection/_searchable_list_widget.py
--rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/selection/_searchable_tree_widget.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/sliders/__init__.py
--rw-r--r--   0        0        0    13740 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/sliders/_generic_range_slider.py
--rw-r--r--   0        0        0    20157 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/sliders/_generic_slider.py
--rw-r--r--   0        0        0    25134 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/sliders/_labeled.py
--rw-r--r--   0        0        0     9489 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/sliders/_range_style.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/sliders/_sliders.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/spinbox/__init__.py
--rw-r--r--   0        0        0     6826 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/spinbox/_intspin.py
--rw-r--r--   0        0        0     8685 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/spinbox/_quantity.py
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/utils/__init__.py
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/utils/_code_syntax_highlight.py
--rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/utils/_ensure_thread.py
--rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/utils/_errormsg_context.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/utils/_img_utils.py
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/utils/_message_handler.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/utils/_misc.py
--rw-r--r--   0        0        0    30760 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/utils/_qthreading.py
--rw-r--r--   0        0        0    14893 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/utils/_throttler.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 superqt-0.6.4/src/superqt/utils/_util.py
--rw-r--r--   0        0        0     5209 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/test_cmap.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/test_code_highlight.py
--rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/test_collapsible.py
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/test_color_combo.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/test_eliding_label.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/test_eliding_line_edit.py
--rw-r--r--   0        0        0     8719 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/test_ensure_thread.py
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/test_enum_comb_box.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/test_iconify.py
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/test_large_int_spinbox.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/test_qmessage_handler.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/test_quantity.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/test_searchable_combobox.py
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/test_searchable_list.py
--rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/test_searchable_tree.py
--rw-r--r--   0        0        0     7972 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/test_threadworker.py
--rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/test_throttler.py
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/test_utils.py
--rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/test_fonticon/test_fonticon.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/test_fonticon/test_plugins.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/test_fonticon/fixtures/fake_plugin/__init__.py
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/test_fonticon/fixtures/fake_plugin/icontest.ttf
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/test_fonticon/fixtures/fake_plugin.dist-info/METADATA
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/test_fonticon/fixtures/fake_plugin.dist-info/entry_points.txt
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/test_fonticon/fixtures/fake_plugin.dist-info/top_level.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/zz_test_sliders/__init__.py
--rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/zz_test_sliders/_testutil.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/zz_test_sliders/test_float.py
--rw-r--r--   0        0        0     6059 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/zz_test_sliders/test_generic_slider.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/zz_test_sliders/test_labeled_slider.py
--rw-r--r--   0        0        0     7726 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/zz_test_sliders/test_range_slider.py
--rw-r--r--   0        0        0     7654 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/zz_test_sliders/test_single_value_sliders.py
--rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 superqt-0.6.4/tests/zz_test_sliders/test_slider.py
--rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 superqt-0.6.4/.gitignore
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 superqt-0.6.4/LICENSE
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 superqt-0.6.4/README.md
--rw-r--r--   0        0        0     5655 2020-02-02 00:00:00.000000 superqt-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 superqt-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0    24220 2020-02-02 00:00:00.000000 superqt-0.6.5/CHANGELOG.md
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/py.typed
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/cmap/__init__.py
+-rw-r--r--   0        0        0     3548 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/cmap/_catalog_combo.py
+-rw-r--r--   0        0        0     8144 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/cmap/_cmap_combo.py
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/cmap/_cmap_item_delegate.py
+-rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/cmap/_cmap_line_edit.py
+-rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/cmap/_cmap_utils.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/collapsible/__init__.py
+-rw-r--r--   0        0        0     7923 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/collapsible/_collapsible.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/combobox/__init__.py
+-rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/combobox/_color_combobox.py
+-rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/combobox/_enum_combobox.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/combobox/_searchable_combo_box.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/elidable/__init__.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/elidable/_eliding.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/elidable/_eliding_label.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/elidable/_eliding_line_edit.py
+-rw-r--r--   0        0        0     7883 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/fonticon/__init__.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/fonticon/_animations.py
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/fonticon/_iconfont.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/fonticon/_plugins.py
+-rw-r--r--   0        0        0    20154 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/fonticon/_qfont_icon.py
+-rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/iconify/__init__.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/qtcompat/__init__.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/selection/__init__.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/selection/_searchable_list_widget.py
+-rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/selection/_searchable_tree_widget.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/sliders/__init__.py
+-rw-r--r--   0        0        0    14428 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/sliders/_generic_range_slider.py
+-rw-r--r--   0        0        0    20299 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/sliders/_generic_slider.py
+-rw-r--r--   0        0        0    26313 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/sliders/_labeled.py
+-rw-r--r--   0        0        0     9656 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/sliders/_range_style.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/sliders/_sliders.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/spinbox/__init__.py
+-rw-r--r--   0        0        0     6826 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/spinbox/_intspin.py
+-rw-r--r--   0        0        0     8685 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/spinbox/_quantity.py
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/utils/__init__.py
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/utils/_code_syntax_highlight.py
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/utils/_ensure_thread.py
+-rw-r--r--   0        0        0     6320 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/utils/_errormsg_context.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/utils/_img_utils.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/utils/_message_handler.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/utils/_misc.py
+-rw-r--r--   0        0        0    30760 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/utils/_qthreading.py
+-rw-r--r--   0        0        0    14893 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/utils/_throttler.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 superqt-0.6.5/src/superqt/utils/_util.py
+-rw-r--r--   0        0        0     5209 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_cmap.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_code_highlight.py
+-rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_collapsible.py
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_color_combo.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_eliding_label.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_eliding_line_edit.py
+-rw-r--r--   0        0        0     8719 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_ensure_thread.py
+-rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_enum_comb_box.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_iconify.py
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_large_int_spinbox.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_qmessage_handler.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_quantity.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_searchable_combobox.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_searchable_list.py
+-rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_searchable_tree.py
+-rw-r--r--   0        0        0     7972 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_threadworker.py
+-rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_throttler.py
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_utils.py
+-rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_fonticon/test_fonticon.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_fonticon/test_plugins.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_fonticon/fixtures/fake_plugin/__init__.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_fonticon/fixtures/fake_plugin/icontest.ttf
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_fonticon/fixtures/fake_plugin.dist-info/METADATA
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_fonticon/fixtures/fake_plugin.dist-info/entry_points.txt
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/test_fonticon/fixtures/fake_plugin.dist-info/top_level.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/zz_test_sliders/__init__.py
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/zz_test_sliders/_testutil.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/zz_test_sliders/test_float.py
+-rw-r--r--   0        0        0     6059 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/zz_test_sliders/test_generic_slider.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/zz_test_sliders/test_labeled_slider.py
+-rw-r--r--   0        0        0     7726 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/zz_test_sliders/test_range_slider.py
+-rw-r--r--   0        0        0     7654 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/zz_test_sliders/test_single_value_sliders.py
+-rw-r--r--   0        0        0     4217 2020-02-02 00:00:00.000000 superqt-0.6.5/tests/zz_test_sliders/test_slider.py
+-rw-r--r--   0        0        0     1016 2020-02-02 00:00:00.000000 superqt-0.6.5/.gitignore
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 superqt-0.6.5/LICENSE
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 superqt-0.6.5/README.md
+-rw-r--r--   0        0        0     5655 2020-02-02 00:00:00.000000 superqt-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     5697 2020-02-02 00:00:00.000000 superqt-0.6.5/PKG-INFO
```

### Comparing `superqt-0.6.4/CHANGELOG.md` & `superqt-0.6.5/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # Changelog
 
+## [v0.6.5](https://github.com/pyapp-kit/superqt/tree/v0.6.5) (2024-05-06)
+
+[Full Changelog](https://github.com/pyapp-kit/superqt/compare/v0.6.4...v0.6.5)
+
+**Fixed bugs:**
+
+- fix: fix a number of issues with Labeled and Range Sliders, add LabelsOnHandle mode. [\#242](https://github.com/pyapp-kit/superqt/pull/242) ([tlambert03](https://github.com/tlambert03))
+
+**Merged pull requests:**
+
+- ci: trying to fix tests on various platforms [\#243](https://github.com/pyapp-kit/superqt/pull/243) ([tlambert03](https://github.com/tlambert03))
+
 ## [v0.6.4](https://github.com/pyapp-kit/superqt/tree/v0.6.4) (2024-04-25)
 
 [Full Changelog](https://github.com/pyapp-kit/superqt/compare/v0.6.3...v0.6.4)
 
 **Fixed bugs:**
 
 - fix: fix inverted appearance [\#240](https://github.com/pyapp-kit/superqt/pull/240) ([tlambert03](https://github.com/tlambert03))
```

### Comparing `superqt-0.6.4/src/superqt/__init__.py` & `superqt-0.6.5/src/superqt/__init__.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/cmap/__init__.py` & `superqt-0.6.5/src/superqt/cmap/__init__.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/cmap/_catalog_combo.py` & `superqt-0.6.5/src/superqt/cmap/_catalog_combo.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/cmap/_cmap_combo.py` & `superqt-0.6.5/src/superqt/cmap/_cmap_combo.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/cmap/_cmap_item_delegate.py` & `superqt-0.6.5/src/superqt/cmap/_cmap_item_delegate.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/cmap/_cmap_line_edit.py` & `superqt-0.6.5/src/superqt/cmap/_cmap_line_edit.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/cmap/_cmap_utils.py` & `superqt-0.6.5/src/superqt/cmap/_cmap_utils.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/collapsible/_collapsible.py` & `superqt-0.6.5/src/superqt/collapsible/_collapsible.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/combobox/__init__.py` & `superqt-0.6.5/src/superqt/combobox/__init__.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/combobox/_color_combobox.py` & `superqt-0.6.5/src/superqt/combobox/_color_combobox.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/combobox/_enum_combobox.py` & `superqt-0.6.5/src/superqt/combobox/_enum_combobox.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/combobox/_searchable_combo_box.py` & `superqt-0.6.5/src/superqt/combobox/_searchable_combo_box.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/elidable/_eliding.py` & `superqt-0.6.5/src/superqt/elidable/_eliding.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/elidable/_eliding_label.py` & `superqt-0.6.5/src/superqt/elidable/_eliding_label.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/elidable/_eliding_line_edit.py` & `superqt-0.6.5/src/superqt/elidable/_eliding_line_edit.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/fonticon/__init__.py` & `superqt-0.6.5/src/superqt/fonticon/__init__.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/fonticon/_animations.py` & `superqt-0.6.5/src/superqt/fonticon/_animations.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/fonticon/_iconfont.py` & `superqt-0.6.5/src/superqt/fonticon/_iconfont.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/fonticon/_plugins.py` & `superqt-0.6.5/src/superqt/fonticon/_plugins.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/fonticon/_qfont_icon.py` & `superqt-0.6.5/src/superqt/fonticon/_qfont_icon.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/iconify/__init__.py` & `superqt-0.6.5/src/superqt/iconify/__init__.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/qtcompat/__init__.py` & `superqt-0.6.5/src/superqt/qtcompat/__init__.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/selection/_searchable_list_widget.py` & `superqt-0.6.5/src/superqt/selection/_searchable_list_widget.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/selection/_searchable_tree_widget.py` & `superqt-0.6.5/src/superqt/selection/_searchable_tree_widget.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/sliders/_generic_range_slider.py` & `superqt-0.6.5/src/superqt/sliders/_generic_range_slider.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         """Hide the bar between the first and last handle."""
         self.setBarVisible(False)
 
     def showBar(self) -> None:
         """Show the bar between the first and last handle."""
         self.setBarVisible(True)
 
-    def applyMacStylePatch(self) -> str:
+    def applyMacStylePatch(self) -> None:
         """Apply a QSS patch to fix sliders on macos>=12 with QT < 6.
 
         see [FAQ](../faq.md#sliders-not-dragging-properly-on-macos-12) for more details.
         """
         super().applyMacStylePatch()
         self._style._macpatch = True
 
@@ -120,29 +120,48 @@
     def sliderPosition(self):
         """Get current value of the widget as a tuple of integers.
 
         If tracking is enabled (the default) this will be identical to value().
         """
         return tuple(float(i) for i in self._position)
 
-    def setSliderPosition(self, pos: Union[float, Sequence[float]], index=None) -> None:
+    def setSliderPosition(  # type: ignore
+        self,
+        pos: Union[float, Sequence[float]],
+        index: Optional[int] = None,
+        *,
+        reversed: bool = False,
+    ) -> None:
         """Set current position of the handles with a sequence of integers.
 
-        If `pos` is a sequence, it must have the same length as `value()`.
-        If it is a scalar, index will be
+        Parameters
+        ----------
+        pos : Union[float, Sequence[float]]
+            The new position of the slider handle(s). If a sequence, it must have the
+            same length as `value()`. If it is a scalar, index will be used to set the
+            position of the handle at that index.
+        index : int | None
+            The index of the handle to set the position of. If None, the "pressedIndex"
+            will be used.
+        reversed : bool
+            Order in which to set the positions.  Can be useful when setting multiple
+            positions, to avoid intermediate overlapping values.
         """
         if isinstance(pos, (list, tuple)):
             val_len = len(self.value())
             if len(pos) != val_len:
                 msg = f"'sliderPosition' must have same length as 'value()' ({val_len})"
                 raise ValueError(msg)
             pairs = list(enumerate(pos))
         else:
             pairs = [(self._pressedIndex if index is None else index, pos)]
 
+        if reversed:
+            pairs = pairs[::-1]
+
         for idx, position in pairs:
             self._position[idx] = self._bound(position, idx)
 
         self._doSliderMove()
 
     def setStyleSheet(self, styleSheet: str) -> None:
         return super().setStyleSheet(self._patch_style(styleSheet))
@@ -218,15 +237,15 @@
             ref = self._position
         if self._bar_is_rigid:
             # NOTE: This assumes monotonically increasing slider positions
             if offset > 0 and ref[-1] + offset > self.maximum():
                 offset = self.maximum() - ref[-1]
             elif ref[0] + offset < self.minimum():
                 offset = self.minimum() - ref[0]
-        self.setSliderPosition([i + offset for i in ref])
+        self.setSliderPosition([i + offset for i in ref], reversed=offset > 0)
 
     def _fixStyleOption(self, option):
         pass
 
     @property
     def _optSliderPositions(self):
         return [self._to_qinteger_space(p - self._minimum) for p in self._position]
```

### Comparing `superqt-0.6.4/src/superqt/sliders/_generic_slider.py` & `superqt-0.6.5/src/superqt/sliders/_generic_slider.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         self.rangeChanged = self._frangeChanged
 
         self.setAttribute(Qt.WidgetAttribute.WA_Hover)
         self.setStyleSheet("")
         if USE_MAC_SLIDER_PATCH:
             self.applyMacStylePatch()
 
-    def applyMacStylePatch(self) -> str:
+    def applyMacStylePatch(self) -> None:
         """Apply a QSS patch to fix sliders on macos>=12 with QT < 6.
 
         see [FAQ](../faq.md#sliders-not-dragging-properly-on-macos-12) for more details.
         """
         self.setStyleSheet(MONTEREY_SLIDER_STYLES_FIX)
 
     # ###############  QtOverrides  #######################
@@ -338,16 +338,20 @@
         return self._type_cast(max(self._minimum, min(self._maximum, value)))
 
     def _fixStyleOption(self, option):
         option.sliderPosition = self._to_qinteger_space(self._position - self._minimum)
         option.sliderValue = self._to_qinteger_space(self._value - self._minimum)
 
     def _to_qinteger_space(self, val, _max=None):
+        """Converts a value to the internal integer space."""
         _max = _max or self.MAX_DISPLAY
-        return int(min(QOVERFLOW, val / (self._maximum - self._minimum) * _max))
+        range_ = self._maximum - self._minimum
+        if range_ == 0:
+            return self._minimum
+        return int(min(QOVERFLOW, val / range_ * _max))
 
     def _pick(self, pt: QPoint) -> int:
         return pt.x() if self.orientation() == Qt.Orientation.Horizontal else pt.y()
 
     def _setSteps(self, single: float, page: float):
         self._singleStep = single
         self._pageStep = page
```

### Comparing `superqt-0.6.4/src/superqt/sliders/_labeled.py` & `superqt-0.6.5/src/superqt/sliders/_labeled.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 import contextlib
 from enum import IntEnum, IntFlag, auto
 from functools import partial
 from typing import Any, Iterable, overload
 
-from qtpy.QtCore import QPoint, QSize, Qt, Signal
+from qtpy import QtGui
+from qtpy.QtCore import Property, QPoint, QSize, Qt, Signal
 from qtpy.QtGui import QFontMetrics, QValidator
 from qtpy.QtWidgets import (
     QAbstractSlider,
-    QApplication,
     QBoxLayout,
     QDoubleSpinBox,
     QHBoxLayout,
     QSlider,
     QSpinBox,
     QStyle,
     QStyleOptionSpinBox,
@@ -28,29 +28,30 @@
 
 class LabelPosition(IntEnum):
     NoLabel = 0
     LabelsAbove = auto()
     LabelsBelow = auto()
     LabelsRight = LabelsAbove
     LabelsLeft = LabelsBelow
+    LabelsOnHandle = auto()
 
 
 class EdgeLabelMode(IntFlag):
     NoLabel = 0
     LabelIsRange = auto()
     LabelIsValue = auto()
 
 
 class _SliderProxy:
     _slider: QSlider
 
-    def value(self) -> int:
+    def value(self) -> Any:
         return self._slider.value()
 
-    def setValue(self, value: int) -> None:
+    def setValue(self, value: Any) -> None:
         self._slider.setValue(value)
 
     def sliderPosition(self) -> int:
         return self._slider.sliderPosition()
 
     def setSliderPosition(self, pos: int) -> None:
         self._slider.setSliderPosition(pos)
@@ -154,14 +155,17 @@
             orientation = args[0]
     parent = kwargs.get("parent", parent)
     return parent, orientation
 
 
 class QLabeledSlider(_SliderProxy, QAbstractSlider):
     editingFinished = Signal()
+    _ivalueChanged = Signal(int)
+    _isliderMoved = Signal(int)
+    _irangeChanged = Signal(int, int)
 
     _slider_class = QSlider
     _slider: QSlider
 
     @overload
     def __init__(self, parent: QWidget | None = ...) -> None: ...
 
@@ -253,16 +257,14 @@
             if self.isVisible():
                 self._label.show()
             self._label.setMode(opt)
             self._label.setValue(self._slider.value())
             self.layout().setContentsMargins(0, 0, 0, 0)
         self._on_slider_range_changed(self.minimum(), self.maximum())
 
-        QApplication.processEvents()
-
     # putting this after labelMode methods for the sake of mypy
     EdgeLabelMode = EdgeLabelMode
 
     # --------------------- private api --------------------
 
     def _on_slider_range_changed(self, min_: int, max_: int) -> None:
         slash = " / " if self._edge_label_mode & EdgeLabelMode.LabelIsValue else ""
@@ -275,16 +277,17 @@
         self.valueChanged.emit(v)
 
     def _setValue(self, value: float) -> None:
         """Convert the value from float to int before setting the slider value."""
         self._slider.setValue(int(value))
 
     def _rename_signals(self) -> None:
-        # for subclasses
-        pass
+        self.valueChanged = self._ivalueChanged
+        self.sliderMoved = self._isliderMoved
+        self.rangeChanged = self._irangeChanged
 
 
 class QLabeledDoubleSlider(QLabeledSlider):
     _slider_class = QDoubleSlider
     _slider: QDoubleSlider
     _fvalueChanged = Signal(float)
     _fsliderMoved = Signal(float)
@@ -382,18 +385,18 @@
         """Return where/whether labels are shown adjacent to slider handles."""
         return self._handle_label_position
 
     def setHandleLabelPosition(self, opt: LabelPosition) -> None:
         """Set where/whether labels are shown adjacent to slider handles."""
         self._handle_label_position = opt
         for lbl in self._handle_labels:
-            if not opt:
-                lbl.hide()
-            else:
-                lbl.show()
+            lbl.setVisible(bool(opt))
+            trans = opt == LabelPosition.LabelsOnHandle
+            # TODO: make double clickable to edit
+            lbl.setAttribute(Qt.WidgetAttribute.WA_TransparentForMouseEvents, trans)
         self.setOrientation(self.orientation())
 
     def edgeLabelMode(self) -> EdgeLabelMode:
         """Return current `EdgeLabelMode`."""
         return self._edge_label_mode
 
     def setEdgeLabelMode(self, opt: EdgeLabelMode) -> None:
@@ -411,15 +414,14 @@
         if opt == EdgeLabelMode.LabelIsValue:
             v0, *_, v1 = self._slider.value()
             self._min_label.setValue(v0)
             self._max_label.setValue(v1)
         elif opt == EdgeLabelMode.LabelIsRange:
             self._min_label.setValue(self._slider.minimum())
             self._max_label.setValue(self._slider.maximum())
-        QApplication.processEvents()
         self._reposition_labels()
 
     def setRange(self, min: int, max: int) -> None:
         self._on_range_changed(min, max)
 
     def _add_labels(self, layout: QBoxLayout, inverted: bool = False) -> None:
         if inverted:
@@ -430,60 +432,65 @@
         layout.addWidget(self._slider)
         layout.addWidget(second)
 
     def setOrientation(self, orientation: Qt.Orientation) -> None:
         """Set orientation, value will be 'horizontal' or 'vertical'."""
         self._slider.setOrientation(orientation)
         inverted = self._slider.invertedAppearance()
+        marg = (0, 0, 0, 0)
         if orientation == Qt.Orientation.Vertical:
             layout: QBoxLayout = QVBoxLayout()
             layout.setSpacing(1)
             self._add_labels(layout, inverted=not inverted)
             # TODO: set margins based on label width
             if self._handle_label_position == LabelPosition.LabelsLeft:
                 marg = (30, 0, 0, 0)
-            elif self._handle_label_position == LabelPosition.NoLabel:
-                marg = (0, 0, 0, 0)
-            else:
+            elif self._handle_label_position == LabelPosition.LabelsRight:
                 marg = (0, 0, 20, 0)
             layout.setAlignment(Qt.AlignmentFlag.AlignCenter)
         else:
             layout = QHBoxLayout()
             layout.setSpacing(7)
             if self._handle_label_position == LabelPosition.LabelsBelow:
                 marg = (0, 0, 0, 25)
-            elif self._handle_label_position == LabelPosition.NoLabel:
-                marg = (0, 0, 0, 0)
-            else:
+            elif self._handle_label_position == LabelPosition.LabelsAbove:
                 marg = (0, 25, 0, 0)
             self._add_labels(layout, inverted=inverted)
 
         # remove old layout
         old_layout = self.layout()
         if old_layout is not None:
             QWidget().setLayout(old_layout)
 
         self.setLayout(layout)
         layout.setContentsMargins(*marg)
         super().setOrientation(orientation)
-        QApplication.processEvents()
         self._reposition_labels()
 
     def setInvertedAppearance(self, a0: bool) -> None:
         self._slider.setInvertedAppearance(a0)
         self.setOrientation(self._slider.orientation())
 
-    def resizeEvent(self, a0) -> None:
+    def resizeEvent(self, a0: Any) -> None:
         super().resizeEvent(a0)
         self._reposition_labels()
 
     # putting this after methods above for the sake of mypy
     LabelPosition = LabelPosition
     EdgeLabelMode = EdgeLabelMode
 
+    def _getBarColor(self) -> QtGui.QBrush:
+        return self._slider._style.brush(self._slider._styleOption)
+
+    def _setBarColor(self, color: str) -> None:
+        self._slider._style.brush_active = color
+
+    barColor = Property(QtGui.QBrush, _getBarColor, _setBarColor)
+    """The color of the bar between the first and last handle."""
+
     # ------------- private methods ----------------
     def _rename_signals(self) -> None:
         self.valueChanged = self._valueChanged
         self.sliderReleased = self._sliderReleased
         self.sliderPressed = self._sliderPressed
 
     def _reposition_labels(self) -> None:
@@ -491,28 +498,34 @@
             not self._handle_labels
             or self._handle_label_position == LabelPosition.NoLabel
         ):
             return
 
         horizontal = self.orientation() == Qt.Orientation.Horizontal
         labels_above = self._handle_label_position == LabelPosition.LabelsAbove
+        labels_on_handle = self._handle_label_position == LabelPosition.LabelsOnHandle
 
         last_edge = None
         labels: Iterable[tuple[int, SliderLabel]] = enumerate(self._handle_labels)
         if self._slider.invertedAppearance():
             labels = reversed(list(labels))
         for i, label in labels:
             rect = self._slider._handleRect(i)
-            dx = -label.width() / 2
+            dx = (-label.width() / 2) + 2
             dy = -label.height() / 2
-            if labels_above:
+            if labels_above:  # or on the right
                 if horizontal:
                     dy *= 3
                 else:
                     dx *= -1
+            elif labels_on_handle:
+                if horizontal:
+                    dy += 0.5
+                else:
+                    dx += 0.5
             else:
                 if horizontal:
                     dy *= -1
                 else:
                     dx *= 3
             pos = self._slider.mapToParent(rect.center())
             pos += QPoint(int(dx + self.label_shift_x), int(dy + self.label_shift_y))
@@ -521,14 +534,15 @@
                 if horizontal:
                     pos.setX(int(max(pos.x(), last_edge.x() + label.width() / 2 + 12)))
                 else:
                     pos.setY(int(min(pos.y(), last_edge.y() - label.height() / 2 - 4)))
             label.move(pos)
             last_edge = pos
             label.clearFocus()
+            label.raise_()
             label.show()
         self.update()
 
     def _min_label_edited(self, val: float) -> None:
         if self._edge_label_mode == EdgeLabelMode.LabelIsRange:
             self.setMinimum(val)
         else:
@@ -608,14 +622,23 @@
 
     def setDecimals(self, prec: int) -> None:
         self._min_label.setDecimals(prec)
         self._max_label.setDecimals(prec)
         for lbl in self._handle_labels:
             lbl.setDecimals(prec)
 
+    def _getBarColor(self) -> QtGui.QBrush:
+        return self._slider._style.brush(self._slider._styleOption)
+
+    def _setBarColor(self, color: str) -> None:
+        self._slider._style.brush_active = color
+
+    barColor = Property(QtGui.QBrush, _getBarColor, _setBarColor)
+    """The color of the bar between the first and last handle."""
+
 
 class SliderLabel(QDoubleSpinBox):
     def __init__(
         self,
         slider: QSlider,
         parent=None,
         alignment=Qt.AlignmentFlag.AlignCenter,
```

### Comparing `superqt-0.6.4/src/superqt/sliders/_range_style.py` & `superqt-0.6.5/src/superqt/sliders/_range_style.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import platform
 import re
 from dataclasses import dataclass, replace
 from typing import TYPE_CHECKING
 
-from qtpy import QT_VERSION
 from qtpy.QtCore import Qt
 from qtpy.QtGui import (
     QBrush,
     QColor,
     QGradient,
     QLinearGradient,
     QPalette,
@@ -136,31 +135,33 @@
     brush_disabled="#D2D2D2",
     horizontal_thickness=3,
     vertical_thickness=3,
     tick_bar_alpha=0.3,
     tick_offset=4,
 )
 
-if QT_VERSION and int(QT_VERSION.split(".")[0]) == 6:
-    CATALINA_STYLE = replace(CATALINA_STYLE, tick_offset=2)
+# I can no longer reproduce the cases in which this was necessary
+# if QT_VERSION and int(QT_VERSION.split(".")[0]) == 6:
+#     CATALINA_STYLE = replace(CATALINA_STYLE, tick_offset=2)
 
 BIG_SUR_STYLE = replace(
     CATALINA_STYLE,
     brush_active="#0A81FE",
     brush_inactive="#D5D5D5",
     brush_disabled="#E6E6E6",
     tick_offset=0,
     horizontal_thickness=4,
     vertical_thickness=4,
     h_offset=-2,
     tick_bar_alpha=0.2,
 )
 
-if QT_VERSION and int(QT_VERSION.split(".")[0]) == 6:
-    BIG_SUR_STYLE = replace(BIG_SUR_STYLE, tick_offset=-3)
+# I can no longer reproduce the cases in which this was necessary
+# if QT_VERSION and int(QT_VERSION.split(".")[0]) == 6:
+#     BIG_SUR_STYLE = replace(BIG_SUR_STYLE, tick_offset=-3)
 
 WINDOWS_STYLE = replace(
     BASE_STYLE,
     brush_active="#550179D7",
     brush_inactive="#330179D7",
     brush_disabled=None,
 )
@@ -225,26 +226,27 @@
         (?P<g>\d+),\s*
         (?P<b>\d+),?\s*(?P<a>\d+)?\)
     """,
     re.X,
 )
 
 
-def parse_color(color: str, default_attr) -> QColor | QGradient:
+def parse_color(color: str, default_attr: str) -> QColor | QGradient:
     qc = QColor(color)
     if qc.isValid():
         return qc
 
     match = rgba_pattern.search(color)
     if match:
         rgba = [int(x) if x else 255 for x in match.groups()]
         return QColor(*rgba)
 
     # try linear gradient:
     match = qlineargrad_pattern.search(color)
+    grad: QGradient
     if match:
         grad = QLinearGradient(*(float(i) for i in match.groups()[:4]))
         grad.setColorAt(0, QColor(match.groupdict()["stop0"]))
         grad.setColorAt(1, QColor(match.groupdict()["stop1"]))
         return grad
 
     # try linear gradient:
@@ -255,19 +257,19 @@
         grad.setColorAt(1, QColor(match.groupdict()["stop1"]))
         return grad
 
     # fallback to dark gray
     return QColor(getattr(SYSTEM_STYLE, default_attr))
 
 
-def update_styles_from_stylesheet(obj: _GenericRangeSlider):
+def update_styles_from_stylesheet(obj: _GenericRangeSlider) -> None:
     qss: str = obj.styleSheet()
 
     parent = obj.parent()
-    while parent is not None:
+    while parent and hasattr(parent, "styleSheet"):
         qss = parent.styleSheet() + qss
         parent = parent.parent()
     qss = QApplication.instance().styleSheet() + qss
     if not qss:
         return
     if MONTEREY_SLIDER_STYLES_FIX in qss:
         qss = qss.replace(MONTEREY_SLIDER_STYLES_FIX, "")
```

### Comparing `superqt-0.6.4/src/superqt/sliders/_sliders.py` & `superqt-0.6.5/src/superqt/sliders/_sliders.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/spinbox/_intspin.py` & `superqt-0.6.5/src/superqt/spinbox/_intspin.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/spinbox/_quantity.py` & `superqt-0.6.5/src/superqt/spinbox/_quantity.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/utils/__init__.py` & `superqt-0.6.5/src/superqt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/utils/_code_syntax_highlight.py` & `superqt-0.6.5/src/superqt/utils/_code_syntax_highlight.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/utils/_ensure_thread.py` & `superqt-0.6.5/src/superqt/utils/_ensure_thread.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # https://gist.github.com/FlorianRhiem/41a1ad9b694c14fb9ac3
 from __future__ import annotations
 
 from concurrent.futures import Future
+from contextlib import suppress
 from functools import wraps
 from typing import TYPE_CHECKING, Any, Callable, ClassVar, overload
 
 from qtpy.QtCore import (
     QCoreApplication,
     QMetaObject,
     QObject,
@@ -37,15 +38,16 @@
         self._kwargs = kwargs
         CallCallable.instances.append(self)
 
     @Slot()
     def call(self):
         CallCallable.instances.remove(self)
         res = self._callable(*self._args, **self._kwargs)
-        self.finished.emit(res)
+        with suppress(RuntimeError):
+            self.finished.emit(res)
 
 
 # fmt: off
 @overload
 def ensure_main_thread(
     await_return: Literal[True],
     timeout: int = 1000,
```

### Comparing `superqt-0.6.4/src/superqt/utils/_errormsg_context.py` & `superqt-0.6.5/src/superqt/utils/_errormsg_context.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/utils/_img_utils.py` & `superqt-0.6.5/src/superqt/utils/_img_utils.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/utils/_message_handler.py` & `superqt-0.6.5/src/superqt/utils/_message_handler.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/utils/_misc.py` & `superqt-0.6.5/src/superqt/utils/_misc.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/utils/_qthreading.py` & `superqt-0.6.5/src/superqt/utils/_qthreading.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/utils/_throttler.py` & `superqt-0.6.5/src/superqt/utils/_throttler.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/src/superqt/utils/_util.py` & `superqt-0.6.5/src/superqt/utils/_util.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/tests/test_cmap.py` & `superqt-0.6.5/tests/test_cmap.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/tests/test_code_highlight.py` & `superqt-0.6.5/tests/test_code_highlight.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/tests/test_collapsible.py` & `superqt-0.6.5/tests/test_collapsible.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/tests/test_color_combo.py` & `superqt-0.6.5/tests/test_color_combo.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/tests/test_eliding_label.py` & `superqt-0.6.5/tests/test_eliding_label.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/tests/test_eliding_line_edit.py` & `superqt-0.6.5/tests/test_eliding_line_edit.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/tests/test_ensure_thread.py` & `superqt-0.6.5/tests/test_ensure_thread.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/tests/test_enum_comb_box.py` & `superqt-0.6.5/tests/test_enum_comb_box.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/tests/test_iconify.py` & `superqt-0.6.5/tests/test_iconify.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/tests/test_large_int_spinbox.py` & `superqt-0.6.5/tests/test_large_int_spinbox.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/tests/test_qmessage_handler.py` & `superqt-0.6.5/tests/test_qmessage_handler.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/tests/test_quantity.py` & `superqt-0.6.5/tests/test_quantity.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/tests/test_searchable_combobox.py` & `superqt-0.6.5/tests/test_searchable_combobox.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/tests/test_searchable_list.py` & `superqt-0.6.5/tests/test_searchable_list.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/tests/test_searchable_tree.py` & `superqt-0.6.5/tests/test_searchable_tree.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/tests/test_threadworker.py` & `superqt-0.6.5/tests/test_threadworker.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/tests/test_throttler.py` & `superqt-0.6.5/tests/test_throttler.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/tests/test_utils.py` & `superqt-0.6.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/tests/test_fonticon/test_fonticon.py` & `superqt-0.6.5/tests/test_fonticon/test_fonticon.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/tests/test_fonticon/test_plugins.py` & `superqt-0.6.5/tests/test_fonticon/test_plugins.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/tests/test_fonticon/fixtures/fake_plugin/icontest.ttf` & `superqt-0.6.5/tests/test_fonticon/fixtures/fake_plugin/icontest.ttf`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/tests/zz_test_sliders/_testutil.py` & `superqt-0.6.5/tests/zz_test_sliders/_testutil.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/tests/zz_test_sliders/test_float.py` & `superqt-0.6.5/tests/zz_test_sliders/test_float.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/tests/zz_test_sliders/test_generic_slider.py` & `superqt-0.6.5/tests/zz_test_sliders/test_generic_slider.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/tests/zz_test_sliders/test_labeled_slider.py` & `superqt-0.6.5/tests/zz_test_sliders/test_labeled_slider.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/tests/zz_test_sliders/test_range_slider.py` & `superqt-0.6.5/tests/zz_test_sliders/test_range_slider.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/tests/zz_test_sliders/test_single_value_sliders.py` & `superqt-0.6.5/tests/zz_test_sliders/test_single_value_sliders.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/tests/zz_test_sliders/test_slider.py` & `superqt-0.6.5/tests/zz_test_sliders/test_slider.py`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/.gitignore` & `superqt-0.6.5/.gitignore`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/LICENSE` & `superqt-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/README.md` & `superqt-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/pyproject.toml` & `superqt-0.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `superqt-0.6.4/PKG-INFO` & `superqt-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: superqt
-Version: 0.6.4
+Version: 0.6.5
 Summary: Missing widgets and components for PyQt/PySide
 Project-URL: Documentation, https://pyapp-kit.github.io/superqt/
 Project-URL: Source, https://github.com/pyapp-kit/superqt
 Project-URL: Tracker, https://github.com/pyapp-kit/superqt/issues
 Project-URL: Changelog, https://github.com/pyapp-kit/superqt/blob/main/CHANGELOG.md
 Author-email: Talley Lambert <talley.lambert@gmail.com>
 License: BSD 3-Clause License
```

