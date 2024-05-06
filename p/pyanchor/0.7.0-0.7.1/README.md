# Comparing `tmp/pyanchor-0.7.0.tar.gz` & `tmp/pyanchor-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyanchor-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyanchor-0.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyanchor-0.7.0.tar` & `pyanchor-0.7.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       37 2023-11-06 20:53:30.682516 pyanchor-0.7.0/.coveragerc
--rw-r--r--   0        0        0       19 2023-11-06 20:53:30.682516 pyanchor-0.7.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      609 2023-11-06 20:53:30.682516 pyanchor-0.7.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      727 2023-11-06 20:53:30.682516 pyanchor-0.7.0/.github/workflows/run_tests.yml
--rw-r--r--   0        0        0     1829 2023-11-06 20:53:30.682516 pyanchor-0.7.0/.gitignore
--rw-r--r--   0        0        0     5226 2023-11-06 20:53:30.682516 pyanchor-0.7.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1078 2023-11-06 20:53:30.682516 pyanchor-0.7.0/LICENSE
--rw-r--r--   0        0        0     5062 2023-11-06 20:53:30.682516 pyanchor-0.7.0/README.md
--rw-r--r--   0        0        0    50295 2023-11-06 20:53:30.682516 pyanchor-0.7.0/assets/example-help.gif
--rw-r--r--   0        0        0    57660 2023-11-06 20:53:30.682516 pyanchor-0.7.0/assets/example-single-page-verbose.gif
--rw-r--r--   0        0        0    43821 2023-11-06 20:53:30.682516 pyanchor-0.7.0/assets/example-single-page.gif
--rw-r--r--   0        0        0   171021 2023-11-06 20:53:30.682516 pyanchor-0.7.0/assets/example-sitemap-verbose.gif
--rw-r--r--   0        0        0    59788 2023-11-06 20:53:30.682516 pyanchor-0.7.0/assets/example-sitemap.gif
--rw-r--r--   0        0        0       62 2023-11-06 20:53:30.682516 pyanchor-0.7.0/pyanchor/__init__.py
--rw-r--r--   0        0        0     2946 2023-11-06 20:53:30.682516 pyanchor-0.7.0/pyanchor/cli.py
--rw-r--r--   0        0        0     5802 2023-11-06 20:53:30.682516 pyanchor-0.7.0/pyanchor/link_checker.py
--rw-r--r--   0        0        0      936 2023-11-06 20:53:30.682516 pyanchor-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      156 2023-11-06 20:53:30.686516 pyanchor-0.7.0/pytest.ini
--rw-r--r--   0        0        0      306 2023-11-06 20:53:30.686516 pyanchor-0.7.0/requirements.in
--rw-r--r--   0        0        0    33829 2023-11-06 20:53:30.686516 pyanchor-0.7.0/requirements.txt
--rw-r--r--   0        0        0        0 2023-11-06 20:53:30.686516 pyanchor-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0      580 2023-11-06 20:53:30.686516 pyanchor-0.7.0/tests/conftest.py
--rw-r--r--   0        0        0     1139 2023-11-06 20:53:30.686516 pyanchor-0.7.0/tests/test_cli.py
--rw-r--r--   0        0        0     1427 2023-11-06 20:53:30.686516 pyanchor-0.7.0/tests/test_link_checker.py
--rw-r--r--   0        0        0       35 2023-11-06 20:53:30.686516 pyanchor-0.7.0/tests/test_webapp/.flaskenv
--rw-r--r--   0        0        0     1143 2023-11-06 20:53:30.686516 pyanchor-0.7.0/tests/test_webapp/app.py
--rw-r--r--   0        0        0      236 2023-11-06 20:53:30.686516 pyanchor-0.7.0/tests/test_webapp/templates/error.html
--rw-r--r--   0        0        0     1034 2023-11-06 20:53:30.686516 pyanchor-0.7.0/tests/test_webapp/templates/index.html
--rw-r--r--   0        0        0     1940 2023-11-06 20:53:30.686516 pyanchor-0.7.0/tests/test_webapp/templates/sitemap.xml
--rw-r--r--   0        0        0      371 2023-11-06 20:53:30.686516 pyanchor-0.7.0/tests/test_webapp/templates/success.html
--rw-r--r--   0        0        0     5950 1970-01-01 00:00:00.000000 pyanchor-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0       37 2024-05-06 21:17:39.909050 pyanchor-0.7.1/.coveragerc
+-rw-r--r--   0        0        0       19 2024-05-06 21:17:39.909050 pyanchor-0.7.1/.github/FUNDING.yml
+-rw-r--r--   0        0        0      609 2024-05-06 21:17:39.909050 pyanchor-0.7.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      727 2024-05-06 21:17:39.909050 pyanchor-0.7.1/.github/workflows/run_tests.yml
+-rw-r--r--   0        0        0     1829 2024-05-06 21:17:39.909050 pyanchor-0.7.1/.gitignore
+-rw-r--r--   0        0        0     5226 2024-05-06 21:17:39.909050 pyanchor-0.7.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1078 2024-05-06 21:17:39.909050 pyanchor-0.7.1/LICENSE
+-rw-r--r--   0        0        0     5062 2024-05-06 21:17:39.909050 pyanchor-0.7.1/README.md
+-rw-r--r--   0        0        0    50295 2024-05-06 21:17:39.909050 pyanchor-0.7.1/assets/example-help.gif
+-rw-r--r--   0        0        0    57660 2024-05-06 21:17:39.909050 pyanchor-0.7.1/assets/example-single-page-verbose.gif
+-rw-r--r--   0        0        0    43821 2024-05-06 21:17:39.909050 pyanchor-0.7.1/assets/example-single-page.gif
+-rw-r--r--   0        0        0   171021 2024-05-06 21:17:39.913050 pyanchor-0.7.1/assets/example-sitemap-verbose.gif
+-rw-r--r--   0        0        0    59788 2024-05-06 21:17:39.913050 pyanchor-0.7.1/assets/example-sitemap.gif
+-rw-r--r--   0        0        0       62 2024-05-06 21:17:39.913050 pyanchor-0.7.1/pyanchor/__init__.py
+-rw-r--r--   0        0        0     2946 2024-05-06 21:17:39.913050 pyanchor-0.7.1/pyanchor/cli.py
+-rw-r--r--   0        0        0     5802 2024-05-06 21:17:39.913050 pyanchor-0.7.1/pyanchor/link_checker.py
+-rw-r--r--   0        0        0      936 2024-05-06 21:17:39.913050 pyanchor-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      156 2024-05-06 21:17:39.913050 pyanchor-0.7.1/pytest.ini
+-rw-r--r--   0        0        0      306 2024-05-06 21:17:39.913050 pyanchor-0.7.1/requirements.in
+-rw-r--r--   0        0        0    33678 2024-05-06 21:17:39.913050 pyanchor-0.7.1/requirements.txt
+-rw-r--r--   0        0        0        0 2024-05-06 21:17:39.913050 pyanchor-0.7.1/tests/__init__.py
+-rw-r--r--   0        0        0      580 2024-05-06 21:17:39.913050 pyanchor-0.7.1/tests/conftest.py
+-rw-r--r--   0        0        0     1139 2024-05-06 21:17:39.913050 pyanchor-0.7.1/tests/test_cli.py
+-rw-r--r--   0        0        0     1427 2024-05-06 21:17:39.913050 pyanchor-0.7.1/tests/test_link_checker.py
+-rw-r--r--   0        0        0       35 2024-05-06 21:17:39.913050 pyanchor-0.7.1/tests/test_webapp/.flaskenv
+-rw-r--r--   0        0        0     1143 2024-05-06 21:17:39.913050 pyanchor-0.7.1/tests/test_webapp/app.py
+-rw-r--r--   0        0        0      236 2024-05-06 21:17:39.913050 pyanchor-0.7.1/tests/test_webapp/templates/error.html
+-rw-r--r--   0        0        0     1034 2024-05-06 21:17:39.913050 pyanchor-0.7.1/tests/test_webapp/templates/index.html
+-rw-r--r--   0        0        0     1940 2024-05-06 21:17:39.913050 pyanchor-0.7.1/tests/test_webapp/templates/sitemap.xml
+-rw-r--r--   0        0        0      371 2024-05-06 21:17:39.913050 pyanchor-0.7.1/tests/test_webapp/templates/success.html
+-rw-r--r--   0        0        0     5950 1970-01-01 00:00:00.000000 pyanchor-0.7.1/PKG-INFO
```

### Comparing `pyanchor-0.7.0/.github/workflows/release.yml` & `pyanchor-0.7.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.0/.github/workflows/run_tests.yml` & `pyanchor-0.7.1/.github/workflows/run_tests.yml`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.0/.gitignore` & `pyanchor-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.0/CODE_OF_CONDUCT.md` & `pyanchor-0.7.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.0/LICENSE` & `pyanchor-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.0/README.md` & `pyanchor-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.0/assets/example-help.gif` & `pyanchor-0.7.1/assets/example-help.gif`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.0/assets/example-single-page-verbose.gif` & `pyanchor-0.7.1/assets/example-single-page-verbose.gif`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.0/assets/example-single-page.gif` & `pyanchor-0.7.1/assets/example-single-page.gif`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.0/assets/example-sitemap-verbose.gif` & `pyanchor-0.7.1/assets/example-sitemap-verbose.gif`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.0/assets/example-sitemap.gif` & `pyanchor-0.7.1/assets/example-sitemap.gif`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.0/pyanchor/cli.py` & `pyanchor-0.7.1/pyanchor/cli.py`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.0/pyanchor/link_checker.py` & `pyanchor-0.7.1/pyanchor/link_checker.py`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.0/pyproject.toml` & `pyanchor-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.0/requirements.txt` & `pyanchor-0.7.1/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,40 +7,39 @@
 attrs==23.1.0 \
     --hash=sha256:1f28b4522cdc2fb4256ac1a020c78acf9cba2c6b461ccd2c126f3aa8e8335d04 \
     --hash=sha256:6279836d581513a26f1bf235f9acd333bc9115683f14f7e8fae46c98fc50e015
     # via pytest
 beautifulsoup4==4.11.1 \
     --hash=sha256:58d5c3d29f5a36ffeb94f02f0d786cd53014cf9b3b3951d42e0080d8a9498d30 \
     --hash=sha256:ad9aa55b65ef2808eb405f46cf74df7fcb7044d5cbc26487f96eb2ef2e436693
