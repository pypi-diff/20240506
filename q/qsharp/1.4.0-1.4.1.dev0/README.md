# Comparing `tmp/qsharp-1.4.0-cp37-abi3-win_arm64.whl.zip` & `tmp/qsharp-1.4.1.dev0-cp37-abi3-win_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 1603175 bytes, number of entries: 14
--rw-r--r--  4.6 unx     2093 b- defN 24-Apr-23 18:12 qsharp-1.4.0.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 24-Apr-23 18:12 qsharp-1.4.0.dist-info/WHEEL
--rw-r--r--  4.6 unx     3090 b- defN 24-Apr-23 18:12 qsharp/.data/qsharp_codemirror.js
--rw-r--r--  4.6 unx    38836 b- defN 24-Apr-23 18:12 qsharp/estimator/_estimator.py
--rw-r--r--  4.6 unx      859 b- defN 24-Apr-23 18:12 qsharp/estimator/__init__.py
--rw-r--r--  4.6 unx     1706 b- defN 24-Apr-23 18:12 qsharp/utils/_utils.py
--rw-r--r--  4.6 unx      146 b- defN 24-Apr-23 18:12 qsharp/utils/__init__.py
--rw-r--r--  4.6 unx      864 b- defN 24-Apr-23 18:12 qsharp/_fs.py
--rw-r--r--  4.6 unx     1848 b- defN 24-Apr-23 18:12 qsharp/_ipython.py
--rw-r--r--  4.6 unx     6375 b- defN 24-Apr-23 18:12 qsharp/_native.pyi
--rw-r--r--  4.6 unx    13210 b- defN 24-Apr-23 18:12 qsharp/_qsharp.py
--rw-r--r--  4.6 unx      902 b- defN 24-Apr-23 18:12 qsharp/__init__.py
--rwxr-xr-x  4.6 unx  3898880 b- defN 24-Apr-23 18:12 qsharp/_native.pyd
--rw-r--r--  4.6 unx     1070 b- defN 24-Apr-23 18:12 qsharp-1.4.0.dist-info/RECORD
-14 files, 3969973 bytes uncompressed, 1601435 bytes compressed:  59.7%
+Zip file size: 1635517 bytes, number of entries: 14
+-rw-r--r--  4.6 unx     2098 b- defN 24-May-06 21:41 qsharp-1.4.1.dev0.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 24-May-06 21:41 qsharp-1.4.1.dev0.dist-info/WHEEL
+-rw-r--r--  4.6 unx     3090 b- defN 24-May-06 21:41 qsharp/.data/qsharp_codemirror.js
+-rw-r--r--  4.6 unx    38836 b- defN 24-May-06 21:41 qsharp/estimator/_estimator.py
+-rw-r--r--  4.6 unx      859 b- defN 24-May-06 21:41 qsharp/estimator/__init__.py
+-rw-r--r--  4.6 unx     1706 b- defN 24-May-06 21:41 qsharp/utils/_utils.py
+-rw-r--r--  4.6 unx      146 b- defN 24-May-06 21:41 qsharp/utils/__init__.py
+-rw-r--r--  4.6 unx      864 b- defN 24-May-06 21:41 qsharp/_fs.py
+-rw-r--r--  4.6 unx     1848 b- defN 24-May-06 21:41 qsharp/_ipython.py
+-rw-r--r--  4.6 unx     6436 b- defN 24-May-06 21:41 qsharp/_native.pyi
+-rw-r--r--  4.6 unx    12818 b- defN 24-May-06 21:41 qsharp/_qsharp.py
+-rw-r--r--  4.6 unx      902 b- defN 24-May-06 21:41 qsharp/__init__.py
+-rwxr-xr-x  4.6 unx  3973120 b- defN 24-May-06 21:41 qsharp/_native.pyd
+-rw-r--r--  4.6 unx     1085 b- defN 24-May-06 21:41 qsharp-1.4.1.dev0.dist-info/RECORD
+14 files, 4043902 bytes uncompressed, 1633747 bytes compressed:  59.6%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
-Filename: qsharp-1.4.0.dist-info/METADATA
+Filename: qsharp-1.4.1.dev0.dist-info/METADATA
 Comment: 
 
