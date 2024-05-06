# Comparing `tmp/xnippy-0.1.0.tar.gz` & `tmp/xnippy-0.1.1.tar.gz`

## Comparing `xnippy-0.1.0.tar` & `xnippy-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,52 @@
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 xnippy-0.1.0/tests/01_config_test.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 xnippy-0.1.0/tests/config.yaml
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 xnippy-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 xnippy-0.1.0/xnippy/__init__.py
--rw-r--r--   0        0        0     9098 2020-02-02 00:00:00.000000 xnippy-0.1.0/xnippy/manager.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 xnippy-0.1.0/xnippy/types.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 xnippy-0.1.0/xnippy/fetcher/__init__.py
--rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 xnippy-0.1.0/xnippy/fetcher/base.py
--rw-r--r--   0        0        0     8310 2020-02-02 00:00:00.000000 xnippy-0.1.0/xnippy/fetcher/snippets.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 xnippy-0.1.0/xnippy/formatter/__init__.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 xnippy-0.1.0/xnippy/formatter/bytes.py
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 xnippy-0.1.0/xnippy/formatter/datetime.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 xnippy-0.1.0/xnippy/formatter/io.py
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 xnippy-0.1.0/xnippy/formatter/path.py
--rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 xnippy-0.1.0/xnippy/formatter/recipe.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 xnippy-0.1.0/xnippy/formatter/string.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 xnippy-0.1.0/xnippy/module/__init__.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 xnippy-0.1.0/xnippy/module/commander.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 xnippy-0.1.0/xnippy/module/errors.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 xnippy-0.1.0/xnippy/module/installer.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 xnippy-0.1.0/xnippy/module/loader.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 xnippy-0.1.0/xnippy/snippet/__init__.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 xnippy-0.1.0/xnippy/snippet/base.py
--rw-r--r--   0        0        0     9119 2020-02-02 00:00:00.000000 xnippy-0.1.0/xnippy/snippet/plugin.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 xnippy-0.1.0/xnippy/snippet/preset.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 xnippy-0.1.0/xnippy/snippet/recipe.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 xnippy-0.1.0/xnippy/snippet/spec.py
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 xnippy-0.1.0/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 xnippy-0.1.0/LICENSE
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 xnippy-0.1.0/README.md
--rwxr-xr-x   0        0        0     1204 2020-02-02 00:00:00.000000 xnippy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 xnippy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 xnippy-0.1.1/pytest.ini
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 xnippy-0.1.1/examples/example_config.yaml
+-rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 xnippy-0.1.1/examples/docs/PLUGIN.md
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 xnippy-0.1.1/examples/docs/PRESET.md
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xnippy-0.1.1/examples/docs/PROJECT_CONFIG.md
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 xnippy-0.1.1/examples/docs/RECIPE.md
+-rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 xnippy-0.1.1/examples/docs/SPEC.md
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 xnippy-0.1.1/examples/plugin/plugin_example/manifest.yaml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 xnippy-0.1.1/examples/plugin/plugin_example/plugin_example.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 xnippy-0.1.1/examples/plugin/plugin_example/utils.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 xnippy-0.1.1/examples/plugin/plugin_example/preset/preset_snippet.yaml
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 xnippy-0.1.1/examples/plugin/plugin_example/recipe/recipe_snippet.yaml
+-rw-r--r--   0        0        0     1630 2020-02-02 00:00:00.000000 xnippy-0.1.1/examples/plugin/plugin_example/spec/spec_snippet.yaml
+-rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 xnippy-0.1.1/tests/01_main_test.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 xnippy-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/__init__.py
+-rw-r--r--   0        0        0    10197 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/main.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/types.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/fetcher/__init__.py
+-rw-r--r--   0        0        0     8219 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/fetcher/base.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/fetcher/plugins.py
+-rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/fetcher/snippets.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/formatter/__init__.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/formatter/bytes.py
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/formatter/datetime.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/formatter/io.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/formatter/path.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/formatter/string.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/module/__init__.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/module/commander.py
+-rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/module/installer.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/module/loader.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/parser/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/parser/classifier.py
+-rw-r--r--   0        0        0     4729 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/parser/recipe.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/raiser/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/raiser/error.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/raiser/except.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/raiser/types.py
+-rw-r--r--   0        0        0     3025 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/raiser/warn.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/snippet/__init__.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/snippet/base.py
+-rw-r--r--   0        0        0    11183 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/snippet/plugin.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/snippet/preset.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/snippet/recipe.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/snippet/spec.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 xnippy-0.1.1/xnippy/yaml/config.yaml
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 xnippy-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 xnippy-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 xnippy-0.1.1/README.md
+-rwxr-xr-x   0        0        0     1312 2020-02-02 00:00:00.000000 xnippy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 xnippy-0.1.1/PKG-INFO
```

### Comparing `xnippy-0.1.0/xnippy/manager.py` & `xnippy-0.1.1/xnippy/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,69 +4,107 @@
 allowing configurations to be handled internally without file creation unless specifically 
 requested by the user through CLI to create them in the home folder.
 """
 
 from __future__ import annotations
 import yaml
 import shutil
-import warnings
 from packaging import version
 from pathlib import Path
-from .fetcher import SnippetsFetcher
+from .fetcher import PlugInFetcher
 from typing import TYPE_CHECKING
 from .formatter import PathFormatter
 from .formatter import IOFormatter
+from .raiser import WarnRaiser
 if TYPE_CHECKING:
-    from .types import SnippetMode, StorageMode, SnippetPath, SnippetType
-    from .types import SnippetsFetcherType, VersionType
-    from typing import List, Dict, Union, Optional
+    from .types import SnippetMode, StorageMode, SnippetPath, PlugInSnippetType
+    from .types import PlugInFetcherType, VersionType
+    from typing import List, Union, Optional
 
 class Manager(PathFormatter):
     """Manages the configuration settings for the application.
 
     This class ensures the existence of the configuration directory, loads or creates the configuration file,
     sets configuration values, and retrieves configuration values. It operates both globally and locally
     depending on the user's choice and the operational context.
     """ 
     config: dict = {}
     _home_dir: 'Path'
     _default_dir: 'Path'
     _local_dir: 'Path'
     _global_dir: 'Path'
+    _config_dir: 'Path'
     _fname: str
     _package_name: str
     _package_version: VersionType
-    _fetchers: Dict[SnippetsFetcherType] = {}
+    _fetcher: PlugInFetcherType
     _compatible_snippets: List[SnippetMode] = ['plugin']
     
     def __init__(self, 
                  package_name: str, 
                  package_version: str, 
-                 package__file__: 'Path',
-                 config_filename: Optional[str] = None) -> None:
+                 package__file__: Union['Path', str],
+                 config_path: Optional[str] = None,
+                 config_filename: str = 'config.yaml') -> None:
         """Initializes the configuration manager.
 
         This constructor sets up paths for the home directory, global and local configuration directories,
         and configuration file. It ensures the configuration directory exists and loads or creates the
         configuration based on its presence.
 
         Args:
             tmpdir (Optional[Path]): Temporary directory for storing configurations, defaults to the home directory.
         """
         self._package_name = package_name
         self._home_dir = self._resolve('~')
-        self._default_dir = self._resolve(package__file__).parent
+        self._default_dir = self._resolve(package__file__).parent / config_path if config_path else self._resolve(package__file__).parent
         self._local_dir = self._resolve(Path.cwd() / f'.{self._package_name}')
         self._global_dir = self._resolve(self._home_dir / f'.{self._package_name}')
-        self._fname = config_filename or 'config.yaml'
+        self._fname = config_filename
         self._package_version = version.parse(package_version)
         self.reload()
 
+    ## Initiation step
+    def reload(self) -> None:
+        """Loads an existing configuration file or creates a new one if it does not exist, filling the 'config' dictionary with settings."""
+        self._set_config_dir()
+        config_file = self.config_dir / self._fname
+        if not config_file.exists() and self.config_dir == self._default_dir:
+            
+            comment = "Preparing default configuration. Use 'create_config' method to initialize."
+            WarnRaiser(self.reload).config_not_found(self.config_dir, comment=comment)
+            config_file = self._resolve(__file__).parent / 'yaml/config.yaml'
+        with open(config_file, 'r') as f:
+            self.config = yaml.safe_load(f)
+        self._reload_plugin_fetcher()
+        
+    def _set_config_dir(self):
+        if isinstance(self.config_created, list):
+            self._config_dir = self._local_dir
+        elif isinstance(self.config_created, str):
+            self._config_dir = self._local_dir if self.config_created == 'local' else self._global_dir
+        else:
+            self._config_dir = self._default_dir
+
+    def _reload_plugin_fetcher(self) -> None:
+        """Retrieves a configured SnippetsFetcher for the specified mode to handle fetching of snippets.
+
+        Args:
+            mode (str): The mode that determines which type of fetcher to return. Valid modes are 'plugin', 'preset', 'spec', and 'recipe'.
+
+        Returns:
+            SnippetsFetcher: A fetcher configured for fetching snippets of the specified type.
+        """
+        self._fetcher = PlugInFetcher(repos=self.config['plugin']['repo'],
+                                      package_name=self._package_name,
+                                      package_version=self._package_version,
+                                      path=self._check_dir())
+    
     @property
-    def created(self) -> Union[StorageMode, list[str], bool]:
+    def config_created(self) -> Union[StorageMode, list[str], bool]:
         """"Checks and returns the location where the configuration folder was created.
 
         Returns:
             Union[Literal['global', 'local'], list[str], bool]: Returns 'global' or 'local' if the config folder was created at that level,
             a list of locations if multiple exist, or False if no config folder is created.
         """
         created = [(f / self._fname).exists() for f in [self._global_dir, self._local_dir]]
@@ -77,133 +115,106 @@
     @property
     def config_dir(self) -> 'Path':
         """Determines and returns the appropriate configuration directory based on the existence and location of the config file.
 
         Returns:
             Path: Path to the configuration directory based on its existence and scope (global or local).
         """
-        if isinstance(self.created, list):
-            return self._local_dir
-        elif isinstance(self.created, str):
-            return self._local_dir if self.created == 'local' else self._global_dir
-        return self._default_dir
-
-    def reload(self) -> None:
-        """Loads an existing configuration file or creates a new one if it does not exist, filling the 'config' dictionary with settings."""
-        with open(self.config_dir / self._fname) as f:
-            self.config = yaml.safe_load(f)
-        self._reload_fetchers()
-    
-    def create(self, target: StorageMode = 'local', 
-               force: bool = False) -> bool:
-        """Creates a configuration file at the specified location.
+        return self._config_dir
+        
+    def create_config(self, target: StorageMode = 'local', 
+                       force: bool = False) -> bool:
+        """Creates a configuration file at the specified target location.
 
         Args:
-            target (Literal['local', 'global']): Target directory for creating the configuration file, defaults to 'local'.
-            force (bool): If True, overwrites the existing configuration file, defaults to False.
+            target (str): Specifies the target directory ('local' or 'global') for creating the configuration file. Defaults to 'local'.
+            force (bool): If set to True, the existing configuration file will be overwritten. Defaults to False.
 
         Returns:
-            bool: True if the file was created successfully, False otherwise.
+            bool: Returns True if the file was successfully created, otherwise False.
         """