-    # via -r .\requirements.in
-black==22.6.0 \
-    --hash=sha256:074458dc2f6e0d3dab7928d4417bb6957bb834434516f21514138437accdbe90 \
-    --hash=sha256:187d96c5e713f441a5829e77120c269b6514418f4513a390b0499b0987f2ff1c \
-    --hash=sha256:2ea29072e954a4d55a2ff58971b83365eba5d3d357352a07a7a4df0d95f51c78 \
-    --hash=sha256:4af5bc0e1f96be5ae9bd7aaec219c901a94d6caa2484c21983d043371c733fc4 \
-    --hash=sha256:560558527e52ce8afba936fcce93a7411ab40c7d5fe8c2463e279e843c0328ee \
-    --hash=sha256:568ac3c465b1c8b34b61cd7a4e349e93f91abf0f9371eda1cf87194663ab684e \
-    --hash=sha256:6797f58943fceb1c461fb572edbe828d811e719c24e03375fd25170ada53825e \
-    --hash=sha256:6c1734ab264b8f7929cef8ae5f900b85d579e6cbfde09d7387da8f04771b51c6 \
-    --hash=sha256:6c6d39e28aed379aec40da1c65434c77d75e65bb59a1e1c283de545fb4e7c6c9 \
-    --hash=sha256:7ba9be198ecca5031cd78745780d65a3f75a34b2ff9be5837045dce55db83d1c \
-    --hash=sha256:94783f636bca89f11eb5d50437e8e17fbc6a929a628d82304c80fa9cd945f256 \
-    --hash=sha256:a218d7e5856f91d20f04e931b6f16d15356db1c846ee55f01bac297a705ca24f \
-    --hash=sha256:a3db5b6409b96d9bd543323b23ef32a1a2b06416d525d27e0f67e74f1446c8f2 \
-    --hash=sha256:ac609cf8ef5e7115ddd07d85d988d074ed00e10fbc3445aee393e70164a2219c \
-    --hash=sha256:b154e6bbde1e79ea3260c4b40c0b7b3109ffcdf7bc4ebf8859169a6af72cd70b \
-    --hash=sha256:b270a168d69edb8b7ed32c193ef10fd27844e5c60852039599f9184460ce0807 \
-    --hash=sha256:b9fd45787ba8aa3f5e0a0a98920c1012c884622c6c920dbe98dbd05bc7c70fbf \
-    --hash=sha256:c85928b9d5f83b23cee7d0efcb310172412fbf7cb9d9ce963bd67fd141781def \
-    --hash=sha256:c9a3ac16efe9ec7d7381ddebcc022119794872abce99475345c5a61aa18c45ad \
-    --hash=sha256:cfaf3895a9634e882bf9d2363fed5af8888802d670f58b279b0bece00e9a872d \
-    --hash=sha256:e439798f819d49ba1c0bd9664427a05aab79bfba777a6db94fd4e56fae0cb849 \
-    --hash=sha256:f586c26118bc6e714ec58c09df0157fe2d9ee195c764f630eb0d8e7ccce72e69 \
-    --hash=sha256:f6fe02afde060bbeef044af7996f335fbe90b039ccf3f5eb8f16df8b20f77666
-    # via -r .\requirements.in
+    # via -r requirements.in
+black==24.3.0 \
+    --hash=sha256:2818cf72dfd5d289e48f37ccfa08b460bf469e67fb7c4abb07edc2e9f16fb63f \
+    --hash=sha256:41622020d7120e01d377f74249e677039d20e6344ff5851de8a10f11f513bf93 \
+    --hash=sha256:4acf672def7eb1725f41f38bf6bf425c8237248bb0804faa3965c036f7672d11 \
+    --hash=sha256:4be5bb28e090456adfc1255e03967fb67ca846a03be7aadf6249096100ee32d0 \
+    --hash=sha256:4f1373a7808a8f135b774039f61d59e4be7eb56b2513d3d2f02a8b9365b8a8a9 \
+    --hash=sha256:56f52cfbd3dabe2798d76dbdd299faa046a901041faf2cf33288bc4e6dae57b5 \
+    --hash=sha256:65b76c275e4c1c5ce6e9870911384bff5ca31ab63d19c76811cb1fb162678213 \
+    --hash=sha256:65c02e4ea2ae09d16314d30912a58ada9a5c4fdfedf9512d23326128ac08ac3d \
+    --hash=sha256:6905238a754ceb7788a73f02b45637d820b2f5478b20fec82ea865e4f5d4d9f7 \
+    --hash=sha256:79dcf34b33e38ed1b17434693763301d7ccbd1c5860674a8f871bd15139e7837 \
+    --hash=sha256:7bb041dca0d784697af4646d3b62ba4a6b028276ae878e53f6b4f74ddd6db99f \
+    --hash=sha256:7d5e026f8da0322b5662fa7a8e752b3fa2dac1c1cbc213c3d7ff9bdd0ab12395 \
+    --hash=sha256:9f50ea1132e2189d8dff0115ab75b65590a3e97de1e143795adb4ce317934995 \
+    --hash=sha256:a0c9c4a0771afc6919578cec71ce82a3e31e054904e7197deacbc9382671c41f \
+    --hash=sha256:aadf7a02d947936ee418777e0247ea114f78aff0d0959461057cae8a04f20597 \
+    --hash=sha256:b5991d523eee14756f3c8d5df5231550ae8993e2286b8014e2fdea7156ed0959 \
+    --hash=sha256:bf21b7b230718a5f08bd32d5e4f1db7fc8788345c8aea1d155fc17852b3410f5 \
+    --hash=sha256:c45f8dff244b3c431b36e3224b6be4a127c6aca780853574c00faf99258041eb \
+    --hash=sha256:c7ed6668cbbfcd231fa0dc1b137d3e40c04c7f786e626b405c62bcd5db5857e4 \
+    --hash=sha256:d7de8d330763c66663661a1ffd432274a2f92f07feeddd89ffd085b5744f85e7 \
+    --hash=sha256:e19cb1c6365fd6dc38a6eae2dcb691d7d83935c10215aef8e6c38edee3f77abd \
+    --hash=sha256:e2af80566f43c85f5797365077fb64a393861a3730bd110971ab7a0c94e873e7
+    # via -r requirements.in
 certifi==2023.7.22 \
     --hash=sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082 \
     --hash=sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9
     # via requests
 charset-normalizer==3.3.2 \
     --hash=sha256:06435b539f889b1f6f4ac1758871aae42dc3a8c0e24ac9e60c2384973ad73027 \
     --hash=sha256:06a81e93cd441c56a9b65d8e1d043daeb97a3d0856d177d5c90ba85acb3db087 \
