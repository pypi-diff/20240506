# Comparing `tmp/mojo_landscaping-1.3.5.tar.gz` & `tmp/mojo_landscaping-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_landscaping-1.3.5.tar", max compression
+gzip compressed data, was "mojo_landscaping-1.3.6.tar", max compression
```

## Comparing `mojo_landscaping-1.3.5.tar` & `mojo_landscaping-1.3.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1083 2024-01-26 02:56:23.556649 mojo_landscaping-1.3.5/LICENSE.txt
--rw-r--r--   0        0        0     1980 2024-01-26 02:56:23.556797 mojo_landscaping-1.3.5/README.rst
--rw-r--r--   0        0        0      860 2024-04-24 04:07:26.555302 mojo_landscaping-1.3.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-26 02:56:23.558283 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/__init__.py
--rw-r--r--   0        0        0        0 2024-01-26 02:56:23.558375 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/agents/__init__.py
--rw-r--r--   0        0        0    10616 2024-01-26 02:56:23.558500 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/agents/localcommandagent.py
--rw-r--r--   0        0        0     2023 2024-01-26 02:56:23.558582 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/agents/poweragentbase.py
--rw-r--r--   0        0        0      888 2024-01-26 02:56:23.558668 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/agents/serialagentbase.py
--rw-r--r--   0        0        0      863 2024-01-26 02:56:23.558750 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/agents/systemagentbase.py
--rw-r--r--   0        0        0        0 2024-01-26 02:56:23.558826 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/client/__init__.py
--rw-r--r--   0        0        0     1655 2024-01-26 02:56:23.558936 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/client/clientbase.py
--rw-r--r--   0        0        0     9168 2024-01-26 02:56:23.559060 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/client/clientcoordinatorbase.py
--rw-r--r--   0        0        0     7291 2024-01-26 02:56:23.559207 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/client/clientcoordinatorcouplingbase.py
--rw-r--r--   0        0        0        0 2024-01-26 02:56:23.559287 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/cluster/__init__.py
--rw-r--r--   0        0        0     1747 2024-01-26 02:56:23.559382 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/cluster/nodebase.py
--rw-r--r--   0        0        0    10817 2024-01-26 02:56:23.559462 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/cluster/nodecoordinatorbase.py
--rw-r--r--   0        0        0     7396 2024-01-26 02:56:23.559533 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/cluster/nodecoordinatorcouplingbase.py
--rw-r--r--   0        0        0     2402 2024-01-26 02:56:23.559631 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/configurationextractor.py
--rw-r--r--   0        0        0      769 2024-01-26 02:56:23.559704 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/constants.py
--rw-r--r--   0        0        0        0 2024-01-26 02:56:23.559778 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/coordinators/__init__.py
--rw-r--r--   0        0        0     6949 2024-01-26 02:56:23.559916 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/coordinators/coordinatorbase.py
--rw-r--r--   0        0        0        0 2024-01-26 02:56:23.560009 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/coupling/__init__.py
--rw-r--r--   0        0        0     1496 2024-01-26 02:56:23.560104 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/coupling/coordinatorcoupling.py
--rw-r--r--   0        0        0     3346 2024-01-26 02:56:23.560189 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/friendlyidentifier.py
--rw-r--r--   0        0        0     5876 2024-01-26 02:56:23.560280 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/includefilters.py
--rw-r--r--   0        0        0    19639 2024-02-16 22:32:11.631790 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/landscape.py
--rw-r--r--   0        0        0    15428 2024-01-26 02:56:23.560725 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/landscapedevice.py
--rw-r--r--   0        0        0     1800 2024-03-29 20:38:14.167319 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/landscapedevicecluster.py
--rw-r--r--   0        0        0     1300 2024-01-26 02:56:23.560909 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/landscapedevicegroup.py
--rw-r--r--   0        0        0      846 2024-01-26 02:56:23.560993 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/landscapeparameters.py
--rw-r--r--   0        0        0    13782 2024-01-26 02:56:23.561075 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/landscapeservice.py
--rw-r--r--   0        0        0     1164 2024-01-26 02:56:23.561163 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/landscapingextensionprotocol.py
--rw-r--r--   0        0        0    17195 2024-03-08 02:21:32.965401 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/layers/landscapeconfigurationlayer.py
--rw-r--r--   0        0        0     2163 2024-01-26 02:56:23.561530 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/layers/landscapeinstallationlayer.py
--rw-r--r--   0        0        0    17352 2024-01-26 02:56:23.561610 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/layers/landscapeintegrationlayer.py
--rw-r--r--   0        0        0    14061 2024-03-29 20:46:40.802157 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/layers/landscapeoperationallayer.py
--rw-r--r--   0        0        0      998 2024-01-26 02:56:23.561816 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/layers/landscapinglayerbase.py
--rw-r--r--   0        0        0      972 2024-01-26 02:56:23.561888 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/layers/topologyintegrationlayer.py
--rw-r--r--   0        0        0     3812 2024-01-26 02:56:23.561978 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/protocolextension.py
--rw-r--r--   0        0        0        0 2024-01-26 02:56:23.562051 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/service/__init__.py
--rw-r--r--   0        0        0     1670 2024-01-26 02:56:23.562154 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/service/servicebase.py
--rw-r--r--   0        0        0     9042 2024-01-26 02:56:23.562249 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/service/servicecoordinatorbase.py
--rw-r--r--   0        0        0     7346 2024-01-26 02:56:23.562352 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/service/servicecoordinatorcouplingbase.py
--rw-r--r--   0        0        0     1695 2024-01-26 02:56:23.562437 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/wellknown.py
--rw-r--r--   0        0        0     3109 1970-01-01 00:00:00.000000 mojo_landscaping-1.3.5/setup.py
--rw-r--r--   0        0        0     2884 1970-01-01 00:00:00.000000 mojo_landscaping-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1556 2024-05-02 06:32:07.439028 mojo_landscaping-1.3.6/LICENSE.txt
+-rw-r--r--   0        0        0     1980 2024-01-26 02:56:23.556797 mojo_landscaping-1.3.6/README.rst
+-rw-r--r--   0        0        0      863 2024-05-06 01:57:39.080509 mojo_landscaping-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-26 02:56:23.558283 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:56:23.558375 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/agents/__init__.py
+-rw-r--r--   0        0        0    10440 2024-05-02 06:31:56.362010 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/agents/localcommandagent.py
+-rw-r--r--   0        0        0     1847 2024-05-02 06:31:56.362168 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/agents/poweragentbase.py
+-rw-r--r--   0        0        0      713 2024-05-02 06:31:56.362306 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/agents/serialagentbase.py
+-rw-r--r--   0        0        0      688 2024-05-02 06:31:56.362466 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/agents/systemagentbase.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:56:23.558826 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/client/__init__.py
+-rw-r--r--   0        0        0     1479 2024-05-02 06:31:56.362619 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/client/clientbase.py
+-rw-r--r--   0        0        0     8993 2024-05-02 06:31:56.362884 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/client/clientcoordinatorbase.py
+-rw-r--r--   0        0        0     7116 2024-05-02 06:31:56.363056 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/client/clientcoordinatorcouplingbase.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:56:23.559287 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/cluster/__init__.py
+-rw-r--r--   0        0        0     1572 2024-05-02 06:31:56.363279 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/cluster/nodebase.py
+-rw-r--r--   0        0        0    10642 2024-05-02 06:31:56.363571 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/cluster/nodecoordinatorbase.py
+-rw-r--r--   0        0        0     7221 2024-05-02 06:31:56.363733 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/cluster/nodecoordinatorcouplingbase.py
+-rw-r--r--   0        0        0     2497 2024-05-02 06:31:56.363887 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/configurationextractor.py
+-rw-r--r--   0        0        0      593 2024-05-02 06:31:56.364052 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/constants.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:56:23.559778 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/coordinators/__init__.py
+-rw-r--r--   0        0        0     6774 2024-05-02 06:31:56.364319 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/coordinators/coordinatorbase.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:56:23.560009 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/coupling/__init__.py
+-rw-r--r--   0        0        0     1321 2024-05-02 06:31:56.364537 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/coupling/coordinatorcoupling.py
+-rw-r--r--   0        0        0     3171 2024-05-02 06:31:56.364728 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/friendlyidentifier.py
+-rw-r--r--   0        0        0     5701 2024-05-02 06:31:56.364899 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/includefilters.py
+-rw-r--r--   0        0        0    19464 2024-05-02 06:31:56.365136 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/landscape.py
+-rw-r--r--   0        0        0    15253 2024-05-02 06:31:56.365559 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/landscapedevice.py
+-rw-r--r--   0        0        0     1625 2024-05-02 06:31:56.365747 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/landscapedevicecluster.py
+-rw-r--r--   0        0        0     1125 2024-05-02 06:31:56.365924 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/landscapedevicegroup.py
+-rw-r--r--   0        0        0      942 2024-05-02 06:31:56.366099 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/landscapeparameters.py
+-rw-r--r--   0        0        0    13607 2024-05-02 06:31:56.366423 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/landscapeservice.py
+-rw-r--r--   0        0        0      988 2024-05-02 06:31:56.366596 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/landscapingextensionprotocol.py
+-rw-r--r--   0        0        0    17020 2024-05-02 06:31:56.366776 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/layers/landscapeconfigurationlayer.py
+-rw-r--r--   0        0        0     1988 2024-05-02 06:31:56.366973 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/layers/landscapeinstallationlayer.py
+-rw-r--r--   0        0        0    17177 2024-05-02 06:31:56.367156 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/layers/landscapeintegrationlayer.py
+-rw-r--r--   0        0        0    14157 2024-05-02 06:31:56.367522 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/layers/landscapeoperationallayer.py
+-rw-r--r--   0        0        0      822 2024-05-02 06:31:56.367677 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/layers/landscapinglayerbase.py
+-rw-r--r--   0        0        0      796 2024-05-02 06:31:56.367848 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/layers/topologyintegrationlayer.py
+-rw-r--r--   0        0        0     3637 2024-05-02 06:31:56.367997 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/protocolextension.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:56:23.562051 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/service/__init__.py
+-rw-r--r--   0        0        0     1495 2024-05-02 06:31:56.368140 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/service/servicebase.py
+-rw-r--r--   0        0        0     8867 2024-05-02 06:31:56.368393 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/service/servicecoordinatorbase.py
+-rw-r--r--   0        0        0     7170 2024-05-02 06:33:52.825410 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/service/servicecoordinatorcouplingbase.py
+-rw-r--r--   0        0        0     1520 2024-05-02 06:31:56.368734 mojo_landscaping-1.3.6/source/packages/mojo/landscaping/wellknown.py
+-rw-r--r--   0        0        0     3112 1970-01-01 00:00:00.000000 mojo_landscaping-1.3.6/setup.py
+-rw-r--r--   0        0        0     2837 1970-01-01 00:00:00.000000 mojo_landscaping-1.3.6/PKG-INFO
```

### Comparing `mojo_landscaping-1.3.5/README.rst` & `mojo_landscaping-1.3.6/README.rst`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.5/pyproject.toml` & `mojo_landscaping-1.3.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [tool.poetry]
 name = "mojo-landscaping"
 description = "Automation Mojo Landscaping Package"
-version = "1.3.5"
+version = "1.3.6"
 authors = ["Myron W Walker"]
 readme = "README.rst"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX"
 ]
 keywords = [
     "python"
 ]
 packages = [{include="mojo", from="source/packages"}]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
-mojo-config = ">=1.3.7 <1.4.0"
-mojo-credentials = ">=1.3.1 <1.4.0"
-mojo-interfaces = ">=1.3.1 <1.4.0"
-mojo-extension = ">=1.3.8 <1.4.0"
-mojo-xmodules = ">=1.3.16 <1.4.0"
+python = ">=3.9,<4.0"
+mojo-config = ">=1.3.19 <1.4.0"
+mojo-credentials = ">=1.3.14 <1.4.0"
+mojo-interfaces = ">=1.3.3 <1.4.0"
+mojo-extension = ">=1.3.18 <1.4.0"
+mojo-xmodules = ">=1.3.19 <1.4.0"
 
 [tool.poetry.group.dev.dependencies]
 myst-parser = "^0.18.1"
 sphinx = ">=1.6,<6"
 sphinx-rtd-theme = "^1.1.1"
 
 [tool.poetry.group.dbio.dependencies]
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/agents/localcommandagent.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/agents/localcommandagent.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,15 @@
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
 
 from typing import Optional, Sequence, Tuple, Union
 
 import subprocess
 import threading
 import time
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/agents/poweragentbase.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/agents/poweragentbase.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,19 +7,15 @@
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
 
 from typing import Union
 
 from mojo.errors.exceptions import ConfigurationError
 
 from mojo.landscaping.protocolextension import ProtocolExtension
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/agents/serialagentbase.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/agents/serialagentbase.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,19 +8,16 @@
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
+
 
 from mojo.interfaces.isystemcontext import ISystemContext
 from mojo.landscaping.protocolextension import ProtocolExtension
 
 class SerialAgentBase(ProtocolExtension, ISystemContext):
     """
     """
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/agents/systemagentbase.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/agents/systemagentbase.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,19 +8,16 @@
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
+
 
 from mojo.interfaces.isystemcontext import ISystemContext
 from mojo.landscaping.protocolextension import ProtocolExtension
 
 class SystemAgentBase(ProtocolExtension, ISystemContext):
     """
     """
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/client/clientbase.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/client/clientbase.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,19 +8,15 @@
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
 
 from typing import TYPE_CHECKING
 
 from mojo.landscaping.landscapedevice import LandscapeDevice
 from mojo.landscaping.friendlyidentifier import FriendlyIdentifier
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/client/clientcoordinatorbase.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/client/clientcoordinatorbase.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,19 +7,16 @@
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
+
 
 from typing import Any, Dict, List, Optional, Tuple, Union, TYPE_CHECKING
 
 import os
 import pprint
 
 from mojo.errors.exceptions import ConfigurationError, NotOverloadedError
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/client/clientcoordinatorcouplingbase.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/client/clientcoordinatorcouplingbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,16 @@
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
+
 
 
 from typing import Any, Dict, List, Tuple, TYPE_CHECKING
 
 from functools import partial
 
 from mojo.errors.exceptions import SemanticError
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/cluster/nodecoordinatorbase.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/cluster/nodecoordinatorbase.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,19 +7,16 @@
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
+
 
 from typing import Any, Dict, List, Optional, Tuple, Union, TYPE_CHECKING
 
 import os
 import pprint
 
 from mojo.errors.exceptions import ConfigurationError, NotOverloadedError
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/cluster/nodecoordinatorcouplingbase.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/cluster/nodecoordinatorcouplingbase.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,19 +6,16 @@
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
+
 
 
 from typing import Any, Dict, List, Tuple, TYPE_CHECKING
 
 from functools import partial
 
 from mojo.errors.exceptions import SemanticError
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/configurationextractor.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/configurationextractor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 
+__author__ = "Myron Walker"
+__copyright__ = "Copyright 2023, Myron W Walker"
+__credits__ = []
+
 from typing import List, Optional, Tuple
 
 import copy
 
 from mojo.interfaces.iexcludefilter import IExcludeFilter
 from mojo.interfaces.iincludefilter import IIncludeFilter
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/coordinators/coordinatorbase.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/coordinators/coordinatorbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,16 @@
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
+
 
 from typing import List, Optional, TYPE_CHECKING
 
 import threading
 import weakref
 
 from mojo.errors.exceptions import NotOverloadedError
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/coupling/coordinatorcoupling.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/coupling/coordinatorcoupling.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,19 +7,16 @@
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
+
 
 from typing import TYPE_CHECKING
 
 from mojo.errors.exceptions import NotOverloadedError
 
 from mojo.xmods.injection.coupling.integrationcoupling import IntegrationCoupling
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/friendlyidentifier.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/friendlyidentifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,16 @@
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
+
 
 from typing import Optional, Union
 
 import re
 
 from mojo.errors.exceptions import SemanticError
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/includefilters.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/includefilters.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,16 @@
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
+
 
 from typing import Any
 
 from mojo.interfaces.iincludefilter import IIncludeFilter
 
 from mojo.landscaping.landscapedevice import LandscapeDevice
 from mojo.landscaping.landscapeservice import LandscapeService
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/landscape.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/landscape.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,19 +6,16 @@
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
+
 
 from typing import Dict, List, Optional, Union
 
 import inspect
 import logging
 import os
 import threading
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/landscapedevice.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/landscapedevice.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,16 @@
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
+
 
 from typing import Callable, Dict, Union, TYPE_CHECKING
 
 import logging
 import os
 import socket
 import threading
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/landscapedevicecluster.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/landscapedevicegroup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,47 @@
 """
-.. module:: landscapedevicecluster
+.. module:: landscapedevicegroup
     :platform: Darwin, Linux, Unix, Windows
-    :synopsis: Module contains the :class:`LandscapeDeviceCluster` object which 
-               represents a cluster of devices that are compute nodes in a
-               computer or storage cluster.
+    :synopsis: Module contains the :class:`LandscapeDeviceGroup` object which is a
+               container object which groups :class:`Landscapedevice` object with
+               thier group name.
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
 
-from typing import Dict
 
-from mojo.landscaping.cluster.nodebase import NodeBase
-from mojo.landscaping.landscapedevicegroup import LandscapeDeviceGroup
 
-class LandscapeDeviceCluster:
+from typing import List
+
+import weakref
+
+from mojo.landscaping.landscapedevice import LandscapeDevice
+
+class LandscapeDeviceGroup:
     """
-        A :class:`LandscapeDeviceCluster` object is used to manage a group of
-        nodes that are part of a computer cluster and a collection of spares
-        that are eligible to participate in the cluster.
+        A :class:`LandscapeDeviceGroup` object is used to group devices to an associated
+        grouping label.
     """
 
-    def __init__(self, name: str, nodes: Dict[str, NodeBase], spares: Dict[str, NodeBase],
-                 group: LandscapeDeviceGroup) -> None:
-        self._name = name
-        self._nodes = nodes
-        self._spares = spares
-        self._group = group
+    def __init__(self, label: str, items: List[LandscapeDevice]) -> None:
+        self._label = label
+        self._items = items
+        
+        self._coord_ref = weakref.ref(self._items[0].coordinator)
         return
-
+    
     @property
-    def group(self) -> LandscapeDeviceGroup:
-        return self._group
+    def coordinator(self):
+        return self._coord_ref()
 
     @property
-    def name(self) -> str:
-        return self._name
+    def items(self):
+        return self._items
 
     @property
-    def nodes(self) -> Dict[str, NodeBase]:
-        return self._nodes
-    
-    @property
-    def spares(self) -> Dict[str, NodeBase]:
-        return self._spares
-
-    def enchance_metadata(self):
-        """
-            Hook function to allow a cluster object the opportunity to enhance its Metadata.
-        """
-        return
+    def label(self):
+        return self._label
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/landscapeparameters.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/landscapeparameters.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,14 +5,19 @@
                overloadable and function signature friendly way to provide customizable parameters
                to the landscape startup functions.
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 
 """
 
+__author__ = "Myron Walker"
+__copyright__ = "Copyright 2023, Myron W Walker"
+__credits__ = []
+
+
 from types import SimpleNamespace
 
 class LandscapeActivationParams(SimpleNamespace):
     disable_device_activation: bool=False
     disable_service_activation: bool=False
     allow_missing_devices: bool=False
     allow_unknown_devices: bool=False
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/landscapeservice.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/landscapeservice.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,16 @@
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
+
 
 from typing import Callable, Dict, Union, TYPE_CHECKING
 
 import logging
 import os
 import threading
 import weakref
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/landscapingextensionprotocol.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/landscapingextensionprotocol.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,19 +6,15 @@
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
 
 
 from typing import List, Protocol, Type
 
 from mojo.xmods.injection.coupling.integrationcoupling import IntegrationCoupling
 
 class LandscapingExtensionProtocol(Protocol):
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/layers/landscapeconfigurationlayer.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/layers/landscapeconfigurationlayer.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,16 @@
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
+
 
 from typing import Any, Dict, List, Optional, Tuple, Union, TYPE_CHECKING
 
 import json
 import os
 import traceback
 import yaml
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/layers/landscapeinstallationlayer.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/layers/landscapeinstallationlayer.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,19 +8,16 @@
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
+
 
 from typing import Dict, TYPE_CHECKING
 
 from mojo.extension.wellknown import ConfiguredSuperFactorySingleton
 
 from mojo.xmods.injection.coupling.integrationcoupling import IntegrationCouplingType
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/layers/landscapeintegrationlayer.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/layers/landscapeintegrationlayer.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,19 +8,16 @@
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
+
 
 from typing import Any, Dict, List, Optional, TYPE_CHECKING
 
 from mojo.errors.exceptions import SemanticError
 
 from mojo.interfaces.iexcludefilter import IExcludeFilter
 from mojo.interfaces.iincludefilter import IIncludeFilter
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/layers/landscapeoperationallayer.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/layers/landscapeoperationallayer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,13 @@
 
+__author__ = "Myron Walker"
+__copyright__ = "Copyright 2023, Myron W Walker"
+__credits__ = []
+
+
 from typing import Any, Dict, List, Optional, Union, TYPE_CHECKING
 
 import os
 
 from mojo.errors.xtraceback import format_exception
 from mojo.errors.exceptions import CheckinError, CheckoutError, SemanticError
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/layers/topologyintegrationlayer.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/layers/topologyintegrationlayer.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,19 +8,15 @@
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
 
 
 from typing import TYPE_CHECKING
 
 from mojo.landscaping.layers.landscapinglayerbase import LandscapingLayerBase
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/protocolextension.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/protocolextension.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,19 +8,16 @@
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
+
 
 from typing import Dict, Union, TYPE_CHECKING
 
 import logging
 import weakref
 
 if TYPE_CHECKING:
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/service/servicecoordinatorbase.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/service/servicecoordinatorbase.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,19 +7,16 @@
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
+
 
 from typing import Any, Dict, List, Optional, Tuple, Union, TYPE_CHECKING
 
 import os
 import pprint
 
 from mojo.errors.exceptions import ConfigurationError, NotOverloadedError
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/service/servicecoordinatorcouplingbase.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/service/servicecoordinatorcouplingbase.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,19 +6,15 @@
 
 .. moduleauthor:: Myron Walker <myron.walker@gmail.com>
 """
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
 
 
 from typing import Any, Dict, List, Tuple, TYPE_CHECKING
 
 from functools import partial
 
 from mojo.errors.exceptions import SemanticError
```

