# Comparing `tmp/psl-2024.4.8.tar.gz` & `tmp/psl-2024.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psl-2024.4.8.tar", last modified: Mon Apr  8 13:04:11 2024, max compression
+gzip compressed data, was "psl-2024.5.6.tar", last modified: Mon May  6 13:04:35 2024, max compression
```

## Comparing `psl-2024.4.8.tar` & `psl-2024.5.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:04:11.621859 psl-2024.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-08 13:03:43.000000 psl-2024.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-08 13:03:43.000000 psl-2024.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-08 13:04:11.621859 psl-2024.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-08 13:03:43.000000 psl-2024.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:04:11.621859 psl-2024.4.8/psl/
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-08 13:03:50.000000 psl-2024.4.8/psl/__init__.py
--rw-------   0 runner    (1001) docker     (127)   131388 2024-04-08 13:03:50.000000 psl-2024.4.8/psl/psl.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 13:03:43.000000 psl-2024.4.8/psl/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 13:04:11.621859 psl-2024.4.8/psl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-08 13:04:11.000000 psl-2024.4.8/psl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-08 13:04:11.000000 psl-2024.4.8/psl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:04:11.000000 psl-2024.4.8/psl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 13:04:01.000000 psl-2024.4.8/psl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-08 13:04:11.000000 psl-2024.4.8/psl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 13:04:11.621859 psl-2024.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-08 13:03:43.000000 psl-2024.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:04:35.715896 psl-2024.5.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-05-06 13:04:09.000000 psl-2024.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-06 13:04:09.000000 psl-2024.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-06 13:04:35.715896 psl-2024.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-06 13:04:09.000000 psl-2024.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:04:35.715896 psl-2024.5.6/psl/
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-06 13:04:15.000000 psl-2024.5.6/psl/__init__.py
+-rw-------   0 runner    (1001) docker     (127)   133574 2024-05-06 13:04:15.000000 psl-2024.5.6/psl/psl.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 13:04:09.000000 psl-2024.5.6/psl/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 13:04:35.715896 psl-2024.5.6/psl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-05-06 13:04:35.000000 psl-2024.5.6/psl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-06 13:04:35.000000 psl-2024.5.6/psl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 13:04:35.000000 psl-2024.5.6/psl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 13:04:25.000000 psl-2024.5.6/psl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-06 13:04:35.000000 psl-2024.5.6/psl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 13:04:35.715896 psl-2024.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-06 13:04:09.000000 psl-2024.5.6/setup.py
```

### Comparing `psl-2024.4.8/LICENSE` & `psl-2024.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `psl-2024.4.8/PKG-INFO` & `psl-2024.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psl
-Version: 2024.4.8
+Version: 2024.5.6
 Summary: Mozilla Public Suffix list as a Python package and updated daily
 Home-page: https://github.com/sethmlarson/psl
 Author: Seth Michael Larson
 Author-email: sethmichaellarson@gmail.com
 License: MPL-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `psl-2024.4.8/README.md` & `psl-2024.5.6/README.md`

 * *Files identical despite different names*

### Comparing `psl-2024.4.8/psl/__init__.py` & `psl-2024.5.6/psl/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import functools
 import pathlib
 import typing
 
-__version__ = "2024.4.8"
-__checksum__ = "99c4f4f86c43fc0696efa7094e54a82ae3dec72a"
+__version__ = "2024.5.6"
+__checksum__ = "7c0c6cfa0fe6e11d438448a2b8c76092ae19abfa"
 __all__ = ["PUBLIC_SUFFIX_URL", "domain_suffixes", "Suffixes", "domain_can_set_cookie"]
 
 
 PUBLIC_SUFFIX_URL = "https://publicsuffix.org/list/public_suffix_list.dat"
 _PUBLIC_SUFFIX_PATH = pathlib.Path(__file__).parent / "psl.txt"
```

### Comparing `psl-2024.4.8/psl/psl.txt` & `psl-2024.5.6/psl/psl.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6872,14 +6872,15 @@
 12chars.dev
 12chars.it
 12chars.pro
 cc.ua
 inf.ua
 ltd.ua
 611.to
+aaa.vodka
 a2hosted.com
 cpserver.com
 graphox.us
 *.devcdnaccesso.com
 *.on-acorn.io
 activetrail.biz
 adaptable.app