@@ -139,18 +138,15 @@
     # via
     #   black
     #   flask
     #   typer
 colorama==0.4.5 \
     --hash=sha256:854bf444933e37f5824ae7bfc1e98d5bce2ebe4160d46b5edf346a89358e99da \
     --hash=sha256:e6c6b4334fc50988a639d9b98aa429a0b57da6e17b9a44f0451f930b6967b7a4
-    # via
-    #   -r .\requirements.in
-    #   click
-    #   pytest
+    # via -r requirements.in
 coverage[toml]==7.3.2 \
     --hash=sha256:0cbf38419fb1a347aaf63481c00f0bdc86889d9fbf3f25109cf96c26b403fda1 \
     --hash=sha256:12d15ab5833a997716d76f2ac1e4b4d536814fc213c85ca72756c19e5a6b3d63 \
     --hash=sha256:149de1d2401ae4655c436a3dced6dd153f4c3309f599c3d4bd97ab172eaf02d9 \
     --hash=sha256:1981f785239e4e39e6444c63a98da3a1db8e971cb9ceb50a945ba6296b43f312 \
     --hash=sha256:2443cbda35df0d35dcfb9bf8f3c02c57c1d6111169e3c85fc1fcc05e0c9f39a3 \
     --hash=sha256:289fe43bf45a575e3ab10b26d7b6f2ddb9ee2dba447499f5401cfb5ecb8196bb \
