# Comparing `tmp/pulp-cli-deb-0.0.7.tar.gz` & `tmp/pulp-cli-deb-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-cli-deb-0.0.7.tar", last modified: Mon Feb 19 16:28:10 2024, max compression
+gzip compressed data, was "pulp-cli-deb-0.1.0.tar", last modified: Mon May  6 16:11:28 2024, max compression
```

## Comparing `pulp-cli-deb-0.0.7.tar` & `pulp-cli-deb-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:28:10.853184 pulp-cli-deb-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-02-19 16:28:10.853184 pulp-cli-deb-0.0.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:28:10.849184 pulp-cli-deb-0.0.7/pulp_cli_deb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-02-19 16:28:10.000000 pulp-cli-deb-0.0.7/pulp_cli_deb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-02-19 16:28:10.000000 pulp-cli-deb-0.0.7/pulp_cli_deb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 16:28:10.000000 pulp-cli-deb-0.0.7/pulp_cli_deb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-19 16:28:10.000000 pulp-cli-deb-0.0.7/pulp_cli_deb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-19 16:28:10.000000 pulp-cli-deb-0.0.7/pulp_cli_deb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-19 16:28:10.000000 pulp-cli-deb-0.0.7/pulp_cli_deb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:28:10.849184 pulp-cli-deb-0.0.7/pulpcore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:28:10.849184 pulp-cli-deb-0.0.7/pulpcore/cli/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:28:10.849184 pulp-cli-deb-0.0.7/pulpcore/cli/deb/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-02-19 16:28:02.000000 pulp-cli-deb-0.0.7/pulpcore/cli/deb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-02-19 16:28:02.000000 pulp-cli-deb-0.0.7/pulpcore/cli/deb/content.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-02-19 16:28:02.000000 pulp-cli-deb-0.0.7/pulpcore/cli/deb/distribution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:28:10.849184 pulp-cli-deb-0.0.7/pulpcore/cli/deb/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:28:10.849184 pulp-cli-deb-0.0.7/pulpcore/cli/deb/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:28:10.849184 pulp-cli-deb-0.0.7/pulpcore/cli/deb/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-02-19 16:28:02.000000 pulp-cli-deb-0.0.7/pulpcore/cli/deb/locale/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-02-19 16:28:02.000000 pulp-cli-deb-0.0.7/pulpcore/cli/deb/publication.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 16:28:02.000000 pulp-cli-deb-0.0.7/pulpcore/cli/deb/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-02-19 16:28:02.000000 pulp-cli-deb-0.0.7/pulpcore/cli/deb/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-02-19 16:28:02.000000 pulp-cli-deb-0.0.7/pulpcore/cli/deb/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-02-19 16:28:02.000000 pulp-cli-deb-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 16:28:10.853184 pulp-cli-deb-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:11:28.004480 pulp-cli-deb-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-06 16:11:28.004480 pulp-cli-deb-0.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:11:28.004480 pulp-cli-deb-0.1.0/pulp_cli_deb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-05-06 16:11:27.000000 pulp-cli-deb-0.1.0/pulp_cli_deb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-06 16:11:28.000000 pulp-cli-deb-0.1.0/pulp_cli_deb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:11:27.000000 pulp-cli-deb-0.1.0/pulp_cli_deb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-06 16:11:27.000000 pulp-cli-deb-0.1.0/pulp_cli_deb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-06 16:11:27.000000 pulp-cli-deb-0.1.0/pulp_cli_deb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-06 16:11:27.000000 pulp-cli-deb-0.1.0/pulp_cli_deb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:11:28.004480 pulp-cli-deb-0.1.0/pulpcore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:11:28.004480 pulp-cli-deb-0.1.0/pulpcore/cli/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:11:28.004480 pulp-cli-deb-0.1.0/pulpcore/cli/deb/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-06 16:11:23.000000 pulp-cli-deb-0.1.0/pulpcore/cli/deb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9221 2024-05-06 16:11:23.000000 pulp-cli-deb-0.1.0/pulpcore/cli/deb/content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-05-06 16:11:23.000000 pulp-cli-deb-0.1.0/pulpcore/cli/deb/distribution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:11:28.004480 pulp-cli-deb-0.1.0/pulpcore/cli/deb/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:11:28.004480 pulp-cli-deb-0.1.0/pulpcore/cli/deb/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:11:28.004480 pulp-cli-deb-0.1.0/pulpcore/cli/deb/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-06 16:11:23.000000 pulp-cli-deb-0.1.0/pulpcore/cli/deb/locale/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-06 16:11:23.000000 pulp-cli-deb-0.1.0/pulpcore/cli/deb/publication.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:11:23.000000 pulp-cli-deb-0.1.0/pulpcore/cli/deb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-06 16:11:23.000000 pulp-cli-deb-0.1.0/pulpcore/cli/deb/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-05-06 16:11:23.000000 pulp-cli-deb-0.1.0/pulpcore/cli/deb/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-05-06 16:11:23.000000 pulp-cli-deb-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 16:11:28.004480 pulp-cli-deb-0.1.0/setup.cfg
```

### Comparing `pulp-cli-deb-0.0.7/PKG-INFO` & `pulp-cli-deb-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pulp-cli-deb
-Version: 0.0.7
+Version: 0.1.0
 Summary: Command line interface to talk to pulpcore's REST API. (Deb plugin commands)
 Author-email: Pulp Team <pulp-list@redhat.com>
 License: GPLv2+
 Project-URL: repository, https://github.com/pulp/pulp-cli-deb
 Project-URL: changelog, https://github.com/pulp/pulp-cli-deb/blob/main/CHANGES.md
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Software Distribution
 Classifier: Typing :: Typed
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulp-cli-deb-0.0.7/pulp_cli_deb.egg-info/PKG-INFO` & `pulp-cli-deb-0.1.0/pulp_cli_deb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pulp-cli-deb
-Version: 0.0.7
+Version: 0.1.0
 Summary: Command line interface to talk to pulpcore's REST API. (Deb plugin commands)
 Author-email: Pulp Team <pulp-list@redhat.com>
 License: GPLv2+
 Project-URL: repository, https://github.com/pulp/pulp-cli-deb
 Project-URL: changelog, https://github.com/pulp/pulp-cli-deb/blob/main/CHANGES.md
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Software Distribution
 Classifier: Typing :: Typed
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulp-cli-deb-0.0.7/pulpcore/cli/deb/__init__.py` & `pulp-cli-deb-0.1.0/pulpcore/cli/deb/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from pulpcore.cli.deb.content import content
 from pulpcore.cli.deb.distribution import distribution
 from pulpcore.cli.deb.publication import publication
 from pulpcore.cli.deb.remote import remote
 from pulpcore.cli.deb.repository import repository
 
