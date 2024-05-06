# Comparing `tmp/distro2sbom-0.4.5-py2.py3-none-any.whl.zip` & `tmp/distro2sbom-0.4.6-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 21786 bytes, number of entries: 15
+Zip file size: 21985 bytes, number of entries: 15
 -rw-r--r--  2.0 unx       76 b- defN 23-Mar-23 23:04 distro2sbom/__init__.py
--rw-r--r--  2.0 unx     7852 b- defN 24-May-03 08:50 distro2sbom/cli.py
+-rw-r--r--  2.0 unx     8198 b- defN 24-May-06 08:43 distro2sbom/cli.py
 -rw-r--r--  2.0 unx      462 b- defN 23-Jul-23 20:45 distro2sbom/test.py
--rw-r--r--  2.0 unx      100 b- defN 24-May-03 08:46 distro2sbom/version.py
+-rw-r--r--  2.0 unx      100 b- defN 24-May-06 08:16 distro2sbom/version.py
 -rw-r--r--  2.0 unx       76 b- defN 23-Mar-23 23:04 distro2sbom/distrobuilder/__init__.py
--rw-r--r--  2.0 unx     3246 b- defN 24-May-03 08:46 distro2sbom/distrobuilder/distrobuilder.py
--rw-r--r--  2.0 unx    13584 b- defN 24-May-03 08:38 distro2sbom/distrobuilder/dpkgbuilder.py
--rw-r--r--  2.0 unx    14116 b- defN 24-May-03 08:46 distro2sbom/distrobuilder/rpmbuilder.py
+-rw-r--r--  2.0 unx     3483 b- defN 24-May-06 08:43 distro2sbom/distrobuilder/distrobuilder.py
+-rw-r--r--  2.0 unx    13690 b- defN 24-May-06 08:45 distro2sbom/distrobuilder/dpkgbuilder.py
+-rw-r--r--  2.0 unx    14207 b- defN 24-May-06 08:43 distro2sbom/distrobuilder/rpmbuilder.py
 -rw-r--r--  2.0 unx     4688 b- defN 24-May-03 08:39 distro2sbom/distrobuilder/windowsbuilder.py
--rw-r--r--  2.0 unx    11357 b- defN 24-May-03 08:50 distro2sbom-0.4.5.dist-info/LICENSE
--rw-r--r--  2.0 unx    11863 b- defN 24-May-03 08:50 distro2sbom-0.4.5.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-May-03 08:50 distro2sbom-0.4.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 24-May-03 08:50 distro2sbom-0.4.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 24-May-03 08:50 distro2sbom-0.4.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1300 b- defN 24-May-03 08:50 distro2sbom-0.4.5.dist-info/RECORD
-15 files, 68895 bytes uncompressed, 19612 bytes compressed:  71.5%
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-06 08:50 distro2sbom-0.4.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx    12163 b- defN 24-May-06 08:50 distro2sbom-0.4.6.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-May-06 08:50 distro2sbom-0.4.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 24-May-06 08:50 distro2sbom-0.4.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 24-May-06 08:50 distro2sbom-0.4.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1300 b- defN 24-May-06 08:50 distro2sbom-0.4.6.dist-info/RECORD
+15 files, 69975 bytes uncompressed, 19811 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -21,26 +21,26 @@
 
 Filename: distro2sbom/distrobuilder/rpmbuilder.py
 Comment: 
 
 Filename: distro2sbom/distrobuilder/windowsbuilder.py
 Comment: 
 
-Filename: distro2sbom-0.4.5.dist-info/LICENSE
+Filename: distro2sbom-0.4.6.dist-info/LICENSE
 Comment: 
 
-Filename: distro2sbom-0.4.5.dist-info/METADATA
+Filename: distro2sbom-0.4.6.dist-info/METADATA
 Comment: 
 
-Filename: distro2sbom-0.4.5.dist-info/WHEEL
+Filename: distro2sbom-0.4.6.dist-info/WHEEL
 Comment: 
 
-Filename: distro2sbom-0.4.5.dist-info/entry_points.txt
+Filename: distro2sbom-0.4.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: distro2sbom-0.4.5.dist-info/top_level.txt
+Filename: distro2sbom-0.4.6.dist-info/top_level.txt
 Comment: 
 
-Filename: distro2sbom-0.4.5.dist-info/RECORD
+Filename: distro2sbom-0.4.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## distro2sbom/cli.py