-        if not self.config:
-            self.load()
         config_dir = self._local_dir if target == 'local' else self._global_dir
         config_dir.mkdir(exist_ok=True)
         config_file = config_dir / self._fname
         if config_file.exists():
             if not force:
-                self._warnings_exists()
+                WarnRaiser(self.create_config).config_exist_when_create()
                 return False
-        with open(config_dir / self._fname, 'w') as f:
+        with open(config_file, 'w') as f:
             yaml.safe_dump(self.config, f, sort_keys=False)
-
-    def remove(self, target: StorageMode, yes: bool = False):
+        self.reload()
+    
+    def delete_config(self, target: StorageMode, yes: bool = False):
         path = self._local_dir if target == 'local' else self._global_dir
+        removed = False
         if path.exists():
             if yes:
                 shutil.rmtree(path)
+                removed = True
             elif IOFormatter.yes_or_no(f'**Caution**: You are about to delete the entire configuration folder at [{path}].\n'
                                        'Are you sure you want to proceed?'):
                 shutil.rmtree(path)
-
-    def get_fetcher(self, mode: SnippetMode) -> SnippetsFetcherType:
-        """Returns the appropriate fetcher based on the mode.
-
-        Args:
-            mode (Literal['plugin', 'preset', 'spec', 'recipe']): The mode determining which type of fetcher to return.
-
-        Returns:
-            SnippetsFetcher: An instance of SnippetsFetcher configured for the specified mode.
-        """
-        return self._fetchers[mode]
-
-    def _get_snippet_fetcher(self, mode: SnippetMode) -> SnippetsFetcherType:
-        """Retrieves a configured SnippetsFetcher for the specified mode to handle fetching of snippets.
-
-        Args:
-            mode (Literal['plugin', 'preset', 'spec', 'recipe']): The specific category of snippets to fetch.
-
-        Returns:
-            SnippetsFetcher: A fetcher configured for fetching snippets of the specified type.
-        """
-        return SnippetsFetcher(repos=self.config['snippets']['repo'],
-                               mode=mode,
-                               path=self._check_dir(mode))
+                removed = True
+        if removed:
+            self.reload()
     