@@ -6955,25 +6956,30 @@
 execute-api.us-west-2.amazonaws.com
 cloudfront.net
 auth.af-south-1.amazoncognito.com
 auth.ap-northeast-1.amazoncognito.com
 auth.ap-northeast-2.amazoncognito.com
 auth.ap-northeast-3.amazoncognito.com
 auth.ap-south-1.amazoncognito.com
+auth.ap-south-2.amazoncognito.com
 auth.ap-southeast-1.amazoncognito.com
 auth.ap-southeast-2.amazoncognito.com
 auth.ap-southeast-3.amazoncognito.com
+auth.ap-southeast-4.amazoncognito.com
 auth.ca-central-1.amazoncognito.com
 auth.eu-central-1.amazoncognito.com
+auth.eu-central-2.amazoncognito.com
 auth.eu-north-1.amazoncognito.com
 auth.eu-south-1.amazoncognito.com
+auth.eu-south-2.amazoncognito.com
 auth.eu-west-1.amazoncognito.com
 auth.eu-west-2.amazoncognito.com
 auth.eu-west-3.amazoncognito.com
 auth.il-central-1.amazoncognito.com
+auth.me-central-1.amazoncognito.com
 auth.me-south-1.amazoncognito.com
 auth.sa-east-1.amazoncognito.com
 auth.us-east-1.amazoncognito.com
 auth-fips.us-east-1.amazoncognito.com
 auth.us-east-2.amazoncognito.com
 auth-fips.us-east-2.amazoncognito.com
 auth-fips.us-gov-west-1.amazoncognito.com
@@ -7005,44 +7011,62 @@
 emrstudio-prod.ap-northeast-2.amazonaws.com
 emrappui-prod.ap-northeast-3.amazonaws.com
 emrnotebooks-prod.ap-northeast-3.amazonaws.com
 emrstudio-prod.ap-northeast-3.amazonaws.com
 emrappui-prod.ap-south-1.amazonaws.com
 emrnotebooks-prod.ap-south-1.amazonaws.com
 emrstudio-prod.ap-south-1.amazonaws.com
+emrappui-prod.ap-south-2.amazonaws.com
+emrnotebooks-prod.ap-south-2.amazonaws.com
+emrstudio-prod.ap-south-2.amazonaws.com
 emrappui-prod.ap-southeast-1.amazonaws.com
 emrnotebooks-prod.ap-southeast-1.amazonaws.com
 emrstudio-prod.ap-southeast-1.amazonaws.com
 emrappui-prod.ap-southeast-2.amazonaws.com
 emrnotebooks-prod.ap-southeast-2.amazonaws.com
 emrstudio-prod.ap-southeast-2.amazonaws.com
 emrappui-prod.ap-southeast-3.amazonaws.com
 emrnotebooks-prod.ap-southeast-3.amazonaws.com
 emrstudio-prod.ap-southeast-3.amazonaws.com
+emrappui-prod.ap-southeast-4.amazonaws.com
+emrnotebooks-prod.ap-southeast-4.amazonaws.com
+emrstudio-prod.ap-southeast-4.amazonaws.com
 emrappui-prod.ca-central-1.amazonaws.com
 emrnotebooks-prod.ca-central-1.amazonaws.com
 emrstudio-prod.ca-central-1.amazonaws.com
+emrappui-prod.ca-west-1.amazonaws.com
+emrnotebooks-prod.ca-west-1.amazonaws.com
+emrstudio-prod.ca-west-1.amazonaws.com
 emrappui-prod.eu-central-1.amazonaws.com
 emrnotebooks-prod.eu-central-1.amazonaws.com
 emrstudio-prod.eu-central-1.amazonaws.com
+emrappui-prod.eu-central-2.amazonaws.com
+emrnotebooks-prod.eu-central-2.amazonaws.com
+emrstudio-prod.eu-central-2.amazonaws.com
 emrappui-prod.eu-north-1.amazonaws.com
 emrnotebooks-prod.eu-north-1.amazonaws.com
 emrstudio-prod.eu-north-1.amazonaws.com
 emrappui-prod.eu-south-1.amazonaws.com
 emrnotebooks-prod.eu-south-1.amazonaws.com
 emrstudio-prod.eu-south-1.amazonaws.com