@@ -196,52 +192,50 @@
     --hash=sha256:e10c39c0452bf6e694511c901426d6b5ac005acc0f78ff265dbe36bf81f808a2 \
     --hash=sha256:e267e9e2b574a176ddb983399dec325a80dbe161f1a32715c780b5d14b5f583a \
     --hash=sha256:f47d39359e2c3779c5331fc740cf4bce6d9d680a7b4b4ead97056a0ae07cb49a \
     --hash=sha256:f6e9589bd04d0461a417562649522575d8752904d35c12907d8c9dfeba588faf \
     --hash=sha256:f94b734214ea6a36fe16e96a70d941af80ff3bfd716c141300d95ebc85339738 \
     --hash=sha256:fa28e909776dc69efb6ed975a63691bc8172b64ff357e663a1bb06ff3c9b589a \
     --hash=sha256:fe494faa90ce6381770746077243231e0b83ff3f17069d748f645617cefe19d4
-    # via
-    #   coverage
-    #   pytest-cov
+    # via pytest-cov
 docutils==0.20.1 \
     --hash=sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6 \
     --hash=sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b
     # via flit
 exceptiongroup==1.1.3 \
     --hash=sha256:097acd85d473d75af5bb98e41b61ff7fe35efe6675e4f9370ec6ec5126d160e9 \
     --hash=sha256:343280667a4585d195ca1cf9cef84a4e178c4b6cf2274caef9859782b567d5e3