-    def _check_dir(self, type_: SnippetMode) -> SnippetPath:
+    def _check_dir(self) -> SnippetPath:
         """Checks and prepares the directory for the specified snippet type, ensuring it exists.
 
-        Args:
-            type_ (Literal['plugin', 'preset', 'spec', 'recipe']): The type of snippet for which the directory is checked.
-
         Returns:
             Tuple[Path, bool]: A tuple containing the path to the directory and a cache flag indicating
                                 if caching is necessary (True if so).
         """
-        path, cache = (self.config_dir / type_, False) if self.created else (None, True)
+        path, cache = (self.config_dir / 'plugin', False) if self.config_created else (None, True)
         if path and not path.exists():
             path.mkdir()
         return path, cache
-    
-    def _reload_fetchers(self):
-        for mode in self._compatible_snippets:
-            self._fetchers[mode] = self._get_snippet_fetcher(mode)
         
-    def avail(self, mode: SnippetMode) -> SnippetsFetcherType:
-        fetcher = self.get_fetcher(mode)
-        return {'remote': fetcher.remote,
-                'local': fetcher.local}
-    
-    def installed(self, mode: SnippetMode) -> SnippetsFetcherType:
-        return self.get_fetcher(mode).local
-    
-    def is_installed(self, 
-                     mode: SnippetMode, 
-                     snippet: SnippetType) -> bool:
-        return any(s.name == snippet.name for s in self.installed(mode))
-    
-    def download(self, 
-                 mode: SnippetMode, 
-                 snippet_name: str,
-                 snippet_version: str,
-                 destination: Optional[Union[Path, str]] = None):
-        """Download snippet by name from selected mode"""
-        if not destination and not self.config_dir.exists():
-            self._warnings_not_exists()
+    @property
+    def avail(self) -> List[PlugInSnippetType]:
+        """Check list of plugins not installed but available in remote repository"""
+        installed = [f'{p.name}=={str(p.version)}' for p in self.installed]
+        return [p for p in self._fetcher.remote if f'{p.name}=={str(p.version)}' not in installed]
+    
+    @property
+    def installed(self) -> List[PlugInSnippetType]:
+        """Check list of installed plugins."""
+        return self._fetcher.local
+    
+    def get(self, plugin_name: str, 
+            plugin_version: Optional[str] = None, 
+            remote: bool = False) -> Union[PlugInSnippetType, List[PlugInSnippetType], None]:
+        """Return PlugInSnippet object."""
+        if plugin_version:
+            keyword = f'{plugin_name}=={plugin_version}'
+            if remote:
+                get_from = {f'{s.name}=={str(s.version)}':s for s in self.avail}
+            else:
+                get_from = {f'{s.name}=={str(s.version)}':s for s in self.installed}
+            if keyword in get_from.keys():
+                return get_from[keyword]
             return None
+        keyword = plugin_name
+        return [s for s in self.installed if keyword == s.name]
+    
+    def is_installed(self, plugin_name: str, version: Optional[str] = None):
+        return True if self.get(plugin_name, version) else False
+    
+    def install(self, plugin_name: str, 
+                plugin_version: Optional[str] = None, 
+                yes: bool = False, target: StorageMode = 'local'):
+        if not self.config_created:
+            WarnRaiser(self.install).config_not_found(self.config_dir)
+            if yes or IOFormatter.yes_or_no(f"Do you want to proceed creating '{target}' configuration?"):
+                self.create_config(target=target)
         
-        destination = self._resolve(destination) if destination else (self.config_dir / mode)
-        destination.mkdir(exist_ok=True)
-        # check local
-        fetcher: SnippetsFetcherType = self.get_fetcher[mode]
-        print(f"++ Fetching avail {mode} snippets from remote repository...")
-        avail = [s for s in fetcher.remote]
-        
-    @staticmethod
-    def _warnings_exists():
-        warnings.warn("Config folder already exists, please use 'force' option if you want overwrite.",
-                      UserWarning)
-    
-    @staticmethod
-    def _warnings_not_exists():
-        warnings.warn("Config folder does not exist, please use 'create' option if you want create.",
-                      UserWarning)
+        plugin = self.get(plugin_name=plugin_name, plugin_version=plugin_version, remote=True)
+        plugin_dir, _ = self._check_dir()
+        plugin_name = f'{plugin_name}_{plugin_version}' if plugin_name else plugin_name
+        if (plugin_dir / plugin_name).exists():
+            WarnRaiser(self.install).file_exist()
+            if yes or IOFormatter.yes_or_no(f"Do you want to overwrite plugin '{target}' configuration?"):
+                plugin.download(dest=plugin_dir, force=yes)
+                return True
+            return False
+        plugin.download(dest=plugin_dir)
+        self.reload()
```

### Comparing `xnippy-0.1.0/xnippy/types.py` & `xnippy-0.1.1/xnippy/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,56 @@
-from typing import NewType, Type, Optional, Union
+from typing import Type, Optional, Union
 from typing import Literal, Tuple, List
 from pathlib import Path
-from .manager import Manager
-from .fetcher import SnippetsFetcher
+from .main import Manager
+from .fetcher import SnippetFetcher
+from .fetcher import PlugInFetcher
 from .fetcher.base import Fetcher
 from .snippet.base import Snippet
 from .snippet import PlugInSnippet
 from .snippet import PresetSnippet
 from .snippet import RecipeSnippet
 from .snippet import SpecSnippet
-from .formatter.recipe import Resource    
 from packaging.version import _Version as VersionType
 