+emrappui-prod.eu-south-2.amazonaws.com
+emrnotebooks-prod.eu-south-2.amazonaws.com
+emrstudio-prod.eu-south-2.amazonaws.com
 emrappui-prod.eu-west-1.amazonaws.com
 emrnotebooks-prod.eu-west-1.amazonaws.com
 emrstudio-prod.eu-west-1.amazonaws.com
 emrappui-prod.eu-west-2.amazonaws.com
 emrnotebooks-prod.eu-west-2.amazonaws.com
 emrstudio-prod.eu-west-2.amazonaws.com
 emrappui-prod.eu-west-3.amazonaws.com
 emrnotebooks-prod.eu-west-3.amazonaws.com
 emrstudio-prod.eu-west-3.amazonaws.com
+emrappui-prod.il-central-1.amazonaws.com
+emrnotebooks-prod.il-central-1.amazonaws.com
+emrstudio-prod.il-central-1.amazonaws.com
 emrappui-prod.me-central-1.amazonaws.com
 emrnotebooks-prod.me-central-1.amazonaws.com
 emrstudio-prod.me-central-1.amazonaws.com
 emrappui-prod.me-south-1.amazonaws.com
 emrnotebooks-prod.me-south-1.amazonaws.com
 emrstudio-prod.me-south-1.amazonaws.com
 emrappui-prod.sa-east-1.amazonaws.com
@@ -7064,28 +7088,33 @@
 emrnotebooks-prod.us-west-1.amazonaws.com
 emrstudio-prod.us-west-1.amazonaws.com
 emrappui-prod.us-west-2.amazonaws.com
 emrnotebooks-prod.us-west-2.amazonaws.com
 emrstudio-prod.us-west-2.amazonaws.com
 *.cn-north-1.airflow.amazonaws.com.cn
 *.cn-northwest-1.airflow.amazonaws.com.cn
+*.af-south-1.airflow.amazonaws.com
+*.ap-east-1.airflow.amazonaws.com
 *.ap-northeast-1.airflow.amazonaws.com
 *.ap-northeast-2.airflow.amazonaws.com
 *.ap-south-1.airflow.amazonaws.com
 *.ap-southeast-1.airflow.amazonaws.com
 *.ap-southeast-2.airflow.amazonaws.com
 *.ca-central-1.airflow.amazonaws.com
 *.eu-central-1.airflow.amazonaws.com
 *.eu-north-1.airflow.amazonaws.com
+*.eu-south-1.airflow.amazonaws.com
 *.eu-west-1.airflow.amazonaws.com
 *.eu-west-2.airflow.amazonaws.com
 *.eu-west-3.airflow.amazonaws.com
+*.me-south-1.airflow.amazonaws.com
 *.sa-east-1.airflow.amazonaws.com
 *.us-east-1.airflow.amazonaws.com
 *.us-east-2.airflow.amazonaws.com
+*.us-west-1.airflow.amazonaws.com
 *.us-west-2.airflow.amazonaws.com
 s3.dualstack.cn-north-1.amazonaws.com.cn
 s3-accesspoint.dualstack.cn-north-1.amazonaws.com.cn
 s3-website.dualstack.cn-north-1.amazonaws.com.cn
 s3.cn-north-1.amazonaws.com.cn
 s3-accesspoint.cn-north-1.amazonaws.com.cn
 s3-deprecated.cn-north-1.amazonaws.com.cn
@@ -7366,14 +7395,26 @@
 s3.us-west-2.amazonaws.com
 s3-accesspoint.us-west-2.amazonaws.com
 s3-accesspoint-fips.us-west-2.amazonaws.com
 s3-deprecated.us-west-2.amazonaws.com
 s3-fips.us-west-2.amazonaws.com
 s3-object-lambda.us-west-2.amazonaws.com
 s3-website.us-west-2.amazonaws.com
+labeling.ap-northeast-1.sagemaker.aws
+labeling.ap-northeast-2.sagemaker.aws
+labeling.ap-south-1.sagemaker.aws
+labeling.ap-southeast-1.sagemaker.aws
+labeling.ap-southeast-2.sagemaker.aws
+labeling.ca-central-1.sagemaker.aws
+labeling.eu-central-1.sagemaker.aws
+labeling.eu-west-1.sagemaker.aws
+labeling.eu-west-2.sagemaker.aws
+labeling.us-east-1.sagemaker.aws
+labeling.us-east-2.sagemaker.aws
+labeling.us-west-2.sagemaker.aws
 notebook.af-south-1.sagemaker.aws
 notebook.ap-east-1.sagemaker.aws
 notebook.ap-northeast-1.sagemaker.aws
 notebook.ap-northeast-2.sagemaker.aws
 notebook.ap-northeast-3.sagemaker.aws
 notebook.ap-south-1.sagemaker.aws
 notebook.ap-south-2.sagemaker.aws