-__version__ = "0.0.7"
+__version__ = "0.1.0"
 
 
 @pulp_group(name="deb")
 def deb_group() -> None:
     pass
```

### Comparing `pulp-cli-deb-0.0.7/pulpcore/cli/deb/content.py` & `pulp-cli-deb-0.1.0/pulpcore/cli/deb/content.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         "deb:deb": PulpAptRepositoryContext,
     },
     href_pattern=PulpAptRepositoryContext.HREF_PATTERN,
     help=_(
         "Repository to add the content to in the form '[[<plugin>:]<resource_type>:]<name>' or by "
         "href."
     ),
-    allowed_with_contexts=(PulpDebPackageContext,),
+    allowed_with_contexts=(PulpDebPackageContext, PulpDebReleaseComponentContext),
 )
 
 
 @pulp_group()
 @type_option(
     choices={
         "generic_content": PulpDebGenericContentContext,
@@ -268,20 +268,32 @@
         "--sha256",
         "artifact",
         required=True,
         help=_("Digest of the artifact to use"),
         callback=_sha256_artifact_callback,
         allowed_with_contexts=(PulpDebPackageContext,),
     ),
+    pulp_option(
+        "--distribution",
+        required=True,
+        help=_("The APT repo distribution to use"),
+        allowed_with_contexts=(PulpDebReleaseComponentContext,),
+    ),
+    pulp_option(
+        "--component",
+        required=True,
+        help=_("The APT repo component to use"),
+        allowed_with_contexts=(PulpDebReleaseComponentContext,),
+    ),
     repository_option,
 ]
 content.add_command(
     create_command(
         decorators=create_options,
-        allowed_with_contexts=(PulpDebPackageContext,),
+        allowed_with_contexts=(PulpDebPackageContext, PulpDebReleaseComponentContext),
     )
 )
 
 
 # upload takes a file-argument and creates the entity from it.
 # upload currently only works for packages.
 # This is a mypy bug getting confused with positional args