+class Resource:
+    def to_dict(self):
+        return self.__dict__
+
 ResourceType = Type[Union[Resource, List[Resource]]]
 
-ConfigManagerType = Type[Manager]
+XnipyManagerType = Type[Manager]
 
 StorageMode = Literal['local', 'global']
 
 FetcherType = Type[Fetcher]
 
-SnippetsFetcherType = Type[SnippetsFetcher]
+SnippetsFetcherType = Type[SnippetFetcher]
+
+PlugInFetcherType = Type[PlugInFetcher]
 
 SnippetType = Type[Snippet]
 
-SnippetPath = NewType[
-    Tuple[Optional(Path), 
-          bool]
-    ]
+SnippetPath = Tuple[Optional[Path], bool]
 
 SnippetMode = Literal[
     'plugin', 'preset', 'spec', 'recipe'
     ]
 
 PlugInSnippetType = Type[PlugInSnippet]
 
 PresetSnippetType = Type[PresetSnippet]
 
 RecipeSnippetType = Type[RecipeSnippet]
 
 SpecSnippetType = Type[SpecSnippet]
 
 __all__ = [
-    'VersionType',
-    'ConfigManagerType', 'StorageMode',
-    'FetcherType', 'SnippetsFetcherType', 
-    'SnippetType', 'SnippetPath', 'SnippetMode', 'FileSnippetMode', 'ConfigSnippetMode',
-    'PlugInSnippetType', 'PresetSnippetType', 'RecipeSnippetType', 'SpecSnippetType', 'ConfigSnippetType'
+    'ResourceType', 'VersionType',
+    'XnipyManagerType', 'StorageMode',
+    'FetcherType', 'SnippetsFetcherType', 'PlugInFetcherType',
+    'SnippetType', 'SnippetPath', 'SnippetMode',
+    'PlugInSnippetType', 
+    'PresetSnippetType', 
+    'RecipeSnippetType', 
+    'SpecSnippetType',
     ]
```

### Comparing `xnippy-0.1.0/xnippy/fetcher/base.py` & `xnippy-0.1.1/xnippy/fetcher/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,36 +29,38 @@
     and download files as needed.
 
     Attributes:
         _auth (Union[List[Tuple[str, str]], Tuple[str, str]]): Authentication credentials for the repository.
         repos (dict): Configuration for the repositories to be accessed.
     """
     _auth: Union[List[Tuple[str, str]], Tuple[str, str]]
-    repos: dict
+    _repos: dict
     
     @staticmethod
     def is_connected():
         """Check if there is an internet connection available by pinging a known URL.
 
         Returns:
             bool: True if the connection is successful, False otherwise.
         """
         try:
-            Fetcher._fetch_from_url('https://api.github.com')
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore", UserWarning)
+                Fetcher._fetch_from_url("https://api.github.com") # this will get status code 403
         except (requests.ConnectTimeout, requests.ConnectionError, requests.RequestException):
             return False
         return True
     
     def _set_auth(self):
         """Set up authentication credentials for accessing configured repositories.
 
         Extracts and sets authentication details for each repository from the provided configurations.
         """
-        if isinstance(self.repos, list):
-            self._auth = [self._fetch_auth(repo) for repo in self.repos]
+        if isinstance(self._repos, list):
+            self._auth = [self._fetch_auth(repo) for repo in self._repos]
     
     @staticmethod
     def _fetch_auth(repo_dict: dict):
         """Fetch authentication credentials from a repository configuration.
 
         Args:
             repo_dict (dict): Repository configuration containing 'auth' fields.
@@ -95,37 +97,37 @@
             url (str): URL of the directory to walk through.
             path (str): Path relative to the repository root.
             auth (Tuple[str, str]): Authentication credentials for accessing the repository.
 
         Yields:
             dict: A dictionary containing the path, directories, and files within the directory.
         """
-        contents = Fetcher._fetch_from_url(url=url, auth=auth).json()
-        dirs, files = Fetcher._fetch_directory_contents(contents)
-        yield {'path':path, 
-               'dirs':{d['name']:d['url'] for d in dirs}, 
-               'files':{f['name']:f['download_url'] for f in files}}
-
-        for dir in dirs:
-            new_path = f"{path}/{dir['name']}" if path else dir['name']
-            new_url = dir['url']
-            yield from Fetcher._walk_dir(url=new_url, path=new_path, auth=auth)
+        if contents := Fetcher._fetch_from_url(url=url, auth=auth):
+            dirs, files = Fetcher._fetch_directory_contents(contents.json())
+            yield {'path':path, 
+                    'dirs':{d['name']:d['url'] for d in dirs}, 
+                    'files':{f['name']:f['download_url'] for f in files}}
+
+            for dir in dirs:
+                new_path = f"{path}/{dir['name']}" if path else dir['name']
+                new_url = dir['url']
+                yield from Fetcher._walk_dir(url=new_url, path=new_path, auth=auth)
     
     @staticmethod
     def _fetch_directory_contents(contents):
         """Categorize contents of a directory into subdirectories and files.
 
         Args:
             contents (list): List of contents from a directory.
 
         Returns:
             tuple: A tuple containing lists of directories and files.
         """
         dirs, files = [], []
-        for i, item in enumerate(contents):
+        for item in contents:
             if item['type'] == 'dir':
                 dirs.append(item)
             elif item['type'] == 'file':
                 files.append(item)
         return dirs, files
     
     @staticmethod
@@ -135,20 +137,23 @@
         Args:
             repo_url (dict): The GitHub repository URL.
             path (Optional[str]): An optional path within the repository.
 
         Returns:
             str: A constructed API endpoint URL based on the repository details.
         """
-        ptrn_github = r'https://(?:[^/]+\.)?github\.com/(?P<owner>[^/]+)/(?P<repo>[^/.]+)(?:\.git])?'
+        ptrn_github = r'https://(?:[^/]+\.)?github\.com/(?P<owner>[^/]+)/(?P<repo>[^/.]+)(?:\.git)?(?:/(?P<path>.*))?'
         if matched := re.match(ptrn_github, repo_url):
             owner = matched['owner']
             repo = matched['repo']