-Filename: qsharp-1.4.0.dist-info/WHEEL
+Filename: qsharp-1.4.1.dev0.dist-info/WHEEL
 Comment: 
 
 Filename: qsharp/.data/qsharp_codemirror.js
 Comment: 
 
 Filename: qsharp/estimator/_estimator.py
 Comment: 
@@ -33,11 +33,11 @@
 
 Filename: qsharp/__init__.py
 Comment: 
 
 Filename: qsharp/_native.pyd
 Comment: 
 
-Filename: qsharp-1.4.0.dist-info/RECORD
+Filename: qsharp-1.4.1.dev0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qsharp/_native.pyi

```diff
@@ -16,17 +16,18 @@
     """
     Target supports the minimal set of capabilities required to run a quantum
     program.
 
     This option maps to the Base Profile as defined by the QIR specification.
     """
 
-    Quantinuum: ClassVar[Any]
+    Adaptive_RI: ClassVar[Any]
     """
-    Target supports Quantinuum profile.
+    Target supports the Adaptive profile with integer computation and qubit
+    reset capabilities.
 
     This profile includes all of the required Adaptive Profile
     capabilities, as well as the optional integer computation and qubit
     reset capabilities, as defined by the QIR specification.
     """
 
     Unrestricted: ClassVar[Any]
```

## qsharp/_qsharp.py

```diff
@@ -19,25 +19,31 @@
 
 class Config:
     _config: Dict[str, str]
     """
     Configuration hints for the language service.
     """
 
-    def __init__(self, target_profile: TargetProfile, language_features: List[str]):
-        if target_profile == TargetProfile.Quantinuum:
-            self._config = {"targetProfile": "quantinuum"}
-            warn("The Quantinuum target profile is a preview feature.")
+    def __init__(
+        self,
+        target_profile: TargetProfile,
+        language_features: Optional[List[str]],
+        manifest: Optional[str],
+    ):
+        if target_profile == TargetProfile.Adaptive_RI:
+            self._config = {"targetProfile": "adaptive_ri"}
+            warn("The Adaptive_RI target profile is a preview feature.")
             warn("Functionality may be incomplete or incorrect.")
         elif target_profile == TargetProfile.Base:
             self._config = {"targetProfile": "base"}
         elif target_profile == TargetProfile.Unrestricted:
             self._config = {"targetProfile": "unrestricted"}
 
         self._config["languageFeatures"] = language_features
+        self._config["manifest"] = manifest
 
     def __repr__(self) -> str:
         return "Q# initialized with configuration: " + str(self._config)
 
     # See https://ipython.readthedocs.io/en/stable/config/integrating.html#rich-display
     # See https://ipython.org/ipython-doc/3/notebook/nbformat.html#display-data
     # This returns a custom MIME-type representation of the Q# configuration.
@@ -51,15 +57,15 @@
         return {"application/x.qsharp-config": self._config}
 
 
 def init(
     *,
     target_profile: TargetProfile = TargetProfile.Unrestricted,
     project_root: Optional[str] = None,
-    language_features: List[str] = [],
+    language_features: Optional[List[str]] = None,
 ) -> Config:
     """
     Initializes the Q# interpreter.
 
     :param target_profile: Setting the target profile allows the Q#
         interpreter to generate programs that are compatible
         with a specific target. See :py:class: `qsharp.TargetProfile`.
@@ -67,57 +73,45 @@
     :param project_root: An optional path to a root directory with a Q# project to include.
         It must contain a qsharp.json project manifest.
     """
     from ._fs import read_file, list_directory, exists, join
 
     global _interpreter
 
+    manifest_contents = None
     manifest_descriptor = None
     if project_root is not None:
         qsharp_json = join(project_root, "qsharp.json")
         if not exists(qsharp_json):
             raise QSharpError(
                 f"{qsharp_json} not found. qsharp.json should exist at the project root and be a valid JSON file."
             )
 
         manifest_descriptor = {}
         manifest_descriptor["manifest_dir"] = project_root
 
         try:
-            (_, file_contents) = read_file(qsharp_json)
+            (_, manifest_contents) = read_file(qsharp_json)
+            manifest_descriptor["manifest"] = manifest_contents
         except Exception as e:
             raise QSharpError(
                 f"Error reading {qsharp_json}. qsharp.json should exist at the project root and be a valid JSON file."
             ) from e
 
-        try:
-            manifest_descriptor["manifest"] = json.loads(file_contents)
-        except Exception as e:
-            raise QSharpError(
-                f"Error parsing {qsharp_json}. qsharp.json should exist at the project root and be a valid JSON file."
-            ) from e
-
-    # if no features were passed in as an argument, use the features from the manifest.
-    # this way we prefer the features from the argument over those from the manifest.
-    if language_features == [] and manifest_descriptor != None:
-        language_features = (
-            manifest_descriptor["manifest"].get("languageFeatures") or []
-        )
-
     _interpreter = Interpreter(
         target_profile,
         language_features,
         manifest_descriptor,
         read_file,
         list_directory,
     )
 
     # Return the configuration information to provide a hint to the
     # language service through the cell output.
-    return Config(target_profile, language_features)
+    return Config(target_profile, language_features, manifest_contents)
 
 
 def get_interpreter() -> Interpreter:
     """
     Returns the Q# interpreter.
 
     :returns: The Q# interpreter.
```

