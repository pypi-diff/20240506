# Comparing `tmp/conan-2.2.3.tar.gz` & `tmp/conan-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/conan-2.2.3.tar", last modified: Wed Apr 17 15:52:04 2024, max compression
+gzip compressed data, was "dist/conan-2.3.0.tar", last modified: Mon May  6 16:43:40 2024, max compression
```

## Comparing `conan-2.2.3.tar` & `conan-2.3.0.tar`

### file list

```diff
@@ -1,368 +1,376 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.672693 conan-2.2.3/
--rw-r--r--   0 root         (0) root         (0)     1084 2024-04-17 15:51:55.000000 conan-2.2.3/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)       18 2024-04-17 15:51:55.000000 conan-2.2.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8618 2024-04-17 15:52:04.672693 conan-2.2.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6335 2024-04-17 15:51:55.000000 conan-2.2.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.635690 conan-2.2.3/conan/
--rw-r--r--   0 root         (0) root         (0)      165 2024-04-17 15:51:55.000000 conan-2.2.3/conan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.636690 conan-2.2.3/conan/api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 15:51:55.000000 conan-2.2.3/conan/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2455 2024-04-17 15:51:55.000000 conan-2.2.3/conan/api/conan_api.py
--rw-r--r--   0 root         (0) root         (0)    12046 2024-04-17 15:51:55.000000 conan-2.2.3/conan/api/model.py
--rw-r--r--   0 root         (0) root         (0)     9460 2024-04-17 15:51:55.000000 conan-2.2.3/conan/api/output.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.638690 conan-2.2.3/conan/api/subapi/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 15:51:55.000000 conan-2.2.3/conan/api/subapi/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11757 2024-04-17 15:51:55.000000 conan-2.2.3/conan/api/subapi/cache.py
--rw-r--r--   0 root         (0) root         (0)      756 2024-04-17 15:51:55.000000 conan-2.2.3/conan/api/subapi/command.py
--rw-r--r--   0 root         (0) root         (0)     9255 2024-04-17 15:51:55.000000 conan-2.2.3/conan/api/subapi/config.py
--rw-r--r--   0 root         (0) root         (0)     4793 2024-04-17 15:51:55.000000 conan-2.2.3/conan/api/subapi/download.py
--rw-r--r--   0 root         (0) root         (0)     2714 2024-04-17 15:51:55.000000 conan-2.2.3/conan/api/subapi/export.py
--rw-r--r--   0 root         (0) root         (0)    11805 2024-04-17 15:51:55.000000 conan-2.2.3/conan/api/subapi/graph.py
--rw-r--r--   0 root         (0) root         (0)     3961 2024-04-17 15:51:55.000000 conan-2.2.3/conan/api/subapi/install.py
--rw-r--r--   0 root         (0) root         (0)    17548 2024-04-17 15:51:55.000000 conan-2.2.3/conan/api/subapi/list.py
--rw-r--r--   0 root         (0) root         (0)     5465 2024-04-17 15:51:55.000000 conan-2.2.3/conan/api/subapi/local.py
--rw-r--r--   0 root         (0) root         (0)     4808 2024-04-17 15:51:55.000000 conan-2.2.3/conan/api/subapi/lockfile.py
--rw-r--r--   0 root         (0) root         (0)     5193 2024-04-17 15:51:55.000000 conan-2.2.3/conan/api/subapi/new.py
--rw-r--r--   0 root         (0) root         (0)     7441 2024-04-17 15:51:55.000000 conan-2.2.3/conan/api/subapi/profiles.py
--rw-r--r--   0 root         (0) root         (0)    13285 2024-04-17 15:51:55.000000 conan-2.2.3/conan/api/subapi/remotes.py
--rw-r--r--   0 root         (0) root         (0)     2176 2024-04-17 15:51:55.000000 conan-2.2.3/conan/api/subapi/remove.py
--rw-r--r--   0 root         (0) root         (0)     1117 2024-04-17 15:51:55.000000 conan-2.2.3/conan/api/subapi/search.py
--rw-r--r--   0 root         (0) root         (0)     6670 2024-04-17 15:51:55.000000 conan-2.2.3/conan/api/subapi/upload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.639690 conan-2.2.3/conan/cli/
--rw-r--r--   0 root         (0) root         (0)      397 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7430 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/args.py
--rw-r--r--   0 root         (0) root         (0)    11875 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/cli.py
--rw-r--r--   0 root         (0) root         (0)     8279 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.642690 conan-2.2.3/conan/cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3994 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/commands/build.py
--rw-r--r--   0 root         (0) root         (0)     7489 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/commands/cache.py
--rw-r--r--   0 root         (0) root         (0)     4609 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/commands/config.py
--rw-r--r--   0 root         (0) root         (0)     9158 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/commands/create.py
--rw-r--r--   0 root         (0) root         (0)     3252 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/commands/download.py
--rw-r--r--   0 root         (0) root         (0)     3157 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/commands/editable.py
--rw-r--r--   0 root         (0) root         (0)     3021 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/commands/export.py
--rw-r--r--   0 root         (0) root         (0)     5798 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/commands/export_pkg.py
--rw-r--r--   0 root         (0) root         (0)    21433 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/commands/graph.py
--rw-r--r--   0 root         (0) root         (0)     2495 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/commands/inspect.py
--rw-r--r--   0 root         (0) root         (0)     4704 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/commands/install.py
--rw-r--r--   0 root         (0) root         (0)    13371 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/commands/list.py
--rw-r--r--   0 root         (0) root         (0)     7511 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/commands/lock.py
--rw-r--r--   0 root         (0) root         (0)     4258 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/commands/new.py
--rw-r--r--   0 root         (0) root         (0)     3244 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/commands/profile.py
--rw-r--r--   0 root         (0) root         (0)    12835 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/commands/remote.py
--rw-r--r--   0 root         (0) root         (0)     6487 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/commands/remove.py
--rw-r--r--   0 root         (0) root         (0)     1787 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/commands/search.py
--rw-r--r--   0 root         (0) root         (0)      753 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/commands/source.py
--rw-r--r--   0 root         (0) root         (0)     4411 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/commands/test.py
--rw-r--r--   0 root         (0) root         (0)     6871 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/commands/upload.py
--rw-r--r--   0 root         (0) root         (0)      653 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/commands/version.py
--rw-r--r--   0 root         (0) root         (0)      490 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/exit_codes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.642690 conan-2.2.3/conan/cli/formatters/
--rw-r--r--   0 root         (0) root         (0)      158 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/formatters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.642690 conan-2.2.3/conan/cli/formatters/graph/
--rw-r--r--   0 root         (0) root         (0)      110 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/formatters/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5535 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/formatters/graph/graph.py
--rw-r--r--   0 root         (0) root         (0)     1689 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/formatters/graph/graph_info_text.py
--rw-r--r--   0 root         (0) root         (0)      144 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/formatters/graph/info_graph_dot.py
--rw-r--r--   0 root         (0) root         (0)    14752 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/formatters/graph/info_graph_html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.643690 conan-2.2.3/conan/cli/formatters/list/
--rw-r--r--   0 root         (0) root         (0)       37 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/formatters/list/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4612 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/formatters/list/binary_html_table.py
--rw-r--r--   0 root         (0) root         (0)      939 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/formatters/list/list.py
--rw-r--r--   0 root         (0) root         (0)    12834 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/formatters/list/search_table_html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.643690 conan-2.2.3/conan/cli/printers/
--rw-r--r--   0 root         (0) root         (0)      331 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/printers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6412 2024-04-17 15:51:55.000000 conan-2.2.3/conan/cli/printers/graph.py
--rw-r--r--   0 root         (0) root         (0)      139 2024-04-17 15:51:55.000000 conan-2.2.3/conan/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.644690 conan-2.2.3/conan/internal/
--rw-r--r--   0 root         (0) root         (0)      419 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.644690 conan-2.2.3/conan/internal/api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19809 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/api/detect_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.646690 conan-2.2.3/conan/internal/api/new/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/api/new/__init__.py
--rw-r--r--   0 root         (0) root         (0)      293 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/api/new/alias_new.py
--rw-r--r--   0 root         (0) root         (0)     2716 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/api/new/autoools_exe.py
--rw-r--r--   0 root         (0) root         (0)     3810 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/api/new/autotools_lib.py
--rw-r--r--   0 root         (0) root         (0)     2916 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/api/new/basic.py
--rw-r--r--   0 root         (0) root         (0)     2041 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/api/new/bazel_exe.py
--rw-r--r--   0 root         (0) root         (0)     4565 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/api/new/bazel_lib.py
--rw-r--r--   0 root         (0) root         (0)     2932 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/api/new/cmake_exe.py
--rw-r--r--   0 root         (0) root         (0)     8212 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/api/new/cmake_lib.py
--rw-r--r--   0 root         (0) root         (0)     3213 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/api/new/local_recipes_index.py
--rw-r--r--   0 root         (0) root         (0)     2334 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/api/new/meson_exe.py
--rw-r--r--   0 root         (0) root         (0)     2769 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/api/new/meson_lib.py
--rw-r--r--   0 root         (0) root         (0)     2207 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/api/new/msbuild_exe.py
--rw-r--r--   0 root         (0) root         (0)    12307 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/api/new/msbuild_lib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.646690 conan-2.2.3/conan/internal/cache/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11189 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/cache/cache.py
--rw-r--r--   0 root         (0) root         (0)     4083 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/cache/conan_reference_layout.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.647691 conan-2.2.3/conan/internal/cache/db/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/cache/db/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3949 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/cache/db/cache_database.py
--rw-r--r--   0 root         (0) root         (0)     9222 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/cache/db/packages_table.py
--rw-r--r--   0 root         (0) root         (0)     5477 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/cache/db/recipes_table.py
--rw-r--r--   0 root         (0) root         (0)     2639 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/cache/db/table.py
--rw-r--r--   0 root         (0) root         (0)     2515 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/cache/home_paths.py
--rw-r--r--   0 root         (0) root         (0)     3114 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/conan_app.py
--rw-r--r--   0 root         (0) root         (0)     5045 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/deploy.py
--rw-r--r--   0 root         (0) root         (0)     3098 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/integrity_check.py
--rw-r--r--   0 root         (0) root         (0)      922 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/internal_tools.py
--rw-r--r--   0 root         (0) root         (0)     1570 2024-04-17 15:51:55.000000 conan-2.2.3/conan/internal/upload_metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.647691 conan-2.2.3/conan/tools/
--rw-r--r--   0 root         (0) root         (0)      384 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.647691 conan-2.2.3/conan/tools/android/
--rw-r--r--   0 root         (0) root         (0)       50 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/android/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1138 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/android/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.648691 conan-2.2.3/conan/tools/apple/
--rw-r--r--   0 root         (0) root         (0)      534 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/apple/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11835 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/apple/apple.py
--rw-r--r--   0 root         (0) root         (0)     2127 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/apple/xcodebuild.py
--rw-r--r--   0 root         (0) root         (0)    16239 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/apple/xcodedeps.py
--rw-r--r--   0 root         (0) root         (0)     5754 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/apple/xcodetoolchain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.648691 conan-2.2.3/conan/tools/build/
--rw-r--r--   0 root         (0) root         (0)     4190 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/build/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11121 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/build/cppstd.py
--rw-r--r--   0 root         (0) root         (0)     2216 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/build/cpu.py
--rw-r--r--   0 root         (0) root         (0)     2302 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/build/cross_building.py
--rw-r--r--   0 root         (0) root         (0)    16208 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/build/flags.py
--rw-r--r--   0 root         (0) root         (0)      563 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/build/stdcpp_library.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.649691 conan-2.2.3/conan/tools/cmake/
--rw-r--r--   0 root         (0) root         (0)      217 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/cmake/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14472 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/cmake/cmake.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.649691 conan-2.2.3/conan/tools/cmake/cmakedeps/
--rw-r--r--   0 root         (0) root         (0)      104 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/cmake/cmakedeps/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10886 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/cmake/cmakedeps/cmakedeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.650691 conan-2.2.3/conan/tools/cmake/cmakedeps/templates/
--rw-r--r--   0 root         (0) root         (0)     3944 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/cmake/cmakedeps/templates/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4451 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/cmake/cmakedeps/templates/config.py
--rw-r--r--   0 root         (0) root         (0)     4061 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/cmake/cmakedeps/templates/config_version.py
--rw-r--r--   0 root         (0) root         (0)     5956 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/cmake/cmakedeps/templates/macros.py
--rw-r--r--   0 root         (0) root         (0)    14900 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/cmake/cmakedeps/templates/target_configuration.py
--rw-r--r--   0 root         (0) root         (0)    20156 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/cmake/cmakedeps/templates/target_data.py
--rw-r--r--   0 root         (0) root         (0)     3656 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/cmake/cmakedeps/templates/targets.py
--rw-r--r--   0 root         (0) root         (0)     4746 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/cmake/layout.py
--rw-r--r--   0 root         (0) root         (0)    16611 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/cmake/presets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.650691 conan-2.2.3/conan/tools/cmake/toolchain/
--rw-r--r--   0 root         (0) root         (0)       52 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/cmake/toolchain/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45120 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/cmake/toolchain/blocks.py
--rw-r--r--   0 root         (0) root         (0)    13892 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/cmake/toolchain/toolchain.py
--rw-r--r--   0 root         (0) root         (0)      171 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/cmake/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.651691 conan-2.2.3/conan/tools/env/
--rw-r--r--   0 root         (0) root         (0)      168 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/env/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26546 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/env/environment.py
--rw-r--r--   0 root         (0) root         (0)     3601 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/env/virtualbuildenv.py
--rw-r--r--   0 root         (0) root         (0)     3561 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/env/virtualrunenv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.652691 conan-2.2.3/conan/tools/files/
--rw-r--r--   0 root         (0) root         (0)      535 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/files/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2672 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/files/conandata.py
--rw-r--r--   0 root         (0) root         (0)     6925 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/files/copy_pattern.py
--rw-r--r--   0 root         (0) root         (0)    24002 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/files/files.py
--rw-r--r--   0 root         (0) root         (0)     4177 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/files/packager.py
--rw-r--r--   0 root         (0) root         (0)     6540 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/files/patches.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.652691 conan-2.2.3/conan/tools/files/symlinks/
--rw-r--r--   0 root         (0) root         (0)      148 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/files/symlinks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2456 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/files/symlinks/symlinks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.654691 conan-2.2.3/conan/tools/gnu/
--rw-r--r--   0 root         (0) root         (0)      320 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/gnu/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6234 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/gnu/autotools.py
--rw-r--r--   0 root         (0) root         (0)     2962 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/gnu/autotoolsdeps.py
--rw-r--r--   0 root         (0) root         (0)    14034 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/gnu/autotoolstoolchain.py
--rw-r--r--   0 root         (0) root         (0)     3698 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/gnu/get_gnu_triplet.py
--rw-r--r--   0 root         (0) root         (0)     3596 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/gnu/gnudeps_flags.py
--rw-r--r--   0 root         (0) root         (0)    27066 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/gnu/makedeps.py
--rw-r--r--   0 root         (0) root         (0)     4290 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/gnu/pkgconfig.py
--rw-r--r--   0 root         (0) root         (0)    19100 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/gnu/pkgconfigdeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.654691 conan-2.2.3/conan/tools/google/
--rw-r--r--   0 root         (0) root         (0)      201 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/google/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3387 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/google/bazel.py
--rw-r--r--   0 root         (0) root         (0)    23416 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/google/bazeldeps.py
--rw-r--r--   0 root         (0) root         (0)     1188 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/google/layout.py
--rw-r--r--   0 root         (0) root         (0)     8113 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/google/toolchain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.655691 conan-2.2.3/conan/tools/intel/
--rw-r--r--   0 root         (0) root         (0)       47 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/intel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6498 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/intel/intel_cc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.655691 conan-2.2.3/conan/tools/layout/
--rw-r--r--   0 root         (0) root         (0)      605 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/layout/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.655691 conan-2.2.3/conan/tools/meson/
--rw-r--r--   0 root         (0) root         (0)       98 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/meson/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4702 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/meson/helpers.py
--rw-r--r--   0 root         (0) root         (0)     5093 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/meson/meson.py
--rw-r--r--   0 root         (0) root         (0)    23068 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/meson/toolchain.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.656691 conan-2.2.3/conan/tools/microsoft/
--rw-r--r--   0 root         (0) root         (0)      558 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/microsoft/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1335 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/microsoft/layout.py
--rw-r--r--   0 root         (0) root         (0)     3312 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/microsoft/msbuild.py
--rw-r--r--   0 root         (0) root         (0)    19246 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/microsoft/msbuilddeps.py
--rw-r--r--   0 root         (0) root         (0)     2967 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/microsoft/nmakedeps.py
--rw-r--r--   0 root         (0) root         (0)     4984 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/microsoft/nmaketoolchain.py
--rw-r--r--   0 root         (0) root         (0)      593 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/microsoft/subsystems.py
--rw-r--r--   0 root         (0) root         (0)    11139 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/microsoft/toolchain.py
--rw-r--r--   0 root         (0) root         (0)    15003 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/microsoft/visual.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.657692 conan-2.2.3/conan/tools/premake/
--rw-r--r--   0 root         (0) root         (0)      103 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/premake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1675 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/premake/premake.py
--rw-r--r--   0 root         (0) root         (0)    10534 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/premake/premakedeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.657692 conan-2.2.3/conan/tools/qbs/
--rw-r--r--   0 root         (0) root         (0)      152 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/qbs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2901 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/qbs/qbs.py
--rw-r--r--   0 root         (0) root         (0)     9897 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/qbs/qbsprofile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.657692 conan-2.2.3/conan/tools/scm/
--rw-r--r--   0 root         (0) root         (0)       77 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/scm/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12771 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/scm/git.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.657692 conan-2.2.3/conan/tools/scons/
--rw-r--r--   0 root         (0) root         (0)       50 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/scons/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2362 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/scons/sconsdeps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.658692 conan-2.2.3/conan/tools/system/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/system/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18002 2024-04-17 15:51:55.000000 conan-2.2.3/conan/tools/system/package_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.636690 conan-2.2.3/conan.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8618 2024-04-17 15:52:04.000000 conan-2.2.3/conan.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9622 2024-04-17 15:52:04.000000 conan-2.2.3/conan.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-17 15:52:04.000000 conan-2.2.3/conan.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2024-04-17 15:52:04.000000 conan-2.2.3/conan.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      469 2024-04-17 15:52:04.000000 conan-2.2.3/conan.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-17 15:52:04.000000 conan-2.2.3/conan.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.659692 conan-2.2.3/conans/
--rw-r--r--   0 root         (0) root         (0)      201 2024-04-17 15:51:55.000000 conan-2.2.3/conans/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.660692 conan-2.2.3/conans/client/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.661692 conan-2.2.3/conans/client/cache/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/cache/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4924 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/cache/cache.py
--rw-r--r--   0 root         (0) root         (0)     2033 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/cache/editable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.661692 conan-2.2.3/conans/client/cmd/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/cmd/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7808 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/cmd/export.py
--rw-r--r--   0 root         (0) root         (0)    12332 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/cmd/uploader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.662692 conan-2.2.3/conans/client/conanfile/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/conanfile/__init__.py
--rw-r--r--   0 root         (0) root         (0)      760 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/conanfile/build.py
--rw-r--r--   0 root         (0) root         (0)     2543 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/conanfile/configure.py
--rw-r--r--   0 root         (0) root         (0)      638 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/conanfile/implementations.py
--rw-r--r--   0 root         (0) root         (0)     2138 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/conanfile/package.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.662692 conan-2.2.3/conans/client/conf/
--rw-r--r--   0 root         (0) root         (0)     7414 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/conf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7899 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/conf/config_installer.py
--rw-r--r--   0 root         (0) root         (0)     1419 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/conf/detect.py
--rw-r--r--   0 root         (0) root         (0)     4582 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/conf/detect_vs.py
--rw-r--r--   0 root         (0) root         (0)     1270 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/conf/required_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.663692 conan-2.2.3/conans/client/downloaders/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/downloaders/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10333 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/downloaders/caching_file_downloader.py
--rw-r--r--   0 root         (0) root         (0)     5595 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/downloaders/download_cache.py
--rw-r--r--   0 root         (0) root         (0)     6706 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/downloaders/file_downloader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.663692 conan-2.2.3/conans/client/generators/
--rw-r--r--   0 root         (0) root         (0)    10315 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/generators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.665692 conan-2.2.3/conans/client/graph/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3546 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/graph/build_mode.py
--rw-r--r--   0 root         (0) root         (0)     5532 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/graph/compatibility.py
--rw-r--r--   0 root         (0) root         (0)     4348 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/graph/compute_pid.py
--rw-r--r--   0 root         (0) root         (0)    15453 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/graph/graph.py
--rw-r--r--   0 root         (0) root         (0)    23117 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/graph/graph_binaries.py
--rw-r--r--   0 root         (0) root         (0)    21937 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/graph/graph_builder.py
--rw-r--r--   0 root         (0) root         (0)     3210 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/graph/graph_error.py
--rw-r--r--   0 root         (0) root         (0)    21344 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/graph/install_graph.py
--rw-r--r--   0 root         (0) root         (0)     4838 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/graph/profile_node_definer.py
--rw-r--r--   0 root         (0) root         (0)     1895 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/graph/provides.py
--rw-r--r--   0 root         (0) root         (0)     7221 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/graph/proxy.py
--rw-r--r--   0 root         (0) root         (0)     6480 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/graph/python_requires.py
--rw-r--r--   0 root         (0) root         (0)     5326 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/graph/range_resolver.py
--rw-r--r--   0 root         (0) root         (0)     2595 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/hook_manager.py
--rw-r--r--   0 root         (0) root         (0)    21840 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/installer.py
--rw-r--r--   0 root         (0) root         (0)    17007 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/loader.py
--rw-r--r--   0 root         (0) root         (0)     1829 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/loader_txt.py
--rw-r--r--   0 root         (0) root         (0)     5413 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/migrations.py
--rw-r--r--   0 root         (0) root         (0)     1971 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/pkg_sign.py
--rw-r--r--   0 root         (0) root         (0)    17325 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/profile_loader.py
--rw-r--r--   0 root         (0) root         (0)    14595 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/remote_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.666692 conan-2.2.3/conans/client/rest/
--rw-r--r--   0 root         (0) root         (0)      838 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/rest/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5837 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/rest/auth_manager.py
--rw-r--r--   0 root         (0) root         (0)     6132 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/rest/client_routes.py
--rw-r--r--   0 root         (0) root         (0)     6923 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/rest/conan_requester.py
--rw-r--r--   0 root         (0) root         (0)     3945 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/rest/file_uploader.py
--rw-r--r--   0 root         (0) root         (0)     2488 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/rest/remote_credentials.py
--rw-r--r--   0 root         (0) root         (0)     5424 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/rest/rest_client.py
--rw-r--r--   0 root         (0) root         (0)     9571 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/rest/rest_client_common.py
--rw-r--r--   0 root         (0) root         (0)    14934 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/rest/rest_client_v2.py
--rw-r--r--   0 root         (0) root         (0)     9149 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/rest_client_local_recipe_index.py
--rw-r--r--   0 root         (0) root         (0)     3903 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.666692 conan-2.2.3/conans/client/store/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/store/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4205 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/store/localdb.py
--rw-r--r--   0 root         (0) root         (0)     8798 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/subsystems.py
--rw-r--r--   0 root         (0) root         (0)     4223 2024-04-17 15:51:55.000000 conan-2.2.3/conans/client/userio.py
--rwxr-xr-x   0 root         (0) root         (0)      118 2024-04-17 15:51:55.000000 conan-2.2.3/conans/conan.py
--rw-r--r--   0 root         (0) root         (0)      699 2024-04-17 15:51:55.000000 conan-2.2.3/conans/conan_server.py
--rw-r--r--   0 root         (0) root         (0)     7419 2024-04-17 15:51:55.000000 conan-2.2.3/conans/errors.py
--rw-r--r--   0 root         (0) root         (0)     3290 2024-04-17 15:51:55.000000 conan-2.2.3/conans/migrations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.668692 conan-2.2.3/conans/model/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 15:51:55.000000 conan-2.2.3/conans/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20506 2024-04-17 15:51:55.000000 conan-2.2.3/conans/model/build_info.py
--rw-r--r--   0 root         (0) root         (0)    12679 2024-04-17 15:51:55.000000 conan-2.2.3/conans/model/conan_file.py
--rw-r--r--   0 root         (0) root         (0)     2991 2024-04-17 15:51:55.000000 conan-2.2.3/conans/model/conanfile_interface.py
--rw-r--r--   0 root         (0) root         (0)    32560 2024-04-17 15:51:55.000000 conan-2.2.3/conans/model/conf.py
--rw-r--r--   0 root         (0) root         (0)     6168 2024-04-17 15:51:55.000000 conan-2.2.3/conans/model/dependencies.py
--rw-r--r--   0 root         (0) root         (0)    13116 2024-04-17 15:51:55.000000 conan-2.2.3/conans/model/graph_lock.py
--rw-r--r--   0 root         (0) root         (0)    15205 2024-04-17 15:51:55.000000 conan-2.2.3/conans/model/info.py
--rw-r--r--   0 root         (0) root         (0)     5423 2024-04-17 15:51:55.000000 conan-2.2.3/conans/model/layout.py
--rw-r--r--   0 root         (0) root         (0)     4883 2024-04-17 15:51:55.000000 conan-2.2.3/conans/model/manifest.py
--rw-r--r--   0 root         (0) root         (0)    17829 2024-04-17 15:51:55.000000 conan-2.2.3/conans/model/options.py
--rw-r--r--   0 root         (0) root         (0)     3861 2024-04-17 15:51:55.000000 conan-2.2.3/conans/model/package_ref.py
--rw-r--r--   0 root         (0) root         (0)     2361 2024-04-17 15:51:55.000000 conan-2.2.3/conans/model/pkg_type.py
--rw-r--r--   0 root         (0) root         (0)     7089 2024-04-17 15:51:55.000000 conan-2.2.3/conans/model/profile.py
--rw-r--r--   0 root         (0) root         (0)     8089 2024-04-17 15:51:55.000000 conan-2.2.3/conans/model/recipe_ref.py
--rw-r--r--   0 root         (0) root         (0)    24648 2024-04-17 15:51:55.000000 conan-2.2.3/conans/model/requires.py
--rw-r--r--   0 root         (0) root         (0)     2171 2024-04-17 15:51:55.000000 conan-2.2.3/conans/model/rest_routes.py
--rw-r--r--   0 root         (0) root         (0)    13805 2024-04-17 15:51:55.000000 conan-2.2.3/conans/model/settings.py
--rw-r--r--   0 root         (0) root         (0)     6184 2024-04-17 15:51:55.000000 conan-2.2.3/conans/model/version.py
--rw-r--r--   0 root         (0) root         (0)     8467 2024-04-17 15:51:55.000000 conan-2.2.3/conans/model/version_range.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.668692 conan-2.2.3/conans/paths/
--rw-r--r--   0 root         (0) root         (0)     2151 2024-04-17 15:51:55.000000 conan-2.2.3/conans/paths/__init__.py
--rw-r--r--   0 root         (0) root         (0)      251 2024-04-17 15:51:55.000000 conan-2.2.3/conans/requirements.txt
--rw-r--r--   0 root         (0) root         (0)      146 2024-04-17 15:51:55.000000 conan-2.2.3/conans/requirements_dev.txt
--rw-r--r--   0 root         (0) root         (0)       69 2024-04-17 15:51:55.000000 conan-2.2.3/conans/requirements_server.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.669693 conan-2.2.3/conans/search/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 15:51:55.000000 conan-2.2.3/conans/search/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3814 2024-04-17 15:51:55.000000 conan-2.2.3/conans/search/query_parse.py
--rw-r--r--   0 root         (0) root         (0)     4474 2024-04-17 15:51:55.000000 conan-2.2.3/conans/search/search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.669693 conan-2.2.3/conans/test/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 15:51:55.000000 conan-2.2.3/conans/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.670693 conan-2.2.3/conans/test/assets/
--rw-r--r--   0 root         (0) root         (0)      510 2024-04-17 15:51:55.000000 conan-2.2.3/conans/test/assets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1651 2024-04-17 15:51:55.000000 conan-2.2.3/conans/test/assets/autotools.py
--rw-r--r--   0 root         (0) root         (0)     3753 2024-04-17 15:51:55.000000 conan-2.2.3/conans/test/assets/cmake.py
--rw-r--r--   0 root         (0) root         (0)    17307 2024-04-17 15:51:55.000000 conan-2.2.3/conans/test/assets/genconanfile.py
--rw-r--r--   0 root         (0) root         (0)     6352 2024-04-17 15:51:55.000000 conan-2.2.3/conans/test/assets/pkg_cmake.py
--rw-r--r--   0 root         (0) root         (0)     6008 2024-04-17 15:51:55.000000 conan-2.2.3/conans/test/assets/sources.py
--rw-r--r--   0 root         (0) root         (0)    11972 2024-04-17 15:51:55.000000 conan-2.2.3/conans/test/assets/visual_project_files.py
--rw-r--r--   0 root         (0) root         (0)    13204 2024-04-17 15:51:55.000000 conan-2.2.3/conans/test/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.671693 conan-2.2.3/conans/test/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 15:51:55.000000 conan-2.2.3/conans/test/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4868 2024-04-17 15:51:55.000000 conan-2.2.3/conans/test/utils/artifactory.py
--rw-r--r--   0 root         (0) root         (0)     2805 2024-04-17 15:51:55.000000 conan-2.2.3/conans/test/utils/file_server.py
--rw-r--r--   0 root         (0) root         (0)     4155 2024-04-17 15:51:55.000000 conan-2.2.3/conans/test/utils/mocks.py
--rw-r--r--   0 root         (0) root         (0)     1155 2024-04-17 15:51:55.000000 conan-2.2.3/conans/test/utils/profiles.py
--rw-r--r--   0 root         (0) root         (0)     2038 2024-04-17 15:51:55.000000 conan-2.2.3/conans/test/utils/scm.py
--rw-r--r--   0 root         (0) root         (0)     3858 2024-04-17 15:51:55.000000 conan-2.2.3/conans/test/utils/server_launcher.py
--rw-r--r--   0 root         (0) root         (0)     3187 2024-04-17 15:51:55.000000 conan-2.2.3/conans/test/utils/test_files.py
--rw-r--r--   0 root         (0) root         (0)    37513 2024-04-17 15:51:55.000000 conan-2.2.3/conans/test/utils/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-17 15:52:04.672693 conan-2.2.3/conans/util/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-17 15:51:55.000000 conan-2.2.3/conans/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2490 2024-04-17 15:51:55.000000 conan-2.2.3/conans/util/config_parser.py
--rw-r--r--   0 root         (0) root         (0)     1849 2024-04-17 15:51:55.000000 conan-2.2.3/conans/util/dates.py
--rw-r--r--   0 root         (0) root         (0)     1301 2024-04-17 15:51:55.000000 conan-2.2.3/conans/util/encrypt.py
--rw-r--r--   0 root         (0) root         (0)     1396 2024-04-17 15:51:55.000000 conan-2.2.3/conans/util/env.py
--rw-r--r--   0 root         (0) root         (0)    11974 2024-04-17 15:51:55.000000 conan-2.2.3/conans/util/files.py
--rw-r--r--   0 root         (0) root         (0)     3657 2024-04-17 15:51:55.000000 conan-2.2.3/conans/util/locks.py
--rw-r--r--   0 root         (0) root         (0)     3729 2024-04-17 15:51:55.000000 conan-2.2.3/conans/util/runners.py
--rw-r--r--   0 root         (0) root         (0)     1416 2024-04-17 15:51:55.000000 conan-2.2.3/conans/util/sha.py
--rw-r--r--   0 root         (0) root         (0)      354 2024-04-17 15:51:55.000000 conan-2.2.3/conans/util/thread.py
--rw-r--r--   0 root         (0) root         (0)     1102 2024-04-17 15:51:55.000000 conan-2.2.3/conans/util/windows.py
--rw-r--r--   0 root         (0) root         (0)       90 2024-04-17 15:51:55.000000 conan-2.2.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      101 2024-04-17 15:52:04.673693 conan-2.2.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     5100 2024-04-17 15:51:55.000000 conan-2.2.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.742570 conan-2.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1084 2024-05-06 16:43:32.000000 conan-2.3.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-06 16:43:32.000000 conan-2.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8377 2024-05-06 16:43:40.743570 conan-2.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6118 2024-05-06 16:43:32.000000 conan-2.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.703566 conan-2.3.0/conan/
+-rw-r--r--   0 root         (0) root         (0)      165 2024-05-06 16:43:32.000000 conan-2.3.0/conan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.704566 conan-2.3.0/conan/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2455 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/conan_api.py
+-rw-r--r--   0 root         (0) root         (0)    13040 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/model.py
+-rw-r--r--   0 root         (0) root         (0)     9460 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/output.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.706567 conan-2.3.0/conan/api/subapi/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13263 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/cache.py
+-rw-r--r--   0 root         (0) root         (0)      756 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/command.py
+-rw-r--r--   0 root         (0) root         (0)     9255 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/config.py
+-rw-r--r--   0 root         (0) root         (0)     4793 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/download.py
+-rw-r--r--   0 root         (0) root         (0)     2714 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/export.py
+-rw-r--r--   0 root         (0) root         (0)    11805 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/graph.py
+-rw-r--r--   0 root         (0) root         (0)     3961 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/install.py
+-rw-r--r--   0 root         (0) root         (0)    17548 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/list.py
+-rw-r--r--   0 root         (0) root         (0)     5524 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/local.py
+-rw-r--r--   0 root         (0) root         (0)     4808 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/lockfile.py
+-rw-r--r--   0 root         (0) root         (0)     5193 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/new.py
+-rw-r--r--   0 root         (0) root         (0)     7441 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/profiles.py
+-rw-r--r--   0 root         (0) root         (0)    13412 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/remotes.py
+-rw-r--r--   0 root         (0) root         (0)     2176 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/remove.py
+-rw-r--r--   0 root         (0) root         (0)     1117 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/search.py
+-rw-r--r--   0 root         (0) root         (0)     6670 2024-05-06 16:43:32.000000 conan-2.3.0/conan/api/subapi/upload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.707567 conan-2.3.0/conan/cli/
+-rw-r--r--   0 root         (0) root         (0)      397 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7430 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/args.py
+-rw-r--r--   0 root         (0) root         (0)    12224 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/cli.py
+-rw-r--r--   0 root         (0) root         (0)     8279 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.710567 conan-2.3.0/conan/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3994 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/build.py
+-rw-r--r--   0 root         (0) root         (0)     7489 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4609 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/config.py
+-rw-r--r--   0 root         (0) root         (0)    10989 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/create.py
+-rw-r--r--   0 root         (0) root         (0)     3252 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/download.py
+-rw-r--r--   0 root         (0) root         (0)     3157 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/editable.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/export.py
+-rw-r--r--   0 root         (0) root         (0)     5798 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/export_pkg.py
+-rw-r--r--   0 root         (0) root         (0)    21213 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/graph.py
+-rw-r--r--   0 root         (0) root         (0)     2495 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/inspect.py
+-rw-r--r--   0 root         (0) root         (0)     4704 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/install.py
+-rw-r--r--   0 root         (0) root         (0)    13371 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/list.py
+-rw-r--r--   0 root         (0) root         (0)     7511 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/lock.py
+-rw-r--r--   0 root         (0) root         (0)     4260 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/new.py
+-rw-r--r--   0 root         (0) root         (0)     3696 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/pkglist.py
+-rw-r--r--   0 root         (0) root         (0)     3553 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/profile.py
+-rw-r--r--   0 root         (0) root         (0)    12835 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/remote.py
+-rw-r--r--   0 root         (0) root         (0)     6487 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/remove.py
+-rw-r--r--   0 root         (0) root         (0)     1787 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/search.py
+-rw-r--r--   0 root         (0) root         (0)      753 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/source.py
+-rw-r--r--   0 root         (0) root         (0)     4411 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/test.py
+-rw-r--r--   0 root         (0) root         (0)     6871 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/upload.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/commands/version.py
+-rw-r--r--   0 root         (0) root         (0)      490 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/exit_codes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.710567 conan-2.3.0/conan/cli/formatters/
+-rw-r--r--   0 root         (0) root         (0)      158 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/formatters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.710567 conan-2.3.0/conan/cli/formatters/graph/
+-rw-r--r--   0 root         (0) root         (0)      110 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/formatters/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5663 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/formatters/graph/graph.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/formatters/graph/graph_info_text.py
+-rw-r--r--   0 root         (0) root         (0)      334 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/formatters/graph/info_graph_dot.py
+-rw-r--r--   0 root         (0) root         (0)    15953 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/formatters/graph/info_graph_html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.711567 conan-2.3.0/conan/cli/formatters/list/
+-rw-r--r--   0 root         (0) root         (0)       37 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/formatters/list/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4612 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/formatters/list/binary_html_table.py
+-rw-r--r--   0 root         (0) root         (0)      939 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/formatters/list/list.py
+-rw-r--r--   0 root         (0) root         (0)    12834 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/formatters/list/search_table_html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.711567 conan-2.3.0/conan/cli/printers/
+-rw-r--r--   0 root         (0) root         (0)      331 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/printers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6412 2024-05-06 16:43:32.000000 conan-2.3.0/conan/cli/printers/graph.py
+-rw-r--r--   0 root         (0) root         (0)      139 2024-05-06 16:43:32.000000 conan-2.3.0/conan/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.712567 conan-2.3.0/conan/internal/
+-rw-r--r--   0 root         (0) root         (0)      419 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.712567 conan-2.3.0/conan/internal/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20992 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/detect_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.714568 conan-2.3.0/conan/internal/api/new/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/new/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      293 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/new/alias_new.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/new/autoools_exe.py
+-rw-r--r--   0 root         (0) root         (0)     3850 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/new/autotools_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2916 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/new/basic.py
+-rw-r--r--   0 root         (0) root         (0)     2041 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/new/bazel_exe.py
+-rw-r--r--   0 root         (0) root         (0)     4565 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/new/bazel_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2932 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/new/cmake_exe.py
+-rw-r--r--   0 root         (0) root         (0)     8212 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/new/cmake_lib.py
+-rw-r--r--   0 root         (0) root         (0)     3213 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/new/local_recipes_index.py
+-rw-r--r--   0 root         (0) root         (0)     2334 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/new/meson_exe.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/new/meson_lib.py
+-rw-r--r--   0 root         (0) root         (0)     2207 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/new/msbuild_exe.py
+-rw-r--r--   0 root         (0) root         (0)    12307 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/api/new/msbuild_lib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.714568 conan-2.3.0/conan/internal/cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11189 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/cache/cache.py
+-rw-r--r--   0 root         (0) root         (0)     4083 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/cache/conan_reference_layout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.715567 conan-2.3.0/conan/internal/cache/db/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/cache/db/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3949 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/cache/db/cache_database.py
+-rw-r--r--   0 root         (0) root         (0)     9222 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/cache/db/packages_table.py
+-rw-r--r--   0 root         (0) root         (0)     5477 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/cache/db/recipes_table.py
+-rw-r--r--   0 root         (0) root         (0)     2639 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/cache/db/table.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/cache/home_paths.py
+-rw-r--r--   0 root         (0) root         (0)     3114 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/conan_app.py
+-rw-r--r--   0 root         (0) root         (0)     5045 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/deploy.py
+-rw-r--r--   0 root         (0) root         (0)     3098 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/integrity_check.py
+-rw-r--r--   0 root         (0) root         (0)      922 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/internal_tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.715567 conan-2.3.0/conan/internal/runner/
+-rw-r--r--   0 root         (0) root         (0)      302 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/runner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14530 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/runner/docker.py
+-rw-r--r--   0 root         (0) root         (0)    12370 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/runner/ssh.py
+-rw-r--r--   0 root         (0) root         (0)     6712 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/runner/wsl.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2024-05-06 16:43:32.000000 conan-2.3.0/conan/internal/upload_metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.716568 conan-2.3.0/conan/tools/
+-rw-r--r--   0 root         (0) root         (0)      384 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.716568 conan-2.3.0/conan/tools/android/
+-rw-r--r--   0 root         (0) root         (0)       50 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/android/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1138 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/android/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.716568 conan-2.3.0/conan/tools/apple/
+-rw-r--r--   0 root         (0) root         (0)      534 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/apple/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12880 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/apple/apple.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/apple/xcodebuild.py
+-rw-r--r--   0 root         (0) root         (0)    16239 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/apple/xcodedeps.py
+-rw-r--r--   0 root         (0) root         (0)     5754 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/apple/xcodetoolchain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.717568 conan-2.3.0/conan/tools/build/
+-rw-r--r--   0 root         (0) root         (0)     4190 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/build/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11121 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/build/cppstd.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/build/cpu.py
+-rw-r--r--   0 root         (0) root         (0)     2302 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/build/cross_building.py
+-rw-r--r--   0 root         (0) root         (0)    16208 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/build/flags.py
+-rw-r--r--   0 root         (0) root         (0)      563 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/build/stdcpp_library.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.718568 conan-2.3.0/conan/tools/cmake/
+-rw-r--r--   0 root         (0) root         (0)      217 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14319 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/cmake.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.718568 conan-2.3.0/conan/tools/cmake/cmakedeps/
+-rw-r--r--   0 root         (0) root         (0)      104 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/cmakedeps/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11138 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/cmakedeps/cmakedeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.719568 conan-2.3.0/conan/tools/cmake/cmakedeps/templates/
+-rw-r--r--   0 root         (0) root         (0)     3944 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/cmakedeps/templates/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4563 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/cmakedeps/templates/config.py
+-rw-r--r--   0 root         (0) root         (0)     4061 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/cmakedeps/templates/config_version.py
+-rw-r--r--   0 root         (0) root         (0)     5956 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/cmakedeps/templates/macros.py
+-rw-r--r--   0 root         (0) root         (0)    14989 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/cmakedeps/templates/target_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    20350 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/cmakedeps/templates/target_data.py
+-rw-r--r--   0 root         (0) root         (0)     3656 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/cmakedeps/templates/targets.py
+-rw-r--r--   0 root         (0) root         (0)     4746 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/layout.py
+-rw-r--r--   0 root         (0) root         (0)    16807 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/presets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.719568 conan-2.3.0/conan/tools/cmake/toolchain/
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/toolchain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45120 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/toolchain/blocks.py
+-rw-r--r--   0 root         (0) root         (0)    13776 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/toolchain/toolchain.py
+-rw-r--r--   0 root         (0) root         (0)      171 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/cmake/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.720568 conan-2.3.0/conan/tools/env/
+-rw-r--r--   0 root         (0) root         (0)      168 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/env/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26546 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/env/environment.py
+-rw-r--r--   0 root         (0) root         (0)     3601 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/env/virtualbuildenv.py
+-rw-r--r--   0 root         (0) root         (0)     3561 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/env/virtualrunenv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.721568 conan-2.3.0/conan/tools/files/
+-rw-r--r--   0 root         (0) root         (0)      535 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/files/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2672 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/files/conandata.py
+-rw-r--r--   0 root         (0) root         (0)     7429 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/files/copy_pattern.py
+-rw-r--r--   0 root         (0) root         (0)    24002 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/files/files.py
+-rw-r--r--   0 root         (0) root         (0)     4177 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/files/packager.py
+-rw-r--r--   0 root         (0) root         (0)     6540 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/files/patches.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.721568 conan-2.3.0/conan/tools/files/symlinks/
+-rw-r--r--   0 root         (0) root         (0)      148 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/files/symlinks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2456 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/files/symlinks/symlinks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.722568 conan-2.3.0/conan/tools/gnu/
+-rw-r--r--   0 root         (0) root         (0)      374 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/gnu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6173 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/gnu/autotools.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/gnu/autotoolsdeps.py
+-rw-r--r--   0 root         (0) root         (0)    13681 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/gnu/autotoolstoolchain.py
+-rw-r--r--   0 root         (0) root         (0)     3986 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/gnu/get_gnu_triplet.py
+-rw-r--r--   0 root         (0) root         (0)     3596 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/gnu/gnudeps_flags.py
+-rw-r--r--   0 root         (0) root         (0)    13632 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/gnu/gnutoolchain.py
+-rw-r--r--   0 root         (0) root         (0)    27066 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/gnu/makedeps.py
+-rw-r--r--   0 root         (0) root         (0)     4290 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/gnu/pkgconfig.py
+-rw-r--r--   0 root         (0) root         (0)    19100 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/gnu/pkgconfigdeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.723568 conan-2.3.0/conan/tools/google/
+-rw-r--r--   0 root         (0) root         (0)      201 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/google/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3387 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/google/bazel.py
+-rw-r--r--   0 root         (0) root         (0)    23672 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/google/bazeldeps.py
+-rw-r--r--   0 root         (0) root         (0)     1188 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/google/layout.py
+-rw-r--r--   0 root         (0) root         (0)     8113 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/google/toolchain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.723568 conan-2.3.0/conan/tools/intel/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/intel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6498 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/intel/intel_cc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.723568 conan-2.3.0/conan/tools/layout/
+-rw-r--r--   0 root         (0) root         (0)      605 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/layout/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.724568 conan-2.3.0/conan/tools/meson/
+-rw-r--r--   0 root         (0) root         (0)       98 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/meson/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4702 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/meson/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     5269 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/meson/meson.py
+-rw-r--r--   0 root         (0) root         (0)    25007 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/meson/toolchain.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.725568 conan-2.3.0/conan/tools/microsoft/
+-rw-r--r--   0 root         (0) root         (0)      558 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/microsoft/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1335 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/microsoft/layout.py
+-rw-r--r--   0 root         (0) root         (0)     3312 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/microsoft/msbuild.py
+-rw-r--r--   0 root         (0) root         (0)    19246 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/microsoft/msbuilddeps.py
+-rw-r--r--   0 root         (0) root         (0)     2967 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/microsoft/nmakedeps.py
+-rw-r--r--   0 root         (0) root         (0)     4984 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/microsoft/nmaketoolchain.py
+-rw-r--r--   0 root         (0) root         (0)      593 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/microsoft/subsystems.py
+-rw-r--r--   0 root         (0) root         (0)    11139 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/microsoft/toolchain.py
+-rw-r--r--   0 root         (0) root         (0)    14962 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/microsoft/visual.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.725568 conan-2.3.0/conan/tools/premake/
+-rw-r--r--   0 root         (0) root         (0)      103 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/premake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/premake/premake.py
+-rw-r--r--   0 root         (0) root         (0)    10534 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/premake/premakedeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.726569 conan-2.3.0/conan/tools/qbs/
+-rw-r--r--   0 root         (0) root         (0)      152 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/qbs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2901 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/qbs/qbs.py
+-rw-r--r--   0 root         (0) root         (0)     9897 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/qbs/qbsprofile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.726569 conan-2.3.0/conan/tools/scm/
+-rw-r--r--   0 root         (0) root         (0)       77 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/scm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13281 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/scm/git.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.726569 conan-2.3.0/conan/tools/scons/
+-rw-r--r--   0 root         (0) root         (0)       50 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/scons/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2362 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/scons/sconsdeps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.726569 conan-2.3.0/conan/tools/system/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/system/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17993 2024-05-06 16:43:32.000000 conan-2.3.0/conan/tools/system/package_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.703566 conan-2.3.0/conan.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8377 2024-05-06 16:43:40.000000 conan-2.3.0/conan.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9839 2024-05-06 16:43:40.000000 conan-2.3.0/conan.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-06 16:43:40.000000 conan-2.3.0/conan.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2024-05-06 16:43:40.000000 conan-2.3.0/conan.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-06 16:43:40.000000 conan-2.3.0/conan.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-06 16:43:40.000000 conan-2.3.0/conan.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.727569 conan-2.3.0/conans/
+-rw-r--r--   0 root         (0) root         (0)      201 2024-05-06 16:43:32.000000 conan-2.3.0/conans/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.729569 conan-2.3.0/conans/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.729569 conan-2.3.0/conans/client/cache/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/cache/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4924 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/cache/cache.py
+-rw-r--r--   0 root         (0) root         (0)     2033 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/cache/editable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.730569 conan-2.3.0/conans/client/cmd/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/cmd/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7883 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/cmd/export.py
+-rw-r--r--   0 root         (0) root         (0)    12622 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/cmd/uploader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.730569 conan-2.3.0/conans/client/conanfile/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/conanfile/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      760 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/conanfile/build.py
+-rw-r--r--   0 root         (0) root         (0)     2543 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/conanfile/configure.py
+-rw-r--r--   0 root         (0) root         (0)      638 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/conanfile/implementations.py
+-rw-r--r--   0 root         (0) root         (0)     2138 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/conanfile/package.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.731569 conan-2.3.0/conans/client/conf/
+-rw-r--r--   0 root         (0) root         (0)     7449 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/conf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7919 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/conf/config_installer.py
+-rw-r--r--   0 root         (0) root         (0)     1419 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/conf/detect.py
+-rw-r--r--   0 root         (0) root         (0)     4582 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/conf/detect_vs.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/conf/required_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.731569 conan-2.3.0/conans/client/downloaders/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/downloaders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10333 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/downloaders/caching_file_downloader.py
+-rw-r--r--   0 root         (0) root         (0)     5595 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/downloaders/download_cache.py
+-rw-r--r--   0 root         (0) root         (0)     6731 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/downloaders/file_downloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.732569 conan-2.3.0/conans/client/generators/
+-rw-r--r--   0 root         (0) root         (0)    10455 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/generators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.733569 conan-2.3.0/conans/client/graph/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/graph/build_mode.py
+-rw-r--r--   0 root         (0) root         (0)     5532 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/graph/compatibility.py
+-rw-r--r--   0 root         (0) root         (0)     4451 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/graph/compute_pid.py
+-rw-r--r--   0 root         (0) root         (0)    15453 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/graph/graph.py
+-rw-r--r--   0 root         (0) root         (0)    23117 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/graph/graph_binaries.py
+-rw-r--r--   0 root         (0) root         (0)    21937 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/graph/graph_builder.py
+-rw-r--r--   0 root         (0) root         (0)     2924 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/graph/graph_error.py
+-rw-r--r--   0 root         (0) root         (0)    21344 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/graph/install_graph.py
+-rw-r--r--   0 root         (0) root         (0)     5186 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/graph/profile_node_definer.py
+-rw-r--r--   0 root         (0) root         (0)     1895 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/graph/provides.py
+-rw-r--r--   0 root         (0) root         (0)     7221 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/graph/proxy.py
+-rw-r--r--   0 root         (0) root         (0)     6480 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/graph/python_requires.py
+-rw-r--r--   0 root         (0) root         (0)     5326 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/graph/range_resolver.py
+-rw-r--r--   0 root         (0) root         (0)     2595 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/hook_manager.py
+-rw-r--r--   0 root         (0) root         (0)    21840 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/installer.py
+-rw-r--r--   0 root         (0) root         (0)    17007 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/loader.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/loader_txt.py
+-rw-r--r--   0 root         (0) root         (0)     5413 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/migrations.py
+-rw-r--r--   0 root         (0) root         (0)     1971 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/pkg_sign.py
+-rw-r--r--   0 root         (0) root         (0)    17816 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/profile_loader.py
+-rw-r--r--   0 root         (0) root         (0)    14595 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/remote_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.735570 conan-2.3.0/conans/client/rest/
+-rw-r--r--   0 root         (0) root         (0)      838 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/rest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5837 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/rest/auth_manager.py
+-rw-r--r--   0 root         (0) root         (0)     6132 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/rest/client_routes.py
+-rw-r--r--   0 root         (0) root         (0)     6936 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/rest/conan_requester.py
+-rw-r--r--   0 root         (0) root         (0)     3945 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/rest/file_uploader.py
+-rw-r--r--   0 root         (0) root         (0)     2650 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/rest/remote_credentials.py
+-rw-r--r--   0 root         (0) root         (0)     5424 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/rest/rest_client.py
+-rw-r--r--   0 root         (0) root         (0)     9776 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/rest/rest_client_common.py
+-rw-r--r--   0 root         (0) root         (0)    14934 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/rest/rest_client_v2.py
+-rw-r--r--   0 root         (0) root         (0)     9149 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/rest_client_local_recipe_index.py
+-rw-r--r--   0 root         (0) root         (0)     3903 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/source.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.735570 conan-2.3.0/conans/client/store/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/store/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4205 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/store/localdb.py
+-rw-r--r--   0 root         (0) root         (0)     8798 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/subsystems.py
+-rw-r--r--   0 root         (0) root         (0)     4223 2024-05-06 16:43:32.000000 conan-2.3.0/conans/client/userio.py
+-rwxr-xr-x   0 root         (0) root         (0)      118 2024-05-06 16:43:32.000000 conan-2.3.0/conans/conan.py
+-rw-r--r--   0 root         (0) root         (0)      699 2024-05-06 16:43:32.000000 conan-2.3.0/conans/conan_server.py
+-rw-r--r--   0 root         (0) root         (0)     7419 2024-05-06 16:43:32.000000 conan-2.3.0/conans/errors.py
+-rw-r--r--   0 root         (0) root         (0)     3290 2024-05-06 16:43:32.000000 conan-2.3.0/conans/migrations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.737570 conan-2.3.0/conans/model/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20506 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/build_info.py
+-rw-r--r--   0 root         (0) root         (0)    12678 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/conan_file.py
+-rw-r--r--   0 root         (0) root         (0)     2991 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/conanfile_interface.py
+-rw-r--r--   0 root         (0) root         (0)    32656 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/conf.py
+-rw-r--r--   0 root         (0) root         (0)     6302 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/dependencies.py
+-rw-r--r--   0 root         (0) root         (0)    13116 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/graph_lock.py
+-rw-r--r--   0 root         (0) root         (0)    15205 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/info.py
+-rw-r--r--   0 root         (0) root         (0)     5423 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/layout.py
+-rw-r--r--   0 root         (0) root         (0)     4883 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/manifest.py
+-rw-r--r--   0 root         (0) root         (0)    17829 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/options.py
+-rw-r--r--   0 root         (0) root         (0)     3861 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/package_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/pkg_type.py
+-rw-r--r--   0 root         (0) root         (0)     7155 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/profile.py
+-rw-r--r--   0 root         (0) root         (0)     8088 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/recipe_ref.py
+-rw-r--r--   0 root         (0) root         (0)    24648 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/requires.py
+-rw-r--r--   0 root         (0) root         (0)     2171 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/rest_routes.py
+-rw-r--r--   0 root         (0) root         (0)    14049 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/settings.py
+-rw-r--r--   0 root         (0) root         (0)     6184 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/version.py
+-rw-r--r--   0 root         (0) root         (0)     8643 2024-05-06 16:43:32.000000 conan-2.3.0/conans/model/version_range.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.738570 conan-2.3.0/conans/paths/
+-rw-r--r--   0 root         (0) root         (0)     2198 2024-05-06 16:43:32.000000 conan-2.3.0/conans/paths/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      251 2024-05-06 16:43:32.000000 conan-2.3.0/conans/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)      191 2024-05-06 16:43:32.000000 conan-2.3.0/conans/requirements_dev.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-06 16:43:32.000000 conan-2.3.0/conans/requirements_runner.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2024-05-06 16:43:32.000000 conan-2.3.0/conans/requirements_server.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.738570 conan-2.3.0/conans/search/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conans/search/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3814 2024-05-06 16:43:32.000000 conan-2.3.0/conans/search/query_parse.py
+-rw-r--r--   0 root         (0) root         (0)     4474 2024-05-06 16:43:32.000000 conan-2.3.0/conans/search/search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.738570 conan-2.3.0/conans/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.739570 conan-2.3.0/conans/test/assets/
+-rw-r--r--   0 root         (0) root         (0)      510 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/assets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1651 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/assets/autotools.py
+-rw-r--r--   0 root         (0) root         (0)     3753 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/assets/cmake.py
+-rw-r--r--   0 root         (0) root         (0)    17307 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/assets/genconanfile.py
+-rw-r--r--   0 root         (0) root         (0)     6352 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/assets/pkg_cmake.py
+-rw-r--r--   0 root         (0) root         (0)     6008 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/assets/sources.py
+-rw-r--r--   0 root         (0) root         (0)    11972 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/assets/visual_project_files.py
+-rw-r--r--   0 root         (0) root         (0)    13188 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.741570 conan-2.3.0/conans/test/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4868 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/utils/artifactory.py
+-rw-r--r--   0 root         (0) root         (0)     2806 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/utils/file_server.py
+-rw-r--r--   0 root         (0) root         (0)     4155 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/utils/mocks.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/utils/profiles.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/utils/scm.py
+-rw-r--r--   0 root         (0) root         (0)     3858 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/utils/server_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     3187 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/utils/test_files.py
+-rw-r--r--   0 root         (0) root         (0)    37579 2024-05-06 16:43:32.000000 conan-2.3.0/conans/test/utils/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-06 16:43:40.742570 conan-2.3.0/conans/util/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-06 16:43:32.000000 conan-2.3.0/conans/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2024-05-06 16:43:32.000000 conan-2.3.0/conans/util/config_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1849 2024-05-06 16:43:32.000000 conan-2.3.0/conans/util/dates.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2024-05-06 16:43:32.000000 conan-2.3.0/conans/util/encrypt.py
+-rw-r--r--   0 root         (0) root         (0)     1396 2024-05-06 16:43:32.000000 conan-2.3.0/conans/util/env.py
+-rw-r--r--   0 root         (0) root         (0)    11974 2024-05-06 16:43:32.000000 conan-2.3.0/conans/util/files.py
+-rw-r--r--   0 root         (0) root         (0)     3657 2024-05-06 16:43:32.000000 conan-2.3.0/conans/util/locks.py
+-rw-r--r--   0 root         (0) root         (0)     3729 2024-05-06 16:43:32.000000 conan-2.3.0/conans/util/runners.py
+-rw-r--r--   0 root         (0) root         (0)     1416 2024-05-06 16:43:32.000000 conan-2.3.0/conans/util/sha.py
+-rw-r--r--   0 root         (0) root         (0)      354 2024-05-06 16:43:32.000000 conan-2.3.0/conans/util/thread.py
+-rw-r--r--   0 root         (0) root         (0)     1016 2024-05-06 16:43:32.000000 conan-2.3.0/conans/util/windows.py
+-rw-r--r--   0 root         (0) root         (0)       90 2024-05-06 16:43:32.000000 conan-2.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      101 2024-05-06 16:43:40.743570 conan-2.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     5218 2024-05-06 16:43:32.000000 conan-2.3.0/setup.py
```

### Comparing `conan-2.2.3/LICENSE.md` & `conan-2.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/PKG-INFO` & `conan-2.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conan
-Version: 2.2.3
+Version: 2.3.0
 Summary: Conan C/C++ package manager
 Home-page: https://conan.io
 Author: JFrog LTD
 Author-email: luism@jfrog.com
 License: MIT
 Project-URL: Documentation, https://docs.conan.io
 Project-URL: Source, https://github.com/conan-io/conan