-            return f"https://api.github.com/repos/{owner}/{repo}/contents/{path}" if path \
-                else f"https://api.github.com/repos/{owner}/{repo}/contents"
+            if matched['path']:
+                path_ = matched['path']
+                path = '/'.join([path_, path]) if path_ else path
+            url = f"https://api.github.com/repos/{owner}/{repo}/contents"
+            return f"{url}/{path}" if path else url
     
     @staticmethod
     def _fetch_from_url(url: str, auth: Tuple[str, str] = None) -> Optional[requests.Response]:
         """Fetch data from a given URL using optional authentication.
 
         Args:
             url (str): The URL from which to fetch data.
@@ -157,15 +162,19 @@
         Returns:
             Optional[requests.Response]: The response object if successful, otherwise None.
         """
         response = requests.get(url, auth=auth)
         if response.status_code == 200:
             return response
         else:
-            warnings.warn(f"Failed to retrieve contents: {response.status_code}", UserWarning)
+            warnings.warn(f"Failed to retrieve contents: {response.status_code}.", UserWarning)
+            if response.status_code == 403:
+                warnings.warn(f"It potentially due to incorect repo address or exceed limit of request."
+                              " Try use API token for giigle", UserWarning)
+            
             return None
 
     @staticmethod
     def _download_buffer(url: dict,
                          chunk_size: int = 8192,
                          auth: Tuple[str, str] = None) -> Union[Generator, bool]:
         """Download file content from a URL in buffered chunks.
```

### Comparing `xnippy-0.1.0/xnippy/fetcher/snippets.py` & `xnippy-0.1.1/xnippy/fetcher/snippets.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,62 +11,87 @@
 """
 
 from __future__ import annotations
 import os
 import warnings
 from pathlib import Path
 from .base import Fetcher
+from xnippy.raiser import WarnRaiser
 from xnippy.snippet import PlugInSnippet, RecipeSnippet, SpecSnippet, PresetSnippet
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from typing import Optional
     from typing import List
-    from xnippy.types import SnippetType, SnippetMode, SnippetPath, StorageMode
+    from xnippy.types import SnippetType, SnippetMode, SnippetPath, StorageMode, VersionType
 
 
 class Snippets(Fetcher):
     """Manages the aggregation of snippets from various sources based on the specified mode.
 
     This class integrates local and remote snippet sources, handling their fetching, storing,
     and updating based on connectivity and cache settings.
     """
     path: Optional[Path]
     mode: SnippetMode
+    package_name: str
+    package_version: VersionType
     is_cache: bool
     _fetched: bool = False
-    _template: List[SnippetType] = []
     _remote_snippets: List[SnippetType] = []
     _local_snippets: List[SnippetType] = []
-    _template_snippets: List[SnippetType] = []
     
     def __init__(self, 
                  repos: dict,
+                 package_name: str,
+                 package_version: VersionType,
                  mode: SnippetMode,
                  path: SnippetPath = (None, False)
                  ) -> None:
         """Initializes the Snippets object with specified repository configurations and operational mode.
 
         Args:
             repos (dict): A dictionary containing repository configurations.
             mode (Literal['plugin', 'preset', 'spec', 'recipe']): The operational mode determining the type of snippets to manage.
             path (Tuple[Optional[Path], bool], optional): A tuple containing the path to local storage and a boolean indicating cache usage.
         """
-        self.repos = repos
+        self._repos = self._inspect_repos(repos)
+        self.package_name = package_name
+        self.package_version = package_version
         self.mode = mode
         self.path = self._resolve(path[0]) if path[0] else path[0]
         self.is_cache = path[1]
         self._set_auth()
         self._fetch_local_contents()
-        self._template = [c[mode]['template'] for c in repos if 'template' in c[mode]]
+        
+    def _inspect_repos(self, repos):
+        inspected = {}
+        for repo in repos:
+            # Check if both 'name' and 'url' keys exist in the repo dictionary
+            name = repo.get('name')
+            url = repo.get('url')
+            
+            if not name or not url:
+                message = f"Given repo '{name}' in configuration file does not comply with the expected configuration."
+                WarnRaiser(self._inspect_repos).custom(message, UserWarning)
+                inspected[name] = None
+            else:
+                inspected[name] = repo
+
+        # Filter out None values and return the list of valid repos
+        filtered_repo = [repo for repo in inspected.values() if repo is not None]
+        if not filtered_repo:
+            message = "No valid repo configurations remain; nothing to download."
+            WarnRaiser(self._inspect_repos).custom(message, UserWarning)
+        return filtered_repo
         
     def _fetch_local_contents(self) -> Optional[list]:
         """Fetches snippets from local storage based on the current mode and path settings.
 
         Gathers contents from the specified directory and converts them into snippets. This operation
-        is skipped if caching is enabled.
+        is skipped if caching mode is enabled. (This means the Xnippy initiated with dedicate space to download Sneppits.)
 
         Returns:
             Optional[list]: Returns None if caching is enabled, otherwise returns a list of fetched local contents.
         """
         if self.is_cache:
             return None
         contents = []
@@ -79,61 +104,44 @@
             
     def _fetch_remote_contents(self) -> None:
         """Fetches snippets from remote repositories if connected and not previously fetched.
 
         Retrieves snippet data from remote sources as specified by the repository configuration
         and converts them into snippet objects. Updates the fetched status upon completion.
         """
-        if self.repos:
-            contents = [self._walk_github_repo(repo_url=repo['url'],
-                                               path=repo[self.mode]['path'],
-                                               auth=self._auth[i]) for i, repo in enumerate(self.repos)]
-            self._convert_contents_to_snippets(contents=contents, remote=True)
-            self._fetched = True        
+        if self._repos:
+            if contents := [self._walk_github_repo(repo_url=repo['url'],
+                                                   path=repo[self.mode]['path'],
+                                                   auth=self._auth[i]) for i, repo in enumerate(self._repos)]:
+                self._convert_contents_to_snippets(contents=contents, remote=True)
+            self._fetched = True
             
     def _convert_contents_to_snippets(self, contents: list, remote: bool = False) -> None:
         """Converts fetched contents from either local or remote sources into snippet objects.
 
         Iterates over fetched contents, creating snippet objects which are then stored appropriately
-        based on their validation status and whether they match predefined templates.
+        based on their validation status.
 
         Args:
             contents (list): List of contents fetched from either local or remote sources.
             remote (bool, optional): Flag indicating whether the contents are from remote sources.
         """
-        for repo_id, contents in enumerate(contents):
-            for c in contents:
+        snippets = []
+        for repo_id, content in enumerate(contents):
+            for c in content:
                 if remote:
-                    snippet = self._snippet(contents=c, auth=self._auth[repo_id], remote=remote)
-                    self._store_remote_snippet(repo_id=repo_id, snippet=snippet)
+                    snippets.append(self._snippet(contents=c, auth=self._auth[repo_id], remote=remote))
+                    storage = self._remote_snippets
                 else:
-                    snippet = self._snippet(contents=c, remote=remote)
-                    if snippet.is_valid and \
-                        snippet.name not in [s.name for s in self._local_snippets]:
-                        self._local_snippets.append(snippet)
+                    snippets.append(self._snippet(contents=c, remote=remote))
+                    storage = self._local_snippets
+        for s in snippets:            
+            if s.is_valid and s.name not in [s_.name for s_ in storage]:
+                storage.append(s)
                         
-    def _store_remote_snippet(self, repo_id: int, snippet: SnippetType):
-        """Stores validated remote snippets into the appropriate lists based on template matching.
-
-        Checks if the snippet is valid and if it matches a template or not. Based on this,
-        the snippet is added to the respective list (template snippets or general remote snippets).
-
-        Args:
-            repo_id (int): The repository ID corresponding to the snippet source.
-            snippet (Snippet): The snippet object to be stored.
-        """
-        if not snippet.is_valid:
-            return None
-        if self._is_template(repo_id, snippet) and \
-            snippet.name not in [s.name for s in self._template_snippets]:
-            self._template_snippets.append(snippet)
-        elif not self._is_template(repo_id, snippet) and \
-            snippet.name not in [s.name for s in self._remote_snippets]:
-            self._remote_snippets.append(snippet)
-            
     @property
     def _snippet(self):
         """Determines the snippet class based on the operational mode.
 
         Returns:
             Type[Snippet]: Returns the class type corresponding to the operational mode (Plugin, Preset, Spec, Recipe, App).
         """
@@ -163,28 +171,15 @@
             if self.is_connected():
                 self._fetch_remote_contents()
                 return self._remote_snippets
             else:
                 warnings.warn("Connection failed. Please check your network settings.")
                 return None
     
-    def _is_template(self, repo_id: int, snippet: SnippetType) -> bool:
-        """Test given snippet is template. This internal method used to exclude template snippets from avail."""
-        return any(snippet.name == t for t in self._template[repo_id])
-    
     @property
     def local(self):
+        self._fetch_local_contents()
         return self._local_snippets
 
     @property
     def is_up_to_date(self):
         return self._fetched
-    
-    def get(self, 
-            name: str, 
-            version: Optional[str], 
-            storage_mode: Optional[StorageMode]):
-        if storage_mode:
-            storage = [self.local if storage_mode == 'local' else self.remote]
-        else:
-            storage = [self.local, self.remote]
-
```

### Comparing `xnippy-0.1.0/xnippy/formatter/bytes.py` & `xnippy-0.1.1/xnippy/formatter/bytes.py`

 * *Files identical despite different names*

### Comparing `xnippy-0.1.0/xnippy/formatter/datetime.py` & `xnippy-0.1.1/xnippy/formatter/datetime.py`

 * *Files identical despite different names*

### Comparing `xnippy-0.1.0/xnippy/formatter/io.py` & `xnippy-0.1.1/xnippy/formatter/io.py`

 * *Files identical despite different names*

### Comparing `xnippy-0.1.0/xnippy/formatter/recipe.py` & `xnippy-0.1.1/xnippy/parser/recipe.py`

 * *Files identical despite different names*

### Comparing `xnippy-0.1.0/xnippy/formatter/string.py` & `xnippy-0.1.1/xnippy/formatter/string.py`

 * *Files identical despite different names*

### Comparing `xnippy-0.1.0/xnippy/module/commander.py` & `xnippy-0.1.1/xnippy/module/commander.py`

 * *Files identical despite different names*

### Comparing `xnippy-0.1.0/xnippy/module/installer.py` & `xnippy-0.1.1/xnippy/module/installer.py`

 * *Files identical despite different names*

### Comparing `xnippy-0.1.0/xnippy/module/loader.py` & `xnippy-0.1.1/xnippy/module/loader.py`

 * *Files identical despite different names*

### Comparing `xnippy-0.1.0/xnippy/snippet/plugin.py` & `xnippy-0.1.1/xnippy/snippet/plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,195 +9,233 @@
 
 Author: Sung-Ho Lee (shlee@unc.edu)
 """
 
 from __future__ import annotations
 import re
 import yaml
-import warnings
+import inspect
 from pathlib import Path
 from tqdm import tqdm
 from .base import Snippet
+from xnippy.raiser import WarnRaiser
 from xnippy.module import ModuleLoader
 from xnippy.module import ModuleInstaller
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from typing import Tuple, Dict, Optional, Union
     
 
 class PlugIn(Snippet):
     """Handles the inspection and management of plugins, either locally or from remote sources.
     
     This class supports dynamic loading of plugins into memory for immediate use without the need for disk storage,
     facilitating rapid development and testing of plugin functionalities.