-    # via -r .\requirements.in
+    # via -r requirements.in
 flask==2.2.5 \
     --hash=sha256:58107ed83443e86067e41eff4631b058178191a355886f8e479e347fa1285fdf \
     --hash=sha256:edee9b0a7ff26621bd5a8c10ff484ae28737a2410d99b0bb9a6850c7fb977aa0
-    # via -r .\requirements.in
+    # via -r requirements.in
 flit==3.7.1 \
     --hash=sha256:06a93a6737fa9380ba85fe8d7f28efb6c93c4f4ee9c7d00cc3375a81f33b91a4 \
     --hash=sha256:3c9bd9c140515bfe62dd938c6610d10d6efb9e35cc647fc614fe5fb3a5036682
-    # via -r .\requirements.in
+    # via -r requirements.in
 flit-core==3.9.0 \
     --hash=sha256:72ad266176c4a3fcfab5f2930d76896059851240570ce9a98733b658cb786eba \
     --hash=sha256:7aada352fb0c7f5538c4fafeddf314d3a6a92ee8e2b1de70482329e42de70301
     # via flit
-idna==3.4 \
-    --hash=sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4 \
-    --hash=sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2
+idna==3.7 \
+    --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
+    --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
     # via requests
 iniconfig==2.0.0 \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
     # via pytest
 itsdangerous==2.1.2 \
     --hash=sha256:2c2349112351b88699d8d4b6b075022c0808887cb7ad10069318a8b0bc88db44 \
     --hash=sha256:5dbbc68b317e5e42f327f9021763545dc3fc3bfe22e6deb96aaf1fc38874156a
     # via flask
