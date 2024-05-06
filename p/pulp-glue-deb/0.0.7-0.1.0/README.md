# Comparing `tmp/pulp-glue-deb-0.0.7.tar.gz` & `tmp/pulp-glue-deb-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-glue-deb-0.0.7.tar", last modified: Mon Feb 19 16:28:09 2024, max compression
+gzip compressed data, was "pulp-glue-deb-0.1.0.tar", last modified: Mon May  6 16:11:26 2024, max compression
```

## Comparing `pulp-glue-deb-0.0.7.tar` & `pulp-glue-deb-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:28:09.669179 pulp-glue-deb-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-02-19 16:28:09.669179 pulp-glue-deb-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 16:28:02.000000 pulp-glue-deb-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:28:09.665179 pulp-glue-deb-0.0.7/pulp_glue/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:28:09.669179 pulp-glue-deb-0.0.7/pulp_glue/deb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 16:28:02.000000 pulp-glue-deb-0.0.7/pulp_glue/deb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6955 2024-02-19 16:28:02.000000 pulp-glue-deb-0.0.7/pulp_glue/deb/context.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 16:28:02.000000 pulp-glue-deb-0.0.7/pulp_glue/deb/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:28:09.669179 pulp-glue-deb-0.0.7/pulp_glue_deb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-02-19 16:28:09.000000 pulp-glue-deb-0.0.7/pulp_glue_deb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-02-19 16:28:09.000000 pulp-glue-deb-0.0.7/pulp_glue_deb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 16:28:09.000000 pulp-glue-deb-0.0.7/pulp_glue_deb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-19 16:28:09.000000 pulp-glue-deb-0.0.7/pulp_glue_deb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-19 16:28:09.000000 pulp-glue-deb-0.0.7/pulp_glue_deb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-02-19 16:28:02.000000 pulp-glue-deb-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 16:28:09.669179 pulp-glue-deb-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:11:26.864481 pulp-glue-deb-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-06 16:11:26.864481 pulp-glue-deb-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:11:23.000000 pulp-glue-deb-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:11:26.860481 pulp-glue-deb-0.1.0/pulp_glue/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:11:26.864481 pulp-glue-deb-0.1.0/pulp_glue/deb/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-06 16:11:23.000000 pulp-glue-deb-0.1.0/pulp_glue/deb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7732 2024-05-06 16:11:23.000000 pulp-glue-deb-0.1.0/pulp_glue/deb/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:11:23.000000 pulp-glue-deb-0.1.0/pulp_glue/deb/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:11:26.864481 pulp-glue-deb-0.1.0/pulp_glue_deb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-06 16:11:26.000000 pulp-glue-deb-0.1.0/pulp_glue_deb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-06 16:11:26.000000 pulp-glue-deb-0.1.0/pulp_glue_deb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:11:26.000000 pulp-glue-deb-0.1.0/pulp_glue_deb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-06 16:11:26.000000 pulp-glue-deb-0.1.0/pulp_glue_deb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-06 16:11:26.000000 pulp-glue-deb-0.1.0/pulp_glue_deb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-06 16:11:23.000000 pulp-glue-deb-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 16:11:26.864481 pulp-glue-deb-0.1.0/setup.cfg
```

### Comparing `pulp-glue-deb-0.0.7/PKG-INFO` & `pulp-glue-deb-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pulp-glue-deb
-Version: 0.0.7
+Version: 0.1.0
 Summary: Version agnostic glue library to talk to pulpcore's REST API. (deb plugin)
 Author-email: Pulp Team <pulp-list@redhat.com>
 License: GPLv2+
 Project-URL: repository, https://github.com/pulp/pulp-cli-deb
 Project-URL: changelog, https://github.com/pulp/pulp-cli-deb/blob/main/CHANGES.md
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Software Distribution
 Classifier: Typing :: Typed
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulp-glue-deb-0.0.7/pulp_glue/deb/context.py` & `pulp-glue-deb-0.1.0/pulp_glue/deb/context.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,137 +4,162 @@
     EntityDefinition,
     PluginRequirement,
     PulpContentContext,
     PulpEntityContext,
     PulpException,
     PulpRepositoryContext,
     PulpRepositoryVersionContext,
-    registered_repository_contexts,
 )
 from pulp_glue.common.i18n import get_translation
 
 translation = get_translation(__name__)
 _ = translation.gettext
 
 
 class PulpDebGenericContentContext(PulpContentContext):
     ENTITY = "deb generic content"
     ENTITIES = "deb generic contents"
     HREF = "deb_generic_content_href"
     ID_PREFIX = "content_deb_generic_contents"
     NEEDS_PLUGINS = [PluginRequirement("deb")]
+    PLUGIN = "deb"
+    RESOURCE_TYPE = "generic_content"
 
 
 class PulpDebInstallerFileIndexContext(PulpContentContext):
     ENTITY = "deb installer file index"
     ENTITIES = "deb installer file indices"
     HREF = "deb_installer_file_index_href"
     ID_PREFIX = "content_deb_installer_file_indices"
     NEEDS_PLUGINS = [PluginRequirement("deb")]