+    
+    Attributes:
+        _contents: Dict = {"path": path of currnet plugin,
+                           "files": list of paths or download urls of file contents,
+                           "dirs": list of paths or access urls of diretory contents}
     """
+    _required_key: list = ['plugin', 'source', 'dependencies'] #, 'package']
     _remote: bool
-    _module_loaded: bool
+    _activated: bool
     _dependencies_tested: bool = False 
     _auth: Tuple[str, str]
     _data: Dict = {}
     _contents: Dict
+    _repository: Optional[str]
+    _include: Dict = {}
     
     def __init__(self, 
                  contents: dict, 
                  auth: Optional[Tuple[str, str]] = None, 
-                 remote: bool = False):
+                 remote: bool = False,
+                 repository: Optional[str] = None):
         """Initializes the plugin with specified contents, authentication for remote access, and remote status.
 
         Args:
             contents (dict): Contains keys of path, dirs, and files, similar to os.walk but structured as a dictionary.
                              Each directory and file is also mapped as a key (filename) to a value (path or download_url).
             auth (Tuple[str, str], optional): Credentials for using the GitHub API if needed.
             remote (bool): True if the plugin is loaded remotely, False otherwise.
         """
         self._auth = auth
         self._contents = contents
         self._remote = remote
+        self._repository = repository if remote else None
         self._content_parser()
 
-    def set(self, skip_dependency_check: bool = False, *args, **kwargs):
+    ## Preparation step: starts
+    def _content_parser(self):
+        """Parses the contents of the plugin based on its current state (local or remote).
+
+        This method sets the plugin's parameters and determines its validity based on the availability
+        and correctness of the required data.
+        """
+        if len(self._contents['files']) == 0:
+            self.is_valid = False
+            return None
+        self._parse_files()
+        self._set_params()
+        
+    def _parse_files(self):
+        """Parse manifest from contents and load."""
+        for filename, file_loc in self._contents['files'].items():
+            if filename.lower() == 'manifest.yaml':
+                self._load_manifest(file_loc)
+            
+    def _load_manifest(self, file_loc: Union[str, Path]):
+        """Loads the plugin's manifest from a remote URL.
+
+        Args:
+            download_url (str): The URL from which to download the manifest.
+
+        This method fetches and parses the plugin's manifest file, setting flags based on the contents.
+        """
+        if self._remote:
+            bytes_data = b''.join(self._download_buffer(file_loc, auth=self._auth))
+            self._manifest = yaml.safe_load(bytes_data)
+        else:
+            with open(file_loc, 'r') as f:
+                self._manifest = yaml.safe_load(f)
+        if any(k not in list(self._manifest.keys()) for k in self._required_key):
+            comment = ["Please verify the manifest file's structure. Ensure it includes all required keys: ",
+                       "'package', 'plugin', 'source', 'dependencies'. For more details, refer to the documentation: ",
+                       "https://github.com/xoani/xnippy/blob/master/examples/docs/PLUGIN.md"]
+            WarnRaiser('self._load_manifest').compliance_warning(comment=''.join(comment))
+            self.is_valid = False
+        else:
+            self.is_valid = True
+            
+    def _set_params(self):
+        try:
+            info = self._manifest['plugin']
+            self.parse_version(info['version'])
+            self.name = info['name']
+            self.package = info['package'] if 'package' in info.keys() else None
+            self.is_valid = True
+        except (KeyError, AttributeError):
+            self.is_valid = False
+        self._activated = False if self._remote else True
+    ## Preperation step: ends
+
+    ## Execution step: starts
+    def run(self, skip_dependency_check: bool = False, *args, **kwargs):
         """Sets the plugin's parameters and ensures dependencies are resolved and the module is loaded.
 
         This method acts as a setup routine by testing dependencies, downloading necessary files,
         and dynamically importing the module and call module with given input arguments.
 
         Args:
-            *args: Variable length argument list.
-            **kwargs: Arbitrary keyword arguments.
+            skip_dependency_check (bool): If True, skips the dependency check.
+            *args: Variable length argument list for the dynamically imported module.
+            **kwargs: Arbitrary keyword arguments for the dynamically imported module.
 
         Returns:
             The result of calling the imported module with provided arguments.
+
+        Raises:
+            ValueError: If the provided arguments do not match the required function signature.
         """
-        if not self._module_loaded:
+        if not self._activated:
             self.download()
+        sig = inspect.signature(self._imported_object)
+        try:
+            # This will raise a TypeError if the arguments do not match the function signature
+            sig.bind(*args, **kwargs)
+        except TypeError as e:
+            raise TypeError(f"Argument mismatch for the imported module: {e}")
         if not self._dependencies_tested and not skip_dependency_check:
             self.resolve_dependencies()
-        return self._imported_module(*args, **kwargs)
+        return self._imported_object(*args, **kwargs)
     
-    def resolve_dependencies(self):
-        """Checks and installs any missing dependencies specified in the plugin's manifest file."""
-        ptrn = r'(\w+)\s*(>=|<=|==|!=|>|<)\s*([0-9]+(?:\.[0-9]+)*)?'
-        deps = self._manifest['dependencies']
-        print(f"++ Resolving python module dependencies...\n  -> {deps}")
-        for module in tqdm(deps, desc=' -Dependencies', ncols=80):
-            if matched := re.match(ptrn, module):
-                self._status = None
-                module_name, version_constraint, version = matched.groups()
-                ModuleInstaller().install(module_name=module_name,
-                                          version_constraint=version_constraint, 
-                                          version=version)
-        self._dependencies_tested = True
-        
+    ## execution start
     def download(self, dest: Optional[Path] = None, force: bool = False):
         """Downloads the plugin to a specified destination or loads it directly into memory if no destination is provided.
         This method also checks if the file already exists at the destination and optionally overwrites it based on the 'force' parameter.
 
         Args:
             dest (Path, optional): The file system destination where the plugin files will be saved.
                                 If None, files are loaded into memory.
             force (bool, optional): If True, existing files at the destination will be overwritten.
                                     Defaults to False.
         """
         if not self._remote:
-            warnings.warn("Attempt to download failed: The plugin is already available "
-                          "locally and cannot be downloaded again.", UserWarning)
+            WarnRaiser(self._activated).download_failed(comment="The plugin is already available locally and cannot be downloaded again.")
             return False
         print(f"\n++ Downloading remote module to '{dest or 'memory'}'.")
         files = self._contents['files'] if dest else self._get_module_files()
         for filename, download_url in tqdm(files.items(), desc=' -Files', ncols=80):
             if dest:
-                plugin_path: Path = (Path(dest).resolve() / self.name)
+                # The plugin will be downloaded on the folder with the name
+                plugin_path: Path = (Path(dest).resolve() / f'{self.name}_{str(self.version)}')
                 plugin_path.mkdir(exist_ok=True)
                 plugin_file: Path = plugin_path / filename
                 if plugin_file.exists() and not force:
-                    warnings.warn(f"Warning: File '{filename}' already exists. Skipping download. Use 'force=True' to overwrite.", 
-                                  UserWarning)
-                    continue  # Skip the download if file exists and force is False
+                    WarnRaiser(self.download).file_exist(filename, comment="Skipping download. Use 'force=True' to overwrite.")
+                    continue
                 with open(plugin_file, 'wb') as f:
                     for chunk in self._download_buffer(download_url, auth=self._auth):
                         f.write(chunk)
             else:
                 # When downloading to memory
                 self._data[filename] = b''.join(self._download_buffer(download_url, auth=self._auth))