```diff
@@ -40,15 +40,14 @@
                 os.environ.get("PATH", "").split(":"),
             )
         )
     )
 
 
 def main(argv=None):
-
     argv = argv or sys.argv
     app_name = "distro2sbom"
     parser = argparse.ArgumentParser(
         prog=app_name,
         description=textwrap.dedent(
             """
             Distro2Sbom generates a Software Bill of Materials for the
@@ -96,14 +95,19 @@
         help="generate SBOM for installed system",
     )
     input_group.add_argument(
         "--root",
         action="store",
         help="location of distribution packages",
     )
+    input_group.add_argument(
+        "--distro-namespace",
+        action="store",
+        help="namespace for distribution",
+    )
 
     output_group = parser.add_argument_group("Output")
     output_group.add_argument(
         "-d",
         "--debug",
         action="store_true",
         default=False,
@@ -141,15 +145,16 @@
         "sbom": "spdx",
         "debug": False,
         "format": "tag",
         "name": None,
         "release": None,
         "package": "",
         "system": False,
-        "root" : ""
+        "root": "",
+        "distro_namespace": "",
     }
 
     raw_args = parser.parse_args(argv[1:])
     args = {key: value for key, value in vars(raw_args).items() if value}
     args = ChainMap(args, defaults)
 
     # Validate CLI parameters
@@ -175,14 +180,15 @@
 
     if args["debug"]:
         print("Distro type:", args["distro"])
         print("Input file:", args["input_file"])
         print("Distro name:", args["name"])
         print("Distro release:", args["release"])
         print("Distro root:", args["root"])
+        print("Distro namespace:", args["distro_namespace"])
         print("Package:", args["package"])
         print("System SBOM:", args["system"])
         print("SBOM type:", args["sbom"])
         print("Format:", bom_format)
         print("Output file:", args["output_file"])
 
     if args["distro"] == "auto":
@@ -201,20 +207,25 @@
         if args["package"] > "" and not inpath(required_apps[distro_type]):
             print(
                 "[ERROR] Unable to produce package information for specified distribution."
             )
             return -1
 
     if distro_type == "deb":
-        sbom_build = DpkgBuilder(args["name"], args["release"], args["debug"], root=args["root"])
+        sbom_build = DpkgBuilder(
+            args["name"], args["release"], args["debug"], root=args["root"]
+        )
     elif distro_type == "rpm":
         sbom_build = RpmBuilder(args["name"], args["release"], args["debug"])
     elif distro_type == "windows":
         sbom_build = WindowsBuilder(args["name"], args["release"], args["debug"])
 
+    if args["distro_namespace"] != "":
+        sbom_build.set_namespace(args["distro_namespace"])
+
     if args["input_file"] != "":
         # Check file exists
         filePath = Path(args["input_file"])
         # Check path exists and is a valid file
         if filePath.exists() and filePath.is_file():
             # Assume that processing can proceed
             sbom_build.parse_data(args["input_file"])
```

## distro2sbom/version.py

```diff
@@ -1,4 +1,4 @@
 # Copyright (C) 2024 Anthony Harrison
 # SPDX-License-Identifier: Apache-2.0
 
-VERSION: str = "0.4.5"
+VERSION: str = "0.4.6"
```

## distro2sbom/distrobuilder/distrobuilder.py

```diff
@@ -9,15 +9,16 @@
 
 
 class DistroBuilder:
     def __init__(self, debug=False):
         self.sbom_packages = {}
         self.sbom_relationships = []
         self.debug = debug
-        self.root = os.environ.get('DISTRO2SBOM_ROOT_PATH', '')
+        self.root = os.environ.get("DISTRO2SBOM_ROOT_PATH", "")
+        self.namespace = ""
 
     def get_data(self):
         pass
 
     def parse_data(self):
         pass
 
@@ -79,7 +80,15 @@
             os_file = open(OS_FILE)
             lines = os_file.readlines()
             for line in lines:
                 if len(line.strip()) > 0:
                     data = line.split("=")
                     metadata[data[0].lower()] = data[1].replace('"', "").strip()
         return metadata
+
+    def set_namespace(self, namespace):
+        self.namespace = namespace
+
+    def get_namespace(self):
+        if self.namespace != "":
+            return f"{self.namespace}/"
+        return self.namespace
```

## distro2sbom/distrobuilder/dpkgbuilder.py