@@ -7402,14 +7443,15 @@
 notebook.us-east-2.sagemaker.aws
 notebook-fips.us-east-2.sagemaker.aws
 notebook.us-gov-east-1.sagemaker.aws
 notebook-fips.us-gov-east-1.sagemaker.aws
 notebook.us-gov-west-1.sagemaker.aws
 notebook-fips.us-gov-west-1.sagemaker.aws
 notebook.us-west-1.sagemaker.aws
+notebook-fips.us-west-1.sagemaker.aws
 notebook.us-west-2.sagemaker.aws
 notebook-fips.us-west-2.sagemaker.aws
 notebook.cn-north-1.sagemaker.com.cn
 notebook.cn-northwest-1.sagemaker.com.cn
 studio.af-south-1.sagemaker.aws
 studio.ap-east-1.sagemaker.aws
 studio.ap-northeast-1.sagemaker.aws
@@ -7419,14 +7461,15 @@
 studio.ap-southeast-1.sagemaker.aws
 studio.ap-southeast-2.sagemaker.aws
 studio.ap-southeast-3.sagemaker.aws
 studio.ca-central-1.sagemaker.aws
 studio.eu-central-1.sagemaker.aws
 studio.eu-north-1.sagemaker.aws
 studio.eu-south-1.sagemaker.aws
+studio.eu-south-2.sagemaker.aws
 studio.eu-west-1.sagemaker.aws
 studio.eu-west-2.sagemaker.aws
 studio.eu-west-3.sagemaker.aws
 studio.il-central-1.sagemaker.aws
 studio.me-central-1.sagemaker.aws
 studio.me-south-1.sagemaker.aws
 studio.sa-east-1.sagemaker.aws
@@ -7513,14 +7556,15 @@
 webview-assets.cloud9.us-east-2.amazonaws.com
 webview-assets.aws-cloud9.us-west-1.amazonaws.com
 vfs.cloud9.us-west-1.amazonaws.com
 webview-assets.cloud9.us-west-1.amazonaws.com
 webview-assets.aws-cloud9.us-west-2.amazonaws.com
 vfs.cloud9.us-west-2.amazonaws.com
 webview-assets.cloud9.us-west-2.amazonaws.com
+awsapps.com
 cn-north-1.eb.amazonaws.com.cn
 cn-northwest-1.eb.amazonaws.com.cn
 elasticbeanstalk.com
 af-south-1.elasticbeanstalk.com
 ap-east-1.elasticbeanstalk.com
 ap-northeast-1.elasticbeanstalk.com
 ap-northeast-2.elasticbeanstalk.com
@@ -7569,14 +7613,15 @@
 poivron.org
 potager.org
 sweetpepper.org
 myasustor.com
 cdn.prod.atlassian-dev.net
 translated.page
 autocode.dev
+myfritz.link
 myfritz.net
 onavstack.net
 *.awdev.ca
 *.advisor.ws
 ecommerce-shop.pl
 b-data.io
 backplaneapp.io
@@ -7595,14 +7640,15 @@
 theshop.jp
 shopselect.net
 base.shop
 beagleboard.io
 *.beget.app
 pages.gay
 betainabox.com
+bielsko.pl
 bnr.la
 bitbucket.io
 blackbaudcdn.net
 of.je
 bluebite.io
 boomla.net
 boutir.com
@@ -7610,14 +7656,15 @@
 square7.ch
 bplaced.com
 bplaced.de
 square7.de
 bplaced.net
 square7.net
 *.s.brave.io
+shop.brendly.hr
 shop.brendly.rs
 browsersafetymark.io
 uk0.bigv.io
 dh.bytemark.co.uk
 vm.bytemark.co.uk
 cafjs.com
 mycd.eu
@@ -7692,36 +7739,52 @@
 *.cloudera.site
 cf-ipfs.com
 cloudflare-ipfs.com
 trycloudflare.com
 pages.dev
 r2.dev
 workers.dev