### Comparing `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/wellknown.py` & `mojo_landscaping-1.3.6/source/packages/mojo/landscaping/wellknown.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 
 __author__ = "Myron Walker"
 __copyright__ = "Copyright 2023, Myron W Walker"
 __credits__ = []
-__version__ = "1.0.0"
-__maintainer__ = "Myron Walker"
-__email__ = "myron.walker@gmail.com"
-__status__ = "Development" # Prototype, Development or Production
-__license__ = "MIT"
+
+
 
 from typing import TYPE_CHECKING
 
 from threading import RLock
 
 from mojo.extension.wellknown import ConfiguredSuperFactorySingleton
```

### Comparing `mojo_landscaping-1.3.5/setup.py` & `mojo_landscaping-1.3.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,32 +15,32 @@
  'mojo.landscaping.layers',
  'mojo.landscaping.service']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['mojo-config>=1.3.7,<1.4.0',
- 'mojo-credentials>=1.3.1,<1.4.0',
- 'mojo-extension>=1.3.8,<1.4.0',
- 'mojo-interfaces>=1.3.1,<1.4.0',
- 'mojo-xmodules>=1.3.16,<1.4.0']
+['mojo-config>=1.3.19,<1.4.0',
+ 'mojo-credentials>=1.3.14,<1.4.0',
+ 'mojo-extension>=1.3.18,<1.4.0',
+ 'mojo-interfaces>=1.3.3,<1.4.0',
+ 'mojo-xmodules>=1.3.19,<1.4.0']
 
 setup_kwargs = {
     'name': 'mojo-landscaping',
-    'version': '1.3.5',
+    'version': '1.3.6',
     'description': 'Automation Mojo Landscaping Package',
     'long_description': '=======================\npython-package-template\n=======================\nThis is a template repository that can be used to quickly create a python package project.\n\n=========================\nFeatures of this Template\n=========================\n* Machine Setup\n* Virtual Environment Setup (Poetry)\n* PyPi Publishing\n* Sphinx Documentation\n\n========================\nHow to Use This Template\n========================\n- Click the \'Use this template\' button\n- Fill in the information to create your repository\n- Checkout your new repository\n- Change the following in \'repository-config.ini\'\n\n  #. \'PROJECT NAME\'\n  #. \'REPOSITORY_NAME\'\n\n- If you have machine dependencies to add, put them in \'setup-ubuntu-machine\'\n- Modify the pyproject.toml file with the correct package-name, author, publishing information, etc.\n- Rename the VSCODE workspace file \'mv workspaces/default-workspace.template workspaces/(project name).template\'\n- Replace the README.rst file with your own README\n- Update the LICENSE.txt file with your copyright information and license.\n- Add your dependencies with python poetry \'poetry add (dependency name)\'\n- Drop your package code in \'source/packages\'\n- Modify the name of your package root in \'pyproject.toml\'\n\n  #. \'packages = [{include="(root folder name)", from="source/packages"}]\'\n\n=================\nCode Organization\n=================\n* .vscode - Common tasks\n* development - This is where the runtime environment scripts are located\n* repository-setup - Scripts for homing your repository and to your checkout and machine setup\n* userguide - Where you put your user guide\n* source/packages - Put your root folder here \'source/packages/(root-module-folder)\'\n* source/sphinx - This is the Sphinx documentation folder\n* workspaces - This is where you add VSCode workspaces templates and where workspaces show up when homed.\n\n==========\nReferences\n==========\n\n- `User Guide <userguide/userguide.rst>`\n- `Coding Standards <userguide/10-00-coding-standards.rst>`\n',
     'author': 'Myron W Walker',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+    'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `mojo_landscaping-1.3.5/PKG-INFO` & `mojo_landscaping-1.3.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: mojo-landscaping
-Version: 1.3.5
+Version: 1.3.6
 Summary: Automation Mojo Landscaping Package
 License: LICENSE.txt
 Keywords: python
 Author: Myron W Walker
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: mojo-config (>=1.3.7,<1.4.0)
-Requires-Dist: mojo-credentials (>=1.3.1,<1.4.0)
-Requires-Dist: mojo-extension (>=1.3.8,<1.4.0)
-Requires-Dist: mojo-interfaces (>=1.3.1,<1.4.0)
-Requires-Dist: mojo-xmodules (>=1.3.16,<1.4.0)
+Requires-Dist: mojo-config (>=1.3.19,<1.4.0)
+Requires-Dist: mojo-credentials (>=1.3.14,<1.4.0)
+Requires-Dist: mojo-extension (>=1.3.18,<1.4.0)
+Requires-Dist: mojo-interfaces (>=1.3.3,<1.4.0)
+Requires-Dist: mojo-xmodules (>=1.3.19,<1.4.0)
 Description-Content-Type: text/x-rst
 
 =======================
 python-package-template
 =======================
 This is a template repository that can be used to quickly create a python package project.
```