+    PLUGIN = "deb"
+    RESOURCE_TYPE = "installer_file_index"
 
 
 class PulpDebInstallerPackageContext(PulpContentContext):
     ENTITY = "deb installer package"
     ENTITIES = "deb installer packages"
     HREF = "deb_installer_package_href"
     ID_PREFIX = "content_deb_installer_packages"
     NEEDS_PLUGINS = [PluginRequirement("deb")]
+    PLUGIN = "deb"
+    RESOURCE_TYPE = "installer_package"
 
 
 class PulpDebPackageIndexContext(PulpContentContext):
     ENTITY = "deb package index"
     ENTITIES = "deb package indices"
     HREF = "deb_package_index_href"
     ID_PREFIX = "content_deb_package_indices"
     NEEDS_PLUGINS = [PluginRequirement("deb")]
+    PLUGIN = "deb"
+    RESOURCE_TYPE = "package_index"
 
 
 class PulpDebPackageReleaseComponentContext(PulpContentContext):
     ENTITY = "deb package release component"
     ENTITIES = "deb package release components"
     HREF = "deb_package_release_component_href"
     ID_PREFIX = "content_deb_package_release_components"
     NEEDS_PLUGINS = [PluginRequirement("deb")]
+    PLUGIN = "deb"
+    RESOURCE_TYPE = "package_release_component"
 
 
 class PulpDebPackageContext(PulpContentContext):
     CAPABILITIES = {"upload": []}
     ENTITY = "deb package"
     ENTITIES = "deb packages"
     HREF = "deb_package_href"
     ID_PREFIX = "content_deb_packages"
     NEEDS_PLUGINS = [PluginRequirement("deb")]
+    PLUGIN = "deb"
+    RESOURCE_TYPE = "package"
 
 
 class PulpDebReleaseArchitectureContext(PulpContentContext):
     ENTITY = "deb release architecture"
     ENTITIES = "deb release architectures"
     HREF = "deb_release_architecture_href"
     ID_PREFIX = "content_deb_release_architectures"
     NEEDS_PLUGINS = [PluginRequirement("deb")]
+    PLUGIN = "deb"
+    RESOURCE_TYPE = "release_architecture"
 
 
 class PulpDebReleaseComponentContext(PulpContentContext):
     ENTITY = "deb release component"
     ENTITIES = "deb release components"
     HREF = "deb_release_component_href"
     ID_PREFIX = "content_deb_release_components"
     NEEDS_PLUGINS = [PluginRequirement("deb")]
+    PLUGIN = "deb"
+    RESOURCE_TYPE = "release_component"
 
 
 class PulpDebReleaseFileContext(PulpContentContext):
     ENTITY = "deb release file"
     ENTITIES = "deb release files"
     HREF = "deb_release_file_href"
     ID_PREFIX = "content_deb_release_files"
     NEEDS_PLUGINS = [PluginRequirement("deb")]
+    PLUGIN = "deb"
+    RESOURCE_TYPE = "release_file"
 
 
 class PulpDebReleaseContext(PulpContentContext):
     ENTITY = "deb release"
     ENTITIES = "deb releases"
     HREF = "deb_release_href"
     ID_PREFIX = "content_deb_releases"
     NEEDS_PLUGINS = [PluginRequirement("deb")]
+    PLUGIN = "deb"
+    RESOURCE_TYPE = "release"
 
 
 class PulpAptDistributionContext(PulpEntityContext):
     ENTITY = _("apt distribution")
     ENTITIES = _("apt distributions")
     HREF = "deb_apt_distribution_href"
     ID_PREFIX = "distributions_deb_apt"
     NEEDS_PLUGINS = [PluginRequirement("deb")]
+    PLUGIN = "deb"
+    RESOURCE_TYPE = "apt"
 
 
 class PulpAptPublicationContext(PulpEntityContext):
     ENTITY = _("apt publication")
     ENTITIES = _("apt publications")
     HREF = "deb_apt_publication_href"
     ID_PREFIX = "publications_deb_apt"
     NEEDS_PLUGINS = [PluginRequirement("deb")]
+    PLUGIN = "deb"
+    RESOURCE_TYPE = "apt"
 
-    def preprocess_body(self, body: EntityDefinition) -> EntityDefinition:
-        body = super().preprocess_body(body)
+    def preprocess_entity(self, body: EntityDefinition, partial: bool = False) -> EntityDefinition:
+        body = super().preprocess_entity(body)
         version = body.pop("version", None)
         if version is not None:
             repository_href = body.pop("repository")
             body["repository_version"] = f"{repository_href}versions/{version}/"
         return body
 
 
 class PulpVerbatimPublicationContext(PulpEntityContext):
     APT_ONLY: ClassVar[Set[str]] = {"simple", "structured", "signing_service"}
     ENTITY = _("verbatim publication")
     ENTITIES = _("verbatim publications")
     HREF = "deb_verbatim_publication_href"
     ID_PREFIX = "publications_deb_verbatim"
     NEEDS_PLUGINS = [PluginRequirement("deb")]