+cust.cloudscale.ch
+objects.lpg.cloudscale.ch
+objects.rma.cloudscale.ch
 wnext.app
 co.ca
 *.otap.co
 co.cz
-c.cdn77.org
+cdn77-storage.com
+rsc.contentproxy9.cz
 cdn77-ssl.net
 r.cdn77.net
-rsc.cdn77.org
 ssl.origin.cdn77-secure.org
+c.cdn77.org
+rsc.cdn77.org
 cloudns.asia
+cloudns.be
 cloudns.biz
-cloudns.club
 cloudns.cc
+cloudns.ch
+cloudns.cl
+cloudns.club
+dnsabr.com
+cloudns.cx
 cloudns.eu
 cloudns.in
 cloudns.info
+dns-cloud.net
+dns-dynamic.net
+cloudns.nz
 cloudns.org
+cloudns.ph
 cloudns.pro
 cloudns.pw
 cloudns.us
 cnpy.gdn
 codeberg.page
+csb.app
+preview.csb.app
 co.nl
 co.no
 webhosting.be
 hosting-cluster.nl
 convex.site
 ac.ru
 edu.ru
@@ -7770,14 +7833,15 @@
 firm.dk
 reg.dk
 store.dk
 dyndns.dappnode.io
 *.dapps.earth
 *.bzz.dapps.earth
 builtwithdark.com
+darklang.io
 demo.datadetect.com
 instance.datadetect.com
 edgestack.me
 ddns5.com
 debian.net
 deno.dev
 deno-staging.dev
@@ -8091,14 +8155,15 @@
 dyn.home-webserver.de
 myhome-server.de
 ddnss.org
 definima.net
 definima.io
 ondigitalocean.app
 *.digitaloceanspaces.com
+us.kg
 bci.dnstrace.pro
 ddnsfree.com
 ddnsgeek.com
 giize.com
 gleeze.com
 kozow.com
 loseyourip.com
@@ -8114,14 +8179,16 @@
 myddns.rocks
 blogsite.xyz
 dynv6.net
 e4.cz
 easypanel.app
 easypanel.host
 *.ewp.live
+at.emf.camp
+rt.ht
 elementor.cloud
 elementor.cool
 en-root.fr
 mytuleap.com
 tuleap-partners.com
 encr.app
 encoreapi.com
@@ -8316,14 +8383,15 @@
 flutterflow.app
 fly.dev
 edgeapp.net
 shw.io
 flynnhosting.net
 forgeblocks.com
 id.forgerock.io
+framer.ai
 framer.app
 framercanvas.com
 framer.media
 framer.photos
 framer.website
 framer.wiki
 *.frusky.de
@@ -8334,14 +8402,29 @@
 fbx-os.fr
 fbxos.fr
 freebox-os.fr
 freeboxos.fr
 freedesktop.org
 freemyip.com
 wien.funkfeuer.at
+daemon.asia
+dix.asia
+mydns.bz
+0am.jp
+0g0.jp
+0j0.jp
+0t0.jp
+mydns.jp
+pgw.jp
+wjg.jp
+keyword-on.net
+live-on.net
+server-on.net
+mydns.tw
+mydns.vc
 *.futurecms.at
 *.ex.futurecms.at
 *.in.futurecms.at
 futurehosting.at
 futuremailing.at
 *.ex.ortsinfo.at
 *.kunden.ortsinfo.at
@@ -8359,15 +8442,17 @@
 api.gov.uk
 gehirn.ne.jp
 usercontent.jp
 gentapps.com
 gentlentapis.com
 lab.ms
 cdn-edges.net
-ghost.io
+localcert.net
+localhostcert.net
+corpnet.work
 gsj.bz
 githubusercontent.com
 githubpreview.dev
 github.io
 gitlab.io
 gitapp.si
 gitpage.si
@@ -8577,34 +8662,36 @@
 blogspot.sn
 blogspot.td
 blogspot.tw
 blogspot.ug
 blogspot.vn
 goupile.fr
 gov.nl
+grayjayleagues.com
 awsmppl.com
 xn--gnstigbestellen-zvb.de
 xn--gnstigliefern-wob.de
 fin.ci
 free.hr
 caa.li
 ua.rs
 conf.se
 hs.zone
 hs.run
 hashbang.sh
 hasura.app
 hasura-app.io
 pages.it.hs-heilbronn.de