-jinja2==3.1.2 \
-    --hash=sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852 \
-    --hash=sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61
+jinja2==3.1.4 \
+    --hash=sha256:4a3aee7acbbe7303aede8e9648d13b8bf88a429282aa6122a993f0ac800cb369 \
+    --hash=sha256:bc5dd2abb727a5319567b7a813e6a2e7318c39f4f487cfe6c89c6f9c7d25197d
     # via flask
 lxml==4.9.3 \
     --hash=sha256:05186a0f1346ae12553d66df1cfce6f251589fea3ad3da4f3ef4e34b2d58c6a3 \
     --hash=sha256:075b731ddd9e7f68ad24c635374211376aa05a281673ede86cbe1d1b3455279d \
     --hash=sha256:081d32421db5df44c41b7f08a334a090a545c54ba977e47fd7cc2deece78809a \
     --hash=sha256:0a3d3487f07c1d7f150894c238299934a2a074ef590b583103a45002035be120 \
     --hash=sha256:0bfd0767c5c1de2551a120673b72e5d4b628737cb05414f03c3277bf9bed3305 \
@@ -328,15 +322,15 @@
     --hash=sha256:ed667f49b11360951e201453fc3967344d0d0263aa415e1619e85ae7fd17b4e0 \
     --hash=sha256:f3df3db1d336b9356dd3112eae5f5c2b8b377f3bc826848567f10bfddfee77e9 \
     --hash=sha256:f6bdac493b949141b733c5345b6ba8f87a226029cbabc7e9e121a413e49441e0 \
     --hash=sha256:fbf521479bcac1e25a663df882c46a641a9bff6b56dc8b0fafaebd2f66fb231b \
     --hash=sha256:fc9b106a1bf918db68619fdcd6d5ad4f972fdd19c01d19bdb6bf63f3589a9ec5 \
     --hash=sha256:fcdd00edfd0a3001e0181eab3e63bd5c74ad3e67152c84f93f13769a40e073a7 \
     --hash=sha256:fe4bda6bd4340caa6e5cf95e73f8fea5c4bfc55763dd42f1b50a94c1b4a2fbd4