+    PLUGIN = "deb"
+    RESOURCE_TYPE = "verbatim"
 
-    def preprocess_body(self, body: EntityDefinition) -> EntityDefinition:
-        body = super().preprocess_body(body)
+    def preprocess_entity(self, body: EntityDefinition, partial: bool = False) -> EntityDefinition:
+        body = super().preprocess_entity(body)
         fields = self.APT_ONLY.intersection(body.keys())
         if fields:
             raise PulpException(
                 _("{} can't be used when creating VerbatimPublications").format(fields)
             )
         version = body.pop("version", None)
         if version is not None:
@@ -146,14 +171,16 @@
 class PulpAptRemoteContext(PulpEntityContext):
     ENTITY = _("apt remote")
     ENTITIES = _("apt remotes")
     HREF = "deb_apt_remote_href"
     ID_PREFIX = "remotes_deb_apt"
     NEEDS_PLUGINS = [PluginRequirement("deb")]
     NULLABLES = {"architectures", "components"}
+    PLUGIN = "deb"
+    RESOURCE_TYPE = "apt"
 
     @staticmethod
     def tuple_to_whitespace_separated_string(field_name: str, body: EntityDefinition) -> None:
         """
         Safely turns a tuple contained in body[field_name] into a whitespace separated string.
         If body[field_name] contains None or (), then field_name is dropped from body.
         If we end up with an empty string, we use None instead.
@@ -161,16 +188,16 @@
         If body[field_name] does not contain a tuple, the behaviour is undefined.
         """
         field = body.pop(field_name, None)
         if field:
             string_field = " ".join(field).strip()
             body[field_name] = string_field if string_field else None
 
-    def preprocess_body(self, body: EntityDefinition) -> EntityDefinition:
-        body = super().preprocess_body(body)
+    def preprocess_entity(self, body: EntityDefinition, partial: bool = False) -> EntityDefinition:
+        body = super().preprocess_entity(body)
         self.tuple_to_whitespace_separated_string("distributions", body)
         if "distributions" in body and body["distributions"] is None:
             raise PulpException("Must have at least one distribution for remote.")
         self.tuple_to_whitespace_separated_string("components", body)
         self.tuple_to_whitespace_separated_string("architectures", body)
         return body
 
@@ -184,11 +211,10 @@
 
 class PulpAptRepositoryContext(PulpRepositoryContext):
     ENTITY = _("apt repository")
     ENTITIES = _("apt repositories")
     HREF = "deb_apt_repository_href"
     ID_PREFIX = "repositories_deb_apt"
     NEEDS_PLUGINS = [PluginRequirement("deb")]
+    PLUGIN = "deb"
+    RESOURCE_TYPE = "apt"
     VERSION_CONTEXT = PulpAptRepositoryVersionContext
-
-
-registered_repository_contexts["deb:apt"] = PulpAptRepositoryContext
```

### Comparing `pulp-glue-deb-0.0.7/pulp_glue_deb.egg-info/PKG-INFO` & `pulp-glue-deb-0.1.0/pulp_glue_deb.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pulp-glue-deb
-Version: 0.0.7
+Version: 0.1.0
 Summary: Version agnostic glue library to talk to pulpcore's REST API. (deb plugin)
 Author-email: Pulp Team <pulp-list@redhat.com>
 License: GPLv2+
 Project-URL: repository, https://github.com/pulp/pulp-cli-deb
 Project-URL: changelog, https://github.com/pulp/pulp-cli-deb/blob/main/CHANGES.md
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Software Distribution
 Classifier: Typing :: Typed
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulp-glue-deb-0.0.7/pyproject.toml` & `pulp-glue-deb-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pulp-glue-deb"
-version = "0.0.7"
+version = "0.1.0"
 description = "Version agnostic glue library to talk to pulpcore's REST API. (deb plugin)"
 readme = "README.md"
-requires-python = ">=3.6"
+requires-python = ">=3.8"
 license = {text = "GPLv2+"}
 authors = [
   {name = "Pulp Team", email = "pulp-list@redhat.com"},
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Environment :: Other Environment",
@@ -19,15 +19,15 @@
   "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3",
   "Topic :: System :: Software Distribution",
   "Typing :: Typed",
 ]
 dependencies = [
-  "pulp-glue>=0.18.2,<0.24.0.dev",
+  "pulp-glue>=0.23.2,<0.26",
 ]
 
 [project.urls]
 repository = "https://github.com/pulp/pulp-cli-deb"
 changelog = "https://github.com/pulp/pulp-cli-deb/blob/main/CHANGES.md"
 
 [tool.setuptools.packages.find]
```