+helioho.st
+heliohost.us
 hepforge.org
 herokuapp.com
 herokussl.com
 ravendb.cloud
 ravendb.community
-ravendb.me
 development.run
 ravendb.run
 homesklep.pl
 *.kin.one
 *.id.pub
 *.kin.pub
 secaas.hk
@@ -8673,14 +8760,15 @@
 se.leg.br
 sp.leg.br
 to.leg.br
 pixolino.com
 na4u.ru
 iopsys.se
 ipifony.net
+is-a.dev
 ir.md
 iservschule.de
 mein-iserv.de
 schulplattform.de
 schulserver.de
 test-iserv.de
 iserv.dev
@@ -8767,14 +8855,16 @@
 mircloud.us
 myjino.ru
 *.hosting.myjino.ru
 *.landing.myjino.ru
 *.spectrum.myjino.ru
 *.vps.myjino.ru
 jotelulu.cloud
+jouwweb.site
+webadorsite.com
 *.triton.zone
 *.cns.joyent.com
 js.org
 kaas.gg
 khplay.nl
 ktistory.com
 kapsi.fi
@@ -8793,22 +8883,22 @@
 git-repos.de
 lcube-server.de
 svn-repos.de
 leadpages.co
 lpages.co
 lpusercontent.com
 lelux.site
+runcontainers.dev
 co.business
 co.education
 co.events
 co.financial
 co.network
 co.place
 co.technology
-app.lmpm.com
 linkyard.cloud
 linkyard-cloud.ch
 members.linode.com
 *.nodebalancer.linode.com
 *.linodeobjects.com
 ip.linodeusercontent.com
 we.bs
@@ -8877,15 +8967,14 @@
 custom.metacentrum.cz
 flt.cloud.muni.cz
 usr.cloud.muni.cz
 meteorapp.com
 eu.meteorapp.com
 co.pl
 *.azurecontainer.io
-cloudapp.azure.com
 azure-api.net
 azureedge.net
 azurefd.net
 azurewebsites.net
 azure-mobile.net
 azurestaticapps.net
 1.azurestaticapps.net
@@ -8926,14 +9015,15 @@
 x.mythic-beasts.com
 yali.mythic-beasts.com
 cust.retrosnub.co.uk
 ui.nabu.casa
 cloud.nospamproxy.com
 netlify.app
 4u.com
+ngo.us
 ngrok.app
 ngrok-free.app
 ngrok.dev
 ngrok-free.dev
 ngrok.io
 ap.ngrok.io
 au.ngrok.io
@@ -8942,14 +9032,15 @@
 jp.ngrok.io
 sa.ngrok.io
 us.ngrok.io
 ngrok.pizza
 ngrok.pro
 torun.pl
 nh-serv.co.uk
+nimsite.uk
 nfshost.com
 ipfs.nftstorage.link
 *.developer.app
 noop.app
 *.northflank.app
 *.build.run
 *.code.run
@@ -9067,45 +9158,50 @@
 servequake.com
 sytes.net
 webhop.me
 zapto.org
 stage.nodeart.io
 pcloud.host
 nyc.mn
+prvcy.page
 static.observableusercontent.com
 cya.gg
 omg.lol
 cloudycluster.net
 omniwe.site
 123hjemmeside.dk
 123hjemmeside.no
 123homepage.it
 123kotisivu.fi
 123minsida.se
 123miweb.es
 123paginaweb.pt
-123sait.ru
 123siteweb.fr
 123webseite.at
 123webseite.de
 123website.be
 123website.ch
 123website.lu
 123website.nl
 service.one
 simplesite.com
 simplesite.com.br
 simplesite.gr
 simplesite.pl
 nid.io
+is-cool.dev
+is-not-a.dev
+localplayer.dev
+is-local.org
 opensocial.site
 opencraft.hosting
 orsites.com
 operaunite.com
 tech.orange
+can.re
 authgear-staging.com
 authgearapps.com
 skygearapp.com
 outsystemscloud.com
 *.webpaas.ovh.net
 *.hosting.ovh.net
 ownprovider.com
@@ -9113,18 +9209,19 @@
 *.owo.codes
 ox.rs
 oy.lc
 pgfog.com
 pagefrontapp.com
 pagexl.com
 *.paywhirl.com