```diff
@@ -22,15 +22,15 @@
         if name is None and release is None:
             self.name = self.system_data["name"].replace(" ", "-")
             self.release = self.system_data["version_id"]
         else:
             self.name = name.replace(" ", "-")
             self.release = release
         self.parent = f"Distro-{self.name}"
-        self.root=root
+        self.root = root
 
     def parse_data(self, filename):
         # Process file containing installed applications
         with open(filename) as dir_file:
             lines = dir_file.readlines()
         if len(lines) > 0:
             # Something to process
@@ -95,15 +95,15 @@
     def get(self, attribute):
         if attribute in self.metadata:
             return self.metadata[attribute].lstrip()
         return ""
 
     def get_metadata_from_file(self, package):
         # Location of Debian copyright files
-        base_file = f"/usr/share/doc/{package}/copyright"
+        base_file = f"{self.root}/usr/share/doc/{package}/copyright"
         copyright_text = ""
         license_text = "NOASSERTION"
         filename = Path(base_file)
         # Check path exists and is a valid file
         if filename.exists() and filename.is_file():
             with open(filename, "r") as f:
                 lines = f.readlines()
@@ -126,18 +126,19 @@
                         if len(license_info) > 0:
                             license_text = license_info
                             license_found = True
 
         return license_text, copyright_text
 
     def dpkg_command(self, command_string):
-        command = f"dpkg"
+        command = "dpkg"
         if self.root != "":
-            command=f"{command} --root {self.root}"
+            command = f"{command} --root {self.root}"
         return self.run_program(f"{command} {command_string}")
+
     def process_package(self, package_name, parent="-"):
         if self.debug:
             print(f"Process package {package_name}. Parent {parent}")
         # Check if we have already processed this package
         if package_name in self.distro_packages:
             self.sbom_relationship.initialise()
             self.sbom_relationship.set_relationship(
@@ -198,19 +199,23 @@
             if self.get("Description") != "":
                 self.sbom_package.set_summary(self.get("Description"))
             if self.get("Homepage") != "":
                 self.sbom_package.set_homepage(self.get("Homepage"))
             # Add copyright information
             if len(copyright) > 0:
                 self.sbom_package.set_copyrighttext(copyright)
-            self.sbom_package.set_purl(f"pkg:deb/{package}@{version}")
+            self.sbom_package.set_purl(
+                f"pkg:deb/{self.get_namespace()}{package}@{version}"
+            )
             if len(supplier) > 1:
                 component_supplier = self.format_supplier(supplier, include_email=False)
-                cpe_version = version.replace(':','\\:')
-                self.sbom_package.set_cpe(f"cpe:2.3:a:{component_supplier.replace(' ', '_').lower()}:{package}:{cpe_version}:*:*:*:*:*:*:*")
+                cpe_version = version.replace(":", "\\:")
+                self.sbom_package.set_cpe(
+                    f"cpe:2.3:a:{component_supplier.replace(' ', '_').lower()}:{package}:{cpe_version}:*:*:*:*:*:*:*"
+                )
             # Store package data
             self.sbom_packages[
                 (self.sbom_package.get_name(), self.sbom_package.get_value("version"))
             ] = self.sbom_package.get_package()
             # Add relationship
             self.sbom_relationship.initialise()
             if parent != "-":
```

## distro2sbom/distrobuilder/rpmbuilder.py