-                self._module_loaded = True  # Mark the module as loaded
-
+                self._activated = True  # Mark the module as loaded
+    
+    def resolve_dependencies(self):
+        """Checks and installs any missing dependencies specified in the plugin's manifest file."""
+        ptrn = r'(\w+)\s*(>=|<=|==|!=|>|<)\s*([0-9]+(?:\.[0-9]+)*)?'
+        deps = self._manifest['dependencies']
+        print(f"++ Resolving python module dependencies...\n  -> {deps}")
+        for module in tqdm(deps, desc=' -Dependencies', ncols=80):
+            if matched := re.match(ptrn, module):
+                self._status = None
+                module_name, version_constraint, version = matched.groups()
+                ModuleInstaller().install(module_name=module_name,
+                                          version_constraint=version_constraint, 
+                                          version=version)
+        self._dependencies_tested = True
 
     def _get_module_files(self):
         return {f:url for f, url in self._contents['files'].items() if f.endswith('.py')} 
-
-    def _content_parser(self):
-        """Parses the contents of the plugin based on its current state (local or remote).
-
-        This method sets the plugin's parameters and determines its validity based on the availability
-        and correctness of the required data.
-        """
-        if len(self._contents['files']) == 0:
-            self.is_valid = False
-            return None
-        self._parse_files()
-        self._set_params()
-
-    def _set_params(self):
-        try:
-            self.parse_version(self._manifest['version'])
-            self.name = self._manifest['name']
-            self.type = self._manifest['subtype']
-            self.is_valid = True
-        except (KeyError, AttributeError):
-            self.is_valid = False
-        self._module_loaded = False if self._remote else True
-
-    def _parse_files(self):
-        """Processes the contents, loading the manifest if necessary."""
-        for filename, file_loc in self._contents['files'].items():
-            if filename.lower() == 'manifest.yaml':
-                self._load_manifest(file_loc)
-
-    def _parse_remote(self):
-        """Processes the contents if the plugin is in a remote state, loading the manifest if necessary."""
-        for filename, download_url in self._contents['files'].items():
-            if filename.lower() == 'manifest.yaml':
-                self._load_manifest(download_url)
-    
-    def _load_manifest(self, file_loc: Union[str, Path]):
-        """Loads the plugin's manifest from a remote URL.
-
-        Args:
-            download_url (str): The URL from which to download the manifest.
-
-        This method fetches and parses the plugin's manifest file, setting flags based on the contents.
-        """
-        if self._remote:
-            bytes_data = b''.join(self._download_buffer(file_loc, auth=self._auth))
-            self._manifest = yaml.safe_load(bytes_data)
-        else:
-            with open(file_loc, 'r') as f:
-                self._manifest = yaml.safe_load(f)
-        if self._manifest['type'] != 'plugin':
-            warnings.warn(f"The type annotation for the '{self._manifest['name']}' plugin manifest is not set as 'plugin.' \
-                    This may cause the plugin to function incorrectly.")
-            self.is_valid = False
     
     @property
-    def _imported_module(self):
+    def _imported_object(self):
         """Dynamically imports the module from loaded data.
 
         This method uses the information from the manifest to import the specified module and method dynamically.
 
         Returns:
             The imported method from the module.
         """
-        source = self._manifest['source']
-        f, c = source.split(':')
-        mloc = self._data[f] if self._remote else self._contents['files'][f]
-        loader = ModuleLoader(mloc)
-        module = loader.get_module(self.name)
-        return getattr(module, c)
-
+        # run include dependency
+        include = self._manifest['source']['include']
+        if isinstance(include, str):
+            include = [include]
+        for filename in include:
+            if filename.endswith('.py'):
+                mloc = self._data[filename] if self._remote else self._contents['files'][filename]
+                loader = ModuleLoader(mloc)
+                module_name = filename.replace(".py", "")
+                module = loader.get_module(module_name)
+                self._include[module_name] = module
+        
+        # load entry point
+        source = self._manifest['source']['entry_point']
+        ptrn = r'(?P<filename>[a-zA-Z0-9_-]+\.py)(?::(?P<target>[a-zA-Z][a-zA-Z0-9\_\-]*))?'
+        if matched := re.match(ptrn, source):
+            filename, target = matched.groups()
+            mloc = self._data[filename] if self._remote else self._contents['files'][filename]
+            loader = ModuleLoader(mloc)
+            module = loader.get_module(self.name)
+            self._include[self.name] = module
+            return getattr(module, target)
+        
     def __repr__(self):
         if self.is_valid:
-            repr = f"PlugInSnippet<{self.type}>::{self.name}=={self.version}"
+            repr = f"PlugInSnippet<{self.package}>::{self.name}=={self.version}"
             if self._remote:
-                repr += '+InMemory' if self._module_loaded else '+Remote'
+                repr += '+InMemory' if self._activated else f'+Remote[{self._repository}]'
             return repr
         else:
             return "PlugInSnippet<?>::InValidPlugin"
```

### Comparing `xnippy-0.1.0/.gitignore` & `xnippy-0.1.1/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -159,8 +159,10 @@
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 .idea/
 
 # OSX cache
 .DS_Store
 
 # xnippy config dir
-.xnippy
+.xnippy
+tests/*.ipynb
+.vscode
```

### Comparing `xnippy-0.1.0/LICENSE` & `xnippy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xnippy-0.1.0/pyproject.toml` & `xnippy-0.1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "xnippy"
-version = "0.1.0"
+dynamic = ['version']
 description = "A Python module for dynamic integration and management of extensible code snippets."
 readme = "README.md"
 license = { text = "MIT" }
 authors = [
     { name = "SungHo Lee", email = "shlee@unc.edu" }
 ]
 maintainers = [
@@ -25,16 +25,24 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10"
 ]
 keywords = ["code snippets", "extensible", "plugin", "dynamic loading"]
 requires-python = ">=3.7"
 dependencies = [
     "pyyaml>=6.0.1",
-    "numpy>=1.18.0",
+    "packaging>=23.0",
     "tqdm>=4.66.1"
 ]
-urls = {"Homepage" = "https://xoani.github.io"}
+urls = {Homepage = "https://xoani.github.io"}
+
+[project.optional-dependencies]
+dev = [
+    "flake8",
+    "pytest",
+    "nbmake",
+    "types-PyYAML"
+]
 
 # Additional configuration specific to hatch can go under 'tool.hatch.*'
 [tool.hatch.version]
 path = "xnippy/__init__.py"
 style = "pep440"
```