-    # via -r .\requirements.in
+    # via -r requirements.in
 markupsafe==2.1.3 \
     --hash=sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e \
     --hash=sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e \
     --hash=sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431 \
     --hash=sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686 \
     --hash=sha256:14ff806850827afd6b07a5f32bd917fb7f45b046ba40c57abdb636674a8b559c \
     --hash=sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559 \
@@ -400,15 +394,17 @@
 mypy-extensions==1.0.0 \
     --hash=sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d \
     --hash=sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782
     # via black
 packaging==23.2 \
     --hash=sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5 \
     --hash=sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7
-    # via pytest
+    # via
+    #   black
+    #   pytest
 pathspec==0.11.2 \
     --hash=sha256:1d6ed233af05e679efb96b1851550ea95bbb64b7c490b0f5aa52996c11e92a20 \
     --hash=sha256:e0d8d0ac2f12da61956eb2306b69f9469b42f4deb0f3cb6ed47b9cce9996ced3
     # via black
 platformdirs==3.11.0 \
     --hash=sha256:cf8ee52a3afdb965072dcc652433e0c7e3e40cf5ea1477cd4b3b1d2eb75495b3 \
     --hash=sha256:e9d171d00af68be50e9202731309c4e658fd8bc76f55c11c7dd760d023bda68e
@@ -417,29 +413,29 @@
     --hash=sha256:cf61ae8f126ac6f7c451172cf30e3e43d3ca77615509771b3a984a0730651e12 \
     --hash=sha256:d89c696a773f8bd377d18e5ecda92b7a3793cbe66c87060a6fb58c7b6e1061f7
     # via pytest
 pytest==7.2.0 \
     --hash=sha256:892f933d339f068883b6fd5a459f03d85bfcb355e4981e146d2c7616c21fef71 \
     --hash=sha256:c4014eb40e10f11f355ad4e3c2fb2c6c6d1919c73f3b5a433de4708202cade59
     # via
-    #   -r .\requirements.in
+    #   -r requirements.in
     #   pytest-cov
 pytest-cov==3.0.0 \
     --hash=sha256:578d5d15ac4a25e5f961c938b85a05b09fdaae9deef3bb6de9a6e766622ca7a6 \
     --hash=sha256:e7f0f5b1617d2210a2cabc266dfe2f4c75a8d32fb89eafb7ad9d06f6d076d470
-    # via -r .\requirements.in
+    # via -r requirements.in
 python-dotenv==0.20.0 \
     --hash=sha256:b7e3b04a59693c42c36f9ab1cc2acc46fa5df8c78e178fc33a8d4cd05c8d498f \
     --hash=sha256:d92a187be61fe482e4fd675b6d52200e7be63a12b724abbf931a40ce4fa92938
-    # via -r .\requirements.in
+    # via -r requirements.in
 requests==2.31.0 \
     --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
     --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
     # via
-    #   -r .\requirements.in
+    #   -r requirements.in
     #   flit
 soupsieve==2.5 \
     --hash=sha256:5663d5a7b3bfaeee0bc4372e7fc48f9cff4940b3eec54a6451cc5299f1097690 \
     --hash=sha256:eaa337ff55a1579b6549dc679565eac1e3d000563bcb1c8ab0d0fefbc0c2cdc7
     # via beautifulsoup4
 tomli==2.0.1 \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