```diff
@@ -22,16 +22,16 @@
         if name is None and release is None:
             self.name = self.system_data["name"].replace(" ", "-")
             self.release = self.system_data["version_id"]
         else:
             self.name = name.replace(" ", "-")
             self.release = release
         self.parent = f"Distro-{self.name}"
-        self.rpm_options = os.environ.get('DISTRO2SBOM_RPM_OPTIONS', '')
-        self.yum_options = os.environ.get('DISTRO2SBOM_YUM_OPTIONS', '')
+        self.rpm_options = os.environ.get("DISTRO2SBOM_RPM_OPTIONS", "")
+        self.yum_options = os.environ.get("DISTRO2SBOM_YUM_OPTIONS", "")
 
     def get_data(self):
         pass
 
     def parse_data(self, filename):
         # Process file containing installed applications
         with open(filename) as dir_file:
@@ -203,19 +203,23 @@
             else:
                 self.sbom_package.set_supplier("UNKNOWN", "NOASSERTION")
             if self.get("Summary") != "":
                 self.sbom_package.set_summary(self.get("Summary"))
             if self.get("URL") != "":
                 self.sbom_package.set_homepage(self.get("URL"))
             # External references
-            self.sbom_package.set_purl(f"pkg:rpm/{package}@{version}")
+            self.sbom_package.set_purl(
+                f"pkg:rpm/{self.get_namespace()}{package}@{version}"
+            )
             if len(supplier) > 1:
                 component_supplier = self.format_supplier(supplier, include_email=False)
-                cpe_version = version.replace(':','\\:')
-                self.sbom_package.set_cpe(f"cpe:2.3:a:{component_supplier.replace(' ', '_').lower()}:{package}:{cpe_version}:*:*:*:*:*:*:*")
+                cpe_version = version.replace(":", "\\:")
+                self.sbom_package.set_cpe(
+                    f"cpe:2.3:a:{component_supplier.replace(' ', '_').lower()}:{package}:{cpe_version}:*:*:*:*:*:*:*"
+                )
             # Store package data
             self.sbom_packages[
                 (self.sbom_package.get_name(), self.sbom_package.get_value("version"))
             ] = self.sbom_package.get_package()
             # Add relationship
             self.sbom_relationship.initialise()
             if parent != "-":
```

## Comparing `distro2sbom-0.4.5.dist-info/LICENSE` & `distro2sbom-0.4.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `distro2sbom-0.4.5.dist-info/METADATA` & `distro2sbom-0.4.6.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: distro2sbom
-Version: 0.4.5
+Version: 0.4.6
 Summary: SBOM generator for system distribution
 Home-page: https://github.com/anthonyharrison/distro2sbom
 Author: Anthony Harrison
 Author-email: anthony.p.harrison@gmail.com
 Maintainer: Anthony Harrison
 Maintainer-email: anthony.p.harrison@gmail.com
 License: Apache-2.0
@@ -50,16 +50,16 @@
 if you are using different versions of python. `virtualenv` is a tool for setting up virtual python environments which
 allows you to have all the dependencies for the tool set up in a single environment, or have different environments set
 up for testing using different versions of Python.
 
 ## Usage
 
 ```
-usage: distro2sbom [-h] [--distro {rpm,deb,windows,auto}] [-i INPUT_FILE] [-n NAME] [-r RELEASE] [-p PACKAGE] [-s] [--root ROOT] 
-                   [-d] [--sbom {spdx,cyclonedx}] [--format {tag,json,yaml}] [-o OUTPUT_FILE] [-V]
+usage: distro2sbom [-h] [--distro {rpm,deb,windows,auto}] [-i INPUT_FILE] [-n NAME] [-r RELEASE] [-p PACKAGE] [-s] [--root ROOT] [--distro-namespace DISTRO_NAMESPACE] [-d] [--sbom {spdx,cyclonedx}]
+                   [--format {tag,json,yaml}] [-o OUTPUT_FILE] [-V]
 
 Distro2Sbom generates a Software Bill of Materials for the specified package or distribution.
 
 options:
   -h, --help            show this help message and exit
   -V, --version         show program's version number and exit
 
@@ -71,14 +71,16 @@
   -n NAME, --name NAME  name of distribution
   -r RELEASE, --release RELEASE
                         release identity of distribution
   -p PACKAGE, --package PACKAGE
                         identity of package within distribution
   -s, --system          generate SBOM for installed system
   --root ROOT           location of distribution packages
+  --distro-namespace DISTRO_NAMESPACE
+                        namespace for distribution
 
 Output:
   -d, --debug           add debug information
   --sbom {spdx,cyclonedx}
                         specify type of sbom to generate (default: spdx)
   --format {tag,json,yaml}
                         specify format of software bill of materials (sbom) (default: tag)
@@ -152,14 +154,16 @@
 This option is not supported if the `--distro` option is set to 'windows'.
 
 The `--system` option is used to generate an SBOM for all the applications installed on the system. Note that this option will take some time to complete as it is dependent on the number of installed applications.
 This option is not supported if the `--distro` option is set to 'windows'.
 
 The `--root` option is used to specify an alternative directory location for the installed packages. This option only applies for 'deb' distributions.
 
+The `--disto-namespace` option is used to specify a namespace to be included in the generated [PURL](https://github.com/package-url/purl-spec) identifiers for the packages.
+
 At least one of the `--input-file`, `--package` or `--system` options must be specified. If multiple options are specified, the `--input-file` option followed by the `--system` option will be assumed.
 
 The `--sbom` option is used to specify the format of the generated SBOM (the default is SPDX). The `--format` option
 can be used to specify the formatting of the SBOM (the default is Tag Value format for a SPDX SBOM). JSON format is supported for both
 SPDX and CycloneDX SBOMs.
 
 The `--output-file` option is used to control the destination of the output generated by the tool. The
```