```

### Comparing `pulp-cli-deb-0.0.7/pulpcore/cli/deb/distribution.py` & `pulp-cli-deb-0.1.0/pulpcore/cli/deb/distribution.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-deb-0.0.7/pulpcore/cli/deb/locale/de/LC_MESSAGES/messages.mo` & `pulp-cli-deb-0.1.0/pulpcore/cli/deb/locale/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `pulp-cli-deb-0.0.7/pulpcore/cli/deb/publication.py` & `pulp-cli-deb-0.1.0/pulpcore/cli/deb/publication.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-deb-0.0.7/pulpcore/cli/deb/remote.py` & `pulp-cli-deb-0.1.0/pulpcore/cli/deb/remote.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     common_remote_update_options,
     create_command,
     destroy_command,
     href_option,
     label_command,
     label_select_option,
     list_command,
+    load_string_callback,
     name_option,
     pass_pulp_context,
     show_command,
     update_command,
 )
 
 translation = get_translation(__name__)
@@ -71,27 +72,37 @@
         click.option(
             "--distribution",
             "distributions",
             multiple=True,
             required=True,
             help=distribution_help,
         ),
+        click.option(
+            "--gpgkey",
+            help=_("Gpg public key to verify origin releases against or @file containing same."),
+            callback=load_string_callback,
+        ),
     ]
 )
 apt_remote_update_options = (
     lookup_options
     + common_remote_update_options
     + apt_remote_common_options
     + [
         click.option(
             "--distribution",
             "distributions",
             multiple=True,
             help=distribution_help,
         ),
+        click.option(
+            "--gpgkey",
+            help=_("Gpg public key to verify origin releases against or @file containing same."),
+            callback=load_string_callback,
+        ),
     ]
 )
 
 remote.add_command(list_command(decorators=[label_select_option]))
 remote.add_command(show_command(decorators=lookup_options))
 remote.add_command(create_command(decorators=apt_remote_create_options))
 remote.add_command(update_command(decorators=apt_remote_update_options))
```

### Comparing `pulp-cli-deb-0.0.7/pulpcore/cli/deb/repository.py` & `pulp-cli-deb-0.1.0/pulpcore/cli/deb/repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     list_command,
     name_option,
     pass_pulp_context,
     pass_repository_context,
     pulp_option,
     repository_content_command,
     repository_href_option,
-    repository_option,
+    repository_lookup_option,
     resource_option,
     retained_versions_option,
     show_command,
     update_command,
     version_command,
 )
 from pulpcore.cli.core.generic import task_command
@@ -89,15 +89,15 @@
 ]
 
 remote_option = resource_option(
     "--remote",
     default_plugin="deb",
     default_type="apt",
     context_table={"deb:apt": PulpAptRemoteContext},
-    needs_plugins=[PluginRequirement("deb", "2.12.0")],
+    needs_plugins=[PluginRequirement("deb", specifier=">=2.12.0")],
 )
 
 
 @click.group()
 @click.option(
     "-t",
     "--type",
@@ -111,21 +111,21 @@
     if repo_type == "apt":
         ctx.obj = PulpAptRepositoryContext(pulp_ctx)
     else:
         raise NotImplementedError()
 
 
 lookup_options = [href_option, name_option]
-nested_lookup_options = [repository_href_option, repository_option]
+nested_lookup_options = [repository_href_option, repository_lookup_option]
 update_options = [
     click.option("--description"),
     remote_option,
     # pulp_option(
     #     "--autopublish/--no-autopublish",
-    #     needs_plugins=[PluginRequirement("deb", "999.0.0")],
+    #     needs_plugins=[PluginRequirement("deb", specifier=">=999.0.0")],
     #     default=None,
     # ),
     retained_versions_option,
 ]
 create_options = update_options + [click.option("--name", required=True)]
 
 repository.add_command(list_command(decorators=[label_select_option]))
@@ -162,41 +162,37 @@
     "--optimize/--no-optimize",
     default=None,
     help=(
         "Using optimize sync, will skip the processing of metadata if the checksum has not changed "
         "since the last sync. This greately improves re-sync performance in such cases. Disable if "
         "the sync result does not match expectations."
     ),
-    needs_plugins=[PluginRequirement("deb", min="2.20.0.dev")],
+    needs_plugins=[PluginRequirement("deb", specifier=">=2.20.0")],
 )
 @pass_repository_context
 def sync(
     repository_ctx: PulpRepositoryContext,
     remote: EntityFieldDefinition,
     mirror: Optional[bool],
     optimize: Optional[bool],
 ) -> None:
     repository = repository_ctx.entity
-    repository_href = repository_ctx.pulp_href
 
     body: Dict[str, Any] = {}
 
     if mirror is not None:
         body["mirror"] = mirror
 
     if optimize is not None:
         body["optimize"] = optimize
 
     if isinstance(remote, PulpEntityContext):
-        body["remote"] = remote.pulp_href
+        body["remote"] = remote
     elif repository["remote"] is None:
         raise click.ClickException(
             _(
                 "Repository '{name}' does not have a default remote. "
                 "Please specify with '--remote'."
             ).format(name=repository["name"])
         )
 
-    repository_ctx.sync(
-        href=repository_href,
-        body=body,
-    )
+    repository_ctx.sync(body=body)
```