@@ -448,21 +444,21 @@
 tomli-w==1.0.0 \
     --hash=sha256:9f2a07e8be30a0729e533ec968016807069991ae2fd921a78d42f429ae5f4463 \
     --hash=sha256:f463434305e0336248cac9c2dc8076b707d8a12d019dd349f5c1e382dd1ae1b9
     # via flit
 typer==0.5.0 \
     --hash=sha256:4c285a5585c94d32c305444af934f0078b6a8ba91464f3f85807c91cd499d195 \
     --hash=sha256:a34409c0029ba7e48cb9e4f54c6400bf4158a6145b5dea32788e7a36ebbcb312
-    # via -r .\requirements.in
+    # via -r requirements.in
 typing-extensions==3.10.0.0 \
     --hash=sha256:0ac0f89795dd19de6b97debb0c6af1c70987fd80a2d62d1958f7e56fcc31b497 \
     --hash=sha256:50b6f157849174217d0656f99dc82fe932884fb250826c18350e159ec6cdf342 \
     --hash=sha256:779383f6086d90c99ae41cf0ff39aac8a7937a9283ce0a414e5dd782f4c94a84
-    # via -r .\requirements.in
+    # via -r requirements.in
 urllib3==2.0.7 \
     --hash=sha256:c97dfde1f7bd43a71c8d2a58e369e9b2bf692d1334ea9f9cae55add7d0dd0f84 \
     --hash=sha256:fdb6d215c776278489906c2f8916e6e7d4f5a9b602ccbcfdf7f016fc8da0596e
     # via requests
-werkzeug==3.0.1 \
-    --hash=sha256:507e811ecea72b18a404947aded4b3390e1db8f826b494d76550ef45bb3b1dcc \
-    --hash=sha256:90a285dc0e42ad56b34e696398b8122ee4c681833fb35b8334a095d82c56da10
+werkzeug==3.0.3 \
+    --hash=sha256:097e5bfda9f0aba8da6b8545146def481d06aa7d3266e7448e2cccf67dd8bd18 \
+    --hash=sha256:fc9645dc43e03e4d630d23143a04a7f947a9a3b5727cd535fdfe155a17cc48c8
     # via flask
```

### Comparing `pyanchor-0.7.0/tests/conftest.py` & `pyanchor-0.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.0/tests/test_cli.py` & `pyanchor-0.7.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.0/tests/test_link_checker.py` & `pyanchor-0.7.1/tests/test_link_checker.py`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.0/tests/test_webapp/app.py` & `pyanchor-0.7.1/tests/test_webapp/app.py`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.0/tests/test_webapp/templates/index.html` & `pyanchor-0.7.1/tests/test_webapp/templates/index.html`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.0/tests/test_webapp/templates/sitemap.xml` & `pyanchor-0.7.1/tests/test_webapp/templates/sitemap.xml`

 * *Files identical despite different names*

### Comparing `pyanchor-0.7.0/PKG-INFO` & `pyanchor-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyanchor
-Version: 0.7.0
+Version: 0.7.1
 Summary: Check you site for broken links!
 Home-page: https://github.com/EndlessTrax/pyanchor/
 Author: Ricky White
 Author-email: ricky@whitelionmedia.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyanchor Version: 0.7.0 Summary: Check you site for
+Metadata-Version: 2.1 Name: pyanchor Version: 0.7.1 Summary: Check you site for
 broken links! Home-page: https://github.com/EndlessTrax/pyanchor/ Author: Ricky
 White Author-email: ricky@whitelionmedia.com Requires-Python: >=3.8
 Description-Content-Type: text/markdown Classifier: License :: OSI Approved ::
 MIT License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: beautifulsoup4==4.11.1
```