## Comparing `qsharp-1.4.0.dist-info/METADATA` & `qsharp-1.4.1.dev0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsharp
-Version: 1.4.0
+Version: 1.4.1.dev0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

## Comparing `qsharp-1.4.0.dist-info/RECORD` & `qsharp-1.4.1.dev0.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-qsharp-1.4.0.dist-info/METADATA,sha256=ZEpIxSR52tfMtiXNU1HDRJnTlr82FC71QTi2AJ8VFs0,2093
-qsharp-1.4.0.dist-info/WHEEL,sha256=xsrEGIMmQ1avWDJ2-RvHLDam8haXzwGnBhrUlFUsLAc,94
+qsharp-1.4.1.dev0.dist-info/METADATA,sha256=Q6w9fa-VldVCe4qGp50ayWtIHcBBLbm-k2YOMUF1tPg,2098
+qsharp-1.4.1.dev0.dist-info/WHEEL,sha256=xsrEGIMmQ1avWDJ2-RvHLDam8haXzwGnBhrUlFUsLAc,94
 qsharp/.data/qsharp_codemirror.js,sha256=72E3fTxGxfBe_bBhPD5-8ul_S61MLVA_JmMJwOXgmhc,3090
 qsharp/estimator/_estimator.py,sha256=LMTJg2xPwhvswlc0ts0zsjRPd82mF5KzYgmHyFFl2PE,38836
 qsharp/estimator/__init__.py,sha256=JK6oDnNX_rgsPnfyFsK0yxMBRinmW8jlc8183BydxXA,859
 qsharp/utils/_utils.py,sha256=s3ausLf4wp08rgRDrcdzSXOYPRQ63isX0umCA9MIq7M,1706
 qsharp/utils/__init__.py,sha256=ejBPCXRttEGKCDehjldx8SryqQfNHXsgsRFK5O-zRU8,146
 qsharp/_fs.py,sha256=RGhwMRUwfxGoPVEPaP39FxyRcPeZoyhB0kb4MwzxE54,864
 qsharp/_ipython.py,sha256=x8J7HatTw15xTg9Ppd-yRmhNz9eY8cBAhruRiHo46bQ,1848
-qsharp/_native.pyi,sha256=w0bBah7mtOnoLcchXMfMoH6PJaf1Bm0lmSJe8574s4U,6375
-qsharp/_qsharp.py,sha256=JcD5z7mFKtvhZ9cX8xUWrGd268tEmyTHJGSWq5gclOs,13210
+qsharp/_native.pyi,sha256=dC3H1V_TpWMVTfDjViMQtWhRELrbMOVFyLzkH1yUN7Q,6436
+qsharp/_qsharp.py,sha256=J-qEF-D2x54NLHdEfnc3GU4FgsLSFF7jplVDiiF-Kkg,12818
 qsharp/__init__.py,sha256=-KmJgZV8ZRqWSIOENAhyE39vYF5eZ_p4W04XZ29YKfs,902
-qsharp/_native.pyd,sha256=9zxfJEZMxSv1YGvpXDGBsIq8s2RNkfGBdhhOApn_EG8,3898880
-qsharp-1.4.0.dist-info/RECORD,,
+qsharp/_native.pyd,sha256=LMpQEicy3E8am90H_4tRc2xGTvc1-brcPVNVkdyANsg,3973120
+qsharp-1.4.1.dev0.dist-info/RECORD,,
```