@@ -42,20 +42,14 @@
           This community also creates and maintains packages in ConanCenter and Bincrafters repositories in Bintray.
         - Stable. Used in production by many companies, since 1.0 there is a commitment not to break package recipes and documented behavior.
         
         
         This is the **developer/maintainer** documentation. For user documentation, go to https://docs.conan.io
         
         
-        | **develop2**            |
-        |-------------------------|
-        | [![Build Status Develop](https://ci.conan.io/buildStatus/icon?job=ConanTestSuite/develop)](https://ci.conan.io/blue/organizations/jenkins/ConanTestSuitev2/activity)  |
-        
-        
-        
         ## Setup
         
         You can run Conan from source in Windows, MacOS, and Linux:
         
         - **Install pip following** [pip docs](https://pip.pypa.io/en/stable/installation/).
         
         - **Clone Conan repository:**
@@ -86,17 +80,17 @@
             Conan commands. Type "conan <command> -h" for help
           ```
         
         ## Contributing to the project
         
         
         Feedback and contribution are always welcome in this project.
-        Please read our [contributing guide](https://github.com/conan-io/conan/blob/develop/.github/CONTRIBUTING.md).
+        Please read our [contributing guide](https://github.com/conan-io/conan/blob/develop2/.github/CONTRIBUTING.md).
         Also, if you plan to contribute, please add some testing for your changes. You can read the [Conan
-        tests guidelines section](https://github.com/conan-io/conan/blob/develop/conans/test/README.md) for
+        tests guidelines section](https://github.com/conan-io/conan/blob/develop2/conans/test/README.md) for
         some advice on how to write tests for Conan.
         
         ### Running the tests
         
         
         **Install Python requirements**
         
@@ -140,15 +134,15 @@
         
         OK
         ```
         
         To run specific tests, you can specify the test name too, something like:
         
         ```bash
-        $ python -m pytest conans/test/unittests/client/cmd/export_test.py::ExportTest::test_export_warning -s
+        $ python -m pytest conans/test/functional/command/export_test.py::TestRevisionModeSCM::test_revision_mode_scm -s
         ```
         
         The `-s` argument can be useful to see some output that otherwise is captured by *pytest*.
         
         Also, you can run tests against an instance of Artifactory. Those tests should add the attribute
         `artifactory_ready`.
         
@@ -185,7 +179,8 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
+Provides-Extra: runners
```

### Comparing `conan-2.2.3/README.md` & `conan-2.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -31,20 +31,14 @@
   This community also creates and maintains packages in ConanCenter and Bincrafters repositories in Bintray.
 - Stable. Used in production by many companies, since 1.0 there is a commitment not to break package recipes and documented behavior.
 
 
 This is the **developer/maintainer** documentation. For user documentation, go to https://docs.conan.io
 
 
-| **develop2**            |
-|-------------------------|
-| [![Build Status Develop](https://ci.conan.io/buildStatus/icon?job=ConanTestSuite/develop)](https://ci.conan.io/blue/organizations/jenkins/ConanTestSuitev2/activity)  |
-
-
-
 ## Setup
 
 You can run Conan from source in Windows, MacOS, and Linux:
 
 - **Install pip following** [pip docs](https://pip.pypa.io/en/stable/installation/).
 
 - **Clone Conan repository:**
@@ -75,17 +69,17 @@
     Conan commands. Type "conan <command> -h" for help
   ```
 
 ## Contributing to the project
 
 
 Feedback and contribution are always welcome in this project.
-Please read our [contributing guide](https://github.com/conan-io/conan/blob/develop/.github/CONTRIBUTING.md).
+Please read our [contributing guide](https://github.com/conan-io/conan/blob/develop2/.github/CONTRIBUTING.md).
 Also, if you plan to contribute, please add some testing for your changes. You can read the [Conan
-tests guidelines section](https://github.com/conan-io/conan/blob/develop/conans/test/README.md) for
+tests guidelines section](https://github.com/conan-io/conan/blob/develop2/conans/test/README.md) for
 some advice on how to write tests for Conan.
 
 ### Running the tests
 
 
 **Install Python requirements**
 
@@ -129,15 +123,15 @@
 
 OK
 ```
 
 To run specific tests, you can specify the test name too, something like:
 
 ```bash
-$ python -m pytest conans/test/unittests/client/cmd/export_test.py::ExportTest::test_export_warning -s
+$ python -m pytest conans/test/functional/command/export_test.py::TestRevisionModeSCM::test_revision_mode_scm -s
 ```
 
 The `-s` argument can be useful to see some output that otherwise is captured by *pytest*.
 
 Also, you can run tests against an instance of Artifactory. Those tests should add the attribute
 `artifactory_ready`.
```

### Comparing `conan-2.2.3/conan/api/conan_api.py` & `conan-2.3.0/conan/api/conan_api.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/api/model.py` & `conan-2.3.0/conan/api/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,17 @@
         return str(self)
 
 
 class MultiPackagesList:
     def __init__(self):
         self.lists = {}
 
+    def setdefault(self, key, default):
+        return self.lists.setdefault(key, default)
+
     def __getitem__(self, name):
         try:
             return self.lists[name]
         except KeyError:
             raise ConanException(f"'{name}' doesn't exist is package list")
 
     def add(self, name, pkg_list):
@@ -59,30 +62,43 @@
     def add_error(self, remote_name, error):
         self.lists[remote_name] = {"error": error}
 
     def serialize(self):
         return {k: v.serialize() if isinstance(v, PackagesList) else v
                 for k, v in self.lists.items()}
 
+    def merge(self, other):
+        for k, v in other.lists.items():
+            self.lists.setdefault(k, PackagesList()).merge(v)
+
     @staticmethod
     def load(file):
         content = json.loads(load(file))
         result = {}
         for remote, pkglist in content.items():
             if "error" in pkglist:
                 result[remote] = pkglist
             else:
                 result[remote] = PackagesList.deserialize(pkglist)
         pkglist = MultiPackagesList()
         pkglist.lists = result
         return pkglist
 
     @staticmethod
+    def from_graph(graph, graph_recipes=None, graph_binaries=None):
+        graph = {"graph": graph.serialize()}
+        return MultiPackagesList._define_graph(graph, graph_recipes, graph_binaries)
+
+    @staticmethod
     def load_graph(graphfile, graph_recipes=None, graph_binaries=None):
         graph = json.loads(load(graphfile))
+        return MultiPackagesList._define_graph(graph, graph_recipes, graph_binaries)
+
+    @staticmethod
+    def _define_graph(graph, graph_recipes=None, graph_binaries=None):
         pkglist = MultiPackagesList()
         cache_list = PackagesList()
         if graph_recipes is None and graph_binaries is None:
             recipes = ["*"]
             binaries = ["*"]
         else:
             recipes = [r.lower() for r in graph_recipes or []]
@@ -139,14 +155,24 @@
         return pkglist
 
 
 class PackagesList:
     def __init__(self):
         self.recipes = {}
 
+    def merge(self, other):
+        def recursive_dict_update(d, u):  # TODO: repeated from conandata.py
+            for k, v in u.items():
+                if isinstance(v, dict):
+                    d[k] = recursive_dict_update(d.get(k, {}), v)
+                else:
+                    d[k] = v
+            return d
+        recursive_dict_update(self.recipes, other.recipes)
+
     def split(self):
         """
         Returns a list of PackageList, splitted one per reference.
         This can be useful to parallelize things like upload, parallelizing per-reference
         """
         result = []
         for r, content in self.recipes.items():
```

### Comparing `conan-2.2.3/conan/api/output.py` & `conan-2.3.0/conan/api/output.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/api/subapi/cache.py` & `conan-2.3.0/conan/api/subapi/cache.py`

 * *Files 10% similar despite different names*

```diff
@@ -151,47 +151,66 @@
             info = tarfile.TarInfo(name="pkglist.json")
             data = serialized.encode('utf-8')
             info.size = len(data)
             tgz.addfile(tarinfo=info, fileobj=BytesIO(data))
             tgz.close()
 
     def restore(self, path):
+        if not os.path.isfile(path):
+            raise ConanException(f"Restore archive doesn't exist in {path}")
         with open(path, mode='rb') as file_handler:
             the_tar = tarfile.open(fileobj=file_handler)
             fileobj = the_tar.extractfile("pkglist.json")
             pkglist = fileobj.read()
             the_tar.extractall(path=self.conan_api.cache_folder)
             the_tar.close()
 
+        # After unzipping the files, we need to update the DB that references these files
         out = ConanOutput()
         package_list = PackagesList.deserialize(json.loads(pkglist))
         cache = ClientCache(self.conan_api.cache_folder, self.conan_api.config.global_conf)
         for ref, ref_bundle in package_list.refs().items():
             ref.timestamp = revision_timestamp_now()
             ref_bundle["timestamp"] = ref.timestamp
-            recipe_layout = cache.get_or_create_ref_layout(ref)
+            recipe_layout = cache.get_or_create_ref_layout(ref)  # DB folder entry
             recipe_folder = ref_bundle["recipe_folder"]
             rel_path = os.path.relpath(recipe_layout.base_folder, cache.cache_folder)
             rel_path = rel_path.replace("\\", "/")
+            # In the case of recipes, they are always "in place", so just checking it
             assert rel_path == recipe_folder, f"{rel_path}!={recipe_folder}"
             out.info(f"Restore: {ref} in {recipe_folder}")
             for pref, pref_bundle in package_list.prefs(ref, ref_bundle).items():
                 pref.timestamp = revision_timestamp_now()
                 pref_bundle["timestamp"] = pref.timestamp
-                pkg_layout = cache.get_or_create_pkg_layout(pref)
-                pkg_folder = pref_bundle["package_folder"]
-                out.info(f"Restore: {pref} in {pkg_folder}")
-                # We need to put the package in the final location in the cache
-                shutil.move(os.path.join(cache.cache_folder, pkg_folder), pkg_layout.package())
-                metadata_folder = pref_bundle.get("metadata_folder")
-                if metadata_folder:
-                    out.info(f"Restore: {pref} metadata in {metadata_folder}")
-                    # We need to put the package in the final location in the cache
-                    shutil.move(os.path.join(cache.cache_folder, metadata_folder),
-                                pkg_layout.metadata())
+                pkg_layout = cache.get_or_create_pkg_layout(pref)  # DB Folder entry
+                unzipped_pkg_folder = pref_bundle["package_folder"]
+                out.info(f"Restore: {pref} in {unzipped_pkg_folder}")
+                # If the DB folder entry is different to the disk unzipped one, we need to move it
+                # This happens for built (not downloaded) packages in the source "conan cache save"
+                db_pkg_folder = os.path.relpath(pkg_layout.package(), cache.cache_folder)
+                db_pkg_folder = db_pkg_folder.replace("\\", "/")
+                if db_pkg_folder != unzipped_pkg_folder:
+                    # If a previous package exists, like a previous restore, then remove it
+                    if os.path.exists(pkg_layout.package()):
+                        shutil.rmtree(pkg_layout.package())
+                    shutil.move(os.path.join(cache.cache_folder, unzipped_pkg_folder),
+                                pkg_layout.package())
+                    pref_bundle["package_folder"] = db_pkg_folder
+                unzipped_metadata_folder = pref_bundle.get("metadata_folder")
+                if unzipped_metadata_folder:
+                    out.info(f"Restore: {pref} metadata in {unzipped_metadata_folder}")
+                    db_metadata_folder = os.path.relpath(pkg_layout.metadata(), cache.cache_folder)
+                    db_metadata_folder = db_metadata_folder.replace("\\", "/")
+                    if db_metadata_folder != unzipped_metadata_folder:
+                        # We need to put the package in the final location in the cache
+                        if os.path.exists(pkg_layout.metadata()):
+                            shutil.rmtree(pkg_layout.metadata())
+                        shutil.move(os.path.join(cache.cache_folder, unzipped_metadata_folder),
+                                    pkg_layout.metadata())
+                        pref_bundle["metadata_folder"] = db_metadata_folder
 
         return package_list
 
     def get_backup_sources(self, package_list=None, exclude=True, only_upload=True):
         """Get list of backup source files currently present in the cache,
         either all of them if no argument, or filtered by those belonging to the references in the package_list
```

### Comparing `conan-2.2.3/conan/api/subapi/command.py` & `conan-2.3.0/conan/api/subapi/command.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/api/subapi/config.py` & `conan-2.3.0/conan/api/subapi/config.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/api/subapi/download.py` & `conan-2.3.0/conan/api/subapi/download.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/api/subapi/export.py` & `conan-2.3.0/conan/api/subapi/export.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/api/subapi/graph.py` & `conan-2.3.0/conan/api/subapi/graph.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/api/subapi/install.py` & `conan-2.3.0/conan/api/subapi/install.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/api/subapi/list.py` & `conan-2.3.0/conan/api/subapi/list.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/api/subapi/local.py` & `conan-2.3.0/conan/api/subapi/local.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 
+from conan.api.output import ConanOutput
 from conan.cli import make_abs_path
 from conan.internal.conan_app import ConanApp
 from conans.client.cache.editable import EditablePackages
 from conans.client.conanfile.build import run_build_method
 from conans.client.graph.graph import CONTEXT_HOST
 from conans.client.graph.profile_node_definer import initialize_conanfile_profile
 from conans.client.source import run_source_method
@@ -56,15 +57,16 @@
         output_folder = make_abs_path(output_folder) if output_folder else None
         # Check the conanfile is there, and name/version matches
         self.editable_packages.add(ref, target_path, output_folder=output_folder)
         return ref
 
     def editable_remove(self, path=None, requires=None, cwd=None):
         if path:
-            path = self._conan_api.local.get_conanfile_path(path, cwd, py=True)
+            path = make_abs_path(path, cwd)
+            path = os.path.join(path, "conanfile.py")
         return self.editable_packages.remove(path, requires)
 
     def editable_list(self):
         return self.editable_packages.edited_refs
 
     def source(self, path, name=None, version=None, user=None, channel=None, remotes=None):
         """ calls the 'source()' method of the current (user folder) conanfile.py
```

### Comparing `conan-2.2.3/conan/api/subapi/lockfile.py` & `conan-2.3.0/conan/api/subapi/lockfile.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/api/subapi/new.py` & `conan-2.3.0/conan/api/subapi/new.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/api/subapi/profiles.py` & `conan-2.3.0/conan/api/subapi/profiles.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/api/subapi/remotes.py` & `conan-2.3.0/conan/api/subapi/remotes.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,15 +253,18 @@
 
 def _load(remotes_file):
     if not os.path.exists(remotes_file):
         remote = Remote(CONAN_CENTER_REMOTE_NAME, "https://center.conan.io", True, False)
         _save(remotes_file, [remote])
         return [remote]
 
-    data = json.loads(load(remotes_file))
+    try:
+        data = json.loads(load(remotes_file))
+    except Exception as e:
+        raise ConanException(f"Error loading JSON remotes file '{remotes_file}': {e}")
     result = []
     for r in data.get("remotes", []):
         remote = Remote(r["name"], r["url"], r["verify_ssl"], r.get("disabled", False),
                         r.get("allowed_packages"), r.get("remote_type"))
         result.append(remote)
     return result
```

### Comparing `conan-2.2.3/conan/api/subapi/remove.py` & `conan-2.3.0/conan/api/subapi/remove.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/api/subapi/search.py` & `conan-2.3.0/conan/api/subapi/search.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/api/subapi/upload.py` & `conan-2.3.0/conan/api/subapi/upload.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/cli/args.py` & `conan-2.3.0/conan/cli/args.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/cli/cli.py` & `conan-2.3.0/conan/cli/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,14 +232,22 @@
         assert isinstance(exception, Exception)
         output.error(traceback.format_exc(), error_type="exception")
         msg = exception_message_safe(exception)
         output.error(msg, error_type="exception")
         return ERROR_UNEXPECTED
 
 
+def _warn_python_version():
+    version = sys.version_info
+    if version.minor == 6:
+        ConanOutput().warning("Python 3.6 is end-of-life since 2021. "
+                              "Conan future versions will drop support for it, "
+                              "please upgrade Python", warn_tag="deprecated")
+
+
 def main(args):
     """ main entry point of the conan application, using a Command to
     parse parameters
 
     Exit codes for conan command:
 
         0: Success (done)
@@ -277,10 +285,11 @@
     if sys.platform == 'win32':
         signal.signal(signal.SIGBREAK, ctrl_break_handler)
 
     cli = Cli(conan_api)
     error = SUCCESS
     try:
         cli.run(args)
+        _warn_python_version()
     except BaseException as e:
         error = cli.exception_exit_error(e)
     sys.exit(error)
```

### Comparing `conan-2.2.3/conan/cli/command.py` & `conan-2.3.0/conan/cli/command.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/cli/commands/build.py` & `conan-2.3.0/conan/cli/commands/build.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/cli/commands/cache.py` & `conan-2.3.0/conan/cli/commands/cache.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/cli/commands/config.py` & `conan-2.3.0/conan/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/cli/commands/create.py` & `conan-2.3.0/conan/cli/commands/create.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from conan.cli.args import add_lockfile_args, add_common_install_arguments
 from conan.cli.command import conan_command, OnceArgument
 from conan.cli.commands.export import common_args_export
 from conan.cli.formatters.graph import format_graph_json
 from conan.cli.printers import print_profiles
 from conan.cli.printers.graph import print_graph_packages, print_graph_basic
 from conan.errors import ConanException
+from conans.client.graph.graph import BINARY_BUILD
 from conans.util.files import mkdir
 
 
 @conan_command(group="Creator", formatters={"json": format_graph_json})
 def create(conan_api, parser, *args):
     """
     Create a package.
@@ -22,22 +23,28 @@
     add_common_install_arguments(parser)
     parser.add_argument("--build-require", action='store_true', default=False,
                         help='Whether the package being created is a build-require (to be used'
                              ' as tool_requires() by other packages)')
     parser.add_argument("-tf", "--test-folder", action=OnceArgument,
                         help='Alternative test folder name. By default it is "test_package". '
                              'Use "" to skip the test stage')
+    parser.add_argument("-tm", "--test-missing", action='store_true', default=False,
+                        help='Run the test_package checks only if the package is built from source'
+                             ' but not if it already existed (using --build=missing)')
     parser.add_argument("-bt", "--build-test", action="append",
                         help="Same as '--build' but only for the test_package requires. By default"
                              " if not specified it will take the '--build' value if specified")
+    raw_args = args[0]
     args = parser.parse_args(*args)
 
+    if args.test_missing and args.test_folder == "":
+        raise ConanException('--test-folder="" is incompatible with --test-missing')
+
     cwd = os.getcwd()
     path = conan_api.local.get_conanfile_path(args.path, cwd, py=True)
-    test_conanfile_path = _get_test_conanfile_path(args.test_folder, path)
     overrides = eval(args.lockfile_overrides) if args.lockfile_overrides else None
     lockfile = conan_api.lockfile.get_lockfile(lockfile=args.lockfile,
                                                conanfile_path=path,
                                                cwd=cwd,
                                                partial=args.lockfile_partial,
                                                overrides=overrides)
     remotes = conan_api.remotes.list(args.remote) if not args.no_remote else []
@@ -52,14 +59,33 @@
     # FIXME: Dirty: package type still raw, not processed yet
     is_build = args.build_require or conanfile.package_type == "build-scripts"
     # The package_type is not fully processed at export
     is_python_require = conanfile.package_type == "python-require"
     lockfile = conan_api.lockfile.update_lockfile_export(lockfile, conanfile, ref, is_build)
 
     print_profiles(profile_host, profile_build)
+    if profile_host.runner and not os.environ.get("CONAN_RUNNER_ENVIRONMENT"):
+        from conan.internal.runner.docker import DockerRunner
+        from conan.internal.runner.ssh import SSHRunner
+        from conan.internal.runner.wsl import WSLRunner
+        try:
+            runner_type = profile_host.runner['type'].lower()
+        except KeyError:
+            raise ConanException(f"Invalid runner configuration. 'type' must be defined")
+        runner_instances_map = {
+            'docker': DockerRunner,
+            # 'ssh': SSHRunner,
+            # 'wsl': WSLRunner,
+        }
+        try:
+            runner_instance = runner_instances_map[runner_type]
+        except KeyError:
+            raise ConanException(f"Invalid runner type '{runner_type}'. Allowed values: {', '.join(runner_instances_map.keys())}")
+        return runner_instance(conan_api, 'create', profile_host, profile_build, args, raw_args).run()
+
     if args.build is not None and args.build_test is None:
         args.build_test = args.build
 
     if is_python_require:
         deps_graph = conan_api.graph.load_graph_requires([], [],
                                                          profile_host=profile_host,
                                                          profile_build=profile_build,
@@ -87,14 +113,22 @@
         print_graph_packages(deps_graph)
 
         conan_api.install.install_binaries(deps_graph=deps_graph, remotes=remotes)
         # We update the lockfile, so it will be updated for later ``test_package``
         lockfile = conan_api.lockfile.update_lockfile(lockfile, deps_graph, args.lockfile_packages,
                                                       clean=args.lockfile_clean)
 
+    test_package_folder = getattr(conanfile, "test_package_folder", None) \
+        if args.test_folder is None else args.test_folder
+    test_conanfile_path = _get_test_conanfile_path(test_package_folder, path)
+    # If the user provide --test-missing and the binary was not built from source, skip test_package
+    if args.test_missing and deps_graph.root.dependencies\
+            and deps_graph.root.dependencies[0].dst.binary != BINARY_BUILD:
+        test_conanfile_path = None  # disable it
+
     if test_conanfile_path:
         # TODO: We need arguments for:
         #  - decide update policy "--test_package_update"
         # If it is a string, it will be injected always, if it is a RecipeReference, then it will
         # be replaced only if ``python_requires = "tested_reference_str"``
         tested_python_requires = ref.repr_notime() if is_python_require else ref
         from conan.cli.commands.test import run_test
```

### Comparing `conan-2.2.3/conan/cli/commands/download.py` & `conan-2.3.0/conan/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/cli/commands/editable.py` & `conan-2.3.0/conan/cli/commands/editable.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/cli/commands/export.py` & `conan-2.3.0/conan/cli/commands/export.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/cli/commands/export_pkg.py` & `conan-2.3.0/conan/cli/commands/export_pkg.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/cli/commands/graph.py` & `conan-2.3.0/conan/cli/commands/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,16 @@
 from conan.cli.formatters.graph import format_graph_html, format_graph_json, format_graph_dot
 from conan.cli.formatters.graph.graph_info_text import format_graph_info
 from conan.cli.printers.graph import print_graph_packages, print_graph_basic
 from conan.errors import ConanException
 from conan.internal.deploy import do_deploys
 from conans.client.graph.graph import BINARY_MISSING
 from conans.client.graph.install_graph import InstallGraph
-from conans.errors import ConanConnectionError, NotFoundException
+from conans.errors import NotFoundException
 from conans.model.recipe_ref import ref_matches, RecipeReference
-from conans.model.version_range import VersionRange
 
 
 def explain_formatter_text(data):
     if "closest_binaries" in data:
         # To be able to reuse the print_list_compact method,
         # we need to wrap this in a MultiPackagesList
         pkglist = data["closest_binaries"]
@@ -210,18 +209,15 @@
                                                          is_build_require=args.build_require)
     else:
         deps_graph = conan_api.graph.load_graph_requires(args.requires, args.tool_requires,
                                                          profile_host, profile_build, lockfile,
                                                          remotes, args.update,
                                                          check_updates=args.check_updates)
     print_graph_basic(deps_graph)
-    if deps_graph.error:
-        ConanOutput().info("Graph error", Color.BRIGHT_RED)
-        ConanOutput().info("    {}".format(deps_graph.error), Color.BRIGHT_RED)
-    else:
+    if not deps_graph.error:
         conan_api.graph.analyze_binaries(deps_graph, args.build, remotes=remotes, update=args.update,
                                          lockfile=lockfile)
         print_graph_packages(deps_graph)
 
         conan_api.install.install_system_requires(deps_graph, only_info=True)
         conan_api.install.install_sources(deps_graph, remotes=remotes)
```

### Comparing `conan-2.2.3/conan/cli/commands/inspect.py` & `conan-2.3.0/conan/cli/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/cli/commands/install.py` & `conan-2.3.0/conan/cli/commands/install.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/cli/commands/list.py` & `conan-2.3.0/conan/cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/cli/commands/lock.py` & `conan-2.3.0/conan/cli/commands/lock.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/cli/commands/new.py` & `conan-2.3.0/conan/cli/commands/new.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     """
     Create a new example recipe and source files from a template.
     """
     parser.add_argument("template", help="Template name, "
                         "either a predefined built-in or a user-provided one. "
                         "Available built-in templates: basic, cmake_lib, cmake_exe, "
                         "meson_lib, meson_exe, msbuild_lib, msbuild_exe, bazel_lib, bazel_exe, "
-                        "autotools_lib, autotools_exe, local_recipes_index"
+                        "autotools_lib, autotools_exe, local_recipes_index. "
                         "E.g. 'conan new cmake_lib -d name=hello -d version=0.1'. "
                         "You can define your own templates too by inputting an absolute path "
                         "as your template, or a path relative to your conan home folder."
                         )
     parser.add_argument("-d", "--define", action="append",
                         help="Define a template argument as key=value, e.g., -d name=mypkg")
     parser.add_argument("-f", "--force", action='store_true', help="Overwrite file if it already exists")
```

### Comparing `conan-2.2.3/conan/cli/commands/profile.py` & `conan-2.3.0/conan/cli/commands/profile.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,20 +54,26 @@
 @conan_subcommand()
 def profile_detect(conan_api, parser, subparser, *args):
     """
     Generate a profile using auto-detected values.
     """
     subparser.add_argument("--name", help="Profile name, 'default' if not specified")
     subparser.add_argument("-f", "--force", action='store_true', help="Overwrite if exists")
+    subparser.add_argument("-e", "--exist-ok", action='store_true',
+                           help="If the profile already exist, do not detect a new one")
     args = parser.parse_args(*args)
 
     profile_name = args.name or "default"
     profile_pathname = conan_api.profiles.get_path(profile_name, os.getcwd(), exists=False)
-    if not args.force and os.path.exists(profile_pathname):
-        raise ConanException(f"Profile '{profile_pathname}' already exists")
+    if os.path.exists(profile_pathname):
+        if args.exist_ok:
+            ConanOutput().info(f"Profile '{profile_name}' already exists, skipping detection")
+            return
+        if not args.force:
+            raise ConanException(f"Profile '{profile_pathname}' already exists")
 
     detected_profile = conan_api.profiles.detect()
     ConanOutput().success("\nDetected profile:")
     cli_out_write(detected_profile.dumps())
 
     contents = detected_profile.dumps()
     ConanOutput().warning("This profile is a guess of your environment, please check it.")
```

### Comparing `conan-2.2.3/conan/cli/commands/remote.py` & `conan-2.3.0/conan/cli/commands/remote.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/cli/commands/remove.py` & `conan-2.3.0/conan/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/cli/commands/search.py` & `conan-2.3.0/conan/cli/commands/search.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/cli/commands/source.py` & `conan-2.3.0/conan/cli/commands/source.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/cli/commands/test.py` & `conan-2.3.0/conan/cli/commands/test.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/cli/commands/upload.py` & `conan-2.3.0/conan/cli/commands/upload.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/cli/formatters/graph/graph.py` & `conan-2.3.0/conan/cli/formatters/graph/graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,24 +50,31 @@
             'topics': self._conanfile.topics
         }
 
 
 class _Grapher(object):
     def __init__(self, deps_graph):
         self._deps_graph = deps_graph
-        self.node_map, self.edges = self._build_graph()
+        self.node_map, self._edges = self._build_graph()
         self._nodes = self.node_map.values()
 
     @property
     def nodes(self):
-        ConanOutput().warning("--format=html rendering using 'graph' object is deprecated and "
+        ConanOutput().warning("--format=html/dot rendering using 'graph' object is deprecated and "
                               "will be removed in future 2.X version. Please upgrade your template "
                               "to use 'deps_graph' instead", warn_tag="deprecated")
         return self._nodes
 
+    @property
+    def edges(self):
+        ConanOutput().warning("--format=html/dot rendering using 'graph' object is deprecated and "
+                              "will be removed in future 2.X version. Please upgrade your template "
+                              "to use 'deps_graph' instead", warn_tag="deprecated")
+        return self._edges
+
     def _build_graph(self):
         graph_nodes = self._deps_graph.by_levels()
         build_time_nodes = self._deps_graph.build_time_nodes()
         graph_nodes = reversed([n for level in graph_nodes for n in level])
 
         _node_map = {}
         for i, node in enumerate(graph_nodes):
@@ -91,18 +98,18 @@
                  BINARY_BUILD: "Khaki",
                  BINARY_MISSING: "OrangeRed",
                  BINARY_UPDATE: "SeaGreen"}.get(node.binary, "White")
         return color
 
 
 def _render_graph(graph, error, template, template_folder):
-    deps_graph = json.dumps(graph.serialize())
+    deps_graph = graph.serialize()
     graph = _Grapher(graph)
     from conans import __version__ as client_version
-    template = Template(template)
+    template = Template(template, autoescape=select_autoescape(['html', 'xml']))
     return template.render(deps_graph=deps_graph, graph=graph, error=error,
                            base_template_path=template_folder, version=client_version)
 
 
 def format_graph_html(result):
     graph = result["graph"]
     conan_api = result["conan_api"]
@@ -122,19 +129,15 @@
     if graph.error:
         raise graph.error
 
 
 def format_graph_dot(result):
     graph = result["graph"]
     conan_api = result["conan_api"]
-    package_filter = result["package_filter"]
-    serial = graph.serialize()
-    # TODO: This is not used, it is necessary to update the renderings to use the serialized graph
-    #  instead of the native graph
-    serial = filter_graph(serial, package_filter)
+
     template_folder = os.path.join(conan_api.cache_folder, "templates")
     user_template = os.path.join(template_folder, "graph.dot")
     template = load(user_template) if os.path.isfile(user_template) else graph_info_dot
     cli_out_write(_render_graph(graph, None, template, template_folder))
     if graph.error:
         raise graph.error
```

### Comparing `conan-2.2.3/conan/cli/formatters/graph/graph_info_text.py` & `conan-2.3.0/conan/cli/formatters/graph/graph_info_text.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/cli/formatters/graph/info_graph_html.py` & `conan-2.3.0/conan/cli/formatters/graph/info_graph_html.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,31 +40,35 @@
                     <label for="collapse_packages">Group packages</label>
                 </div>
                  <div>
                     <input type="checkbox" onchange="showPackageType()" id="show_package_type"/>
                     <label for="show_package_type">Show package type</label>
                 </div>
                  <div>
-                    <input type="search" placeholder="Search package..." oninput="searchPackage(this)">
+                    <input type="search" placeholder="Search packages..." oninput="searchPackages(this)">
+                </div>
+                 <div>
+                    <input type="search" placeholder="Exclude packages..." title="Add a comma to exclude an additional package" oninput="excludePackages(this)">
                 </div>
                 <div>
                     <input type="checkbox" onchange="showhideclass('controls')" id="show_controls"/>
                     <label for="show_controls">Show graph controls</label>
                 </div>
                 <div id="controls" class="controls" style="padding:5; display:none"></div>
                 <div id="details"  style="padding:10;" class="noPrint">Package info: Click on one package to show information</div>
                 <div id="error" style="padding:10;" class="noPrint"></div>
             </div>
         </div>
 
         <script type="text/javascript">
-            const graph_data = {{ deps_graph }};
+            const graph_data = {{ deps_graph | tojson }};
             let hide_build = false;
             let hide_test = false;
-            let search_pkg = null;
+            let search_pkgs = null;
+            let excluded_pkgs = null;
             let collapse_packages = false;
             let show_package_type = false;
             let color_map = {Cache: "SkyBlue",
                              Download: "LightGreen",
                              Build: "Yellow",
                              Missing: "Orange",
                              Update: "SeaGreen",
@@ -97,30 +101,45 @@
                         label = node.recipe == "Consumer"? "conanfile": "CLI";
                     if (collapse_packages) {
                         let existing = collapsed_packages[label];
                         targets[node_id] = existing;
                         if (existing) continue;
                         collapsed_packages[label] = node_id;
                     }
+                    if (excluded_pkgs) {
+                        let patterns = excluded_pkgs.split(',')
+                            .map(pattern => pattern.trim())
+                            .filter(pattern => pattern.length > 0)
+                            .map(pattern => pattern.replace(/[-\/\\^$*+?.()|[\]{}]/g, '\\$&'));
+                        if (patterns.some(pattern => label.match(pattern))) {
+                            continue;
+                        }
+                    }
                     if (show_package_type) {
                          label = "<b>" + label + "\n" + "<i>" + node.package_type + "</i>";
                     }
                     borderWidth = 1;
                     borderColor = "SkyBlue";
                     font = {multi: 'html'};
                     shapeProperties = {};
                     let color = color_map[node.binary]
                     if (conflict && conflict.branch1.dst_id == node_id){
                         font.color = "white";
                         color = "Black";
                         shape = "circle";
                     }
-                    if (search_pkg && label.match(search_pkg)) {
-                        borderWidth = 3;
-                        borderColor = "Magenta";
+                    if (search_pkgs) {
+                        let patterns = search_pkgs.split(',')
+                            .map(pattern => pattern.trim())
+                            .filter(pattern => pattern.length > 0)
+                            .map(pattern => pattern.replace(/[-\/\\^$*+?.()|[\]{}]/g, '\\$&'));
+                        if (patterns.some(pattern => label.match(pattern))) {
+                            borderWidth = 3;
+                            borderColor = "Magenta";
+                        }
                     }
                     if (node.test) {
                         font.background = "lightgrey";
                         shapeProperties = {borderDashes: true};
                     }
                     if (node.recipe == "Platform") {
                         font.background = "Violet";
@@ -257,21 +276,21 @@
                 let ids = properties.nodes;
                 let ids_edges = properties.edges;
                 let control = document.getElementById("details");
                 while (control.firstChild) {
                     control.removeChild(control.firstChild);
                 }
                 if(ids[0] || ids_edges[0]) {
-                    console.log("Selected ", ids_edges[0], global_edges.length);
-                    console.log("   selected", global_edges[ids_edges[0]]);
                     selected = graph_data["nodes"][ids[0]] || global_edges[ids_edges[0]];
                     let div = document.createElement('div');
                     let f = Object.fromEntries(Object.entries(selected).filter(([_, v]) => v != null));
-                    div.innerHTML = "<pre>" + JSON.stringify(f, undefined, 2) + "</pre>";
-                    control.appendChild(div);
+                    div.innerText = JSON.stringify(f, undefined, 2);
+                    let div2 = document.createElement('div');
+                    div2.innerHTML = "<pre>" + div.innerHTML + "</pre>";
+                    control.appendChild(div2);
                 }
                 else {
                     control.innerHTML = "<b>Info</b>: Click on a package or edge for more info";
                 }
             });
             function draw() {
                 let scale = network.getScale();
@@ -289,16 +308,20 @@
                 hide_test = !hide_test;
                 draw();
             }
             function collapsePackages() {
                 collapse_packages = !collapse_packages;
                 draw();
             }
-            function searchPackage(e) {
-                search_pkg = e.value;
+            function searchPackages(e) {
+                search_pkgs = e.value;
+                draw();
+            }
+            function excludePackages(e) {
+                excluded_pkgs = e.value;
                 draw();
             }
             function showPackageType(e) {
                 show_package_type = !show_package_type;
                 draw();
             }
             function showhideclass(id) {
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 graph_info_html = r"""
 Show build-requires
 Show test-requires
 ??Group packages
 ??Show package type
 [Unknown INPUT type]
+[Unknown INPUT type]
 ??Show graph controls
 Package info: Click on one package to show information
 """
```

### Comparing `conan-2.2.3/conan/cli/formatters/list/binary_html_table.py` & `conan-2.3.0/conan/cli/formatters/list/binary_html_table.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/cli/formatters/list/list.py` & `conan-2.3.0/conan/cli/formatters/list/list.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/cli/formatters/list/search_table_html.py` & `conan-2.3.0/conan/cli/formatters/list/search_table_html.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/cli/printers/graph.py` & `conan-2.3.0/conan/cli/printers/graph.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/internal/api/detect_api.py` & `conan-2.3.0/conan/internal/api/detect_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,15 +163,14 @@
             "detect_musl_libc() only works on Linux"
         )
         return None
 
     d = tempfile.mkdtemp()
     tmp_file = os.path.join(d, "err")
     try:
-        ldd_output = None
         with open(tmp_file, 'w') as stderr:
             check_output_runner(f"{ldd}", stderr=stderr, ignore_error=True)
         ldd_output = load(tmp_file)
         version = _parse_musl_libc(ldd_output)
         if version is None:
             first_line = ldd_output.partition("\n")[0]
             ConanOutput(scope="detect_api").warning(
@@ -357,57 +356,60 @@
         """
     output = ConanOutput(scope="detect_api")
     cc = os.environ.get("CC", "")
     cxx = os.environ.get("CXX", "")
     if cc or cxx:  # Env defined, use them
         output.info("CC and CXX: %s, %s " % (cc or "None", cxx or "None"))
         command = cc or cxx
+        if "/usr/bin/cc" == command or "/usr/bin/c++" == command:  # Symlinks of linux "alternatives"
+            return _cc_compiler(command)
         if "clang" in command.lower():
-            return _clang_compiler(command)
+            return detect_clang_compiler(command)
         if "gnu-cc" in command or "gcc" in command or "g++" in command or "c++" in command:
-            gcc, gcc_version, compiler_exe = _gcc_compiler(command)
+            gcc, gcc_version, compiler_exe = detect_gcc_compiler(command)
             if platform.system() == "Darwin" and gcc is None:
                 output.error("%s detected as a frontend using apple-clang. "
                              "Compiler not supported" % command)
             return gcc, gcc_version, compiler_exe
         if "icpx" in command or "icx" in command:
-            intel, intel_version, compiler_exe = _intel_compiler(command)
+            intel, intel_version, compiler_exe = detect_intel_compiler(command)
             return intel, intel_version, compiler_exe
         if platform.system() == "SunOS" and command.lower() == "cc":
-            return _sun_cc_compiler(command)
+            return detect_suncc_compiler(command)
         if (platform.system() == "Windows" and command.rstrip('"').endswith(("cl", "cl.exe"))
-            and "clang" not in command):
-            return _msvc_cl_compiler(command)
+                and "clang" not in command):
+            return detect_cl_compiler(command)
 
         # I am not able to find its version
         output.error("Not able to automatically detect '%s' version" % command)
         return None, None, None
 
     if platform.system() == "Windows":
-        version = _detect_vs_ide_version()
-        version = {"17": "193", "16": "192", "15": "191"}.get(str(version))  # Map to compiler
-        if version:
-            return 'msvc', Version(version), None
+        compiler, version, compiler_exe = detect_msvc_compiler()
+        if compiler:
+            return compiler, version, compiler_exe
 
     if platform.system() == "SunOS":
-        sun_cc, sun_cc_version, compiler_exe = _sun_cc_compiler()
+        sun_cc, sun_cc_version, compiler_exe = detect_suncc_compiler()
         if sun_cc:
             return sun_cc, sun_cc_version, compiler_exe
 
     if platform.system() in ["Darwin", "FreeBSD"]:
-        clang, clang_version, compiler_exe = _clang_compiler()  # prioritize clang
+        clang, clang_version, compiler_exe = detect_clang_compiler()  # prioritize clang
         if clang:
             return clang, clang_version, compiler_exe
         return None, None, None
-    else:
-        gcc, gcc_version, compiler_exe = _gcc_compiler()
+    else:  # linux like system
+        compiler, compiler_version, compiler_exe = _cc_compiler()
+        if compiler:
+            return compiler, compiler_version, compiler_exe
+        gcc, gcc_version, compiler_exe = detect_gcc_compiler()
         if gcc:
             return gcc, gcc_version, compiler_exe
-        return _clang_compiler()
-    return None, None, None
+        return detect_clang_compiler()
 
 
 def default_msvc_ide_version(version):
     version = {"193": "17", "192": "16", "191": "15"}.get(str(version))
     if version:
         return Version(version)
 
@@ -420,15 +422,30 @@
         path = vs_path or vs_installation_path(version)
         if path:
             ConanOutput(scope="detect_api").info("Found msvc %s" % version)
             return Version(version)
     return None
 
 
-def _gcc_compiler(compiler_exe="gcc"):
+def _cc_compiler(compiler_exe="cc"):
+    # Try to detect the "cc" linux system "alternative". It could point to gcc or clang
+    try:
+        ret, out = detect_runner('%s --version' % compiler_exe)
+        if ret != 0:
+            return None, None, None
+        compiler = "clang" if "clang" in out else "gcc"
+        installed_version = re.search(r"([0-9]+(\.[0-9])?)", out).group()
+        if installed_version:
+            ConanOutput(scope="detect_api").info("Found cc=%s-%s" % (compiler, installed_version))
+            return compiler, Version(installed_version), compiler_exe
+    except (Exception,):  # to disable broad-except
+        return None, None, None
+
+
+def detect_gcc_compiler(compiler_exe="gcc"):
     try:
         if platform.system() == "Darwin":
             # In Mac OS X check if gcc is a fronted using apple-clang
             _, out = detect_runner("%s --version" % compiler_exe)
             out = out.lower()
             if "clang" in out:
                 return None, None, None
@@ -449,28 +466,30 @@
 
 
 def detect_compiler():
     ConanOutput(scope="detect_api").warning("detect_compiler() is deprecated, use detect_default_compiler()", warn_tag="deprecated")
     compiler, version, _ = detect_default_compiler()
     return compiler, version
 
-def _intel_compiler(compiler_exe="icx"):
+
+def detect_intel_compiler(compiler_exe="icx"):
     try:
         ret, out = detect_runner("%s --version" % compiler_exe)
         if ret != 0:
             return None, None
         compiler = "intel-cc"
         installed_version = re.search(r"(202[0-9]+(\.[0-9])?)", out).group()
         if installed_version:
             ConanOutput(scope="detect_api").info("Found %s %s" % (compiler, installed_version))
             return compiler, Version(installed_version), compiler_exe
     except (Exception,):  # to disable broad-except
         return None, None, None
 
-def _sun_cc_compiler(compiler_exe="cc"):
+
+def detect_suncc_compiler(compiler_exe="cc"):
     try:
         _, out = detect_runner('%s -V' % compiler_exe)
         compiler = "sun-cc"
         installed_version = re.search(r"Sun C.*([0-9]+\.[0-9]+)", out)
         if installed_version:
             installed_version = installed_version.group(1)
         else:
@@ -478,15 +497,15 @@
         if installed_version:
             ConanOutput(scope="detect_api").info("Found %s %s" % (compiler, installed_version))
             return compiler, Version(installed_version), compiler_exe
     except (Exception,):  # to disable broad-except
         return None, None, None
 
 
-def _clang_compiler(compiler_exe="clang"):
+def detect_clang_compiler(compiler_exe="clang"):
     try:
         ret, out = detect_runner('%s --version' % compiler_exe)
         if ret != 0:
             return None, None, None
         if "Apple" in out:
             compiler = "apple-clang"
         elif "clang version" in out:
@@ -497,15 +516,23 @@
         if installed_version:
             ConanOutput(scope="detect_api").info("Found %s %s" % (compiler, installed_version))
             return compiler, Version(installed_version), compiler_exe
     except (Exception,):  # to disable broad-except
         return None, None, None
 
 
-def _msvc_cl_compiler(compiler_exe="cl"):
+def detect_msvc_compiler():
+    version = _detect_vs_ide_version()
+    version = {"17": "193", "16": "192", "15": "191"}.get(str(version))  # Map to compiler
+    if version:
+        return 'msvc', Version(version), None
+    return None, None, None
+
+
+def detect_cl_compiler(compiler_exe="cl"):
     """ only if CC/CXX env-vars are defined pointing to cl.exe, and the VS environment must
     be active to have them in the path
     """
     try:
         compiler_exe = compiler_exe.strip('"')
         ret, out = detect_runner(f'"{compiler_exe}" /?')
         if ret != 0:
```

### Comparing `conan-2.2.3/conan/internal/api/new/autoools_exe.py` & `conan-2.3.0/conan/internal/api/new/autoools_exe.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from conan.tools.files import chdir
 
 
 class {{package_name}}Conan(ConanFile):
     name = "{{name}}"
     version = "{{version}}"
     package_type = "application"
+    win_bash = True
 
     # Optional metadata
     license = "<Put the package license here>"
     author = "<Put your name here> <And your email here>"
     url = "<Package recipe repository url here, for issues about the package>"
     description = "<Description of {package_name} here>"
     topics = ("<Put some tag here>", "<here>", "<and here>")
```

### Comparing `conan-2.2.3/conan/internal/api/new/autotools_lib.py` & `conan-2.3.0/conan/internal/api/new/autotools_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from conan.tools.apple import fix_apple_shared_install_name
 
 
 class {{package_name}}Conan(ConanFile):
     name = "{{name}}"
     version = "{{version}}"
     package_type = "library"
+    win_bash = True
 
     # Optional metadata
     license = "<Put the package license here>"
     author = "<Put your name here> <And your email here>"
     url = "<Package recipe repository url here, for issues about the package>"
     description = "<Description of {package_name} here>"
     topics = ("<Put some tag here>", "<here>", "<and here>")
@@ -88,14 +89,15 @@
 from conan.tools.layout import basic_layout
 from conan.tools.build import can_run
 
 
 class {{package_name}}TestConan(ConanFile):
     settings = "os", "compiler", "build_type", "arch"
     generators = "AutotoolsDeps", "AutotoolsToolchain"
+    win_bash = True
 
     def requirements(self):
         self.requires(self.tested_reference_str)
 
     def build(self):
         autotools = Autotools(self)
         autotools.autoreconf()
```

### Comparing `conan-2.2.3/conan/internal/api/new/basic.py` & `conan-2.3.0/conan/internal/api/new/basic.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/internal/api/new/bazel_exe.py` & `conan-2.3.0/conan/internal/api/new/bazel_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/internal/api/new/bazel_lib.py` & `conan-2.3.0/conan/internal/api/new/bazel_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/internal/api/new/cmake_exe.py` & `conan-2.3.0/conan/internal/api/new/cmake_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/internal/api/new/cmake_lib.py` & `conan-2.3.0/conan/internal/api/new/cmake_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/internal/api/new/local_recipes_index.py` & `conan-2.3.0/conan/internal/api/new/local_recipes_index.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/internal/api/new/meson_exe.py` & `conan-2.3.0/conan/internal/api/new/meson_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/internal/api/new/meson_lib.py` & `conan-2.3.0/conan/internal/api/new/meson_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/internal/api/new/msbuild_exe.py` & `conan-2.3.0/conan/internal/api/new/msbuild_exe.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/internal/api/new/msbuild_lib.py` & `conan-2.3.0/conan/internal/api/new/msbuild_lib.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/internal/cache/cache.py` & `conan-2.3.0/conan/internal/cache/cache.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/internal/cache/conan_reference_layout.py` & `conan-2.3.0/conan/internal/cache/conan_reference_layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/internal/cache/db/cache_database.py` & `conan-2.3.0/conan/internal/cache/db/cache_database.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/internal/cache/db/packages_table.py` & `conan-2.3.0/conan/internal/cache/db/packages_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,28 +35,28 @@
         where_dict = {
             self.columns.reference: str(pref.ref),
             self.columns.rrev: pref.ref.revision,
             self.columns.pkgid: pref.package_id,
             self.columns.prev: pref.revision,
         }
         where_expr = ' AND '.join(
-            [f'{k}="{v}" ' if v is not None else f'{k} IS NULL' for k, v in where_dict.items()])
+            [f"{k}='{v}' " if v is not None else f'{k} IS NULL' for k, v in where_dict.items()])
         return where_expr
 
     def _set_clause(self, pref: PkgReference, path=None, build_id=None):
         set_dict = {
             self.columns.reference: str(pref.ref),
             self.columns.rrev: pref.ref.revision,
             self.columns.pkgid: pref.package_id,
             self.columns.prev: pref.revision,
             self.columns.path: path,
             self.columns.timestamp: pref.timestamp,
             self.columns.build_id: build_id,
         }
-        set_expr = ', '.join([f'{k} = "{v}"' for k, v in set_dict.items() if v is not None])
+        set_expr = ', '.join([f"{k} = '{v}'" for k, v in set_dict.items() if v is not None])
         return set_expr
 
     def get(self, pref: PkgReference):
         """ Returns the row matching the reference or fails """
         where_clause = self._where_clause(pref)
         query = f'SELECT * FROM {self.table_name} ' \
                 f'WHERE {where_clause};'
@@ -103,70 +103,70 @@
     def update_lru(self, pref):
         assert pref.revision is not None
         # TODO: InstallGraph is dropping the pref.timestamp, cannot be checked here yet
         # assert pref.timestamp is not None, f"PREF _TIMESSTAMP IS NONE {repr(pref)}"
         where_clause = self._where_clause(pref)
         lru = timestamp_now()
         query = f"UPDATE {self.table_name} " \
-                f'SET {self.columns.lru} = "{lru}" ' \
+                f"SET {self.columns.lru} = '{lru}' " \
                 f"WHERE {where_clause};"
         with self.db_connection() as conn:
             conn.execute(query)
 
     def remove_build_id(self, pref):
         where_clause = self._where_clause(pref)
         query = f"UPDATE {self.table_name} " \
-                f'SET {self.columns.build_id} = "null" ' \
+                f"SET {self.columns.build_id} = 'null' " \
                 f"WHERE {where_clause};"
         with self.db_connection() as conn:
             try:
                 conn.execute(query)
             except sqlite3.IntegrityError:
                 raise ConanReferenceAlreadyExistsInDB(f"Reference '{repr(pref)}' already exists")
 
     def remove_recipe(self, ref: RecipeReference):
         # can't use the _where_clause, because that is an exact match on the package_id, etc
         query = f"DELETE FROM {self.table_name} " \
-                f'WHERE {self.columns.reference} = "{str(ref)}" ' \
-                f'AND {self.columns.rrev} = "{ref.revision}" '
+                f"WHERE {self.columns.reference} = '{str(ref)}' " \
+                f"AND {self.columns.rrev} = '{ref.revision}' "
         with self.db_connection() as conn:
             conn.execute(query)
 
     def remove(self, pref: PkgReference):
         where_clause = self._where_clause(pref)
         query = f"DELETE FROM {self.table_name} " \
                 f"WHERE {where_clause};"
         with self.db_connection() as conn:
             conn.execute(query)
 
     def get_package_revisions_references(self, pref: PkgReference, only_latest_prev=False):
         assert pref.ref.revision, "To search package revisions you must provide a recipe revision."
         assert pref.package_id, "To search package revisions you must provide a package id."
-        check_prev = f'AND {self.columns.prev} = "{pref.revision}" ' if pref.revision else ''
+        check_prev = f"AND {self.columns.prev} = '{pref.revision}' " if pref.revision else ""
         if only_latest_prev:
             query = f'SELECT {self.columns.reference}, ' \
                     f'{self.columns.rrev}, ' \
                     f'{self.columns.pkgid}, ' \
                     f'{self.columns.prev}, ' \
                     f'{self.columns.path}, ' \
                     f'MAX({self.columns.timestamp}), ' \
                     f'{self.columns.build_id}, ' \
                     f'{self.columns.lru} ' \
                     f'FROM {self.table_name} ' \
-                    f'WHERE {self.columns.rrev} = "{pref.ref.revision}" ' \
-                    f'AND {self.columns.reference} = "{str(pref.ref)}" ' \
-                    f'AND {self.columns.pkgid} = "{pref.package_id}" ' \
+                    f"WHERE {self.columns.rrev} = '{pref.ref.revision}' " \
+                    f"AND {self.columns.reference} = '{str(pref.ref)}' " \
+                    f"AND {self.columns.pkgid} = '{pref.package_id}' " \
                     f'{check_prev} ' \
                     f'AND {self.columns.prev} IS NOT NULL ' \
                     f'GROUP BY {self.columns.pkgid} '
         else:
             query = f'SELECT * FROM {self.table_name} ' \
-                    f'WHERE {self.columns.rrev} = "{pref.ref.revision}" ' \
-                    f'AND {self.columns.reference} = "{str(pref.ref)}" ' \
-                    f'AND {self.columns.pkgid} = "{pref.package_id}" ' \
+                    f"WHERE {self.columns.rrev} = '{pref.ref.revision}' " \
+                    f"AND {self.columns.reference} = '{str(pref.ref)}' " \
+                    f"AND {self.columns.pkgid} = '{pref.package_id}' " \
                     f'{check_prev} ' \
                     f'AND {self.columns.prev} IS NOT NULL ' \
                     f'ORDER BY {self.columns.timestamp} DESC'
         with self.db_connection() as conn:
             r = conn.execute(query)
             for row in r.fetchall():
                 yield self._as_dict(self.row_type(*row))
@@ -181,20 +181,20 @@
                     f'{self.columns.pkgid}, ' \
                     f'{self.columns.prev}, ' \
                     f'{self.columns.path}, ' \
                     f'MAX({self.columns.timestamp}), ' \
                     f'{self.columns.build_id}, ' \
                     f'{self.columns.lru} ' \
                     f'FROM {self.table_name} ' \
-                    f'WHERE {self.columns.rrev} = "{ref.revision}" ' \
-                    f'AND {self.columns.reference} = "{str(ref)}" ' \
+                    f"WHERE {self.columns.rrev} = '{ref.revision}' " \
+                    f"AND {self.columns.reference} = '{str(ref)}' " \
                     f'GROUP BY {self.columns.pkgid} '
         else:
             query = f'SELECT * FROM {self.table_name} ' \
-                    f'WHERE {self.columns.rrev} = "{ref.revision}" ' \
-                    f'AND {self.columns.reference} = "{str(ref)}" ' \
+                    f"WHERE {self.columns.rrev} = '{ref.revision}' " \
+                    f"AND {self.columns.reference} = '{str(ref)}' " \
                     f'AND {self.columns.prev} IS NOT NULL ' \
                     f'ORDER BY {self.columns.timestamp} DESC'
         with self.db_connection() as conn:
             r = conn.execute(query)
             for row in r.fetchall():
                 yield self._as_dict(self.row_type(*row))
```

### Comparing `conan-2.2.3/conan/internal/cache/db/recipes_table.py` & `conan-2.3.0/conan/internal/cache/db/recipes_table.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     def _where_clause(self, ref):
         assert isinstance(ref, RecipeReference)
         where_dict = {
             self.columns.reference: str(ref),
             self.columns.rrev: ref.revision,
         }
         where_expr = ' AND '.join(
-            [f'{k}="{v}" ' if v is not None else f'{k} IS NULL' for k, v in where_dict.items()])
+            [f"{k}='{v}' " if v is not None else f'{k} IS NULL' for k, v in where_dict.items()])
         return where_expr
 
     def create(self, path, ref: RecipeReference):
         assert ref is not None
         assert ref.revision is not None
         assert ref.timestamp is not None
         placeholders = ', '.join(['?' for _ in range(len(self.columns))])
@@ -50,27 +50,27 @@
             except sqlite3.IntegrityError:
                 raise ConanReferenceAlreadyExistsInDB(f"Reference '{repr(ref)}' already exists")
 
     def update_timestamp(self, ref: RecipeReference):
         assert ref.revision is not None
         assert ref.timestamp is not None
         query = f"UPDATE {self.table_name} " \
-                f'SET {self.columns.timestamp} = "{ref.timestamp}" ' \
-                f'WHERE {self.columns.reference}="{str(ref)}" ' \
-                f'AND {self.columns.rrev} = "{ref.revision}" '
+                f"SET {self.columns.timestamp} = '{ref.timestamp}' " \
+                f"WHERE {self.columns.reference}='{str(ref)}' " \
+                f"AND {self.columns.rrev} = '{ref.revision}' "
         with self.db_connection() as conn:
             conn.execute(query)
 
     def update_lru(self, ref):
         assert ref.revision is not None
         assert ref.timestamp is not None
         where_clause = self._where_clause(ref)
         lru = timestamp_now()
         query = f"UPDATE {self.table_name} " \
-                f'SET {self.columns.lru} = "{lru}" ' \
+                f"SET {self.columns.lru} = '{lru}' " \
                 f"WHERE {where_clause};"
         with self.db_connection() as conn:
             conn.execute(query)
 
     def remove(self, ref: RecipeReference):
         where_clause = self._where_clause(ref)
         query = f"DELETE FROM {self.table_name} " \
@@ -91,16 +91,16 @@
         with self.db_connection() as conn:
             r = conn.execute(query)
             result = [self._as_dict(self.row_type(*row)) for row in r.fetchall()]
         return result
 
     def get_recipe(self, ref: RecipeReference):
         query = f'SELECT * FROM {self.table_name} ' \
-                f'WHERE {self.columns.reference}="{str(ref)}" ' \
-                f'AND {self.columns.rrev} = "{ref.revision}" '
+                f"WHERE {self.columns.reference}='{str(ref)}' " \
+                f"AND {self.columns.rrev} = '{ref.revision}' "
         with self.db_connection() as conn:
             r = conn.execute(query)
             row = r.fetchone()
             if not row:
                 raise ConanReferenceDoesNotExistInDB(f"Recipe '{ref.repr_notime()}' not found")
             ret = self._as_dict(self.row_type(*row))
         return ret
@@ -108,28 +108,28 @@
     def get_latest_recipe(self, ref: RecipeReference):
         query = f'SELECT {self.columns.reference}, ' \
                 f'{self.columns.rrev}, ' \
                 f'{self.columns.path}, ' \
                 f'MAX({self.columns.timestamp}), ' \
                 f'{self.columns.lru} ' \
                 f'FROM {self.table_name} ' \
-                f'WHERE {self.columns.reference} = "{str(ref)}" ' \
+                f"WHERE {self.columns.reference} = '{str(ref)}' " \
                 f'GROUP BY {self.columns.reference} '  # OTHERWISE IT FAILS THE MAX()
 
         with self.db_connection() as conn:
             r = conn.execute(query)
             row = r.fetchone()
             if row is None:
                 raise ConanReferenceDoesNotExistInDB(f"Recipe '{ref}' not found")
             ret = self._as_dict(self.row_type(*row))
         return ret
 
     def get_recipe_revisions_references(self, ref: RecipeReference):
         assert ref.revision is None
         query = f'SELECT * FROM {self.table_name} ' \
-                f'WHERE {self.columns.reference} = "{str(ref)}" ' \
+                f"WHERE {self.columns.reference} = '{str(ref)}' " \
                 f'ORDER BY {self.columns.timestamp} DESC'
 
         with self.db_connection() as conn:
             r = conn.execute(query)
             ret = [self._as_dict(self.row_type(*row))["ref"] for row in r.fetchall()]
         return ret
```

### Comparing `conan-2.2.3/conan/internal/cache/db/table.py` & `conan-2.3.0/conan/internal/cache/db/table.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/internal/cache/home_paths.py` & `conan-2.3.0/conan/internal/cache/home_paths.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/internal/conan_app.py` & `conan-2.3.0/conan/internal/conan_app.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/internal/deploy.py` & `conan-2.3.0/conan/internal/deploy.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/internal/integrity_check.py` & `conan-2.3.0/conan/internal/integrity_check.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/internal/internal_tools.py` & `conan-2.3.0/conan/internal/internal_tools.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/internal/upload_metadata.py` & `conan-2.3.0/conan/internal/upload_metadata.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/android/utils.py` & `conan-2.3.0/conan/tools/android/utils.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/apple/__init__.py` & `conan-2.3.0/conan/tools/apple/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/apple/apple.py` & `conan-2.3.0/conan/tools/apple/apple.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,74 +26,90 @@
 
 def to_apple_arch(conanfile, default=None):
     """converts conan-style architecture into Apple-style arch"""
     arch_ = conanfile.settings.get_safe("arch")
     return _to_apple_arch(arch_, default)
 
 
-def apple_sdk_path(conanfile):
+def apple_sdk_path(conanfile, is_cross_building=True):
     sdk_path = conanfile.conf.get("tools.apple:sdk_path")
     if not sdk_path:
         # XCRun already knows how to extract os.sdk from conanfile.settings
         sdk_path = XCRun(conanfile).sdk_path
+    if not sdk_path and is_cross_building:
+        raise ConanException(
+            "Apple SDK path not found. For cross-compilation, you must "
+            "provide a valid SDK path in 'tools.apple:sdk_path' config."
+        )
     return sdk_path
 
 
 def get_apple_sdk_fullname(conanfile):
     """
     Returns the 'os.sdk' + 'os.sdk_version ' value. Every user should specify it because
     there could be several ones depending on the OS architecture.
 
     Note: In case of MacOS it'll be the same for all the architectures.
     """
     os_ = conanfile.settings.get_safe('os')
     os_sdk = conanfile.settings.get_safe('os.sdk')
     os_sdk_version = conanfile.settings.get_safe('os.sdk_version') or ""
-
     if os_sdk:
         return "{}{}".format(os_sdk, os_sdk_version)
     elif os_ == "Macos":  # it has only a single value for all the architectures
         return "{}{}".format("macosx", os_sdk_version)
     elif is_apple_os(conanfile):
         raise ConanException("Please, specify a suitable value for os.sdk.")
 
 
-def apple_min_version_flag(os_version, os_sdk, subsystem):
+def apple_min_version_flag(conanfile):
     """compiler flag name which controls deployment target"""
-    if not os_version or not os_sdk:
-        return ''
+    os_ = conanfile.settings.get_safe('os')
+    os_sdk = conanfile.settings.get_safe('os.sdk')
+    os_sdk = os_sdk or ("macosx" if os_ == "Macos" else None)
+    os_version = conanfile.settings.get_safe("os.version")
+    if not os_sdk or not os_version:
+        # Legacy behavior
+        return ""
+    if conanfile.settings.get_safe("os.subsystem") == 'catalyst':
+        os_sdk = "iphoneos"
+    return {
+        "macosx": f"-mmacosx-version-min={os_version}",
+        "iphoneos": f"-mios-version-min={os_version}",
+        "iphonesimulator": f"-mios-simulator-version-min={os_version}",
+        "watchos": f"-mwatchos-version-min={os_version}",
+        "watchsimulator": f"-mwatchos-simulator-version-min={os_version}",
+        "appletvos": f"-mtvos-version-min={os_version}",
+        "appletvsimulator": f"-mtvos-simulator-version-min={os_version}",
+        "xros": f"-target arm64-apple-xros{os_version}",
+        "xrsimulator": f"-target arm64-apple-xros{os_version}-simulator",
+    }.get(os_sdk, "")
 
-    # FIXME: This guess seems wrong, nothing has to be guessed, but explicit
-    flag = ''
-    if 'macosx' in os_sdk:
-        flag = '-mmacosx-version-min'
-    elif 'iphoneos' in os_sdk:
-        flag = '-mios-version-min'
-    elif 'iphonesimulator' in os_sdk:
-        flag = '-mios-simulator-version-min'
-    elif 'watchos' in os_sdk:
-        flag = '-mwatchos-version-min'
-    elif 'watchsimulator' in os_sdk:
-        flag = '-mwatchos-simulator-version-min'
-    elif 'appletvos' in os_sdk:
-        flag = '-mtvos-version-min'
-    elif 'appletvsimulator' in os_sdk:
-        flag = '-mtvos-simulator-version-min'
-    elif 'xros' in os_sdk:
-        # need early return as string did not fit into the "normal" schema
-        return f'-target arm64-apple-xros{os_version}'
-    elif 'xrsimulator' in os_sdk:
-        # need early return as string did not fit into the "normal" schema
-        return f'-target arm64-apple-xros{os_version}-simulator'
-
-    if subsystem == 'catalyst':
-        # especial case, despite Catalyst is macOS, it requires an iOS version argument
-        flag = '-mios-version-min'
 
-    return f"{flag}={os_version}" if flag else ''
+def resolve_apple_flags(conanfile, is_cross_building=False):
+    """
+    Gets the most common flags in Apple systems. If it's a cross-building context
+    SDK path is mandatory so if it could raise an exception if SDK is not found.
+
+    :param conanfile: <ConanFile> instance.
+    :param is_cross_building: boolean to indicate if it's a cross-building context.
+    :return: tuple of Apple flags (apple_min_version_flag, apple_arch, apple_isysroot_flag).
+    """
+    if not is_apple_os(conanfile):
+        # Keeping legacy defaults
+        return "", None, None
+
+    apple_arch_flag = apple_isysroot_flag = None
+    if is_cross_building:
+        arch = to_apple_arch(conanfile)
+        sdk_path = apple_sdk_path(conanfile, is_cross_building=is_cross_building)
+        apple_isysroot_flag = f"-isysroot {sdk_path}" if sdk_path else ""
+        apple_arch_flag = f"-arch {arch}" if arch else ""
+    min_version_flag = apple_min_version_flag(conanfile)
+    return min_version_flag, apple_arch_flag, apple_isysroot_flag
 
 
 class XCRun:
     """
     XCRun is a wrapper for the Apple **xcrun** tool used to get information for building.
     """
```

### Comparing `conan-2.2.3/conan/tools/apple/xcodebuild.py` & `conan-2.3.0/conan/tools/apple/xcodebuild.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/apple/xcodedeps.py` & `conan-2.3.0/conan/tools/apple/xcodedeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/apple/xcodetoolchain.py` & `conan-2.3.0/conan/tools/apple/xcodetoolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/build/__init__.py` & `conan-2.3.0/conan/tools/build/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/build/cppstd.py` & `conan-2.3.0/conan/tools/build/cppstd.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/build/cpu.py` & `conan-2.3.0/conan/tools/build/cpu.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/build/cross_building.py` & `conan-2.3.0/conan/tools/build/cross_building.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/build/flags.py` & `conan-2.3.0/conan/tools/build/flags.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/build/stdcpp_library.py` & `conan-2.3.0/conan/tools/build/stdcpp_library.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/cmake/cmake.py` & `conan-2.3.0/conan/tools/cmake/cmake.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,29 +81,25 @@
         :param stdout: Use it to redirect stdout to this stream
         :param stderr: Use it to redirect stderr to this stream
         """
         self._conanfile.output.info("Running CMake.configure()")
         cmakelist_folder = self._conanfile.source_folder
         if build_script_folder:
             cmakelist_folder = os.path.join(self._conanfile.source_folder, build_script_folder)
+        cmakelist_folder = cmakelist_folder.replace("\\", "/")
 
         build_folder = self._conanfile.build_folder
-        generator_folder = self._conanfile.generators_folder
-
         mkdir(self._conanfile, build_folder)
 
         arg_list = [self._cmake_program]
         if self._generator:
             arg_list.append('-G "{}"'.format(self._generator))
         if self._toolchain_file:
-            if os.path.isabs(self._toolchain_file):
-                toolpath = self._toolchain_file
-            else:
-                toolpath = os.path.join(generator_folder, self._toolchain_file)
-            arg_list.append('-DCMAKE_TOOLCHAIN_FILE="{}"'.format(toolpath.replace("\\", "/")))
+            toolpath = self._toolchain_file.replace("\\", "/")
+            arg_list.append('-DCMAKE_TOOLCHAIN_FILE="{}"'.format(toolpath))
         if self._conanfile.package_folder:
             pkg_folder = self._conanfile.package_folder.replace("\\", "/")
             arg_list.append('-DCMAKE_INSTALL_PREFIX="{}"'.format(pkg_folder))
 
         if not variables:
             variables = {}
         self._cache_variables.update(variables)
```

### Comparing `conan-2.2.3/conan/tools/cmake/cmakedeps/cmakedeps.py` & `conan-2.3.0/conan/tools/cmake/cmakedeps/cmakedeps.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from conan.tools.cmake.cmakedeps.templates.macros import MacrosTemplate
 from conan.tools.cmake.cmakedeps.templates.target_configuration import TargetConfigurationTemplate
 from conan.tools.cmake.cmakedeps.templates.target_data import ConfigDataTemplate
 from conan.tools.cmake.cmakedeps.templates.targets import TargetsTemplate
 from conan.tools.files import save
 from conans.client.generators import relativize_generated_file
 from conan.errors import ConanException
+from conans.model.dependencies import get_transitive_requires
 
 
 class CMakeDeps(object):
 
     def __init__(self, conanfile):
         self._conanfile = conanfile
         self.arch = self._conanfile.settings.get_safe("arch")
@@ -216,7 +217,11 @@
             set(CONANDEPS_LEGACY {% for t in configs %} {{t.root_target_name}} {% endfor %})
             """)
 
         template = Template(template, trim_blocks=True, lstrip_blocks=True,
                             undefined=jinja2.StrictUndefined)
         conandeps = template.render({"configs": configs})
         save(self._conanfile, "conandeps_legacy.cmake", conandeps)
+
+    def get_transitive_requires(self, conanfile):
+        # Prepared to filter transitive tool-requires with visible=True
+        return get_transitive_requires(self._conanfile, conanfile)
```

### Comparing `conan-2.2.3/conan/tools/cmake/cmakedeps/templates/__init__.py` & `conan-2.3.0/conan/tools/cmake/cmakedeps/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/cmake/cmakedeps/templates/config.py` & `conan-2.3.0/conan/tools/cmake/cmakedeps/templates/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,14 +33,17 @@
                 "config_suffix": self.config_suffix,
                 "check_components_exist": self.cmakedeps.check_components_exist,
                 "targets_include_file": targets_include}
 
     @property
     def template(self):
         return textwrap.dedent("""\
+        {%- macro pkg_var(pkg_name, var, config_suffix) -%}
+             {{'${'+pkg_name+'_'+var+config_suffix+'}'}}
+        {%- endmacro -%}
         ########## MACROS ###########################################################################
         #############################################################################################
 
         # Requires CMake > 3.15
         if(${CMAKE_VERSION} VERSION_LESS "3.15")
             message(FATAL_ERROR "The 'CMakeDeps' generator only works with CMake >= 3.15")
         endif()
@@ -53,38 +56,38 @@
 
         include(${CMAKE_CURRENT_LIST_DIR}/cmakedeps_macros.cmake)
         include(${CMAKE_CURRENT_LIST_DIR}/{{ targets_include_file }})
         include(CMakeFindDependencyMacro)
 
         check_build_type_defined()
 
-        foreach(_DEPENDENCY {{ '${' + pkg_name + '_FIND_DEPENDENCY_NAMES' + '}' }} )
+        foreach(_DEPENDENCY {{ pkg_var(pkg_name, 'FIND_DEPENDENCY_NAMES', '') }} )
             # Check that we have not already called a find_package with the transitive dependency
             if(NOT {{ '${_DEPENDENCY}' }}_FOUND)
                 find_dependency({{ '${_DEPENDENCY}' }} REQUIRED ${${_DEPENDENCY}_FIND_MODE})
             endif()
         endforeach()
 
         set({{ file_name }}_VERSION_STRING "{{ version }}")
-        set({{ file_name }}_INCLUDE_DIRS {{ '${' + pkg_name + '_INCLUDE_DIRS' + config_suffix + '}' }} )
-        set({{ file_name }}_INCLUDE_DIR {{ '${' + pkg_name + '_INCLUDE_DIRS' + config_suffix + '}' }} )
-        set({{ file_name }}_LIBRARIES {{ '${' + pkg_name + '_LIBRARIES' + config_suffix + '}' }} )
-        set({{ file_name }}_DEFINITIONS {{ '${' + pkg_name + '_DEFINITIONS' + config_suffix + '}' }} )
+        set({{ file_name }}_INCLUDE_DIRS {{ pkg_var(pkg_name, 'INCLUDE_DIRS', config_suffix) }} )
+        set({{ file_name }}_INCLUDE_DIR {{ pkg_var(pkg_name, 'INCLUDE_DIRS', config_suffix) }} )
+        set({{ file_name }}_LIBRARIES {{ pkg_var(pkg_name, 'LIBRARIES', config_suffix) }} )
+        set({{ file_name }}_DEFINITIONS {{ pkg_var(pkg_name, 'DEFINITIONS', config_suffix) }} )
 
         # Only the first installed configuration is included to avoid the collision
-        foreach(_BUILD_MODULE {{ '${' + pkg_name + '_BUILD_MODULES_PATHS' + config_suffix + '}' }} )
+        foreach(_BUILD_MODULE {{ pkg_var(pkg_name, 'BUILD_MODULES_PATHS', config_suffix) }} )
             message({% raw %}${{% endraw %}{{ file_name }}_MESSAGE_MODE} "Conan: Including build module from '${_BUILD_MODULE}'")
             include({{ '${_BUILD_MODULE}' }})
         endforeach()
 
         {% if check_components_exist %}
         # Check that the specified components in the find_package(Foo COMPONENTS x y z) are there
         # This is the variable filled by CMake with the requested components in find_package
         if({{ file_name }}_FIND_COMPONENTS)
-            foreach(_FIND_COMPONENT {{ '${'+file_name+'_FIND_COMPONENTS}' }})
+            foreach(_FIND_COMPONENT {{ pkg_var(file_name, 'FIND_COMPONENTS', '') }})
                 if (TARGET ${_FIND_COMPONENT})
                     message({% raw %}${{% endraw %}{{ file_name }}_MESSAGE_MODE} "Conan: Component '${_FIND_COMPONENT}' found in package '{{ pkg_name }}'")
                 else()
                     message(FATAL_ERROR "Conan: Component '${_FIND_COMPONENT}' NOT found in package '{{ pkg_name }}'")
                 endif()
             endforeach()
         endif()
```

### Comparing `conan-2.2.3/conan/tools/cmake/cmakedeps/templates/config_version.py` & `conan-2.3.0/conan/tools/cmake/cmakedeps/templates/config_version.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/cmake/cmakedeps/templates/macros.py` & `conan-2.3.0/conan/tools/cmake/cmakedeps/templates/macros.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/cmake/cmakedeps/templates/target_configuration.py` & `conan-2.3.0/conan/tools/cmake/cmakedeps/templates/target_configuration.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import textwrap
 
 from conan.tools.cmake.cmakedeps.templates import CMakeDepsFileTemplate
-from conans.model.dependencies import get_transitive_requires
 
 """
 
 FooTarget-release.cmake
 
 """
 
@@ -41,166 +40,169 @@
 
     @property
     def template(self):
         return textwrap.dedent("""\
         # Avoid multiple calls to find_package to append duplicated properties to the targets
         include_guard()
 
-        {%- macro tvalue(pkg_name, comp_name, var, config_suffix) -%}
+        {%- macro comp_var(pkg_name, comp_name, var, config_suffix) -%}
             {{'${'+pkg_name+'_'+comp_name+'_'+var+config_suffix+'}'}}
         {%- endmacro -%}
+        {%- macro pkg_var(pkg_name, var, config_suffix) -%}
+            {{'${'+pkg_name+'_'+var+config_suffix+'}'}}
+        {%- endmacro -%}
 
         ########### VARIABLES #######################################################################
         #############################################################################################
         set({{ pkg_name }}_FRAMEWORKS_FOUND{{ config_suffix }} "") # Will be filled later
-        conan_find_apple_frameworks({{ pkg_name }}_FRAMEWORKS_FOUND{{ config_suffix }} "{{ '${' }}{{ pkg_name }}_FRAMEWORKS{{ config_suffix }}}" "{{ '${' }}{{ pkg_name }}_FRAMEWORK_DIRS{{ config_suffix }}}")
+        conan_find_apple_frameworks({{ pkg_name }}_FRAMEWORKS_FOUND{{ config_suffix }} "{{ pkg_var(pkg_name, 'FRAMEWORKS', config_suffix) }}" "{{ pkg_var(pkg_name, 'FRAMEWORK_DIRS', config_suffix) }}")
 
         set({{ pkg_name }}_LIBRARIES_TARGETS "") # Will be filled later
 
 
         ######## Create an interface target to contain all the dependencies (frameworks, system and conan deps)
         if(NOT TARGET {{ pkg_name+'_DEPS_TARGET'}})
             add_library({{ pkg_name+'_DEPS_TARGET'}} INTERFACE IMPORTED)
         endif()
 
         set_property(TARGET {{ pkg_name + '_DEPS_TARGET'}}
                      APPEND PROPERTY INTERFACE_LINK_LIBRARIES
-                     $<$<CONFIG:{{configuration}}>:{{ '${'+pkg_name+'_FRAMEWORKS_FOUND'+config_suffix+'}' }}>
-                     $<$<CONFIG:{{configuration}}>:{{ '${'+pkg_name+'_SYSTEM_LIBS'+config_suffix+'}' }}>
+                     $<$<CONFIG:{{configuration}}>:{{ pkg_var(pkg_name, 'FRAMEWORKS_FOUND', config_suffix) }}>
+                     $<$<CONFIG:{{configuration}}>:{{ pkg_var(pkg_name, 'SYSTEM_LIBS', config_suffix) }}>
                      $<$<CONFIG:{{configuration}}>:{{ deps_targets_names }}>)
 
         ####### Find the libraries declared in cpp_info.libs, create an IMPORTED target for each one and link the
         ####### {{pkg_name}}_DEPS_TARGET to all of them
-        conan_package_library_targets("{{ '${' }}{{ pkg_name }}_LIBS{{ config_suffix }}}"    # libraries
-                                      "{{ '${' }}{{ pkg_name }}_LIB_DIRS{{ config_suffix }}}" # package_libdir
-                                      "{{ '${' }}{{ pkg_name }}_BIN_DIRS{{ config_suffix }}}" # package_bindir
-                                      "{{ '${' }}{{ pkg_name }}_LIBRARY_TYPE{{ config_suffix }}}"
-                                      "{{ '${' }}{{ pkg_name }}_IS_HOST_WINDOWS{{ config_suffix }}}"
+        conan_package_library_targets("{{ pkg_var(pkg_name, 'LIBS', config_suffix) }}"    # libraries
+                                      "{{ pkg_var(pkg_name, 'LIB_DIRS', config_suffix) }}" # package_libdir
+                                      "{{ pkg_var(pkg_name, 'BIN_DIRS', config_suffix) }}" # package_bindir
+                                      "{{ pkg_var(pkg_name, 'LIBRARY_TYPE', config_suffix) }}"
+                                      "{{ pkg_var(pkg_name, 'IS_HOST_WINDOWS', config_suffix) }}"
                                       {{ pkg_name + '_DEPS_TARGET'}}
                                       {{ pkg_name }}_LIBRARIES_TARGETS  # out_libraries_targets
                                       "{{ config_suffix }}"
                                       "{{ pkg_name }}"    # package_name
-                                      "{{ '${' }}{{ pkg_name }}_NO_SONAME_MODE{{ config_suffix }}}")  # soname
+                                      "{{ pkg_var(pkg_name, 'NO_SONAME_MODE', config_suffix) }}")  # soname
 
         # FIXME: What is the result of this for multi-config? All configs adding themselves to path?
-        set(CMAKE_MODULE_PATH {{ '${' }}{{ pkg_name }}_BUILD_DIRS{{ config_suffix }}} {{ '${' }}CMAKE_MODULE_PATH})
+        set(CMAKE_MODULE_PATH {{ pkg_var(pkg_name, 'BUILD_DIRS', config_suffix) }} {{ '${' }}CMAKE_MODULE_PATH})
         {% if not components_names %}
 
         ########## GLOBAL TARGET PROPERTIES {{ configuration }} ########################################
             set_property(TARGET {{root_target_name}}
                          APPEND PROPERTY INTERFACE_LINK_LIBRARIES
-                         $<$<CONFIG:{{configuration}}>:{{ '${'+pkg_name+'_OBJECTS'+config_suffix+'}' }}>
-                         $<$<CONFIG:{{configuration}}>:${{'{'}}{{pkg_name}}_LIBRARIES_TARGETS}>
+                         $<$<CONFIG:{{configuration}}>:{{ pkg_var(pkg_name, 'OBJECTS', config_suffix) }}>
+                         $<$<CONFIG:{{configuration}}>:{{ pkg_var(pkg_name, 'LIBRARIES_TARGETS', '') }}>
                          )
 
-            if("{{ '${' }}{{ pkg_name }}_LIBS{{ config_suffix }}}" STREQUAL "")
+            if("{{ pkg_var(pkg_name, 'LIBS', config_suffix) }}" STREQUAL "")
                 # If the package is not declaring any "cpp_info.libs" the package deps, system libs,
                 # frameworks etc are not linked to the imported targets and we need to do it to the
                 # global target
                 set_property(TARGET {{root_target_name}}
                              APPEND PROPERTY INTERFACE_LINK_LIBRARIES
                              {{pkg_name}}_DEPS_TARGET)
             endif()
 
             set_property(TARGET {{root_target_name}}
                          APPEND PROPERTY INTERFACE_LINK_OPTIONS
-                         $<$<CONFIG:{{configuration}}>:${{'{'}}{{pkg_name}}_LINKER_FLAGS{{config_suffix}}}>)
+                         $<$<CONFIG:{{configuration}}>:{{ pkg_var(pkg_name, 'LINKER_FLAGS', config_suffix) }}>)
             set_property(TARGET {{root_target_name}}
                          APPEND PROPERTY INTERFACE_INCLUDE_DIRECTORIES
-                         $<$<CONFIG:{{configuration}}>:${{'{'}}{{pkg_name}}_INCLUDE_DIRS{{config_suffix}}}>)
+                         $<$<CONFIG:{{configuration}}>:{{ pkg_var(pkg_name, 'INCLUDE_DIRS', config_suffix) }}>)
             # Necessary to find LINK shared libraries in Linux
             set_property(TARGET {{root_target_name}}
                          APPEND PROPERTY INTERFACE_LINK_DIRECTORIES
-                         $<$<CONFIG:{{configuration}}>:${{'{'}}{{pkg_name}}_LIB_DIRS{{config_suffix}}}>)
+                         $<$<CONFIG:{{configuration}}>:{{ pkg_var(pkg_name, 'LIB_DIRS', config_suffix) }}>)
             set_property(TARGET {{root_target_name}}
                          APPEND PROPERTY INTERFACE_COMPILE_DEFINITIONS
-                         $<$<CONFIG:{{configuration}}>:${{'{'}}{{pkg_name}}_COMPILE_DEFINITIONS{{config_suffix}}}>)
+                         $<$<CONFIG:{{configuration}}>:{{ pkg_var(pkg_name, 'COMPILE_DEFINITIONS', config_suffix) }}>)
             set_property(TARGET {{root_target_name}}
                          APPEND PROPERTY INTERFACE_COMPILE_OPTIONS
-                         $<$<CONFIG:{{configuration}}>:${{'{'}}{{pkg_name}}_COMPILE_OPTIONS{{config_suffix}}}>)
+                         $<$<CONFIG:{{configuration}}>:{{ pkg_var(pkg_name, 'COMPILE_OPTIONS', config_suffix) }}>)
 
             {%- if set_interface_link_directories %}
 
             # This is only used for '#pragma comment(lib, "foo")' (automatic link)
             set_property(TARGET {{root_target_name}}
                          APPEND PROPERTY INTERFACE_LINK_DIRECTORIES
-                         $<$<CONFIG:{{configuration}}>:${{'{'}}{{pkg_name}}_LIB_DIRS{{config_suffix}}}>)
+                         $<$<CONFIG:{{configuration}}>:{{ pkg_var(pkg_name, 'LIB_DIRS', config_suffix) }}>)
             {%- endif %}
 
 
         {%- else %}
 
         ########## COMPONENTS TARGET PROPERTIES {{ configuration }} ########################################
 
             {%- for comp_variable_name, comp_target_name in components_names %}
 
 
             ########## COMPONENT {{ comp_target_name }} #############
 
                 set({{ pkg_name }}_{{ comp_variable_name }}_FRAMEWORKS_FOUND{{ config_suffix }} "")
-                conan_find_apple_frameworks({{ pkg_name }}_{{ comp_variable_name }}_FRAMEWORKS_FOUND{{ config_suffix }} "{{ '${'+pkg_name+'_'+comp_variable_name+'_FRAMEWORKS'+config_suffix+'}' }}" "{{ '${'+pkg_name+'_'+comp_variable_name+'_FRAMEWORK_DIRS'+config_suffix+'}' }}")
+                conan_find_apple_frameworks({{ pkg_name }}_{{ comp_variable_name }}_FRAMEWORKS_FOUND{{ config_suffix }} "{{ comp_var(pkg_name, comp_variable_name, 'FRAMEWORKS', config_suffix) }}" "{{ comp_var(pkg_name, comp_variable_name, 'FRAMEWORK_DIRS', config_suffix) }}")
 
                 set({{ pkg_name }}_{{ comp_variable_name }}_LIBRARIES_TARGETS "")
 
                 ######## Create an interface target to contain all the dependencies (frameworks, system and conan deps)
                 if(NOT TARGET {{ pkg_name + '_' + comp_variable_name + '_DEPS_TARGET'}})
                     add_library({{ pkg_name + '_' + comp_variable_name + '_DEPS_TARGET'}} INTERFACE IMPORTED)
                 endif()
 
                 set_property(TARGET {{ pkg_name + '_' + comp_variable_name + '_DEPS_TARGET'}}
                              APPEND PROPERTY INTERFACE_LINK_LIBRARIES
-                             $<$<CONFIG:{{configuration}}>:{{ '${'+pkg_name+'_'+comp_variable_name+'_FRAMEWORKS_FOUND'+config_suffix+'}' }}>
-                             $<$<CONFIG:{{configuration}}>:{{ '${'+pkg_name+'_'+comp_variable_name+'_SYSTEM_LIBS'+config_suffix+'}' }}>
-                             $<$<CONFIG:{{configuration}}>:{{ '${'+pkg_name+'_'+comp_variable_name+'_DEPENDENCIES'+config_suffix+'}' }}>
+                             $<$<CONFIG:{{configuration}}>:{{ comp_var(pkg_name, comp_variable_name, 'FRAMEWORKS_FOUND', config_suffix) }}>
+                             $<$<CONFIG:{{configuration}}>:{{ comp_var(pkg_name, comp_variable_name, 'SYSTEM_LIBS', config_suffix) }}>
+                             $<$<CONFIG:{{configuration}}>:{{ comp_var(pkg_name, comp_variable_name, 'DEPENDENCIES', config_suffix) }}>
                              )
 
                 ####### Find the libraries declared in cpp_info.component["xxx"].libs,
                 ####### create an IMPORTED target for each one and link the '{{pkg_name}}_{{comp_variable_name}}_DEPS_TARGET' to all of them
-                conan_package_library_targets("{{ '${'+pkg_name+'_'+comp_variable_name+'_LIBS'+config_suffix+'}' }}"
-                                      "{{ '${'+pkg_name+'_'+comp_variable_name+'_LIB_DIRS'+config_suffix+'}' }}"
-                                      "{{ '${'+pkg_name+'_'+comp_variable_name+'_BIN_DIRS'+config_suffix+'}' }}" # package_bindir
-                                      "{{ '${'+pkg_name+'_'+comp_variable_name+'_LIBRARY_TYPE'+config_suffix+'}' }}"
-                                      "{{ '${'+pkg_name+'_'+comp_variable_name+'_IS_HOST_WINDOWS'+config_suffix+'}' }}"
+                conan_package_library_targets("{{ comp_var(pkg_name, comp_variable_name, 'LIBS', config_suffix) }}"
+                                      "{{ comp_var(pkg_name, comp_variable_name, 'LIB_DIRS', config_suffix) }}"
+                                      "{{ comp_var(pkg_name, comp_variable_name, 'BIN_DIRS', config_suffix) }}" # package_bindir
+                                      "{{ comp_var(pkg_name, comp_variable_name, 'LIBRARY_TYPE', config_suffix) }}"
+                                      "{{ comp_var(pkg_name, comp_variable_name, 'IS_HOST_WINDOWS', config_suffix) }}"
                                       {{ pkg_name + '_' + comp_variable_name + '_DEPS_TARGET'}}
-                                      {{ pkg_name }}_{{ comp_variable_name }}_LIBRARIES_TARGETS
+                                      {{ pkg_name + '_' + comp_variable_name + '_LIBRARIES_TARGETS'}}
                                       "{{ config_suffix }}"
                                       "{{ pkg_name }}_{{ comp_variable_name }}"
-                                      "{{ '${'+pkg_name+'_'+comp_variable_name+'_NO_SONAME_MODE'+config_suffix+'}' }}")
+                                      "{{ comp_var(pkg_name, comp_variable_name, 'NO_SONAME_MODE', config_suffix) }}")
 
 
                 ########## TARGET PROPERTIES #####################################
                 set_property(TARGET {{comp_target_name}}
                              APPEND PROPERTY INTERFACE_LINK_LIBRARIES
-                             $<$<CONFIG:{{configuration}}>:{{ '${'+pkg_name+'_'+comp_variable_name+'_OBJECTS'+config_suffix+'}' }}>
-                             $<$<CONFIG:{{configuration}}>:${{'{'}}{{pkg_name}}_{{comp_variable_name}}_LIBRARIES_TARGETS}>
+                             $<$<CONFIG:{{configuration}}>:{{ comp_var(pkg_name, comp_variable_name, 'OBJECTS', config_suffix) }}>
+                             $<$<CONFIG:{{configuration}}>:{{ comp_var(pkg_name, comp_variable_name, 'LIBRARIES_TARGETS', '') }}>
                              )
 
-                if("{{ '${' }}{{ pkg_name }}_{{comp_variable_name}}_LIBS{{ config_suffix }}}" STREQUAL "")
+                if("{{ comp_var(pkg_name, comp_variable_name, 'LIBS', config_suffix) }}" STREQUAL "")
                     # If the component is not declaring any "cpp_info.components['foo'].libs" the system, frameworks etc are not
                     # linked to the imported targets and we need to do it to the global target
                     set_property(TARGET {{comp_target_name}}
                                  APPEND PROPERTY INTERFACE_LINK_LIBRARIES
                                  {{pkg_name}}_{{comp_variable_name}}_DEPS_TARGET)
                 endif()
 
                 set_property(TARGET {{ comp_target_name }} APPEND PROPERTY INTERFACE_LINK_OPTIONS
-                             $<$<CONFIG:{{ configuration }}>:{{tvalue(pkg_name, comp_variable_name, 'LINKER_FLAGS', config_suffix)}}>)
+                             $<$<CONFIG:{{ configuration }}>:{{ comp_var(pkg_name, comp_variable_name, 'LINKER_FLAGS', config_suffix) }}>)
                 set_property(TARGET {{ comp_target_name }} APPEND PROPERTY INTERFACE_INCLUDE_DIRECTORIES
-                             $<$<CONFIG:{{ configuration }}>:{{tvalue(pkg_name, comp_variable_name, 'INCLUDE_DIRS', config_suffix)}}>)
+                             $<$<CONFIG:{{ configuration }}>:{{ comp_var(pkg_name, comp_variable_name, 'INCLUDE_DIRS', config_suffix) }}>)
                 set_property(TARGET {{comp_target_name }} APPEND PROPERTY INTERFACE_LINK_DIRECTORIES
-                             $<$<CONFIG:{{ configuration }}>:{{tvalue(pkg_name, comp_variable_name, 'LIB_DIRS', config_suffix)}}>)
+                             $<$<CONFIG:{{ configuration }}>:{{ comp_var(pkg_name, comp_variable_name, 'LIB_DIRS', config_suffix) }}>)
                 set_property(TARGET {{ comp_target_name }} APPEND PROPERTY INTERFACE_COMPILE_DEFINITIONS
-                             $<$<CONFIG:{{ configuration }}>:{{tvalue(pkg_name, comp_variable_name, 'COMPILE_DEFINITIONS', config_suffix)}}>)
+                             $<$<CONFIG:{{ configuration }}>:{{ comp_var(pkg_name, comp_variable_name, 'COMPILE_DEFINITIONS', config_suffix) }}>)
                 set_property(TARGET {{ comp_target_name }} APPEND PROPERTY INTERFACE_COMPILE_OPTIONS
-                             $<$<CONFIG:{{ configuration }}>:{{tvalue(pkg_name, comp_variable_name, 'COMPILE_OPTIONS', config_suffix)}}>)
+                             $<$<CONFIG:{{ configuration }}>:{{ comp_var(pkg_name, comp_variable_name, 'COMPILE_OPTIONS', config_suffix) }}>)
 
                 {%- if set_interface_link_directories %}
                 # This is only used for '#pragma comment(lib, "foo")' (automatic link)
                 set_property(TARGET {{ comp_target_name }} APPEND PROPERTY INTERFACE_LINK_DIRECTORIES
-                             $<$<CONFIG:{{ configuration }}>:{{tvalue(pkg_name, comp_variable_name, 'LIB_DIRS', config_suffix)}}>)
+                             $<$<CONFIG:{{ configuration }}>:{{ comp_var(pkg_name, comp_variable_name, 'LIB_DIRS', config_suffix) }}>)
 
                 {%- endif %}
             {%endfor %}
 
 
             ########## AGGREGATED GLOBAL TARGET WITH THE COMPONENTS #####################
             {%- for comp_variable_name, comp_target_name in components_names %}
@@ -231,15 +233,15 @@
         """
           - [{foo}::{bar}, ] of the required
         """
         ret = []
 
         # Get a list of dependencies target names
         # Declared cppinfo.requires or .components[].requires
-        transitive_reqs = get_transitive_requires(self.cmakedeps._conanfile, self.conanfile)
+        transitive_reqs = self.cmakedeps.get_transitive_requires(self.conanfile)
         if self.conanfile.cpp_info.required_components:
             for dep_name, component_name in self.conanfile.cpp_info.required_components:
                 try:
                     # if not dep_name, it is internal, from current self.conanfile
                     req = transitive_reqs[dep_name] if dep_name is not None else self.conanfile
                 except KeyError:
                     # if it raises it means the required component is not in the direct_host
```

### Comparing `conan-2.2.3/conan/tools/cmake/cmakedeps/templates/target_data.py` & `conan-2.3.0/conan/tools/cmake/cmakedeps/templates/target_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import textwrap
 
 from conan.tools.cmake.cmakedeps import FIND_MODE_NONE, FIND_MODE_CONFIG, FIND_MODE_MODULE, \
     FIND_MODE_BOTH
 from conan.tools.cmake.cmakedeps.templates import CMakeDepsFileTemplate
 from conan.errors import ConanException
-from conans.model.dependencies import get_transitive_requires
 
 
 """
 
 foo-release-x86_64-data.cmake
 
 """
@@ -80,14 +79,20 @@
         # to account for all WindowsStore, WindowsCE and Windows OS in settings
         return "Windows" in self.conanfile.settings.get_safe("os", "")
 
     @property
     def template(self):
         # This will be at: XXX-release-data.cmake
         ret = textwrap.dedent("""\
+              {%- macro comp_var(pkg_name, comp_name, var, config_suffix) -%}
+                 {{'${'+pkg_name+'_'+comp_name+'_'+var+config_suffix+'}'}}
+              {%- endmacro -%}
+              {%- macro pkg_var(pkg_name, var, config_suffix) -%}
+                 {{'${'+pkg_name+'_'+var+config_suffix+'}'}}
+              {%- endmacro -%}
               ########### AGGREGATED COMPONENTS AND DEPENDENCIES FOR THE MULTI CONFIG #####################
               #############################################################################################
 
               {% if components_names %}
               list(APPEND {{ pkg_name }}_COMPONENT_NAMES {{ components_names }})
               list(REMOVE_DUPLICATES {{ pkg_name }}_COMPONENT_NAMES)
               {% else %}
@@ -128,20 +133,20 @@
               set({{ pkg_name }}_FRAMEWORKS{{ config_suffix }} {{ global_cpp.frameworks }})
               set({{ pkg_name }}_BUILD_DIRS{{ config_suffix }} {{ global_cpp.build_paths }})
               set({{ pkg_name }}_NO_SONAME_MODE{{ config_suffix }} {{ global_cpp.no_soname }})
 
 
               # COMPOUND VARIABLES
               set({{ pkg_name }}_COMPILE_OPTIONS{{ config_suffix }}
-                  "$<$<COMPILE_LANGUAGE:CXX>{{ ':${' }}{{ pkg_name }}_COMPILE_OPTIONS_CXX{{ config_suffix }}}>"
-                  "$<$<COMPILE_LANGUAGE:C>{{ ':${' }}{{ pkg_name }}_COMPILE_OPTIONS_C{{ config_suffix }}}>")
+                  "$<$<COMPILE_LANGUAGE:CXX>:{{ pkg_var(pkg_name, 'COMPILE_OPTIONS_CXX', config_suffix) }}>"
+                  "$<$<COMPILE_LANGUAGE:C>:{{ pkg_var(pkg_name, 'COMPILE_OPTIONS_C', config_suffix) }}>")
               set({{ pkg_name }}_LINKER_FLAGS{{ config_suffix }}
-                  "$<$<STREQUAL{{ ':$' }}<TARGET_PROPERTY:TYPE>,SHARED_LIBRARY>{{ ':${' }}{{ pkg_name }}_SHARED_LINK_FLAGS{{ config_suffix }}}>"
-                  "$<$<STREQUAL{{ ':$' }}<TARGET_PROPERTY:TYPE>,MODULE_LIBRARY>{{ ':${' }}{{ pkg_name }}_SHARED_LINK_FLAGS{{ config_suffix }}}>"
-                  "$<$<STREQUAL{{ ':$' }}<TARGET_PROPERTY:TYPE>,EXECUTABLE>{{ ':${' }}{{ pkg_name }}_EXE_LINK_FLAGS{{ config_suffix }}}>")
+                  "$<$<STREQUAL{{ ':$' }}<TARGET_PROPERTY:TYPE>,SHARED_LIBRARY>:{{ pkg_var(pkg_name, 'SHARED_LINK_FLAGS', config_suffix) }}>"
+                  "$<$<STREQUAL{{ ':$' }}<TARGET_PROPERTY:TYPE>,MODULE_LIBRARY>:{{ pkg_var(pkg_name, 'SHARED_LINK_FLAGS', config_suffix) }}>"
+                  "$<$<STREQUAL{{ ':$' }}<TARGET_PROPERTY:TYPE>,EXECUTABLE>:{{ pkg_var(pkg_name, 'EXE_LINK_FLAGS', config_suffix) }}>")
 
 
               set({{ pkg_name }}_COMPONENTS{{ config_suffix }} {{ components_names }})
               {%- for comp_variable_name, comp_target_name, cpp in components_cpp %}
 
               ########### COMPONENT {{ comp_target_name }} VARIABLES ############################################
 
@@ -163,21 +168,21 @@
               set({{ pkg_name }}_{{ comp_variable_name }}_DEPENDENCIES{{ config_suffix }} {{ cpp.public_deps }})
               set({{ pkg_name }}_{{ comp_variable_name }}_SHARED_LINK_FLAGS{{ config_suffix }} {{ cpp.sharedlinkflags_list }})
               set({{ pkg_name }}_{{ comp_variable_name }}_EXE_LINK_FLAGS{{ config_suffix }} {{ cpp.exelinkflags_list }})
               set({{ pkg_name }}_{{ comp_variable_name }}_NO_SONAME_MODE{{ config_suffix }} {{ cpp.no_soname }})
 
               # COMPOUND VARIABLES
               set({{ pkg_name }}_{{ comp_variable_name }}_LINKER_FLAGS{{ config_suffix }}
-                      $<$<STREQUAL:$<TARGET_PROPERTY:TYPE>,SHARED_LIBRARY>{{ ':${' }}{{ pkg_name }}_{{ comp_variable_name }}_SHARED_LINK_FLAGS{{ config_suffix }}}>
-                      $<$<STREQUAL:$<TARGET_PROPERTY:TYPE>,MODULE_LIBRARY>{{ ':${' }}{{ pkg_name }}_{{ comp_variable_name }}_SHARED_LINK_FLAGS{{ config_suffix }}}>
-                      $<$<STREQUAL:$<TARGET_PROPERTY:TYPE>,EXECUTABLE>{{ ':${' }}{{ pkg_name }}_{{ comp_variable_name }}_EXE_LINK_FLAGS{{ config_suffix }}}>
+                      $<$<STREQUAL:$<TARGET_PROPERTY:TYPE>,SHARED_LIBRARY>:{{ comp_var(pkg_name, comp_variable_name, 'SHARED_LINK_FLAGS', config_suffix) }}>
+                      $<$<STREQUAL:$<TARGET_PROPERTY:TYPE>,MODULE_LIBRARY>:{{ comp_var(pkg_name, comp_variable_name, 'SHARED_LINK_FLAGS', config_suffix) }}>
+                      $<$<STREQUAL:$<TARGET_PROPERTY:TYPE>,EXECUTABLE>:{{ comp_var(pkg_name, comp_variable_name, 'EXE_LINK_FLAGS', config_suffix) }}>
               )
               set({{ pkg_name }}_{{ comp_variable_name }}_COMPILE_OPTIONS{{ config_suffix }}
-                  "$<$<COMPILE_LANGUAGE:CXX>{{ ':${' }}{{ pkg_name }}_{{ comp_variable_name }}_COMPILE_OPTIONS_CXX{{ config_suffix }}}>"
-                  "$<$<COMPILE_LANGUAGE:C>{{ ':${' }}{{ pkg_name }}_{{ comp_variable_name }}_COMPILE_OPTIONS_C{{ config_suffix }}}>")
+                  "$<$<COMPILE_LANGUAGE:CXX>:{{ comp_var(pkg_name, comp_variable_name, 'COMPILE_OPTIONS_CXX', config_suffix) }}>"
+                  "$<$<COMPILE_LANGUAGE:C>:{{ comp_var(pkg_name, comp_variable_name, 'COMPILE_OPTIONS_C', config_suffix) }}>")
 
               {%- endfor %}
           """)
         return ret
 
     def _get_global_cpp_cmake(self):
         global_cppinfo = self.conanfile.cpp_info.aggregated_components()
@@ -192,15 +197,15 @@
             else self.conanfile.package_folder
 
     def _get_required_components_cpp(self):
         """Returns a list of (component_name, DepsCppCMake)"""
         ret = []
         sorted_comps = self.conanfile.cpp_info.get_sorted_components()
         pfolder_var_name = "{}_PACKAGE_FOLDER{}".format(self.pkg_name, self.config_suffix)
-        transitive_requires = get_transitive_requires(self.cmakedeps._conanfile, self.conanfile)
+        transitive_requires = self.cmakedeps.get_transitive_requires(self.conanfile)
         for comp_name, comp in sorted_comps.items():
             deps_cpp_cmake = _TargetDataContext(comp, pfolder_var_name, self._root_folder,
                                                 self.require, self.cmake_package_type,
                                                 self.is_host_windows, self.conanfile, self.cmakedeps,
                                                 comp_name)
 
             public_comp_deps = []
@@ -226,27 +231,27 @@
         ret.reverse()
         return ret
 
     def _get_dependency_filenames(self):
         if self.require.build:
             return []
 
-        transitive_reqs = get_transitive_requires(self.cmakedeps._conanfile, self.conanfile)
+        transitive_reqs = self.cmakedeps.get_transitive_requires(self.conanfile)
         # Previously it was filtering here components, but not clear why the file dependency
         # should be skipped if components are not being required, why would it declare a
         # dependency to it?
         ret = [self.cmakedeps.get_cmake_package_name(r, self.generating_module)
                for r in transitive_reqs.values()]
         return ret
 
     def _get_dependencies_find_modes(self):
         ret = {}
         if self.require.build:
             return ret
-        deps = get_transitive_requires(self.cmakedeps._conanfile, self.conanfile)
+        deps = self.cmakedeps.get_transitive_requires(self.conanfile)
         for dep in deps.values():
             dep_file_name = self.cmakedeps.get_cmake_package_name(dep, self.generating_module)
             find_mode = self.cmakedeps.get_find_mode(dep)
             default_value = "NO_MODULE" if not self.generating_module else "MODULE"
             values = {
                 FIND_MODE_NONE: "",
                 FIND_MODE_CONFIG: "NO_MODULE",
```

### Comparing `conan-2.2.3/conan/tools/cmake/cmakedeps/templates/targets.py` & `conan-2.3.0/conan/tools/cmake/cmakedeps/templates/targets.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/cmake/layout.py` & `conan-2.3.0/conan/tools/cmake/layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/cmake/presets.py` & `conan-2.3.0/conan/tools/cmake/presets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import os
 import platform
+import textwrap
 
-from conan.api.output import ConanOutput
+from conan.api.output import ConanOutput, Color
 from conan.tools.cmake.layout import get_build_folder_custom_vars
 from conan.tools.cmake.toolchain.blocks import GenericSystemBlock
 from conan.tools.cmake.utils import is_multi_configuration
 from conan.tools.build import build_jobs
 from conan.tools.microsoft import is_msvc
 from conans.client.graph.graph import RECIPE_CONSUMER
 from conan.errors import ConanException
@@ -24,14 +25,19 @@
 
 class _CMakePresets:
     """ Conan generated main CMakePresets.json inside the generators_folder
     """
     @staticmethod
     def generate(conanfile, toolchain_file, generator, cache_variables, preset_prefix, buildenv, runenv,
                  cmake_executable):
+        toolchain_file = os.path.abspath(os.path.join(conanfile.generators_folder, toolchain_file))
+        try:  # Make it relative to the build dir if possible
+            toolchain_file = os.path.relpath(toolchain_file, conanfile.build_folder)
+        except ValueError:
+            pass
         cache_variables = cache_variables or {}
         if platform.system() == "Windows" and generator == "MinGW Makefiles":
             if "CMAKE_SH" not in cache_variables:
                 cache_variables["CMAKE_SH"] = "CMAKE_SH-NOTFOUND"
 
         cmake_make_program = conanfile.conf.get("tools.gnu:make_program",
                                                 default=cache_variables.get("CMAKE_MAKE_PROGRAM"))
@@ -70,15 +76,15 @@
             data["configurePresets"] = [configure_preset]
         else:
             data = _CMakePresets._contents(conanfile, toolchain_file, cache_variables, generator,
                                            preset_prefix, buildenv, runenv, cmake_executable)
 
         preset_content = json.dumps(data, indent=4)
         save(preset_path, preset_content)
-        ConanOutput(str(conanfile)).info("CMakeToolchain generated: CMakePresets.json")
+        ConanOutput(str(conanfile)).info(f"CMakeToolchain generated: {preset_path}")
         return preset_path, data
 
     @staticmethod
     def _insert_preset(data, preset_type, preset):
         presets = data.setdefault(preset_type, [])
         preset_name = preset["name"]
         positions = [index for index, p in enumerate(presets) if p["name"] == preset_name]
@@ -168,21 +174,19 @@
 
         try:
             is_consumer = conanfile._conan_node.recipe == RECIPE_CONSUMER and \
                           conanfile.tested_reference_str is None
         except:
             is_consumer = False
         if is_consumer:
-            conanfile.output.info(
-                f"Preset '{name}' added to CMakePresets.json. Invoke it manually using "
-                f"'cmake --preset {name}' if using CMake>=3.23")
-            conanfile.output.info(f"If your CMake version is not compatible with "
-                                  f"CMakePresets (<3.23) call cmake like: 'cmake <path> "
-                                  f"-G {_format_val(generator)} {add_toolchain_cache}"
-                                  f"{cache_variables_info}'")
+            msg = textwrap.dedent(f"""\
+                CMakeToolchain: Preset '{name}' added to CMakePresets.json.
+                    (cmake>=3.23) cmake --preset {name}
+                    (cmake<3.23) cmake <path> -G {_format_val(generator)} {add_toolchain_cache} {cache_variables_info}""")
+            conanfile.output.info(msg, fg=Color.CYAN)
         return ret
 
     @staticmethod
     def _common_preset_fields(conanfile, multiconfig, preset_prefix):
         build_type = conanfile.settings.get_safe("build_type")
         configure_preset_name = _CMakePresets._configure_preset_name(conanfile, multiconfig)
         build_preset_name = _CMakePresets._build_and_test_preset_name(conanfile)
@@ -279,22 +283,23 @@
             data = json.loads(load(user_presets_path))
             if "conan" not in data.get("vendor", {}):
                 # The file is not ours, we cannot overwrite it
                 return
 
         if inherited_user:
             _IncludingPresets._clean_user_inherits(data, preset_data)
-        data = _IncludingPresets._append_user_preset_path(data, preset_path)
+
+        try:  # Make it relative to the CMakeUserPresets.json if possible
+            preset_path = os.path.relpath(preset_path, output_dir)
+        except ValueError:
+            pass
+        data = _IncludingPresets._append_user_preset_path(data, preset_path, output_dir)
 
         data = json.dumps(data, indent=4)
-        try:
-            presets_path = os.path.relpath(user_presets_path, conanfile.generators_folder)
-        except ValueError:  # in Windows this fails if in another drive
-            presets_path = user_presets_path
-        ConanOutput(str(conanfile)).info(f"CMakeToolchain generated: {presets_path}")
+        ConanOutput(str(conanfile)).info(f"CMakeToolchain generated: {user_presets_path}")
         save(user_presets_path, data)
 
     @staticmethod
     def _collect_user_inherits(output_dir, preset_prefix):
         # Collect all the existing targets in the user files, to create empty conan- presets
         # so things doesn't break for multi-platform, when inherits don't exist
         collected_targets = {}
@@ -322,23 +327,24 @@
         for preset_type in "configurePresets", "buildPresets", "testPresets":
             presets = preset_data.get(preset_type, [])
             presets_names = [p["name"] for p in presets]
             other = data.get(preset_type, [])
             other[:] = [p for p in other if p["name"] not in presets_names]
 
     @staticmethod
-    def _append_user_preset_path(data, preset_path):
+    def _append_user_preset_path(data, preset_path, output_dir):
         """ - Appends a 'include' to preset_path if the schema supports it.
             - Otherwise it merges to "data" all the configurePresets, buildPresets etc from the
               read preset_path.
         """
         if "include" not in data:
             data["include"] = []
         # Clear the folders that have been deleted
-        data["include"] = [i for i in data.get("include", []) if os.path.exists(i)]
+        data["include"] = [i for i in data.get("include", [])
+                           if os.path.exists(os.path.join(output_dir, i))]
         if preset_path not in data["include"]:
             data["include"].append(preset_path)
         return data
 
 
 def load_cmake_presets(folder):
     try:
```

### Comparing `conan-2.2.3/conan/tools/cmake/toolchain/blocks.py` & `conan-2.3.0/conan/tools/cmake/toolchain/blocks.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/cmake/toolchain/toolchain.py` & `conan-2.3.0/conan/tools/cmake/toolchain/toolchain.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,24 +223,24 @@
     def generate(self):
         """
           This method will save the generated files to the conanfile.generators_folder
         """
         check_duplicated_generator(self, self._conanfile)
         toolchain_file = self._conanfile.conf.get("tools.cmake.cmaketoolchain:toolchain_file")
         if toolchain_file is None:  # The main toolchain file generated only if user dont define
-            save(os.path.join(self._conanfile.generators_folder, self.filename), self.content)
-            ConanOutput(str(self._conanfile)).info(f"CMakeToolchain generated: {self.filename}")
+            toolchain_file = self.filename
+            save(os.path.join(self._conanfile.generators_folder, toolchain_file), self.content)
+            ConanOutput(str(self._conanfile)).info(f"CMakeToolchain generated: {toolchain_file}")
         # If we're using Intel oneAPI, we need to generate the environment file and run it
         if self._conanfile.settings.get_safe("compiler") == "intel-cc":
             IntelCC(self._conanfile).generate()
         # Generators like Ninja or NMake requires an active vcvars
         elif self.generator is not None and "Visual" not in self.generator:
             VCVars(self._conanfile).generate()
-        toolchain = os.path.abspath(os.path.join(self._conanfile.generators_folder,
-                                                 toolchain_file or self.filename))
+
         cache_variables = {}
         for name, value in self.cache_variables.items():
             if isinstance(value, bool):
                 cache_variables[name] = "ON" if value else "OFF"
             elif isinstance(value, _PackageOption):
                 if str(value).lower() in ["true", "false", "none"]:
                     cache_variables[name] = "ON" if bool(value) else "OFF"
@@ -262,15 +262,15 @@
             buildenv = {name: value for name, value in
                         build_env.items(variable_reference="$penv{{{name}}}")}
             runenv = {name: value for name, value in
                       run_env.items(variable_reference="$penv{{{name}}}")}
 
             cmake_executable = self._conanfile.conf.get("tools.cmake:cmake_program", None) or self._find_cmake_exe()
 
-        write_cmake_presets(self._conanfile, toolchain, self.generator, cache_variables,
+        write_cmake_presets(self._conanfile, toolchain_file, self.generator, cache_variables,
                             self.user_presets_path, self.presets_prefix, buildenv, runenv,
                             cmake_executable)
 
     def _get_generator(self, recipe_generator):
         # Returns the name of the generator to be used by CMake
         conanfile = self._conanfile
```

### Comparing `conan-2.2.3/conan/tools/env/environment.py` & `conan-2.3.0/conan/tools/env/environment.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/env/virtualbuildenv.py` & `conan-2.3.0/conan/tools/env/virtualbuildenv.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/env/virtualrunenv.py` & `conan-2.3.0/conan/tools/env/virtualrunenv.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/files/__init__.py` & `conan-2.3.0/conan/tools/files/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/files/conandata.py` & `conan-2.3.0/conan/tools/files/conandata.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/files/copy_pattern.py` & `conan-2.3.0/conan/tools/files/copy_pattern.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+import filecmp
 import fnmatch
 import os
 import shutil
 
 from conans.errors import ConanException
 from conans.util.files import mkdir
 
 
 def copy(conanfile, pattern, src, dst, keep_path=True, excludes=None,
-         ignore_case=True):
+         ignore_case=True, overwrite_equal=False):
     """
     Copy the files matching the pattern (fnmatch) at the src folder to a dst folder.
 
     :param conanfile: The current recipe object. Always use ``self``.
     :param pattern: (Required) An fnmatch file pattern of the files that should be copied.
            It must not start with ``..`` relative path or an exception will be raised.
     :param src: (Required) Source folder in which those files will be searched. This folder
@@ -21,14 +22,17 @@
     :param keep_path: (Optional, defaulted to ``True``) Means if you want to keep the relative
            path when you copy the files from the src folder to the dst one.
     :param excludes: (Optional, defaulted to ``None``) A tuple/list of fnmatch patterns or even a
            single one to be excluded from the copy.
     :param ignore_case: (Optional, defaulted to ``True``) If enabled, it will do a
            case-insensitive pattern matching. will do a case-insensitive pattern matching when
            ``True``
+    :param overwrite_equal: (Optional, default ``False``). If the file to be copied already exists
+           in the destination folder, only really copy it if it seems different (different size,
+           different modification time)
     :return: list of copied files
     """
     if src == dst:
         raise ConanException("copy() 'src' and 'dst' arguments must have different values")
     if pattern.startswith(".."):
         raise ConanException("copy() it is not possible to use relative patterns starting with '..'")
     if src is None:
@@ -36,15 +40,15 @@
 
     # This is necessary to add the trailing / so it is not reported as symlink
     src = os.path.join(src, "")
     excluded_folder = dst
     files_to_copy, files_symlinked_to_folders = _filter_files(src, pattern, excludes, ignore_case,
                                                               excluded_folder)
 
-    copied_files = _copy_files(files_to_copy, src, dst, keep_path)
+    copied_files = _copy_files(files_to_copy, src, dst, keep_path, overwrite_equal)
     copied_files.extend(_copy_files_symlinked_to_folders(files_symlinked_to_folders, src, dst))
     if conanfile:  # Some usages still pass None
         copied = '\n    '.join(files_to_copy)
         conanfile.output.debug(f"copy(pattern={pattern}) copied {len(copied_files)} files\n"
                                f"  from {src}\n"
                                f"  to {dst}\n"
                                f"  Files:\n    {copied}")
@@ -104,36 +108,39 @@
             files_to_copy = [f for f in files_to_copy if not fnmatch.fnmatch(f.lower(), exclude)]
         else:
             files_to_copy = [f for f in files_to_copy if not fnmatch.fnmatchcase(f, exclude)]
 
     return files_to_copy, files_symlinked_to_folders
 
 
-def _copy_files(files, src, dst, keep_path):
+def _copy_files(files, src, dst, keep_path, overwrite_equal):
     """ executes a multiple file copy from [(src_file, dst_file), (..)]
     managing symlinks if necessary
     """
     copied_files = []
     for filename in files:
         abs_src_name = os.path.join(src, filename)
         filename = filename if keep_path else os.path.basename(filename)
         abs_dst_name = os.path.normpath(os.path.join(dst, filename))
         parent_folder = os.path.dirname(abs_dst_name)
         if parent_folder:  # There are cases where this folder will be empty for relative paths
             os.makedirs(parent_folder, exist_ok=True)
 
         if os.path.islink(abs_src_name):
-            linkto = os.readlink(abs_src_name)  # @UndefinedVariable
+            linkto = os.readlink(abs_src_name)
             try:
                 os.remove(abs_dst_name)
             except OSError:
                 pass
-            os.symlink(linkto, abs_dst_name)  # @UndefinedVariable
+            os.symlink(linkto, abs_dst_name)
         else:
-            shutil.copy2(abs_src_name, abs_dst_name)
+            # Avoid the copy if the file exists and has the exact same signature (size + mod time)
+            if overwrite_equal or not os.path.exists(abs_dst_name) \
+                    or not filecmp.cmp(abs_src_name, abs_dst_name):
+                shutil.copy2(abs_src_name, abs_dst_name)
         copied_files.append(abs_dst_name)
     return copied_files
 
 
 def _copy_files_symlinked_to_folders(files_symlinked_to_folders, src, dst):
     """Copy the files that are symlinks to folders from src to dst.
        The files are already filtered with the specified pattern"""
```

### Comparing `conan-2.2.3/conan/tools/files/files.py` & `conan-2.3.0/conan/tools/files/files.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/files/packager.py` & `conan-2.3.0/conan/tools/files/packager.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/files/patches.py` & `conan-2.3.0/conan/tools/files/patches.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/files/symlinks/symlinks.py` & `conan-2.3.0/conan/tools/files/symlinks/symlinks.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/gnu/autotools.py` & `conan-2.3.0/conan/tools/gnu/autotools.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 
         self._configure_args = "{} {}".format(self._configure_args, cmd_args_to_string(configure_args))
 
         configure_cmd = "{}/configure".format(script_folder)
         subsystem = deduce_subsystem(self._conanfile, scope="build")
         configure_cmd = subsystem_path(subsystem, configure_cmd)
         cmd = '"{}" {}'.format(configure_cmd, self._configure_args)
-        self._conanfile.output.info("Calling:\n > %s" % cmd)
         self._conanfile.run(cmd)
 
     def make(self, target=None, args=None):
         """
         Call the make program.
 
         :param target: (Optional, Defaulted to ``None``): Choose which target to build. This allows
```

### Comparing `conan-2.2.3/conan/tools/gnu/autotoolsdeps.py` & `conan-2.3.0/conan/tools/gnu/autotoolsdeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/gnu/autotoolstoolchain.py` & `conan-2.3.0/conan/tools/gnu/autotoolstoolchain.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
+from conan.errors import ConanException
 from conan.internal import check_duplicated_generator
 from conan.internal.internal_tools import raise_on_universal_arch
-from conan.tools.apple.apple import apple_min_version_flag, is_apple_os, to_apple_arch, apple_sdk_path
-from conan.tools.apple.apple import get_apple_sdk_fullname
+from conan.tools.apple.apple import is_apple_os, resolve_apple_flags
 from conan.tools.build import cmd_args_to_string, save_toolchain_args
 from conan.tools.build.cross_building import cross_building
-from conan.tools.build.flags import architecture_flag, build_type_flags, cppstd_flag, build_type_link_flags, libcxx_flags
+from conan.tools.build.flags import architecture_flag, build_type_flags, cppstd_flag, \
+    build_type_link_flags, \
+    libcxx_flags
 from conan.tools.env import Environment
 from conan.tools.gnu.get_gnu_triplet import _get_gnu_triplet
 from conan.tools.microsoft import VCVars, msvc_runtime_flag, unix_path, check_min_vs, is_msvc
-from conan.errors import ConanException
 from conans.model.pkg_type import PackageType
 
 
 class AutotoolsToolchain:
+
     def __init__(self, conanfile, namespace=None, prefix="/"):
         """
-
         :param conanfile: The current recipe object. Always use ``self``.
         :param namespace: This argument avoids collisions when you have multiple toolchain calls in
                the same recipe. By setting this argument, the *conanbuild.conf* file used to pass
                information to the build helper will be named as *<namespace>_conanbuild.conf*. The default
                value is ``None`` meaning that the name of the generated file is *conanbuild.conf*. This
                namespace must be also set with the same value in the constructor of the Autotools build
                helper so that it reads the information from the proper file.
@@ -52,58 +53,51 @@
         self.libcxx, self.gcc_cxx11_abi = libcxx_flags(self._conanfile)
         self.fpic = self._conanfile.options.get_safe("fPIC")
         self.msvc_runtime_flag = self._get_msvc_runtime_flag()
         self.msvc_extra_flags = self._msvc_extra_flags()
 
         # Cross build triplets
         self._host = self._conanfile.conf.get("tools.gnu:host_triplet")
-        self._build = None
+        self._build = self._conanfile.conf.get("tools.gnu:build_triplet")
         self._target = None
 
-        self.apple_arch_flag = self.apple_isysroot_flag = None
-
-        os_sdk = get_apple_sdk_fullname(conanfile)
-        os_version = conanfile.settings.get_safe("os.version")
-        subsystem = conanfile.settings.get_safe("os.subsystem")
-        self.apple_min_version_flag = apple_min_version_flag(os_version, os_sdk, subsystem)
-
-        self.sysroot_flag = None
-
-        if cross_building(self._conanfile):
+        is_cross_building = cross_building(self._conanfile)
+        if is_cross_building:
             os_host = conanfile.settings.get_safe("os")
             arch_host = conanfile.settings.get_safe("arch")
             os_build = conanfile.settings_build.get_safe('os')
             arch_build = conanfile.settings_build.get_safe('arch')
 
             compiler = self._conanfile.settings.get_safe("compiler")
             if not self._host:
-                self._host = _get_gnu_triplet(os_host, arch_host, compiler=compiler)
+                self._host = _get_gnu_triplet(os_host, arch_host, compiler=compiler)["triplet"]
             # Build triplet
-            self._build = _get_gnu_triplet(os_build, arch_build, compiler=compiler)
-            # Apple Stuff
-            if os_build == "Macos" and is_apple_os(conanfile):
-                # SDK path is mandatory for cross-building
-                sdk_path = apple_sdk_path(self._conanfile)
-                if not sdk_path:
-                    raise ConanException("You must provide a valid SDK path for cross-compilation.")
-                apple_arch = to_apple_arch(self._conanfile)
-                # https://man.archlinux.org/man/clang.1.en#Target_Selection_Options
-                self.apple_arch_flag = "-arch {}".format(apple_arch) if apple_arch else None
-                # -isysroot makes all includes for your library relative to the build directory
-                self.apple_isysroot_flag = "-isysroot {}".format(sdk_path) if sdk_path else None
+            if not self._build:
+                self._build = _get_gnu_triplet(os_build, arch_build, compiler=compiler)["triplet"]
 
         sysroot = self._conanfile.conf.get("tools.build:sysroot")
         sysroot = sysroot.replace("\\", "/") if sysroot is not None else None
         self.sysroot_flag = "--sysroot {}".format(sysroot) if sysroot else None
 
         self.configure_args = self._default_configure_shared_flags() + \
                               self._default_configure_install_flags() + \
                               self._get_triplets()
         self.autoreconf_args = self._default_autoreconf_flags()
         self.make_args = []
+        # Apple stuff
+        is_cross_building_osx = (is_cross_building
+                                 and conanfile.settings_build.get_safe('os') == "Macos"
+                                 and is_apple_os(conanfile))
+        min_flag, arch_flag, isysroot_flag = resolve_apple_flags(conanfile,
+                                                                 is_cross_building=is_cross_building_osx)
+        # https://man.archlinux.org/man/clang.1.en#Target_Selection_Options
+        self.apple_arch_flag = arch_flag
+        # -isysroot makes all includes for your library relative to the build directory
+        self.apple_isysroot_flag = isysroot_flag
+        self.apple_min_version_flag = min_flag
 
     def _get_msvc_runtime_flag(self):
         flag = msvc_runtime_flag(self._conanfile)
         if flag:
             flag = "-{}".format(flag)
         return flag
 
@@ -162,15 +156,15 @@
         return self._filter_list_empty_fields(ret)
 
     def environment(self):
         env = Environment()
         compilers_by_conf = self._conanfile.conf.get("tools.build:compiler_executables", default={},
                                                      check_type=dict)
         if compilers_by_conf:
-            compilers_mapping = {"c": "CC", "cpp": "CXX", "cuda": "NVCC", "fortran": "FC"}
+            compilers_mapping = {"c": "CC", "cpp": "CXX", "cuda": "NVCC", "fortran": "FC", "rc": "RC"}
             for comp, env_var in compilers_mapping.items():
                 if comp in compilers_by_conf:
                     compiler = compilers_by_conf[comp]
                     # https://github.com/conan-io/conan/issues/13780
                     compiler = unix_path(self._conanfile, compiler)
                     env.define(env_var, compiler)
         env.append("CPPFLAGS", ["-D{}".format(d) for d in self.defines])
```

### Comparing `conan-2.2.3/conan/tools/gnu/get_gnu_triplet.py` & `conan-2.3.0/conan/tools/gnu/get_gnu_triplet.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,11 @@
 from conan.errors import ConanException
 
 
-def _get_gnu_triplet(os_, arch, compiler=None):
-    """
-    Returns string with <machine>-<vendor>-<op_system> triplet (<vendor> can be omitted in practice)
-
-    :param os_: os to be used to create the triplet
-    :param arch: arch to be used to create the triplet
-    :param compiler: compiler used to create the triplet (only needed fo windows)
-    """
-
-    if os_ == "Windows" and compiler is None:
-        raise ConanException("'compiler' parameter for 'get_gnu_triplet()' is not specified and "
-                             "needed for os=Windows")
-
+def _get_gnu_arch(os_, arch):
     # Calculate the arch
     machine = {"x86": "i686",
                "x86_64": "x86_64",
                "armv8": "aarch64",
                "armv8_32": "aarch64",  # https://wiki.linaro.org/Platform/arm64-ilp32
                "armv8.3": "aarch64",
                "asm.js": "asmjs",
@@ -63,15 +51,18 @@
         elif 'riscv32' in arch:
             machine = "riscv32"
 
     if machine is None:
         raise ConanException("Unknown '%s' machine, Conan doesn't know how to "
                              "translate it to the GNU triplet, please report at "
                              " https://github.com/conan-io/conan/issues" % arch)
+    return machine
 
+
+def _get_gnu_os(os_, arch, compiler=None):
     # Calculate the OS
     if compiler == "gcc":
         windows_op = "w64-mingw32"
     else:
         windows_op = "unknown-windows"
 
     op_system = {"Windows": windows_op,
@@ -94,9 +85,28 @@
             op_system += "eabi"
 
         if (arch == "armv5hf" or arch == "armv7hf") and os_ == "Linux":
             op_system += "hf"
 
         if arch == "armv8_32" and os_ == "Linux":
             op_system += "_ilp32"  # https://wiki.linaro.org/Platform/arm64-ilp32
+    return op_system
+
 
-    return "%s-%s" % (machine, op_system)
+def _get_gnu_triplet(os_, arch, compiler=None):
+    """
+    Returns string with <machine>-<vendor>-<op_system> triplet (<vendor> can be omitted in practice)
+
+    :param os_: os to be used to create the triplet
+    :param arch: arch to be used to create the triplet
+    :param compiler: compiler used to create the triplet (only needed fo windows)
+    """
+    if os_ == "Windows" and compiler is None:
+        raise ConanException("'compiler' parameter for 'get_gnu_triplet()' is not specified and "
+                             "needed for os=Windows")
+    machine = _get_gnu_arch(os_, arch)
+    op_system = _get_gnu_os(os_, arch, compiler=compiler)
+    return {
+        'machine': machine,
+        'system': op_system,
+        'triplet': f"{machine}-{op_system}"
+    }
```

### Comparing `conan-2.2.3/conan/tools/gnu/gnudeps_flags.py` & `conan-2.3.0/conan/tools/gnu/gnudeps_flags.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/gnu/makedeps.py` & `conan-2.3.0/conan/tools/gnu/makedeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/gnu/pkgconfig.py` & `conan-2.3.0/conan/tools/gnu/pkgconfig.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/gnu/pkgconfigdeps.py` & `conan-2.3.0/conan/tools/gnu/pkgconfigdeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/google/bazel.py` & `conan-2.3.0/conan/tools/google/bazel.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/google/bazeldeps.py` & `conan-2.3.0/conan/tools/google/bazeldeps.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 def _get_package_reference_name(dep):
     """
     Get the reference name for the given package
     """
     return dep.ref.name
 
 
-def _get_repository_name(dep):
+def _get_repository_name(dep, is_build_require=False):
     pkg_name = dep.cpp_info.get_property("bazel_repository_name") or _get_package_reference_name(dep)
-    return f"build-{pkg_name}" if dep.context == "build" else pkg_name
+    return f"build-{pkg_name}" if is_build_require else pkg_name
 
 
 def _get_target_name(dep):
     pkg_name = dep.cpp_info.get_property("bazel_target_name") or _get_package_reference_name(dep)
     return pkg_name
 
 
@@ -452,17 +452,19 @@
                             undefined=StrictUndefined)
         content = template.render(context)
         save(self.build_file_pah, content)
 
 
 class _InfoGenerator:
 
-    def __init__(self, conanfile, dep):
+    def __init__(self, conanfile, dep, require):
         self._conanfile = conanfile
         self._dep = dep
+        self._req = require
+        self._is_build_require = require.build
         self._transitive_reqs = get_transitive_requires(self._conanfile, dep)
 
     def _get_cpp_info_requires_names(self, cpp_info):
         """
         Get all the valid names from the requirements ones given a CppInfo object.
 
         For instance, those requirements could be coming from:
@@ -487,15 +489,15 @@
             pkg_ref_name, comp_ref_name = req.split("::") if "::" in req else (dep_ref_name, req)
             prefix = ":"  # Requirements declared in the same BUILD file
             # For instance, dep == "hello/1.0" and req == "other::cmp1" -> hello != other
             if dep_ref_name != pkg_ref_name:
                 try:
                     req_conanfile = self._transitive_reqs[pkg_ref_name]
                     # Requirements declared in another dependency BUILD file
-                    prefix = f"@{_get_repository_name(req_conanfile)}//:"
+                    prefix = f"@{_get_repository_name(req_conanfile, is_build_require=self._is_build_require)}//:"
                 except KeyError:
                     continue  # If the dependency is not in the transitive, might be skipped
             else:  # For instance, dep == "hello/1.0" and req == "hello::cmp1" -> hello == hello
                 req_conanfile = self._dep
             comp_name = _get_component_name(req_conanfile, comp_ref_name)
             ret.append(f"{prefix}{comp_name}")
         return ret
@@ -523,24 +525,26 @@
     @property
     def root_package_info(self):
         """
         Get the whole package information
 
         :return: `_BazelTargetInfo` object with the package information
         """
-        repository_name = _get_repository_name(self._dep)
+        repository_name = _get_repository_name(self._dep, is_build_require=self._is_build_require)
         pkg_name = _get_target_name(self._dep)
         # At first, let's check if we have defined some global requires, e.g., "other::cmp1"
         requires = self._get_cpp_info_requires_names(self._dep.cpp_info)
         # If we have found some component requires it would be enough
         if not requires:
             # If no requires were found, let's try to get all the direct dependencies,
             # e.g., requires = "other_pkg/1.0"
-            requires = [f"@{_get_repository_name(req)}//:{_get_target_name(req)}"
-                        for req in self._transitive_reqs.values()]
+            requires = [
+                f"@{_get_repository_name(req, is_build_require=self._is_build_require)}//:{_get_target_name(req)}"
+                for req in self._transitive_reqs.values()
+            ]
         cpp_info = self._dep.cpp_info
         return _BazelTargetInfo(repository_name, pkg_name, requires, cpp_info)
 
 
 class BazelDeps:
 
     def __init__(self, conanfile):
@@ -563,15 +567,15 @@
             load_conan_dependencies()
         """
         check_duplicated_generator(self, self._conanfile)
         requirements = _get_requirements(self._conanfile, self.build_context_activated)
         deps_info = []
         for require, dep in requirements:
             # Bazel info generator
-            info_generator = _InfoGenerator(self._conanfile, dep)
+            info_generator = _InfoGenerator(self._conanfile, dep, require)
             root_package_info = info_generator.root_package_info
             components_info = info_generator.components_info
             # Generating single BUILD files per dependency
             bazel_generator = _BazelBUILDGenerator(self._conanfile, dep,
                                                    root_package_info, components_info)
             bazel_generator.generate()
             # Saving pieces of information from each BUILD file
```

### Comparing `conan-2.2.3/conan/tools/google/layout.py` & `conan-2.3.0/conan/tools/google/layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/google/toolchain.py` & `conan-2.3.0/conan/tools/google/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/intel/intel_cc.py` & `conan-2.3.0/conan/tools/intel/intel_cc.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/layout/__init__.py` & `conan-2.3.0/conan/tools/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/meson/helpers.py` & `conan-2.3.0/conan/tools/meson/helpers.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/meson/meson.py` & `conan-2.3.0/conan/tools/meson/meson.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,32 +25,30 @@
         :param reconfigure: ``bool`` value that adds ``--reconfigure`` param to the final command.
         """
         if reconfigure:
             self._conanfile.output.warning("reconfigure param has been deprecated."
                                            " Removing in Conan 2.x.", warn_tag="deprecated")
         source_folder = self._conanfile.source_folder
         build_folder = self._conanfile.build_folder
-        cmd = "meson setup"
         generators_folder = self._conanfile.generators_folder
         cross = os.path.join(generators_folder, MesonToolchain.cross_filename)
         native = os.path.join(generators_folder, MesonToolchain.native_filename)
-        meson_filenames = []
-        if os.path.exists(cross):
-            cmd_param = " --cross-file"
-            meson_filenames.append(cross)
-        else:
-            cmd_param = " --native-file"
-            meson_filenames.append(native)
-
+        is_cross_build = os.path.exists(cross)
         machine_files = self._conanfile.conf.get("tools.meson.mesontoolchain:extra_machine_files",
                                                  default=[], check_type=list)
-        if machine_files:
-            meson_filenames.extend(machine_files)
-
-        cmd += "".join([f'{cmd_param} "{meson_option}"' for meson_option in meson_filenames])
+        cmd = "meson setup "
+        if is_cross_build:
+            machine_files.insert(0, cross)
+            cmd += " ".join([f'--cross-file "{file}"' for file in machine_files])
+        if os.path.exists(native):
+            if not is_cross_build:  # machine files are only appended to the cross or the native one
+                machine_files.insert(0, native)
+                cmd += " ".join([f'--native-file "{file}"' for file in machine_files])
+            else:  # extra native file for cross-building scenarios
+                cmd += f' --native-file "{native}"'
         cmd += ' "{}" "{}"'.format(build_folder, source_folder)
         # Issue related: https://github.com/mesonbuild/meson/issues/12880
         cmd += ' --prefix=/'  # this must be an absolute path, otherwise, meson complains
         self._conanfile.output.info("Meson configure cmd: {}".format(cmd))
         self._conanfile.run(cmd)
 
     def build(self, target=None):
```

### Comparing `conan-2.2.3/conan/tools/meson/toolchain.py` & `conan-2.3.0/conan/tools/meson/toolchain.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,76 +1,127 @@
 import os
 import textwrap
 
-from jinja2 import Template
+from jinja2 import Template, StrictUndefined
 
 from conan.errors import ConanException
 from conan.internal import check_duplicated_generator
 from conan.internal.internal_tools import raise_on_universal_arch
-from conan.tools.apple.apple import to_apple_arch, is_apple_os, apple_min_version_flag, \
-    apple_sdk_path, get_apple_sdk_fullname
+from conan.tools.apple.apple import is_apple_os, apple_min_version_flag, \
+    resolve_apple_flags
 from conan.tools.build.cross_building import cross_building
 from conan.tools.build.flags import libcxx_flags
 from conan.tools.env import VirtualBuildEnv
 from conan.tools.meson.helpers import *
 from conan.tools.microsoft import VCVars, msvc_runtime_flag
 from conans.util.files import save
 
 
 class MesonToolchain(object):
     """
     MesonToolchain generator
     """
-
     native_filename = "conan_meson_native.ini"
     cross_filename = "conan_meson_cross.ini"
 
-    _meson_file_template = textwrap.dedent("""
+    _meson_file_template = textwrap.dedent("""\
     [properties]
     {% for it, value in properties.items() -%}
     {{it}} = {{value}}
     {% endfor %}
 
     [constants]
     preprocessor_definitions = [{% for it, value in preprocessor_definitions.items() -%}
     '-D{{ it }}="{{ value}}"'{%- if not loop.last %}, {% endif %}{% endfor %}]
 
     [project options]
     {% for it, value in project_options.items() -%}
     {{it}} = {{value}}
     {% endfor %}
 
+    {% for subproject, listkeypair in subproject_options -%}
+    [{{subproject}}:project options]
+    {% for keypair in listkeypair -%}
+    {% for it, value in keypair.items() -%}
+    {{it}} = {{value}}
+    {% endfor %}
+    {% endfor %}
+    {% endfor %}
+
     [binaries]
-    {% if c %}c = {{c}}{% endif %}
-    {% if cpp %}cpp = {{cpp}}{% endif %}
-    {% if ld %}ld = {{ld}}{% endif %}
+    {% if c %}
+    c = {{c}}
+    {% endif %}
+    {% if cpp %}
+    cpp = {{cpp}}
+    {% endif %}
+    {% if ld %}
+    ld = {{ld}}
+    {% endif %}
     {% if is_apple_system %}
-    {% if objc %}objc = '{{objc}}'{% endif %}
-    {% if objcpp %}objcpp = '{{objcpp}}'{% endif %}
+    {% if objc %}
+    objc = '{{objc}}'
+    {% endif %}
+    {% if objcpp %}
+    objcpp = '{{objcpp}}'
+    {% endif %}
+    {% endif %}
+    {% if c_ld %}
+    c_ld = '{{c_ld}}'
+    {% endif %}
+    {% if cpp_ld %}
+    cpp_ld = '{{cpp_ld}}'
+    {% endif %}
+    {% if ar %}
+    ar = '{{ar}}'
+    {% endif %}
+    {% if strip %}
+    strip = '{{strip}}'
+    {% endif %}
+    {% if as %}
+    as = '{{as}}'
+    {% endif %}
+    {% if windres %}
+    windres = '{{windres}}'
+    {% endif %}
+    {% if pkgconfig %}
+    pkgconfig = '{{pkgconfig}}'
+    {% endif %}
+    {% if pkgconfig %}
+    pkg-config = '{{pkgconfig}}'
     {% endif %}
-    {% if c_ld %}c_ld = '{{c_ld}}'{% endif %}
-    {% if cpp_ld %}cpp_ld = '{{cpp_ld}}'{% endif %}
-    {% if ar %}ar = '{{ar}}'{% endif %}
-    {% if strip %}strip = '{{strip}}'{% endif %}
-    {% if as %}as = '{{as}}'{% endif %}
-    {% if windres %}windres = '{{windres}}'{% endif %}
-    {% if pkgconfig %}pkgconfig = '{{pkgconfig}}'{% endif %}
-    {% if pkgconfig %}pkg-config = '{{pkgconfig}}'{% endif %}
 
     [built-in options]
-    {% if buildtype %}buildtype = '{{buildtype}}'{% endif %}
-    {% if debug %}debug = {{debug}}{% endif %}
-    {% if default_library %}default_library = '{{default_library}}'{% endif %}
-    {% if b_vscrt %}b_vscrt = '{{b_vscrt}}' {% endif %}
-    {% if b_ndebug %}b_ndebug = {{b_ndebug}}{% endif %}
-    {% if b_staticpic %}b_staticpic = {{b_staticpic}}{% endif %}
-    {% if cpp_std %}cpp_std = '{{cpp_std}}' {% endif %}
-    {% if backend %}backend = '{{backend}}' {% endif %}
-    {% if pkg_config_path %}pkg_config_path = '{{pkg_config_path}}'{% endif %}
-    {% if build_pkg_config_path %}build.pkg_config_path = '{{build_pkg_config_path}}'{% endif %}
+    {% if buildtype %}
+    buildtype = '{{buildtype}}'
+    {% endif %}
+    {% if default_library %}
+    default_library = '{{default_library}}'
+    {% endif %}
+    {% if b_vscrt %}
+    b_vscrt = '{{b_vscrt}}'
+    {% endif %}
+    {% if b_ndebug %}
+    b_ndebug = {{b_ndebug}}
+    {% endif %}
+    {% if b_staticpic %}
+    b_staticpic = {{b_staticpic}}
+    {% endif %}
+    {% if cpp_std %}
+    cpp_std = '{{cpp_std}}'
+    {% endif %}
+    {% if backend %}
+    backend = '{{backend}}'
+    {% endif %}
+    {% if pkg_config_path %}
+    pkg_config_path = '{{pkg_config_path}}'
+    {% endif %}
+    {% if build_pkg_config_path %}
+    build.pkg_config_path = '{{build_pkg_config_path}}'
+    {% endif %}
     # C/C++ arguments
     c_args = {{c_args}} + preprocessor_definitions
     c_link_args = {{c_link_args}}
     cpp_args = {{cpp_args}} + preprocessor_definitions
     cpp_link_args = {{cpp_link_args}}
     {% if is_apple_system %}
     # Objective-C/C++ arguments
@@ -85,24 +136,32 @@
     system = '{{values["system"]}}'
     cpu_family = '{{values["cpu_family"]}}'
     cpu = '{{values["cpu"]}}'
     endian = '{{values["endian"]}}'
     {% endfor %}
     """)
 
-    def __init__(self, conanfile, backend=None):
+    def __init__(self, conanfile, backend=None, native=False):
         """
         :param conanfile: ``< ConanFile object >`` The current recipe object. Always use ``self``.
         :param backend: ``str`` ``backend`` Meson variable value. By default, ``ninja``.
+        :param native: ``bool`` Indicates whether you want Conan to create the
+                       ``conan_meson_native.ini`` in a cross-building context. Notice that it only
+                       makes sense if your project's ``meson.build`` uses the ``native=true``
+                       (see also https://mesonbuild.com/Cross-compilation.html#mixing-host-and-build-targets).
         """
         raise_on_universal_arch(conanfile)
         self._conanfile = conanfile
-        self._os = self._conanfile.settings.get_safe("os")
+        self._native = native
         self._is_apple_system = is_apple_os(self._conanfile)
-
+        is_cross_building = cross_building(conanfile, skip_x64_x86=True)
+        if not is_cross_building and native:
+            raise ConanException("You can only pass native=True if you're cross-building, "
+                                 "otherwise, it could cause unexpected results.")
+        self._conanfile_conf = self._conanfile.conf_build if native else self._conanfile.conf
         # Values are kept as Python built-ins so users can modify them more easily, and they are
         # only converted to Meson file syntax for rendering
         # priority: first user conf, then recipe, last one is default "ninja"
         self._backend = conanfile.conf.get("tools.meson.mesontoolchain:backend",
                                            default=backend or 'ninja')
         build_type = self._conanfile.settings.get_safe("build_type")
         self._buildtype = {"Debug": "debug",  # Note, it is not "'debug'"
@@ -141,28 +200,28 @@
         self.project_options = {
             "wrap_mode": "nofallback"  # https://github.com/conan-io/conan/issues/10671
         }
         #: Dict-like object that defines Meson ``preprocessor definitions``
         self.preprocessor_definitions = {}
         # Add all the default dirs
         self.project_options.update(self._get_default_dirs())
-
+        #: Dict-like object that defines Meson ``subproject options``.
+        self.subproject_options = {}
         #: Defines the Meson ``pkg_config_path`` variable
         self.pkg_config_path = self._conanfile.generators_folder
         #: Defines the Meson ``build.pkg_config_path`` variable (build context)
         # Issue: https://github.com/conan-io/conan/issues/12342
         # Issue: https://github.com/conan-io/conan/issues/14935
         self.build_pkg_config_path = None
         self.libcxx, self.gcc_cxx11_abi = libcxx_flags(self._conanfile)
-
         #: Dict-like object with the build, host, and target as the Meson machine context
         self.cross_build = {}
         default_comp = ""
         default_comp_cpp = ""
-        if cross_building(conanfile, skip_x64_x86=True):
+        if native is False and is_cross_building:
             os_host = conanfile.settings.get_safe("os")
             arch_host = conanfile.settings.get_safe("arch")
             os_build = conanfile.settings_build.get_safe('os')
             arch_build = conanfile.settings_build.get_safe('arch')
             self.cross_build["build"] = to_meson_machine(os_build, arch_build)
             self.cross_build["host"] = to_meson_machine(os_host, arch_host)
             self.properties["needs_exe_wrapper"] = True
@@ -183,18 +242,19 @@
                 default_comp_cpp = "g++"
 
         if "Visual" in compiler or compiler == "msvc":
             default_comp = "cl"
             default_comp_cpp = "cl"
 
         # Read configuration for compilers
-        compilers_by_conf = self._conanfile.conf.get("tools.build:compiler_executables", default={},
+        compilers_by_conf = self._conanfile_conf.get("tools.build:compiler_executables", default={},
                                                      check_type=dict)
         # Read the VirtualBuildEnv to update the variables
-        build_env = VirtualBuildEnv(self._conanfile, auto_generate=True).vars()
+        build_env = self._conanfile.buildenv_build.vars(self._conanfile) if native else (
+            VirtualBuildEnv(self._conanfile, auto_generate=True).vars())
         #: Sets the Meson ``c`` variable, defaulting to the ``CC`` build environment value.
         #: If provided as a blank-separated string, it will be transformed into a list.
         #: Otherwise, it remains a single string.
         self.c = compilers_by_conf.get("c") or build_env.get("CC") or default_comp
         #: Sets the Meson ``cpp`` variable, defaulting to the ``CXX`` build environment value.
         #: If provided as a blank-separated string, it will be transformed into a list.
         #: Otherwise, it remains a single string.
@@ -218,15 +278,15 @@
         self.strip = build_env.get("STRIP")
         #: Defines the Meson ``as`` variable. Defaulted to ``AS`` build environment value
         self.as_ = build_env.get("AS")
         #: Defines the Meson ``windres`` variable. Defaulted to ``WINDRES`` build environment value
         self.windres = build_env.get("WINDRES")
         #: Defines the Meson ``pkgconfig`` variable. Defaulted to ``PKG_CONFIG``
         #: build environment value
-        self.pkgconfig = (self._conanfile.conf.get("tools.gnu:pkg_config", check_type=str) or
+        self.pkgconfig = (self._conanfile_conf.get("tools.gnu:pkg_config", check_type=str) or
                           build_env.get("PKG_CONFIG"))
         #: Defines the Meson ``c_args`` variable. Defaulted to ``CFLAGS`` build environment value
         self.c_args = self._get_env_list(build_env.get("CFLAGS", []))
         #: Defines the Meson ``c_link_args`` variable. Defaulted to ``LDFLAGS`` build
         #: environment value
         self.c_link_args = self._get_env_list(build_env.get("LDFLAGS", []))
         #: Defines the Meson ``cpp_args`` variable. Defaulted to ``CXXFLAGS`` build environment value
@@ -252,15 +312,16 @@
         self.objc_link_args = []
         #: Defines the Meson ``objcpp_args`` variable. Defaulted to ``OBJCXXFLAGS`` build environment value
         self.objcpp_args = []
         #: Defines the Meson ``objcpp_link_args`` variable. Defaulted to ``LDFLAGS`` build environment value
         self.objcpp_link_args = []
 
         self._resolve_apple_flags_and_variables(build_env, compilers_by_conf)
-        self._resolve_android_cross_compilation()
+        if native is False:
+            self._resolve_android_cross_compilation()
 
     def _get_default_dirs(self):
         """
         Get all the default directories from cpp.package.
 
         Issues related:
             - https://github.com/conan-io/conan/issues/9713
@@ -293,42 +354,33 @@
         if libdir:
             ret["libdir"] = libdir
         return ret
 
     def _resolve_apple_flags_and_variables(self, build_env, compilers_by_conf):
         if not self._is_apple_system:
             return
-        # SDK path is mandatory for cross-building
-        sdk_path = apple_sdk_path(self._conanfile)
-        if not sdk_path and self.cross_build:
-            raise ConanException(
-                "Apple SDK path not found. For cross-compilation, you must "
-                "provide a valid SDK path in 'tools.apple:sdk_path' config."
-            )
         # Calculating the main Apple flags
-        os_sdk = get_apple_sdk_fullname(self._conanfile)
-        arch = to_apple_arch(self._conanfile)
-        self.apple_arch_flag = ["-arch", arch] if arch else []
-        self.apple_isysroot_flag = ["-isysroot", sdk_path] if sdk_path else []
-        os_version = self._conanfile.settings.get_safe("os.version")
-        subsystem = self._conanfile.settings.get_safe("os.subsystem")
-        self.apple_min_version_flag = [apple_min_version_flag(os_version, os_sdk, subsystem)]
+        min_flag, arch_flag, isysroot_flag = (
+            resolve_apple_flags(self._conanfile, is_cross_building=self.cross_build))
+        self.apple_arch_flag = arch_flag.split() if arch_flag else []
+        self.apple_isysroot_flag = isysroot_flag.split() if isysroot_flag else []
+        self.apple_min_version_flag = [apple_min_version_flag(self._conanfile)]
         # Objective C/C++ ones
         self.objc = compilers_by_conf.get("objc", "clang")
         self.objcpp = compilers_by_conf.get("objcpp", "clang++")
         self.objc_args = self._get_env_list(build_env.get('OBJCFLAGS', []))
         self.objc_link_args = self._get_env_list(build_env.get('LDFLAGS', []))
         self.objcpp_args = self._get_env_list(build_env.get('OBJCXXFLAGS', []))
         self.objcpp_link_args = self._get_env_list(build_env.get('LDFLAGS', []))
 
     def _resolve_android_cross_compilation(self):
         if not self.cross_build or not self.cross_build["host"]["system"] == "android":
             return
 
-        ndk_path = self._conanfile.conf.get("tools.android:ndk_path")
+        ndk_path = self._conanfile_conf.get("tools.android:ndk_path")
         if not ndk_path:
             raise ConanException("You must provide a NDK path. Use 'tools.android:ndk_path' "
                                  "configuration field.")
 
         arch = self._conanfile.settings.get_safe("arch")
         os_build = self.cross_build["build"]["system"]
         ndk_bin = os.path.join(ndk_path, "toolchains", "llvm", "prebuilt", "{}-x86_64".format(os_build), "bin")
@@ -341,24 +393,26 @@
         compiler_extension = ".cmd" if os_build == "Windows" else ""
         self.c = os.path.join(ndk_bin, "{}{}-clang{}".format(android_target, android_api_level, compiler_extension))
         self.cpp = os.path.join(ndk_bin, "{}{}-clang++{}".format(android_target, android_api_level, compiler_extension))
         self.ar = os.path.join(ndk_bin, "llvm-ar")
 
     def _get_extra_flags(self):
         # Now, it's time to get all the flags defined by the user
-        cxxflags = self._conanfile.conf.get("tools.build:cxxflags", default=[], check_type=list)
-        cflags = self._conanfile.conf.get("tools.build:cflags", default=[], check_type=list)
-        sharedlinkflags = self._conanfile.conf.get("tools.build:sharedlinkflags", default=[], check_type=list)
-        exelinkflags = self._conanfile.conf.get("tools.build:exelinkflags", default=[], check_type=list)
-        linker_scripts = self._conanfile.conf.get("tools.build:linker_scripts", default=[], check_type=list)
+        cxxflags = self._conanfile_conf.get("tools.build:cxxflags", default=[], check_type=list)
+        cflags = self._conanfile_conf.get("tools.build:cflags", default=[], check_type=list)
+        sharedlinkflags = self._conanfile_conf.get("tools.build:sharedlinkflags", default=[], check_type=list)
+        exelinkflags = self._conanfile_conf.get("tools.build:exelinkflags", default=[], check_type=list)
+        linker_scripts = self._conanfile_conf.get("tools.build:linker_scripts", default=[], check_type=list)
         linker_script_flags = ['-T"' + linker_script + '"' for linker_script in linker_scripts]
+        defines = [f"-D{d}" for d in self._conanfile.conf.get("tools.build:defines", default=[], check_type=list)]
         return {
             "cxxflags": cxxflags,
             "cflags": cflags,
-            "ldflags": sharedlinkflags + exelinkflags + linker_script_flags
+            "ldflags": sharedlinkflags + exelinkflags + linker_script_flags,
+            "defines": defines
         }
 
     @staticmethod
     def _get_env_list(v):
         # FIXME: Should Environment have the "check_type=None" keyword as Conf?
         return v.strip().split() if not isinstance(v, list) else v
 
@@ -372,36 +426,45 @@
                 return v
             ret = [x.strip() for x in v.split() if x]
             return f"'{ret[0]}'" if len(ret) == 1 else ret
 
         apple_flags = self.apple_isysroot_flag + self.apple_arch_flag + self.apple_min_version_flag
         extra_flags = self._get_extra_flags()
 
-        self.c_args.extend(apple_flags + extra_flags["cflags"])
-        self.cpp_args.extend(apple_flags + extra_flags["cxxflags"])
+        self.c_args.extend(apple_flags + extra_flags["cflags"] + extra_flags["defines"])
+        self.cpp_args.extend(apple_flags + extra_flags["cxxflags"] + extra_flags["defines"])
         self.c_link_args.extend(apple_flags + extra_flags["ldflags"])
         self.cpp_link_args.extend(apple_flags + extra_flags["ldflags"])
         # Objective C/C++
-        self.objc_args.extend(self.c_args)
-        self.objcpp_args.extend(self.cpp_args)
+        self.objc_args.extend(self.c_args + extra_flags["defines"])
+        self.objcpp_args.extend(self.cpp_args + extra_flags["defines"])
         # These link_args have already the LDFLAGS env value so let's add only the new possible ones
         self.objc_link_args.extend(apple_flags + extra_flags["ldflags"])
         self.objcpp_link_args.extend(apple_flags + extra_flags["ldflags"])
 
         if self.libcxx:
             self.cpp_args.append(self.libcxx)
             self.cpp_link_args.append(self.libcxx)
         if self.gcc_cxx11_abi:
             self.cpp_args.append("-D{}".format(self.gcc_cxx11_abi))
 
+        subproject_options = {}
+        for subproject, listkeypair in self.subproject_options.items():
+            if listkeypair is not None and listkeypair is not []:
+                subproject_options[subproject] = []
+                for keypair in listkeypair:
+                    subproject_options[subproject].append({k: to_meson_value(v) for k, v in keypair.items()})
+
         return {
             # https://mesonbuild.com/Machine-files.html#properties
             "properties": {k: to_meson_value(v) for k, v in self.properties.items()},
             # https://mesonbuild.com/Machine-files.html#project-specific-options
             "project_options": {k: to_meson_value(v) for k, v in self.project_options.items()},
+            # https://mesonbuild.com/Subprojects.html#build-options-in-subproject
+            "subproject_options": subproject_options.items(),
             # https://mesonbuild.com/Builtin-options.html#directories
             # https://mesonbuild.com/Machine-files.html#binaries
             # https://mesonbuild.com/Reference-tables.html#compiler-and-linker-selection-variables
             "c": _sanitize_format(self.c),
             "cpp": _sanitize_format(self.cpp),
             "ld": _sanitize_format(self.ld),
             "objc": self.objc,
@@ -435,28 +498,37 @@
             "build_pkg_config_path": self.build_pkg_config_path,
             "preprocessor_definitions": self.preprocessor_definitions,
             "cross_build": self.cross_build,
             "is_apple_system": self._is_apple_system
         }
 
     @property
+    def _filename(self):
+        if self.cross_build and self._native:
+            return self.native_filename
+        elif self.cross_build:
+            return self.cross_filename
+        else:
+            return self.native_filename
+
+    @property
     def _content(self):
         """
         Gets content of the file to be used by Meson as its context.
 
         :return: ``str`` whole Meson context content.
         """
         context = self._context()
-        content = Template(self._meson_file_template).render(context)
+        content = Template(self._meson_file_template, trim_blocks=True, lstrip_blocks=True,
+                           undefined=StrictUndefined).render(context)
         return content
 
     def generate(self):
         """
         Creates a ``conan_meson_native.ini`` (if native builds) or a
         ``conan_meson_cross.ini`` (if cross builds) with the proper content.
         If Windows OS, it will be created a ``conanvcvars.bat`` as well.
         """
         check_duplicated_generator(self, self._conanfile)
-        filename = self.native_filename if not self.cross_build else self.cross_filename
-        save(filename, self._content)
+        save(self._filename, self._content)
         # FIXME: Should we check the OS and compiler to call VCVars?
         VCVars(self._conanfile).generate()
```

### Comparing `conan-2.2.3/conan/tools/microsoft/__init__.py` & `conan-2.3.0/conan/tools/microsoft/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/microsoft/layout.py` & `conan-2.3.0/conan/tools/microsoft/layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/microsoft/msbuild.py` & `conan-2.3.0/conan/tools/microsoft/msbuild.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/microsoft/msbuilddeps.py` & `conan-2.3.0/conan/tools/microsoft/msbuilddeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/microsoft/nmakedeps.py` & `conan-2.3.0/conan/tools/microsoft/nmakedeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/microsoft/nmaketoolchain.py` & `conan-2.3.0/conan/tools/microsoft/nmaketoolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/microsoft/subsystems.py` & `conan-2.3.0/conan/tools/microsoft/subsystems.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/microsoft/toolchain.py` & `conan-2.3.0/conan/tools/microsoft/toolchain.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/microsoft/visual.py` & `conan-2.3.0/conan/tools/microsoft/visual.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,21 @@
                 raise ConanException("Visual Studio Runtime version (v140-v143) not defined")
             vcvars_ver = {"v140": "14.0",
                           "v141": "14.1",
                           "v142": "14.2",
                           "v143": "14.3"}.get(toolset_version)
         else:
             vs_version = vs_ide_version(conanfile)
-            vcvars_ver = _vcvars_vers(conanfile, compiler, vs_version)
+            if int(vs_version) <= 14:
+                vcvars_ver = None
+            else:
+                compiler_version = str(conanfile.settings.compiler.version)
+                compiler_update = conanfile.settings.get_safe("compiler.update", "")
+                # The equivalent of compiler 19.26 is toolset 14.26
+                vcvars_ver = "14.{}{}".format(compiler_version[-1], compiler_update)
         vcvarsarch = _vcvars_arch(conanfile)
 
         winsdk_version = conanfile.conf.get("tools.microsoft:winsdk_version", check_type=str)
         winsdk_version = winsdk_version or conanfile.settings.get_safe("os.version")
         # The vs_install_path is like
         # C:\Program Files (x86)\Microsoft Visual Studio\2019\Community
         # C:\Program Files (x86)\Microsoft Visual Studio\2017\Community
@@ -156,15 +162,15 @@
         from conan.tools.env.environment import create_env_script
         conan_vcvars_bat = f"{CONAN_VCVARS}.bat"
         create_env_script(conanfile, content, conan_vcvars_bat, scope)
         _create_deactivate_vcvars_file(conanfile, conan_vcvars_bat)
 
         is_ps1 = conanfile.conf.get("tools.env.virtualenv:powershell", check_type=bool, default=False)
         if is_ps1:
-            content_ps1 = textwrap.dedent(f"""\
+            content_ps1 = textwrap.dedent(rf"""\
             if (-not $env:VSCMD_ARG_VCVARS_VER){{
                 Push-Location "$PSScriptRoot"
                 cmd /c "conanvcvars.bat&set" |
                 foreach {{
                   if ($_ -match "=") {{
                     $v = $_.split("=", 2); set-item -force -path "ENV:\$($v[0])"  -value "$($v[1])"
                   }}
@@ -173,26 +179,26 @@
                 write-host conanvcvars.ps1: Activated environment}}
             """)
             conan_vcvars_ps1 = f"{CONAN_VCVARS}.ps1"
             create_env_script(conanfile, content_ps1, conan_vcvars_ps1, scope)
             _create_deactivate_vcvars_file(conanfile, conan_vcvars_ps1)
 
 
-
 def _create_deactivate_vcvars_file(conanfile, filename):
     deactivate_filename = f"deactivate_{filename}"
     message = f"[{deactivate_filename}]: vcvars env cannot be deactivated"
     is_ps1 = filename.endswith(".ps1")
     if is_ps1:
         content = f"Write-Host {message}"
     else:
         content = f"echo {message}"
     path = os.path.join(conanfile.generators_folder, deactivate_filename)
     save(path, content)
 
+
 def vs_ide_version(conanfile):
     """
     Gets the VS IDE version as string. It'll use the ``compiler.version`` (if exists) and/or the
     ``tools.microsoft.msbuild:vs_version`` if ``compiler`` is ``msvc``.
 
     :param conanfile: ``< ConanFile object >`` The current recipe object. Always use ``self``.
     :return: ``str`` Visual IDE version number.
@@ -294,15 +300,15 @@
 
     arch = None
     if arch_build == 'x86_64':
         arch = {'x86': "amd64_x86",
                 'x86_64': 'amd64',
                 'armv7': 'amd64_arm',
                 'armv8': 'amd64_arm64',
-                'arm64ec':'amd64_arm64'}.get(arch_host)
+                'arm64ec': 'amd64_arm64'}.get(arch_host)
     elif arch_build == 'x86':
         arch = {'x86': 'x86',
                 'x86_64': 'x86_amd64',
                 'armv7': 'x86_arm',
                 'armv8': 'x86_arm64'}.get(arch_host)
     elif arch_build == 'armv8':
         arch = {'x86': 'arm64_x86',
@@ -312,26 +318,14 @@
 
     if not arch:
         raise ConanException('vcvars unsupported architectures %s-%s' % (arch_build, arch_host))
 
     return arch
 
 
-def _vcvars_vers(conanfile, compiler, vs_version):
-    if int(vs_version) <= 14:
-        return None
-
-    assert compiler == "msvc"
-    # Code similar to CMakeToolchain toolset one
-    compiler_version = str(conanfile.settings.compiler.version)
-    # The equivalent of compiler 192 is toolset 14.2
-    vcvars_ver = "14.{}".format(compiler_version[-1])
-    return vcvars_ver
-
-
 def is_msvc(conanfile, build_context=False):
     """
     Validates if the current compiler is ``msvc``.
 
     :param conanfile: ``< ConanFile object >`` The current recipe object. Always use ``self``.
     :param build_context: If True, will use the settings from the build context, not host ones
     :return: ``bool`` True, if the host compiler is ``msvc``, otherwise, False.
```

### Comparing `conan-2.2.3/conan/tools/premake/premake.py` & `conan-2.3.0/conan/tools/premake/premake.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/premake/premakedeps.py` & `conan-2.3.0/conan/tools/premake/premakedeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/qbs/qbs.py` & `conan-2.3.0/conan/tools/qbs/qbs.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/qbs/qbsprofile.py` & `conan-2.3.0/conan/tools/qbs/qbsprofile.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/scm/git.py` & `conan-2.3.0/conan/tools/scm/git.py`

 * *Files 10% similar despite different names*

```diff
@@ -193,41 +193,49 @@
         Get the current repository top folder with ``git rev-parse --show-toplevel``
 
         :return: Repository top folder.
         """
         folder = self.run("rev-parse --show-toplevel")
         return folder.replace("\\", "/")
 
-    def clone(self, url, target="", args=None):
+    def clone(self, url, target="", args=None, hide_url=True):
         """
         Performs a ``git clone <url> <args> <target>`` operation, where target is the target directory.
 
         :param url: URL of remote repository.
         :param target: Target folder.
         :param args: Extra arguments to pass to the git clone as a list.
+        :param hide_url: Hides the URL from the log output to prevent accidental
+                     credential leaks. Can be disabled by passing ``False``.
         """
         args = args or []
         if os.path.exists(url):
             url = url.replace("\\", "/")  # Windows local directory
         mkdir(self.folder)
         self._conanfile.output.info("Cloning git repo")
         target_path = f'"{target}"' if target else ""  # quote in case there are spaces in path
         # Avoid printing the clone command, it can contain tokens
-        self.run('clone "{}" {} {}'.format(url, " ".join(args), target_path), hidden_output=url)
+        self.run('clone "{}" {} {}'.format(url, " ".join(args), target_path),
+                 hidden_output=url if hide_url else None)
 
-    def fetch_commit(self, url, commit):
+    def fetch_commit(self, url, commit, hide_url=True):
         """
-        Experimental: does a 1 commit fetch and checkout, instead of a full clone,
+        Experimental: does a single commit fetch and checkout, instead of a full clone,
         should be faster.
+
+        :param url: URL of remote repository.
+        :param commit: The commit ref to checkout.
+        :param hide_url: Hides the URL from the log output to prevent accidental
+                     credential leaks. Can be disabled by passing ``False``.
         """
         if os.path.exists(url):
             url = url.replace("\\", "/")  # Windows local directory
         self._conanfile.output.info("Shallow fetch of git repo")
         self.run('init')
-        self.run(f'remote add origin "{url}"', hidden_output=url)
+        self.run(f'remote add origin "{url}"', hidden_output=url if hide_url else None)
         self.run(f'fetch --depth 1 origin {commit}')
         self.run('checkout FETCH_HEAD')
 
     def checkout(self, commit):
         """
         Checkouts the given commit using ``git checkout <commit>``.
```

### Comparing `conan-2.2.3/conan/tools/scons/sconsdeps.py` & `conan-2.3.0/conan/tools/scons/sconsdeps.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conan/tools/system/package_manager.py` & `conan-2.3.0/conan/tools/system/package_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     def get_default_tool(self):
         os_name = platform.system()
         if os_name in ["Linux", "FreeBSD"]:
             import distro
             os_name = distro.id() or os_name
         elif os_name == "Windows" and self._conanfile.conf.get("tools.microsoft.bash:subsystem") == "msys2":
             os_name = "msys2"
-        manager_mapping = {"apt-get": ["Linux", "ubuntu", "debian", "raspbian", "linuxmint", 'astra', 'elbrus', 'altlinux'],
+        manager_mapping = {"apt-get": ["Linux", "ubuntu", "debian", "raspbian", "linuxmint", 'astra', 'elbrus', 'altlinux', 'pop'],
                            "apk": ["alpine"],
                            "yum": ["pidora", "scientific", "xenserver", "amazon", "oracle", "amzn",
                                    "almalinux", "rocky"],
                            "dnf": ["fedora", "rhel", "centos", "mageia", "nobara"],
                            "brew": ["Darwin"],
                            "pacman": ["arch", "manjaro", "msys2", "endeavouros"],
                            "choco": ["Windows"],
@@ -57,15 +57,15 @@
         # in case we did not detect any exact match, check
         # if the name is contained inside the returned distro name
         # like for opensuse, that can have opensuse-version names
         for tool, distros in manager_mapping.items():
             for d in distros:
                 if d in os_name:
                     return tool
-                
+
         # No default package manager was found for the system,
         # so notify the user
         self._conanfile.output.info("A default system package manager couldn't be found for {}, "
                                     "system packages will not be installed.".format(os_name))
 
     def get_package_name(self, package, host_package=True):
         # Only if the package is for building, for example a library,
```

### Comparing `conan-2.2.3/conan.egg-info/PKG-INFO` & `conan-2.3.0/conan.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conan
-Version: 2.2.3
+Version: 2.3.0
 Summary: Conan C/C++ package manager
 Home-page: https://conan.io
 Author: JFrog LTD
 Author-email: luism@jfrog.com
 License: MIT
 Project-URL: Documentation, https://docs.conan.io
 Project-URL: Source, https://github.com/conan-io/conan
@@ -42,20 +42,14 @@
           This community also creates and maintains packages in ConanCenter and Bincrafters repositories in Bintray.
         - Stable. Used in production by many companies, since 1.0 there is a commitment not to break package recipes and documented behavior.
         
         
         This is the **developer/maintainer** documentation. For user documentation, go to https://docs.conan.io
         
         
-        | **develop2**            |
-        |-------------------------|
-        | [![Build Status Develop](https://ci.conan.io/buildStatus/icon?job=ConanTestSuite/develop)](https://ci.conan.io/blue/organizations/jenkins/ConanTestSuitev2/activity)  |
-        
-        
-        
         ## Setup
         
         You can run Conan from source in Windows, MacOS, and Linux:
         
         - **Install pip following** [pip docs](https://pip.pypa.io/en/stable/installation/).
         
         - **Clone Conan repository:**
@@ -86,17 +80,17 @@
             Conan commands. Type "conan <command> -h" for help
           ```
         
         ## Contributing to the project
         
         
         Feedback and contribution are always welcome in this project.
-        Please read our [contributing guide](https://github.com/conan-io/conan/blob/develop/.github/CONTRIBUTING.md).
+        Please read our [contributing guide](https://github.com/conan-io/conan/blob/develop2/.github/CONTRIBUTING.md).
         Also, if you plan to contribute, please add some testing for your changes. You can read the [Conan
-        tests guidelines section](https://github.com/conan-io/conan/blob/develop/conans/test/README.md) for
+        tests guidelines section](https://github.com/conan-io/conan/blob/develop2/conans/test/README.md) for
         some advice on how to write tests for Conan.
         
         ### Running the tests
         
         
         **Install Python requirements**
         
@@ -140,15 +134,15 @@
         
         OK
         ```
         
         To run specific tests, you can specify the test name too, something like:
         
         ```bash
-        $ python -m pytest conans/test/unittests/client/cmd/export_test.py::ExportTest::test_export_warning -s
+        $ python -m pytest conans/test/functional/command/export_test.py::TestRevisionModeSCM::test_revision_mode_scm -s
         ```
         
         The `-s` argument can be useful to see some output that otherwise is captured by *pytest*.
         
         Also, you can run tests against an instance of Artifactory. Those tests should add the attribute
         `artifactory_ready`.
         
@@ -185,7 +179,8 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
+Provides-Extra: runners
```

### Comparing `conan-2.2.3/conan.egg-info/SOURCES.txt` & `conan-2.3.0/conan.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 conan/cli/commands/export_pkg.py
 conan/cli/commands/graph.py
 conan/cli/commands/inspect.py
 conan/cli/commands/install.py
 conan/cli/commands/list.py
 conan/cli/commands/lock.py
 conan/cli/commands/new.py
+conan/cli/commands/pkglist.py
 conan/cli/commands/profile.py
 conan/cli/commands/remote.py
 conan/cli/commands/remove.py
 conan/cli/commands/search.py
 conan/cli/commands/source.py
 conan/cli/commands/test.py
 conan/cli/commands/upload.py
@@ -100,14 +101,18 @@
 conan/internal/cache/conan_reference_layout.py
 conan/internal/cache/home_paths.py
 conan/internal/cache/db/__init__.py
 conan/internal/cache/db/cache_database.py
 conan/internal/cache/db/packages_table.py
 conan/internal/cache/db/recipes_table.py
 conan/internal/cache/db/table.py
+conan/internal/runner/__init__.py
+conan/internal/runner/docker.py
+conan/internal/runner/ssh.py
+conan/internal/runner/wsl.py
 conan/tools/__init__.py
 conan/tools/android/__init__.py
 conan/tools/android/utils.py
 conan/tools/apple/__init__.py
 conan/tools/apple/apple.py
 conan/tools/apple/xcodebuild.py
 conan/tools/apple/xcodedeps.py
@@ -149,14 +154,15 @@
 conan/tools/files/symlinks/symlinks.py
 conan/tools/gnu/__init__.py
 conan/tools/gnu/autotools.py
 conan/tools/gnu/autotoolsdeps.py
 conan/tools/gnu/autotoolstoolchain.py
 conan/tools/gnu/get_gnu_triplet.py
 conan/tools/gnu/gnudeps_flags.py
+conan/tools/gnu/gnutoolchain.py
 conan/tools/gnu/makedeps.py
 conan/tools/gnu/pkgconfig.py
 conan/tools/gnu/pkgconfigdeps.py
 conan/tools/google/__init__.py
 conan/tools/google/bazel.py
 conan/tools/google/bazeldeps.py
 conan/tools/google/layout.py
@@ -192,14 +198,15 @@
 conans/__init__.py
 conans/conan.py
 conans/conan_server.py
 conans/errors.py
 conans/migrations.py
 conans/requirements.txt
 conans/requirements_dev.txt
+conans/requirements_runner.txt
 conans/requirements_server.txt
 conans/client/__init__.py
 conans/client/hook_manager.py
 conans/client/installer.py
 conans/client/loader.py
 conans/client/loader_txt.py
 conans/client/migrations.py
```

### Comparing `conan-2.2.3/conans/client/cache/cache.py` & `conan-2.3.0/conans/client/cache/cache.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/cache/editable.py` & `conan-2.3.0/conans/client/cache/editable.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/cmd/export.py` & `conan-2.3.0/conans/client/cmd/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     conanfile = loader.load_export(conanfile_path, name, version, user, channel, graph_lock,
                                    remotes=remotes)
 
     ref = RecipeReference(conanfile.name, conanfile.version,  conanfile.user, conanfile.channel)
     ref.validate_ref(allow_uppercase=global_conf.get("core:allow_uppercase_pkg_names",
                                                      check_type=bool))
 
+    conanfile.conf = global_conf.get_conanfile_conf(ref, is_consumer=True)
     conanfile.display_name = str(ref)
     conanfile.output.scope = conanfile.display_name
     scoped_output = conanfile.output
 
     recipe_layout = cache.create_export_recipe_layout(ref)
 
     hook_manager.execute("pre_export", conanfile=conanfile)
```

### Comparing `conan-2.2.3/conans/client/cmd/uploader.py` & `conan-2.3.0/conans/client/cmd/uploader.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from conan.internal.conan_app import ConanApp
 from conan.api.output import ConanOutput
 from conans.client.source import retrieve_exports_sources
 from conans.errors import ConanException, NotFoundException
 from conans.paths import (CONAN_MANIFEST, CONANFILE, EXPORT_SOURCES_TGZ_NAME,
                           EXPORT_TGZ_NAME, PACKAGE_TGZ_NAME, CONANINFO)
 from conans.util.files import (clean_dirty, is_dirty, gather_files,
-                               gzopen_without_timestamps, set_dirty_context_manager, mkdir)
+                               gzopen_without_timestamps, set_dirty_context_manager, mkdir,
+                               human_size)
 
 UPLOAD_POLICY_FORCE = "force-upload"
 UPLOAD_POLICY_SKIP = "skip-upload"
 
 
 class UploadUpstreamChecker:
     """ decides if something needs to be uploaded or force-uploaded checking if that exact
@@ -216,31 +217,33 @@
                 self.upload_recipe(ref, bundle, remote)
             for pref, prev_bundle in upload_data.prefs(ref, bundle).items():
                 if prev_bundle.get("upload"):
                     self.upload_package(pref, prev_bundle, remote)
 
     def upload_recipe(self, ref, bundle, remote):
         output = ConanOutput(scope=str(ref))
-        output.info(f"Uploading recipe '{ref.repr_notime()}'")
-        t1 = time.time()
         cache_files = bundle["files"]
 
+        output.info(f"Uploading recipe '{ref.repr_notime()}' ({_total_size(cache_files)})")
+
+        t1 = time.time()
         self._app.remote_manager.upload_recipe(ref, cache_files, remote)
 
         duration = time.time() - t1
         output.debug(f"Upload {ref} in {duration} time")
         return ref
 
     def upload_package(self, pref, prev_bundle, remote):
         output = ConanOutput(scope=str(pref.ref))
-        output.info(f"Uploading package '{pref.repr_notime()}'")
         cache_files = prev_bundle["files"]
         assert (pref.revision is not None), "Cannot upload a package without PREV"
         assert (pref.ref.revision is not None), "Cannot upload a package without RREV"
 
+        output.info(f"Uploading package '{pref.repr_notime()}' ({_total_size(cache_files)})")
+
         t1 = time.time()
         self._app.remote_manager.upload_package(pref, cache_files, remote)
         duration = time.time() - t1
         output.debug(f"Upload {pref} in {duration} time")
 
 
 def compress_files(files, name, dest_dir, compresslevel=None, ref=None):
@@ -255,7 +258,15 @@
             # recursive is False in case it is a symlink to a folder
             tgz.add(abs_path, filename, recursive=False)
         tgz.close()
 
     duration = time.time() - t1
     ConanOutput().debug(f"{name} compressed in {duration} time")
     return tgz_path
+
+
+def _total_size(cache_files):
+    total_size = 0
+    for file in cache_files.values():
+        stat = os.stat(file)
+        total_size += stat.st_size
+    return human_size(total_size)
```

### Comparing `conan-2.2.3/conans/client/conanfile/build.py` & `conan-2.3.0/conans/client/conanfile/build.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/conanfile/configure.py` & `conan-2.3.0/conans/client/conanfile/configure.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/conanfile/implementations.py` & `conan-2.3.0/conans/client/conanfile/implementations.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/conanfile/package.py` & `conan-2.3.0/conans/client/conanfile/package.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/conf/__init__.py` & `conan-2.3.0/conans/client/conf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,16 @@
                     "6", "6.1", "6.2", "6.3", "6.4", "6.5",
                     "7", "7.1", "7.2", "7.3", "7.4", "7.5",
                     "8", "8.1", "8.2", "8.3", "8.4", "8.5",
                     "9", "9.1", "9.2", "9.3", "9.4", "9.5",
                     "10", "10.1", "10.2", "10.3", "10.4", "10.5",
                     "11", "11.1", "11.2", "11.3", "11.4",
                     "12", "12.1", "12.2", "12.3",
-                    "13", "13.1", "13.2"]
+                    "13", "13.1", "13.2", 
+                    "14", "14.1"]
         libcxx: [libstdc++, libstdc++11]
         threads: [null, posix, win32]  # Windows MinGW
         exception: [null, dwarf2, sjlj, seh]  # Windows MinGW
         cppstd: [null, 98, gnu98, 11, gnu11, 14, gnu14, 17, gnu17, 20, gnu20, 23, gnu23]
     msvc:
         version: [170, 180, 190, 191, 192, 193]
         update: [null, 0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
```

### Comparing `conan-2.2.3/conans/client/conf/config_installer.py` & `conan-2.3.0/conans/client/conf/config_installer.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 class _ConanIgnoreMatcher:
     def __init__(self, conanignore_path, ignore=None):
         conanignore_path = os.path.abspath(conanignore_path)
         self._ignored_entries = {".conanignore"}
         if os.path.exists(conanignore_path):
             with open(conanignore_path, 'r') as conanignore:
                 for line in conanignore:
-                    line_content = line.strip()
-                    if line_content != "":
+                    line_content = line.split("#", maxsplit=1)[0].strip()
+                    if line_content:
                         self._ignored_entries.add(line_content)
         if ignore:
             self._ignored_entries.update(ignore)
 
     def matches(self, path):
         for ignore_entry in self._ignored_entries:
             if fnmatch.fnmatch(path, ignore_entry):
```

### Comparing `conan-2.2.3/conans/client/conf/detect.py` & `conan-2.3.0/conans/client/conf/detect.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/conf/detect_vs.py` & `conan-2.3.0/conans/client/conf/detect_vs.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/conf/required_version.py` & `conan-2.3.0/conans/client/conf/required_version.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/downloaders/caching_file_downloader.py` & `conan-2.3.0/conans/client/downloaders/caching_file_downloader.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/downloaders/download_cache.py` & `conan-2.3.0/conans/client/downloaders/download_cache.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/downloaders/file_downloader.py` & `conan-2.3.0/conans/client/downloaders/file_downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
                 raise NotFoundException("Not found: %s" % url)
             elif response.status_code == 403:
                 if auth is None or (hasattr(auth, "token") and auth.token is None):
                     # TODO: This is a bit weird, why this conversion? Need to investigate
                     raise AuthenticationException(response_to_str(response))
                 raise ForbiddenException(response_to_str(response))
             elif response.status_code == 401:
-                raise AuthenticationException()
+                raise AuthenticationException(response_to_str(response))
             raise ConanException("Error %d downloading file %s" % (response.status_code, url))
 
         def get_total_length():
             if range_start:
                 content_range = response.headers.get("Content-Range", "")
                 match = re.match(r"^bytes (\d+)-(\d+)/(\d+)", content_range)
                 if not match or range_start != int(match.group(1)):
```

### Comparing `conan-2.2.3/conans/client/generators/__init__.py` & `conan-2.3.0/conans/client/generators/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,27 +4,34 @@
 import importlib
 
 from conan.internal.cache.home_paths import HomePaths
 from conans.client.subsystems import deduce_subsystem, subsystem_path
 from conans.errors import ConanException, conanfile_exception_formatter
 from conans.util.files import save, mkdir, chdir
 
-_generators = {"CMakeToolchain": "conan.tools.cmake", "CMakeDeps": "conan.tools.cmake",
+_generators = {"CMakeToolchain": "conan.tools.cmake",
+               "CMakeDeps": "conan.tools.cmake",
                "MesonToolchain": "conan.tools.meson",
-               "MSBuildDeps": "conan.tools.microsoft", "MSBuildToolchain": "conan.tools.microsoft",
-               "NMakeToolchain": "conan.tools.microsoft", "NMakeDeps": "conan.tools.microsoft",
+               "MSBuildDeps": "conan.tools.microsoft",
+               "MSBuildToolchain": "conan.tools.microsoft",
+               "NMakeToolchain": "conan.tools.microsoft",
+               "NMakeDeps": "conan.tools.microsoft",
                "VCVars": "conan.tools.microsoft",
                "QbsProfile": "conan.tools.qbs.qbsprofile",
                "VirtualRunEnv": "conan.tools.env.virtualrunenv",
                "VirtualBuildEnv": "conan.tools.env.virtualbuildenv",
-               "AutotoolsDeps": "conan.tools.gnu", "AutotoolsToolchain": "conan.tools.gnu",
+               "AutotoolsDeps": "conan.tools.gnu",
+               "AutotoolsToolchain": "conan.tools.gnu",
+               "GnuToolchain": "conan.tools.gnu",
                "PkgConfigDeps": "conan.tools.gnu",
-               "BazelDeps": "conan.tools.google", "BazelToolchain": "conan.tools.google",
+               "BazelDeps": "conan.tools.google",
+               "BazelToolchain": "conan.tools.google",
                "IntelCC": "conan.tools.intel",
-               "XcodeDeps": "conan.tools.apple", "XcodeToolchain": "conan.tools.apple",
+               "XcodeDeps": "conan.tools.apple",
+               "XcodeToolchain": "conan.tools.apple",
                "PremakeDeps": "conan.tools.premake",
                "MakeDeps": "conan.tools.gnu",
                "SConsDeps": "conan.tools.scons"
                }
 
 
 def _get_generator_class(generator_name):
```

### Comparing `conan-2.2.3/conans/client/graph/build_mode.py` & `conan-2.3.0/conans/client/graph/build_mode.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/graph/compatibility.py` & `conan-2.3.0/conans/client/graph/compatibility.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/graph/compute_pid.py` & `conan-2.3.0/conans/client/graph/compute_pid.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,19 +53,20 @@
                                python_requires=python_requires,
                                conf=conanfile.conf.copy_conaninfo_conf(),
                                config_version=config_version.copy() if config_version else None)
     conanfile.original_info = conanfile.info.clone()
 
     if hasattr(conanfile, "validate_build"):
         with conanfile_exception_formatter(conanfile, "validate_build"):
-            try:
-                conanfile.validate_build()
-            except ConanInvalidConfiguration as e:
-                # This 'cant_build' will be ignored if we don't have to build the node.
-                node.cant_build = str(e)
+            with conanfile_remove_attr(conanfile, ['cpp_info'], "validate_build"):
+                try:
+                    conanfile.validate_build()
+                except ConanInvalidConfiguration as e:
+                    # This 'cant_build' will be ignored if we don't have to build the node.
+                    node.cant_build = str(e)
 
     run_validate_package_id(conanfile)
 
     if conanfile.info.settings_target:
         # settings_target has beed added to conan package via package_id api
         conanfile.original_info.settings_target = conanfile.info.settings_target
```

### Comparing `conan-2.2.3/conans/client/graph/graph.py` & `conan-2.3.0/conans/client/graph/graph.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/graph/graph_binaries.py` & `conan-2.3.0/conans/client/graph/graph_binaries.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/graph/graph_builder.py` & `conan-2.3.0/conans/client/graph/graph_builder.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/graph/graph_error.py` & `conan-2.3.0/conans/client/graph/graph_error.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,27 +21,23 @@
                 "name": self.require.ref.name,
                 "branch1": {"src_id": self.base_previous.id, "src_ref": str(self.base_previous.ref),
                             "dst_id": dst_id, "require": self.prev_require.serialize()},
                 "branch2": {"src_id": self.node.id, "src_ref": str(self.node.ref),
                             "require": self.require.serialize()}}
 
     def __str__(self):
-        if self.node.ref is not None and self.base_previous.ref is not None:
-            return f"Version conflict: {self.node.ref}->{self.require.ref}, " \
-                   f"{self.base_previous.ref}->{self.prev_require.ref}."
-        else:
-            conflicting_node = self.node.ref or self.base_previous.ref
-            conflicting_node_msg = ""
-            if conflicting_node is not None:
-                conflicting_node_msg = f"\nConflict originates from {conflicting_node}\n"
-            return f"Version conflict: " \
-                   f"Conflict between {self.require.ref} and {self.prev_require.ref} in the graph." \
-                   f"{conflicting_node_msg}" \
-                   f"\nRun conan graph info with your recipe and add --format=html " \
-                   f"to inspect the graph errors in an easier to visualize way."
+        conflicting_node = self.node.ref or self.base_previous.ref
+        conflicting_node_msg = ""
+        if conflicting_node is not None:
+            conflicting_node_msg = f"\nConflict originates from {conflicting_node}\n"
+        return f"Version conflict: " \
+               f"Conflict between {self.require.ref} and {self.prev_require.ref} in the graph." \
+               f"{conflicting_node_msg}" \
+               f"\nRun 'conan graph info ... --format=html > graph.html' " \
+               f"and open 'graph.html' to inspect the conflict graphically."
 
 
 class GraphLoopError(GraphError):
 
     def __init__(self, node, require, ancestor):
         self.node = node
         self.require = require
```

### Comparing `conan-2.2.3/conans/client/graph/install_graph.py` & `conan-2.3.0/conans/client/graph/install_graph.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/graph/profile_node_definer.py` & `conan-2.3.0/conans/client/graph/profile_node_definer.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,16 +22,21 @@
     # build(gcc) -(r)-> build(openssl/zlib) => settings_host=profile_build, settings_target=None
     # build(gcc) -(br)-> build(gcc) => settings_host=profile_build, settings_target=profile_build
     # profile host
     settings_host = _per_package_settings(conanfile, profile_host, ref)
     settings_build = _per_package_settings(conanfile, profile_build, ref)
     if is_build_require or base_context == CONTEXT_BUILD:
         _initialize_conanfile(conanfile, profile_build, settings_build.copy(), ref)
+        conanfile.buildenv_build = None
+        conanfile.conf_build = None
     else:
         _initialize_conanfile(conanfile, profile_host, settings_host, ref)
+        # Host profile with some build profile information
+        conanfile.buildenv_build = profile_build.buildenv.get_profile_env(ref, conanfile._conan_is_consumer)
+        conanfile.conf_build = profile_build.conf.get_conanfile_conf(ref, conanfile._conan_is_consumer)
     conanfile.settings_build = settings_build
     conanfile.settings_target = None
 
     if is_build_require:
         if base_context == CONTEXT_BUILD:
             conanfile.settings_target = settings_build.copy()
         else:
```

### Comparing `conan-2.2.3/conans/client/graph/provides.py` & `conan-2.3.0/conans/client/graph/provides.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/graph/proxy.py` & `conan-2.3.0/conans/client/graph/proxy.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/graph/python_requires.py` & `conan-2.3.0/conans/client/graph/python_requires.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/graph/range_resolver.py` & `conan-2.3.0/conans/client/graph/range_resolver.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/hook_manager.py` & `conan-2.3.0/conans/client/hook_manager.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/installer.py` & `conan-2.3.0/conans/client/installer.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/loader.py` & `conan-2.3.0/conans/client/loader.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/loader_txt.py` & `conan-2.3.0/conans/client/loader_txt.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/migrations.py` & `conan-2.3.0/conans/client/migrations.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/pkg_sign.py` & `conan-2.3.0/conans/client/pkg_sign.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/profile_loader.py` & `conan-2.3.0/conans/client/profile_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,15 +226,16 @@
     def get_profile(profile_text, base_profile=None):
         # Trying to strip comments might be problematic if things contain #
         doc = ConfigParser(profile_text, allowed_fields=["tool_requires",
                                                          "system_tools",  # DEPRECATED: platform_tool_requires
                                                          "platform_requires",
                                                          "platform_tool_requires", "settings",
                                                          "options", "conf", "buildenv", "runenv",
-                                                         "replace_requires", "replace_tool_requires"])
+                                                         "replace_requires", "replace_tool_requires",
+                                                         "runner"])
 
         # Parse doc sections into Conan model, Settings, Options, etc
         settings, package_settings = _ProfileValueParser._parse_settings(doc)
         options = Options.loads(doc.options) if doc.options else None
         tool_requires = _ProfileValueParser._parse_tool_requires(doc)
 
         doc_platform_requires = doc.platform_requires or ""
@@ -298,17 +299,30 @@
             base_profile.options.update_options(options)
         if conf is not None:
             base_profile.conf.update_conf_definition(conf)
         if buildenv is not None:
             base_profile.buildenv.update_profile_env(buildenv)
         if runenv is not None:
             base_profile.runenv.update_profile_env(runenv)
+
+
+        runner = _ProfileValueParser._parse_key_value(doc.runner) if doc.runner else {}
+        base_profile.runner.update(runner)
         return base_profile
 
     @staticmethod
+    def _parse_key_value(raw_info):
+        result = OrderedDict()
+        for br_line in raw_info.splitlines():
+            tokens = br_line.split("=", 1)
+            pattern, req_list = tokens
+            result[pattern.strip()] = req_list.strip()
+        return result
+
+    @staticmethod
     def _parse_tool_requires(doc):
         result = OrderedDict()
         if doc.tool_requires:
             # FIXME CHECKS OF DUPLICATED?
             for br_line in doc.tool_requires.splitlines():
                 tokens = br_line.split(":", 1)
                 if len(tokens) == 1:
```

### Comparing `conan-2.2.3/conans/client/remote_manager.py` & `conan-2.3.0/conans/client/remote_manager.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/rest/__init__.py` & `conan-2.3.0/conans/client/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/rest/auth_manager.py` & `conan-2.3.0/conans/client/rest/auth_manager.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/rest/client_routes.py` & `conan-2.3.0/conans/client/rest/client_routes.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/rest/conan_requester.py` & `conan-2.3.0/conans/client/rest/conan_requester.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,17 +28,14 @@
     def __init__(self, cache_folder):
         self._urls = {}
         if not cache_folder:
             return
         creds_path = os.path.join(cache_folder, "source_credentials.json")
         if not os.path.exists(creds_path):
             return
-        template = Template(load(creds_path))
-        content = template.render({"platform": platform, "os": os})
-        content = json.loads(content)
 
         def _get_auth(credentials):
             result = {}
             has_auth = False
             if "token" in credentials:
                 result["token"] = credentials["token"]
                 has_auth = True
@@ -48,18 +45,21 @@
                 has_auth = True
             if has_auth:
                 return result
             else:
                 raise ConanException(f"Unknown credentials method for '{credentials['url']}'")
 
         try:
+            template = Template(load(creds_path))
+            content = template.render({"platform": platform, "os": os})
+            content = json.loads(content)
             self._urls = {credentials["url"]: _get_auth(credentials)
                           for credentials in content["credentials"]}
-        except KeyError as e:
-            raise ConanException(f"Authentication error, wrong source_credentials.json layout: {e}")
+        except Exception as e:
+            raise ConanException(f"Error loading 'source_credentials.json' {creds_path}: {repr(e)}")
 
     def add_auth(self, url, kwargs):
         for u, creds in self._urls.items():
             if url.startswith(u):
                 token = creds.get("token")
                 if token:
                     kwargs["headers"]["Authorization"] = f"Bearer {token}"
```

### Comparing `conan-2.2.3/conans/client/rest/file_uploader.py` & `conan-2.3.0/conans/client/rest/file_uploader.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/rest/remote_credentials.py` & `conan-2.3.0/conans/client/rest/remote_credentials.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,21 +13,24 @@
 class RemoteCredentials:
     def __init__(self, cache_folder, global_conf):
         self._global_conf = global_conf
         self._urls = {}
         creds_path = os.path.join(cache_folder, "credentials.json")
         if not os.path.exists(creds_path):
             return
-        template = Template(load(creds_path))
-        content = template.render({"platform": platform, "os": os})
-        content = json.loads(content)
+        try:
+            template = Template(load(creds_path))
+            content = template.render({"platform": platform, "os": os})
+            content = json.loads(content)
 
-        self._urls = {credentials["remote"]: {"user": credentials["user"],
-                                              "password": credentials["password"]}
-                      for credentials in content["credentials"]}
+            self._urls = {credentials["remote"]: {"user": credentials["user"],
+                                                  "password": credentials["password"]}
+                          for credentials in content["credentials"]}
+        except Exception as e:
+            raise ConanException(f"Error loading 'credentials.json' {creds_path}: {repr(e)}")
 
     def auth(self, remote, user=None, password=None):
         if user is not None and password is not None:
             return user, password
 
         # First prioritize the cache "credentials.json" file
         creds = self._urls.get(remote)
```

### Comparing `conan-2.2.3/conans/client/rest/rest_client.py` & `conan-2.3.0/conans/client/rest/rest_client.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/rest/rest_client_common.py` & `conan-2.3.0/conans/client/rest/rest_client_common.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,19 +138,22 @@
         if user and password:
             # This can happen in "conan remote login" cmd. Instead of empty token, use HttpBasic
             auth = HTTPBasicAuth(user, password)
         else:
             auth = self.auth
         ret = self.requester.get(url, auth=auth, headers=self.custom_headers, verify=self.verify_ssl)
 
-        server_capabilities = ret.headers.get('X-Conan-Server-Capabilities', "")
+        server_capabilities = ret.headers.get('X-Conan-Server-Capabilities')
         if not server_capabilities and not ret.ok:
             # Old Artifactory might return 401/403 without capabilities, we don't want
             # to cache them #5687, so raise the exception and force authentication
             raise get_exception_from_error(ret.status_code)(response_to_str(ret))
+        if server_capabilities is None:
+            # Some servers returning 200-ok, even if not valid repo
+            raise ConanException(f"Remote {self.remote_url} doesn't seem like a valid Conan remote")
 
         return [cap.strip() for cap in server_capabilities.split(",") if cap]
 
     def get_json(self, url, data=None, headers=None):
         req_headers = self.custom_headers.copy()
         req_headers.update(headers or {})
         if data:  # POST request
```

### Comparing `conan-2.2.3/conans/client/rest/rest_client_v2.py` & `conan-2.3.0/conans/client/rest/rest_client_v2.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/rest_client_local_recipe_index.py` & `conan-2.3.0/conans/client/rest_client_local_recipe_index.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/source.py` & `conan-2.3.0/conans/client/source.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/store/localdb.py` & `conan-2.3.0/conans/client/store/localdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     def clean(self, remote_url=None):
         with self._connect() as connection:
             try:
                 cursor = connection.cursor()
                 query = "DELETE FROM %s" % REMOTES_USER_TABLE
                 if remote_url:
-                    query += ' WHERE remote_url="{}"'.format(remote_url)
+                    query += " WHERE remote_url='{}'".format(remote_url)
                 cursor.execute(query)
                 try:
                     # https://github.com/ghaering/pysqlite/issues/109
                     connection.isolation_level = None
                     cursor.execute('VACUUM')  # Make sure the DB is cleaned, drop doesn't do that
                 except OperationalError:
                     pass
@@ -70,15 +70,15 @@
             connection.close()
 
     def get_login(self, remote_url):
         """ Returns login credentials. This method is also in charge of expiring them. """
         with self._connect() as connection:
             try:
                 statement = connection.cursor()
-                statement.execute('select user, token, refresh_token from %s where remote_url="%s"'
+                statement.execute("select user, token, refresh_token from %s where remote_url='%s'"
                                   % (REMOTES_USER_TABLE, remote_url))
                 rs = statement.fetchone()
                 if not rs:
                     return None, None, None
                 name = rs[0]
                 token = self._decode(rs[1])
                 refresh_token = self._decode(rs[2])
```

### Comparing `conan-2.2.3/conans/client/subsystems.py` & `conan-2.3.0/conans/client/subsystems.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/client/userio.py` & `conan-2.3.0/conans/client/userio.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/conan_server.py` & `conan-2.3.0/conans/conan_server.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/errors.py` & `conan-2.3.0/conans/errors.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/migrations.py` & `conan-2.3.0/conans/migrations.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/model/build_info.py` & `conan-2.3.0/conans/model/build_info.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/model/conan_file.py` & `conan-2.3.0/conans/model/conan_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from conans.client.subsystems import command_env_wrapper
 from conans.errors import ConanException
 from conans.model.build_info import MockInfoProperty
 from conans.model.conf import Conf
 from conans.model.dependencies import ConanFileDependencies
 from conans.model.layout import Folders, Infos, Layouts
 from conans.model.options import Options
-
 from conans.model.requires import Requirements
 from conans.model.settings import Settings
 
 
 class ConanFile:
     """
     The base class for all package recipes
```

### Comparing `conan-2.2.3/conans/model/conanfile_interface.py` & `conan-2.3.0/conans/model/conanfile_interface.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/model/conf.py` & `conan-2.3.0/conans/model/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,14 +82,15 @@
     "tools.files.download:retry": "Number of retries in case of failure when downloading",
     "tools.files.download:retry_wait": "Seconds to wait between download attempts",
     "tools.files.download:verify": "If set, overrides recipes on whether to perform SSL verification for their downloaded files. Only recommended to be set while testing",
     "tools.graph:skip_binaries": "Allow the graph to skip binaries not needed in the current configuration (True by default)",
     "tools.gnu:make_program": "Indicate path to make program",
     "tools.gnu:define_libcxx11_abi": "Force definition of GLIBCXX_USE_CXX11_ABI=1 for libstdc++11",
     "tools.gnu:pkg_config": "Path to pkg-config executable used by PkgConfig build helper",
+    "tools.gnu:build_triplet": "Custom build triplet to pass to Autotools scripts",
     "tools.gnu:host_triplet": "Custom host triplet to pass to Autotools scripts",
     "tools.google.bazel:configs": "List of Bazel configurations to be used as 'bazel build --config=config1 ...'",
     "tools.google.bazel:bazelrc_path": "List of paths to bazelrc files to be used as 'bazel --bazelrc=rcpath1 ... build'",
     "tools.meson.mesontoolchain:backend": "Any Meson backend: ninja, vs, vs2010, vs2012, vs2013, vs2015, vs2017, vs2019, xcode",
     "tools.meson.mesontoolchain:extra_machine_files": "List of paths for any additional native/cross file references to be appended to the existing Conan ones",
     "tools.microsoft:winsdk_version": "Use this winsdk_version in vcvars",
     "tools.microsoft.msbuild:vs_version": "Defines the IDE version (15, 16, 17) when using the msvc compiler. Necessary if compiler.version specifies a toolset that is not the IDE default",
@@ -108,15 +109,15 @@
     "tools.system.package_manager:sudo_askpass": "Use the '-A' argument if using sudo in Linux to invoke the system package manager (False by default)",
     "tools.apple:sdk_path": "Path to the SDK to be used",
     "tools.apple:enable_bitcode": "(boolean) Enable/Disable Bitcode Apple Clang flags",
     "tools.apple:enable_arc": "(boolean) Enable/Disable ARC Apple Clang flags",
     "tools.apple:enable_visibility": "(boolean) Enable/Disable Visibility Apple Clang flags",
     "tools.env.virtualenv:powershell": "If it is set to True it will generate powershell launchers if os=Windows",
     # Compilers/Flags configurations
-    "tools.build:compiler_executables": "Defines a Python dict-like with the compilers path to be used. Allowed keys {'c', 'cpp', 'cuda', 'objc', 'objcxx', 'rc', 'fortran', 'asm', 'hip', 'ispc'}",
+    "tools.build:compiler_executables": "Defines a Python dict-like with the compilers path to be used. Allowed keys {'c', 'cpp', 'cuda', 'objc', 'objcxx', 'rc', 'fortran', 'asm', 'hip', 'ispc', 'ld', 'ar'}",
     "tools.build:cxxflags": "List of extra CXX flags used by different toolchains like CMakeToolchain, AutotoolsToolchain and MesonToolchain",
     "tools.build:cflags": "List of extra C flags used by different toolchains like CMakeToolchain, AutotoolsToolchain and MesonToolchain",
     "tools.build:defines": "List of extra definition flags used by different toolchains like CMakeToolchain and AutotoolsToolchain",
     "tools.build:sharedlinkflags": "List of extra flags used by CMakeToolchain for CMAKE_SHARED_LINKER_FLAGS_INIT variable",
     "tools.build:exelinkflags": "List of extra flags used by CMakeToolchain for CMAKE_EXE_LINKER_FLAGS_INIT variable",
     "tools.build:linker_scripts": "List of linker script files to pass to the linker used by different toolchains like CMakeToolchain, AutotoolsToolchain, and MesonToolchain",
     # Package ID composition
```

### Comparing `conan-2.2.3/conans/model/dependencies.py` & `conan-2.3.0/conans/model/dependencies.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,11 +161,13 @@
         return self.filter({"build": True})
 
 
 def get_transitive_requires(consumer, dependency):
     """ the transitive requires that we need are the consumer ones, not the current dependencey
     ones, so we get the current ones, then look for them in the consumer, and return those
     """
-    pkg_deps = dependency.dependencies.filter({"direct": True})
+    # The build dependencies cannot be transitive in generators like CMakeDeps,
+    # even if users make them visible
+    pkg_deps = dependency.dependencies.filter({"direct": True, "build": False})
     result = consumer.dependencies.transitive_requires(pkg_deps)
     result = result.filter({"skip": False})
     return result
```

### Comparing `conan-2.2.3/conans/model/graph_lock.py` & `conan-2.3.0/conans/model/graph_lock.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/model/info.py` & `conan-2.3.0/conans/model/info.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/model/layout.py` & `conan-2.3.0/conans/model/layout.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/model/manifest.py` & `conan-2.3.0/conans/model/manifest.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/model/options.py` & `conan-2.3.0/conans/model/options.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/model/package_ref.py` & `conan-2.3.0/conans/model/package_ref.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/model/pkg_type.py` & `conan-2.3.0/conans/model/pkg_type.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/model/profile.py` & `conan-2.3.0/conans/model/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         self.replace_requires = {}
         self.replace_tool_requires = {}
         self.platform_tool_requires = []
         self.platform_requires = []
         self.conf = ConfDefinition()
         self.buildenv = ProfileEnvironment()
         self.runenv = ProfileEnvironment()
+        self.runner = {}
 
         # Cached processed values
         self.processed_settings = None  # Settings with values, and smart completion
         self._package_settings_values = None
 
     def __repr__(self):
         return self.dumps()
@@ -120,14 +121,15 @@
                 r = RecipeReference.loads(req) \
                      if not isinstance(req, RecipeReference) else req
                 existing[r.name] = req
             self.tool_requires[pattern] = list(existing.values())
 
         self.replace_requires.update(other.replace_requires)
         self.replace_tool_requires.update(other.replace_tool_requires)
+        self.runner.update(other.runner)
 
         current_platform_tool_requires = {r.name: r for r in self.platform_tool_requires}
         current_platform_tool_requires.update({r.name: r for r in other.platform_tool_requires})
         self.platform_tool_requires = list(current_platform_tool_requires.values())
         current_platform_requires = {r.name: r for r in self.platform_requires}
         current_platform_requires.update({r.name: r for r in other.platform_requires})
         self.platform_requires = list(current_platform_requires.values())
```

### Comparing `conan-2.2.3/conans/model/recipe_ref.py` & `conan-2.3.0/conans/model/recipe_ref.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,16 +145,16 @@
         if validation_pattern.match(str(self.version)) is None:
             raise ConanException(f"Invalid package version '{self.version}'")
         if self.user and validation_pattern.match(self.user) is None:
             raise ConanException(f"Invalid package user '{self.user}'")
         if self.channel and validation_pattern.match(self.channel) is None:
             raise ConanException(f"Invalid package channel '{self.channel}'")
 
-        # Warn if they use .+- in the name/user/channel, as it can be problematic for generators
-        pattern = re.compile(r'[.+-]')
+         # Warn if they use .+ in the name/user/channel, as it can be problematic for generators
+        pattern = re.compile(r'[.+]')
         if pattern.search(self.name):
             ConanOutput().warning(f"Name containing special chars is discouraged '{self.name}'")
         if self.user and pattern.search(self.user):
             ConanOutput().warning(f"User containing special chars is discouraged '{self.user}'")
         if self.channel and pattern.search(self.channel):
             ConanOutput().warning(f"Channel containing special chars is discouraged "
                                   f"'{self.channel}'")
```

### Comparing `conan-2.2.3/conans/model/requires.py` & `conan-2.3.0/conans/model/requires.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/model/rest_routes.py` & `conan-2.3.0/conans/model/rest_routes.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/model/settings.py` & `conan-2.3.0/conans/model/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,47 +14,52 @@
 def undefined_field(name, field, fields=None, value=None):
     value_str = " for '%s'" % value if value else ""
     result = ["'%s.%s' doesn't exist%s" % (name, field, value_str),
               "'%s' possible configurations are %s" % (name, fields or "none")]
     return ConanException("\n".join(result))
 
 
-class SettingsItem(object):
+class SettingsItem:
     """ represents a setting value and its child info, which could be:
     - A range of valid values: [Debug, Release] (for settings.compiler.runtime of VS)
     - List [None, "ANY"] to accept None or any value
     - A dict {subsetting: definition}, e.g. {version: [], runtime: []} for VS
     """
-    def __init__(self, definition, name):
+    def __init__(self, definition, name, value):
+        self._definition = definition  # range of possible values
         self._name = name  # settings.compiler
-        self._value = None  # gcc
+        self._value = value  # gcc
+
+    @staticmethod
+    def new(definition, name):
+        if definition is None:
+            raise ConanException(f"Definition of settings.yml '{name}' cannot be null")
         if isinstance(definition, dict):
-            self._definition = {}
+            parsed_definitions = {}
             # recursive
             for k, v in definition.items():
                 # None string from yaml definition maps to python None, means not-defined value
                 k = str(k) if k is not None else None
-                self._definition[k] = Settings(v, name, k)
+                parsed_definitions[k] = Settings(v, name, k)
         else:
             # list or tuple of possible values, it can include "ANY"
-            self._definition = [str(v) if v is not None else None for v in definition]
+            parsed_definitions = [str(v) if v is not None else None for v in definition]
+        return SettingsItem(parsed_definitions, name, None)
 
     def __contains__(self, value):
         return value in (self._value or "")
 
     def copy(self):
         """ deepcopy, recursive
         """
-        result = SettingsItem({}, name=self._name)
-        result._value = self._value
         if not isinstance(self._definition, dict):
-            result._definition = self._definition  # Not necessary to copy this, not mutable
+            definition = self._definition  # Not necessary to copy this, not mutable
         else:
-            result._definition = {k: v.copy() for k, v in self._definition.items()}
-        return result
+            definition = {k: v.copy() for k, v in self._definition.items()}
+        return SettingsItem(definition, self._name, self._value)
 
     def copy_conaninfo_settings(self):
         """ deepcopy, recursive
         This function adds "ANY" to lists, to allow the ``package_id()`` method to modify some of
         values, but not all, just the "final" values without subsettings.
         We cannot let usres manipulate to random strings
         things that contain subsettings like ``compiler``, because that would leave the thing
@@ -62,23 +67,20 @@
         anymore. So with this change the options are:
         - If you need more "binary-compatible" descriptions of a compiler, lets say like
         "gcc_or_clang", then you need to add that string to settings.yml. And add the subsettings
         that you want for it.
         - Settings that are "final" (lists), like build_type, or arch or compiler.version they
         can get any value without issues.
         """
-        result = SettingsItem({}, name=self._name)
-        result._value = self._value
         if not isinstance(self._definition, dict):
-            result._definition = self._definition[:] + ["ANY"]
+            definition = self._definition[:] + ["ANY"]
         else:
-            result._definition = {k: v.copy_conaninfo_settings()
-                                  for k, v in self._definition.items()}
-            result._definition["ANY"] = Settings()
-        return result
+            definition = {k: v.copy_conaninfo_settings() for k, v in self._definition.items()}
+            definition["ANY"] = Settings()
+        return SettingsItem(definition, self._name, self._value)
 
     def __bool__(self):
         if not self._value:
             return False
         return self._value.lower() not in ["false", "none", "0", "off"]
 
     def __str__(self):
@@ -184,31 +186,30 @@
             raise ConanException("settings.yml: null setting can't have subsettings")
         definition = definition or {}
         if not isinstance(definition, dict):
             val = "" if parent_value == "settings" else f"={parent_value}"
             raise ConanException(f"Invalid settings.yml format: '{name}{val}' is not a dictionary")
         self._name = name  # settings, settings.compiler
         self._parent_value = parent_value  # gcc, x86
-        self._data = {k: SettingsItem(v, "%s.%s" % (name, k))
-                      for k, v in definition.items()}
+        self._data = {k: SettingsItem.new(v, f"{name}.{k}") for k, v in definition.items()}
         self._frozen = False
 
     def serialize(self):
         """
         Returns a dictionary with all the settings (and sub-settings) as ``field: value``
         """
         ret = []
         for _, s in self._data.items():
             # TODO: Refactor it and use s.serialize()
             ret.extend(s.values_list)
         return dict(ret)
 
     def get_safe(self, name, default=None):
         """
-        Get the setting value avoiding
+        Get the setting value avoiding throwing if it does not exist or has been removed
         :param name:
         :param default:
         :return:
         """
         try:
             tmp = self
             for prop in name.split("."):
@@ -227,15 +228,18 @@
         if "." in name:
             setting, remainder = name.split(".", 1)  # setting=compiler, remainder = cppstd
             try:
                 self._data[setting].rm_safe(remainder)  # call rm_safe("cppstd") for the "compiler"
             except KeyError:
                 pass
         else:
-            self._data.pop(name, None)
+            if name == "*":
+                self.clear()
+            else:
+                self._data.pop(name, None)
 
     def copy(self):
         """ deepcopy, recursive
         """
         result = Settings({}, name=self._name, parent_value=self._parent_value)
         result._data = {k: v.copy() for k, v in self._data.items()}
         return result
```

### Comparing `conan-2.2.3/conans/model/version.py` & `conan-2.3.0/conans/model/version.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/model/version_range.py` & `conan-2.3.0/conans/model/version_range.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,14 +84,16 @@
             index = 0
         else:
             index = 1
         if operator in (">", "<"):
             if expression[1] == "=":
                 operator += "="
                 index = 2
+        elif expression[1] == "=":
+            raise ConanException(f"Invalid version range operator '{operator}=' in {expression}, you should probably use {operator} instead.")
         version = expression[index:]
         if version == "":
             raise ConanException(f'Error parsing version range "{expression}"')
         if operator == "~":  # tilde minor
             if "-" not in version:
                 version += "-"
             v = Version(version)
@@ -107,15 +109,15 @@
                 return len(main)
 
             initial_index = first_non_zero(v.main)
             return [_Condition(">=", v), _Condition("<", v.upper_bound(initial_index))]
         else:
             return [_Condition(operator, Version(version))]
 
-    def _valid(self, version, conf_resolve_prepreleases):
+    def valid(self, version, conf_resolve_prepreleases):
         if version.pre:
             # Follow the expression desires only if core.version_ranges:resolve_prereleases is None,
             # else force to the conf's value
             if conf_resolve_prepreleases is None:
                 if not self.prerelease:
                     return False
             elif conf_resolve_prepreleases is False:
@@ -176,15 +178,15 @@
         :param resolve_prerelease: If ``True``, ensure prereleases can be resolved in this range
         If ``False``, prerelases can NOT be resolved in this range
         If ``None``, prereleases are resolved only if this version range expression says so
         :return: Whether the version is inside the range
         """
         assert isinstance(version, Version), type(version)
         for condition_set in self.condition_sets:
-            if condition_set._valid(version, resolve_prerelease):
+            if condition_set.valid(version, resolve_prerelease):
                 return True
         return False
 
     def intersection(self, other):
         conditions = []
 
         def _calculate_limits(operator, lhs, rhs):
```

### Comparing `conan-2.2.3/conans/paths/__init__.py` & `conan-2.3.0/conans/paths/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # coding=utf-8
 import os
 import platform
 from pathlib import Path
 
+from conans.errors import ConanException
+
 if platform.system() == "Windows":
     from conans.util.windows import conan_expand_user
 else:
     conan_expand_user = os.path.expanduser
 
 DEFAULT_CONAN_HOME = ".conan2"
 
@@ -42,15 +44,15 @@
     user_home = _user_home_from_conanrc_file() or os.getenv("CONAN_HOME")
     if user_home is None:
         # the default, in the user home
         user_home = os.path.join(conan_expand_user("~"), DEFAULT_CONAN_HOME)
     else:  # Do an expansion, just in case the user is using ~/something/here
         user_home = conan_expand_user(user_home)
     if not os.path.isabs(user_home):
-        raise Exception("Invalid CONAN_HOME value '%s', "
+        raise ConanException("Invalid CONAN_HOME value '%s', "
                         "please specify an absolute or path starting with ~/ "
                         "(relative to user home)" % user_home)
     return user_home
 
 
 # Files
 CONANFILE = 'conanfile.py'
```

### Comparing `conan-2.2.3/conans/search/query_parse.py` & `conan-2.3.0/conans/search/query_parse.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/search/search.py` & `conan-2.3.0/conans/search/search.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/test/assets/autotools.py` & `conan-2.3.0/conans/test/assets/autotools.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/test/assets/cmake.py` & `conan-2.3.0/conans/test/assets/cmake.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/test/assets/genconanfile.py` & `conan-2.3.0/conans/test/assets/genconanfile.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/test/assets/pkg_cmake.py` & `conan-2.3.0/conans/test/assets/pkg_cmake.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/test/assets/sources.py` & `conan-2.3.0/conans/test/assets/sources.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/test/assets/visual_project_files.py` & `conan-2.3.0/conans/test/assets/visual_project_files.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/test/conftest.py` & `conan-2.3.0/conans/test/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 
 tools_locations = {
     "clang": {"disabled": True},
     'visual_studio': {"default": "15",
                       "15": {},
                       "16": {"disabled": True},
-                      "17": {"disabled": True}},
+                      "17": {}},
     'pkg_config': {
         "exe": "pkg-config",
         "default": "0.28",
         "0.28": {
             "path": {
                 # Using chocolatey in Windows -> choco install pkgconfiglite --version 0.28
                 'Windows': "C:/ProgramData/chocolatey/lib/pkgconfiglite/tools/pkg-config-lite-0.28-1/bin",
```

### Comparing `conan-2.2.3/conans/test/utils/artifactory.py` & `conan-2.3.0/conans/test/utils/artifactory.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/test/utils/file_server.py` & `conan-2.3.0/conans/test/utils/file_server.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             return bottle.HTTPError(403, "Access denied.")
 
         @app.route("/basic-auth/<file>", method=["GET"])
         def get_user_passwd(file):
             auth = bottle.request.auth
             if auth is not None:
                 if auth != ("user", "password"):
-                    return bottle.HTTPError(401, "Not authorized")
+                    return bottle.HTTPError(401, "Bad credentials")
                 return bottle.static_file(file, store)
 
             auth = bottle.request.headers.get("Authorization")
             if auth is None or auth != "Bearer password":
                 return bottle.HTTPError(401, "Not authorized")
             return bottle.static_file(file, store)
```

### Comparing `conan-2.2.3/conans/test/utils/mocks.py` & `conan-2.3.0/conans/test/utils/mocks.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/test/utils/profiles.py` & `conan-2.3.0/conans/test/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/test/utils/scm.py` & `conan-2.3.0/conans/test/utils/scm.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/test/utils/server_launcher.py` & `conan-2.3.0/conans/test/utils/server_launcher.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/test/utils/test_files.py` & `conan-2.3.0/conans/test/utils/test_files.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/test/utils/tools.py` & `conan-2.3.0/conans/test/utils/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -361,18 +361,20 @@
     sys.stdin = target
     try:
         yield
     finally:
         sys.stdin = original_stdin
 
 
-class TestClient(object):
+class TestClient:
     """ Test wrap of the conans application to launch tests in the same way as
     in command line
     """
+    # Preventing Pytest collects any tests from here
+    __test__ = False
 
     def __init__(self, cache_folder=None, current_folder=None, servers=None, inputs=None,
                  requester_class=None, path_with_spaces=True,
                  default_server_user=None, light=False, custom_commands_folder=None):
         """
         current_folder: Current execution folder
         servers: dict of {remote_name: TestServer}
```

### Comparing `conan-2.2.3/conans/util/config_parser.py` & `conan-2.3.0/conans/util/config_parser.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/util/dates.py` & `conan-2.3.0/conans/util/dates.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/util/encrypt.py` & `conan-2.3.0/conans/util/encrypt.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/util/env.py` & `conan-2.3.0/conans/util/env.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/util/files.py` & `conan-2.3.0/conans/util/files.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/util/locks.py` & `conan-2.3.0/conans/util/locks.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/util/runners.py` & `conan-2.3.0/conans/util/runners.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/util/sha.py` & `conan-2.3.0/conans/util/sha.py`

 * *Files identical despite different names*

### Comparing `conan-2.2.3/conans/util/windows.py` & `conan-2.3.0/conans/util/windows.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,23 +5,22 @@
     """ wrapper to the original expanduser function, to workaround python returning
     verbatim %USERPROFILE% when some other app (git for windows) sets HOME envvar
     """
     path = str(path)
     if path[:1] != '~':
         return path
     # In win these variables should exist and point to user directory, which
-    # must exist. Using context to avoid permanent modification of os.environ
-    old_env = dict(os.environ)
+    # must exist.
     try:
         home = os.environ.get("HOME")
         # Problematic cases of wrong HOME variable
         # - HOME = %USERPROFILE% verbatim, as messed by some other tools
         # - MSYS console, that defines a different user home in /c/mingw/msys/users/xxx
         # In these cases, it is safe to remove it and rely on USERPROFILE directly
         if home and (not os.path.exists(home) or
                      (os.getenv("MSYSTEM") and os.getenv("USERPROFILE"))):
             del os.environ["HOME"]
         result = os.path.expanduser(path)
     finally:
-        os.environ.clear()
-        os.environ.update(old_env)
+        if home is not None:
+            os.environ["HOME"] = home
     return result
```

### Comparing `conan-2.2.3/setup.py` & `conan-2.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     with open(path.join(this_directory, 'README.md')) as f:
         long_description = f.read()
     return long_description
 
 
 project_requirements = get_requires("conans/requirements.txt")
 dev_requirements = get_requires("conans/requirements_dev.txt")
+runners_requirements = get_requires("conans/requirements_runner.txt")
 excluded_server_packages = ["conans.server*"]
 exclude = excluded_test_packages + excluded_server_packages
 
 
 setup(
     name='conan',
     python_requires='>=3.6',
@@ -108,18 +109,19 @@
     # requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
     install_requires=project_requirements,
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). You can install these using the following syntax,
     # for example:
-    # $ pip install -e .[dev,test]
+    # $ pip install -e .[dev,test,runners]
     extras_require={
         'dev': dev_requirements,
         'test': dev_requirements,
+        'runners': runners_requirements
     },
 
     # If there are data files included in your packages that need to be
     # installed, specify them here.  If using Python 2.6 or less, then these
     # have to be included in MANIFEST.in as well.
     package_data={
         'conans': ['*.txt'],
```