## Comparing `distro2sbom-0.4.5.dist-info/RECORD` & `distro2sbom-0.4.6.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 distro2sbom/__init__.py,sha256=UXoScW29szuUhsP-AvPIJLEPeX_U31M1gxYUSooemy8,76
-distro2sbom/cli.py,sha256=Yvt0o09GKRhWMnKsjFUbQBUMpHvn0iTCiJxiEZ3tc9c,7852
+distro2sbom/cli.py,sha256=cop3JRp7jnBrMCsbKnrq8oDquijFAK9Wr14f6S8OkB8,8198
 distro2sbom/test.py,sha256=m8yYYiZq9QUIqcNAKQOGPvboIvnZ8WrZUH2ELMm4c4E,462
-distro2sbom/version.py,sha256=RhzVdAnIAIeNpoZLjlCpx5ZgkvJyztkiWp-TZKe5hDc,100
+distro2sbom/version.py,sha256=KxkwQjgAzKRSXN26UOvPkrvpNQxLbFUq87labC4nDlA,100
 distro2sbom/distrobuilder/__init__.py,sha256=UXoScW29szuUhsP-AvPIJLEPeX_U31M1gxYUSooemy8,76
-distro2sbom/distrobuilder/distrobuilder.py,sha256=x_s_YoojCQsV5rUzdzSrzpd1zxXaXXM1G1AaRDZ-N4M,3246
-distro2sbom/distrobuilder/dpkgbuilder.py,sha256=70Et6Su52hUbmMSsL_m0Jf7Oxytsk-OTT1fnabnQLUA,13584
-distro2sbom/distrobuilder/rpmbuilder.py,sha256=p2Kphbayy_C6Vvd86xL2qzWMtRFEm_PIbSFhbt7wLc8,14116
+distro2sbom/distrobuilder/distrobuilder.py,sha256=km5suBxuVuJJWzKGi5aN_FQ1bLRLYrvtVd8cG1a0qas,3483
+distro2sbom/distrobuilder/dpkgbuilder.py,sha256=pVy23fsa0Jlvg95asp4Xm8lCt9PX986uCVUD-x1hFfY,13690
+distro2sbom/distrobuilder/rpmbuilder.py,sha256=jBCNkhqhCMcM7X7pCUpt4PKNYCm1gqBBF4wrmQN_Cdc,14207
 distro2sbom/distrobuilder/windowsbuilder.py,sha256=P-1xTEqHZHTEGobkbycf_Wgfa2KhlPRx5MqKVcQPLFY,4688
-distro2sbom-0.4.5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-distro2sbom-0.4.5.dist-info/METADATA,sha256=xCHP_ZP-Sw3iQwJHDVz01G41UvKqGbVuvWvKYBDz6eY,11863
-distro2sbom-0.4.5.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-distro2sbom-0.4.5.dist-info/entry_points.txt,sha256=r5RioA3bp_Kbd1UJ5L1BTfSea9qEISrGmoSKSAHFBOU,53
-distro2sbom-0.4.5.dist-info/top_level.txt,sha256=wj3FBpfTya_uiJ4egUDQ4vv-BO5G5swycPOUc7qymJM,12
-distro2sbom-0.4.5.dist-info/RECORD,,
+distro2sbom-0.4.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+distro2sbom-0.4.6.dist-info/METADATA,sha256=dcXQ2aaImEj5USpfZ-ynxt3Eq5iaBQbe_p11ObjS850,12163
+distro2sbom-0.4.6.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+distro2sbom-0.4.6.dist-info/entry_points.txt,sha256=r5RioA3bp_Kbd1UJ5L1BTfSea9qEISrGmoSKSAHFBOU,53
+distro2sbom-0.4.6.dist-info/top_level.txt,sha256=wj3FBpfTya_uiJ4egUDQ4vv-BO5G5swycPOUc7qymJM,12
+distro2sbom-0.4.6.dist-info/RECORD,,
```