-bar0.net
-bar1.net
-bar2.net
-rdv.to
+*.xmit.co
+xmit.dev
+srv.us
+gh.srv.us
+gl.srv.us
 art.pl
 gliwice.pl
 krakow.pl
 poznan.pl
 wroc.pl
 zakopane.pl
 pantheonsite.io
@@ -9153,15 +9250,14 @@
 postman-echo.com
 pstmn.io
 mock.pstmn.io
 httpbin.org
 prequalifyme.today
 xen.prgmr.com
 priv.at
-prvcy.page
 *.dweb.link
 protonet.io
 chirurgiens-dentistes-en-france.fr
 byen.site
 pubtls.org
 pythonanywhere.com
 eu.pythonanywhere.com
@@ -9174,16 +9270,19 @@
 servername.us
 instances.spawn.cc
 instantcloud.cn
 ras.ru
 qa2.com
 qcx.io
 *.sys.qcx.io
-dev-myqnapcloud.com
+myqnapcloud.cn
 alpha-myqnapcloud.com
+dev-myqnapcloud.com
+mycloudnas.com
+mynascloud.com
 myqnapcloud.com
 *.quipelements.com
 vapor.cloud
 vaporcloud.io
 rackmaze.com
 rackmaze.net
 g.vbrplsbx.io
@@ -9329,14 +9428,15 @@
 scalebook.scw.cloud
 smartlabeling.scw.cloud
 dedibox.fr
 schokokeks.net
 gov.scot
 service.gov.scot
 scrysec.com
+client.scrypted.io
 firewall-gateway.com
 firewall-gateway.de
 my-gateway.de
 my-router.de
 spdns.de
 spdns.eu
 firewall-gateway.net
@@ -9376,20 +9476,23 @@
 medecin.fr
 notaires.fr
 pharmacien.fr
 port.fr
 veterinaire.fr
 small-web.org
 vp4.me
-snowflake.app
-privatelink.snowflake.app
+*.snowflake.app
+*.privatelink.snowflake.app
 streamlit.app
 streamlitapp.com
 try-snowplow.com
 srht.site
+w-corp-staticblitz.com
+w-credentialless-staticblitz.com
+w-staticblitz.com
 stackhero-network.com
 runs.onstackit.cloud
 stackit.gg
 stackit.rocks
 stackit.run
 stackit.zone
 musician.io
@@ -9548,14 +9651,15 @@
 uber.space
 *.uberspace.de
 hk.com
 hk.org
 ltd.hk
 inc.hk
 it.com
+unison-services.cloud
 name.pm
 sch.tf
 biz.wf
 sch.wf
 org.yt
 virtualuser.de
 virtual-user.de
@@ -9566,62 +9670,25 @@
 2038.io
 vercel.app
 vercel.dev
 now.sh
 router.management
 v-info.info
 voorloper.cloud
-neko.am
-nyaa.am
-be.ax
-cat.ax
-es.ax
-eu.ax
-gg.ax
-mc.ax
-us.ax
-xy.ax
-nl.ci
-xx.gl
-app.gp
-blog.gt
-de.gt
-to.gt
-be.gy
-cc.hn
-io.kg
-jp.kg
-tv.kg
-uk.kg
-us.kg
-de.ls
-at.md
-de.md
-jp.md
-to.md
-indie.porn
-vxl.sh
-ch.tc
-me.tc
-we.tc
-nyan.to
-at.vg
-blog.vu
-dev.vu
-me.vu
 v.ua
 *.vultrobjects.com
 wafflecell.com
 webflow.io
 webflowtest.io
 *.webhare.dev
 reserve-online.net
 reserve-online.com
 bookonline.app
 hotelwithflight.com
+*.wadl.top
 wedeploy.io
 wedeploy.me
 wedeploy.sh
 remotewd.com
 pages.wiardweb.com
 wmflabs.org
 toolforge.org
```

### Comparing `psl-2024.4.8/psl.egg-info/PKG-INFO` & `psl-2024.5.6/psl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psl
-Version: 2024.4.8
+Version: 2024.5.6
 Summary: Mozilla Public Suffix list as a Python package and updated daily
 Home-page: https://github.com/sethmlarson/psl
 Author: Seth Michael Larson
 Author-email: sethmichaellarson@gmail.com
 License: MPL-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `psl-2024.4.8/setup.py` & `psl-2024.5.6/setup.py`

 * *Files identical despite different names*

