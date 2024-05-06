# Comparing `tmp/crocodeel-1.0.2.tar.gz` & `tmp/crocodeel-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crocodeel-1.0.2.tar", max compression
+gzip compressed data, was "crocodeel-1.0.3.tar", max compression
```

## Comparing `crocodeel-1.0.2.tar` & `crocodeel-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0    35147 2024-04-24 15:38:44.141401 crocodeel-1.0.2/COPYING
--rw-r--r--   0        0        0     4295 2024-05-02 16:07:23.139970 crocodeel-1.0.2/README.md
--rw-r--r--   0        0        0       85 2024-05-03 08:13:17.952711 crocodeel-1.0.2/crocodeel/__init__.py
--rw-r--r--   0        0        0     1751 2024-05-03 08:13:25.136762 crocodeel-1.0.2/crocodeel/ab_table_utils.py
--rw-r--r--   0        0        0     1788 2024-05-03 08:13:17.952711 crocodeel-1.0.2/crocodeel/conta_event.py
--rw-r--r--   0        0        0     6465 2024-05-03 08:13:17.952711 crocodeel-1.0.2/crocodeel/crocodeel.py
--rw-r--r--   0        0        0      670 2024-05-03 08:13:17.952711 crocodeel-1.0.2/crocodeel/easy_wf.py
--rw-r--r--   0        0        0   623880 2024-04-30 19:52:39.027352 crocodeel-1.0.2/crocodeel/models/crocodeel_rf_Mar2023.joblib
--rw-r--r--   0        0        0     6268 2024-05-03 08:13:17.952711 crocodeel-1.0.2/crocodeel/plot_conta.py
--rw-r--r--   0        0        0      629 2024-05-03 08:46:25.511715 crocodeel-1.0.2/crocodeel/rf_model.py
--rw-r--r--   0        0        0    16530 2024-05-03 08:13:17.952711 crocodeel-1.0.2/crocodeel/search_conta.py
--rw-r--r--   0        0        0   119253 2024-04-30 19:52:39.027352 crocodeel-1.0.2/crocodeel/test_data/mgs_profiles_test.tsv
--rw-r--r--   0        0        0    49550 2024-04-30 19:52:39.027352 crocodeel-1.0.2/crocodeel/test_data/results/contamination_events.pdf
--rw-r--r--   0        0        0     2051 2024-04-30 19:52:39.031353 crocodeel-1.0.2/crocodeel/test_data/results/contamination_events.tsv
--rw-r--r--   0        0        0     2008 2024-05-03 08:29:12.351775 crocodeel-1.0.2/crocodeel/test_install.py
--rw-r--r--   0        0        0     1377 2024-05-03 08:51:36.590064 crocodeel-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     5397 1970-01-01 00:00:00.000000 crocodeel-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35147 2024-05-06 16:01:16.847576 crocodeel-1.0.3/COPYING
+-rw-r--r--   0        0        0     4273 2024-05-06 16:01:16.851576 crocodeel-1.0.3/README.md
+-rw-r--r--   0        0        0       85 2024-05-06 16:01:16.851576 crocodeel-1.0.3/crocodeel/__init__.py
+-rw-r--r--   0        0        0     1792 2024-05-06 16:01:16.851576 crocodeel-1.0.3/crocodeel/ab_table_utils.py
+-rw-r--r--   0        0        0     2011 2024-05-06 16:01:16.851576 crocodeel-1.0.3/crocodeel/conta_event.py
+-rw-r--r--   0        0        0     6776 2024-05-06 16:01:16.851576 crocodeel-1.0.3/crocodeel/crocodeel.py
+-rw-r--r--   0        0        0      670 2024-05-06 16:01:16.851576 crocodeel-1.0.3/crocodeel/easy_wf.py
+-rw-r--r--   0        0        0     1005 2024-05-06 16:01:16.851576 crocodeel-1.0.3/crocodeel/execution_description.py
+-rw-r--r--   0        0        0   623880 2024-05-06 16:01:16.851576 crocodeel-1.0.3/crocodeel/models/crocodeel_rf_Mar2023.joblib
+-rw-r--r--   0        0        0     6410 2024-05-06 16:01:16.851576 crocodeel-1.0.3/crocodeel/plot_conta.py
+-rw-r--r--   0        0        0      731 2024-05-06 16:01:16.851576 crocodeel-1.0.3/crocodeel/rf_model.py
+-rw-r--r--   0        0        0    16557 2024-05-06 16:01:16.851576 crocodeel-1.0.3/crocodeel/search_conta.py
+-rw-r--r--   0        0        0   119253 2024-05-06 16:01:16.851576 crocodeel-1.0.3/crocodeel/test_data/mgs_profiles_test.tsv
+-rw-r--r--   0        0        0    49550 2024-05-06 16:01:16.851576 crocodeel-1.0.3/crocodeel/test_data/results/contamination_events.pdf
+-rw-r--r--   0        0        0     2051 2024-05-06 16:01:16.851576 crocodeel-1.0.3/crocodeel/test_data/results/contamination_events.tsv
+-rw-r--r--   0        0        0     2008 2024-05-06 16:01:16.851576 crocodeel-1.0.3/crocodeel/test_install.py
+-rw-r--r--   0        0        0     1377 2024-05-06 16:01:16.851576 crocodeel-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5375 1970-01-01 00:00:00.000000 crocodeel-1.0.3/PKG-INFO
```

### Comparing `crocodeel-1.0.2/COPYING` & `crocodeel-1.0.3/COPYING`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.2/README.md` & `crocodeel-1.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #  CroCoDeEL : **CRO**ss-sample **CO**ntamination **DE**tection and **E**stimation of its **L**evels 🐊
 
-[![install with conda](https://img.shields.io/conda/vn/fplazaonate/crocodeel?color=green&label=fplazaonate%2Fcrocodeel&logo=anaconda)](https://anaconda.org/fplazaonate/crocodeel)
+[![install with conda](https://img.shields.io/conda/vn/bioconda/crocodeel?color=green&label=bioconda%2Fcrocodeel&logo=anaconda)](https://anaconda.org/bioconda/crocodeel)
 [![PyPI](https://img.shields.io/pypi/v/crocodeel?label=pypi%20package)](https://pypi.org/project/crocodeel/)
 
 ## Introduction
 
 CroCoDeEL is a tool that detects cross-sample (aka well-to-well) contamination in shotgun metagenomic data.\
 It accurately identifies contaminated samples but also pinpoints contamination sources and estimates contamination rates.\
 CroCoDeEL relies only on species abundance tables and does not need negative controls.
 
 ## Installation
 
-CroCoDeEL can be easily installed with conda:
+CroCoDeEL is available on bioconda:
 ```
-conda create --name crocodeel_env -c conda-forge -c fplazaonate crocodeel
+conda create --name crocodeel_env -c conda-forge -c bioconda crocodeel
 conda activate crocodeel_env
 ```
 
 Alternatively, you can use pip:
 ```
 pip install crocodeel
 ```
```

### Comparing `crocodeel-1.0.2/crocodeel/ab_table_utils.py` & `crocodeel-1.0.3/crocodeel/ab_table_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import logging
 import sys
 from typing import TextIO
+from pathlib import Path
 import numpy as np
 import pandas as pd
 
 
 def read(fh: TextIO) -> pd.DataFrame:
     # Read table
-    logging.info('Reading %s', fh.name)
+    logging.info('Reading %s', Path(fh.name).resolve())
     species_ab_table = pd.read_csv(fh, sep="\t", header=0, index_col=0)
     logging.info(
         "Abundance table quantifies %d species in %d samples",
         species_ab_table.shape[0],
         species_ab_table.shape[1],
     )
```

### Comparing `crocodeel-1.0.2/crocodeel/conta_event.py` & `crocodeel-1.0.3/crocodeel/conta_event.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,23 @@
     probability: float = field(default=0.0)
     contamination_specific_species: list[str] = field(default_factory=lambda: [])
 
 
 class ContaminationEventIO:
     @staticmethod
     def read_tsv(fh: TextIO) -> Iterator[ContaminationEvent]:
+        # Ugly hack to skip comment lines
+        pos = 0
+        while fh :
+            line = fh.readline()
+            if not line.startswith("#"):
+                break
+            pos = fh.tell()
+        fh.seek(pos)
+
         tsv_reader = csv.DictReader(fh, delimiter="\t")
 
         for row in tsv_reader:
             contamination_specific_species = row[
                 "contamination_specific_species"
             ].split(",")
```

### Comparing `crocodeel-1.0.2/crocodeel/crocodeel.py` & `crocodeel-1.0.3/crocodeel/crocodeel.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: utf-8 -*-
 
 import sys
 import argparse
 import logging
 import multiprocessing
 from importlib.metadata import version
+from crocodeel.execution_description import ExecutionDescription
 from crocodeel.search_conta import run_search_conta
 from crocodeel.plot_conta import run_plot_conta, Defaults as plot_conta_defaults
 from crocodeel.easy_wf import run_easy_wf
 from crocodeel.test_install import run_test_install
 
 
 def set_logging() -> None:
@@ -33,15 +34,15 @@
 
     return value
 
 
 def get_arguments() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="crocodeel")
     parser.add_argument(
-        "-v", "--version", action="version", version=f"%(prog)s version { version('crocodeel')}"
+        "-v", "--version", action="version", version=f"%(prog)s version { version("crocodeel")}"
     )
 
 
     subparsers = parser.add_subparsers(
         title="positional arguments",
         help="Select subcommand",
         dest="command",
@@ -188,14 +189,20 @@
 
     return parser.parse_args(args=sys.argv[1:] or ["--help"])
 
 
 def main() -> None:
     set_logging()
     args = get_arguments()
+
+    # Add comment line in output file describing execution context
+    if args.command in ("search_conta","easy_wf"):
+        exec_desc = ExecutionDescription(args.species_ab_table_fh.name)
+        print(exec_desc, file = args.conta_events_fh)
+
     if args.command == "search_conta":
         run_search_conta(vars(args))
     elif args.command == "plot_conta":
         run_plot_conta(vars(args))
     elif args.command == "easy_wf":
         run_easy_wf(vars(args))
     elif args.command == "test_install":
```

### Comparing `crocodeel-1.0.2/crocodeel/easy_wf.py` & `crocodeel-1.0.3/crocodeel/easy_wf.py`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.2/crocodeel/models/crocodeel_rf_Mar2023.joblib` & `crocodeel-1.0.3/crocodeel/models/crocodeel_rf_Mar2023.joblib`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.2/crocodeel/plot_conta.py` & `crocodeel-1.0.3/crocodeel/plot_conta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import BinaryIO, Any, Final
 from functools import partial
 import logging
+from pathlib import Path
 from time import perf_counter
 from matplotlib.backends.backend_pdf import PdfPages
 import matplotlib.pyplot as plt
 import pandas as pd
 import numpy as np
 import tqdm
 from crocodeel.conta_event import ContaminationEvent, ContaminationEventIO
@@ -17,29 +18,33 @@
     else:
         species_ab_table = ab_table_utils.read(args["species_ab_table_fh"])
         args["species_ab_table_fh"].close()
         species_ab_table = ab_table_utils.normalize(species_ab_table)
 
     conta_events = list(ContaminationEventIO.read_tsv(args["conta_events_fh"]))
     if args["conta_events_fh"].mode == 'r':
-        logging.info("%d contamination events loaded", len(conta_events))
+        logging.info(
+            "%d contamination events loaded from %s",
+            len(conta_events),
+            Path(args["conta_events_fh"].name).resolve(),
+        )
     args["conta_events_fh"].close()
 
     start = perf_counter()
     logging.info("Generation of the PDF report started")
     ContaminationPlotsReport(
         species_ab_table=species_ab_table,
         conta_events=conta_events,
         nrow=args["nrow"],
         ncol=args["ncol"],
         no_contamination_line=args["no_conta_line"],
         color_contamination_specific_species=args["color_conta_species"],
     ).save_to_pdf(args["pdf_report_fh"])
     logging.info("PDF report generated in %.1f seconds", np.round(perf_counter() - start, 1))
-    logging.info("PDF report saved in %s", args["pdf_report_fh"].name)
+    logging.info("PDF report saved in %s", Path(args["pdf_report_fh"].name).resolve())
     args["pdf_report_fh"].close()
 
 
 class Defaults:
     MIN_NROW: Final[int] = 1
     NROW: Final[int] = 4
     MAX_NROW: Final[int] = 11
```

### Comparing `crocodeel-1.0.2/crocodeel/rf_model.py` & `crocodeel-1.0.3/crocodeel/rf_model.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,9 +11,13 @@
     RF_MODEL_FILE: Final[Path] = Path(
         importlib.resources.files().joinpath("models", "crocodeel_rf_Mar2023.joblib")
     )
 
     @staticmethod
     def load() -> RandomForestClassifier:
         with warnings.catch_warnings():
-            warnings.filterwarnings(action='ignore',category=InconsistentVersionWarning)
+            warnings.filterwarnings(action="ignore", category=InconsistentVersionWarning)
             return joblib.load(RandomForestModel.RF_MODEL_FILE)
+
+    @staticmethod
+    def get_version() -> str:
+        return RandomForestModel.RF_MODEL_FILE.stem
```

### Comparing `crocodeel-1.0.2/crocodeel/search_conta.py` & `crocodeel-1.0.3/crocodeel/search_conta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from multiprocessing import Pool
 from functools import partial
 from itertools import product
 import logging
+from pathlib import Path
 from time import perf_counter
 from typing import Final, Any
 import numpy as np
 import pandas as pd
 import tqdm
 from sklearn.linear_model import RANSACRegressor, LinearRegression
 from sklearn.metrics import mean_squared_error
@@ -36,16 +37,16 @@
     contaminated_samples = {conta_event.target for conta_event in conta_events}
     logging.info("%d contamination events detected", len(conta_events))
     logging.info("%d/%d samples contaminated", len(contaminated_samples), species_ab_table.shape[1])
 
     conta_events.sort(key=lambda e: e.rate, reverse=True)
     ContaminationEventIO.write_tsv(conta_events, args['conta_events_fh'])
     logging.info(
-        "Contamination events sorted by decreasing contamination rate saved in %s",
-        args["conta_events_fh"].name,
+        "Contamination events sorted by decreasing rate saved in %s",
+        Path(args["conta_events_fh"].name).resolve(),
     )
     if args["conta_events_fh"].mode == 'w':
         args["conta_events_fh"].close()
 
     logging.warning("Contamination events may be false positives, "
                     "especially when dealing with samples with similar species abundance profiles "
                     "(longitudinal data, animals raised together)")
```

### Comparing `crocodeel-1.0.2/crocodeel/test_data/mgs_profiles_test.tsv` & `crocodeel-1.0.3/crocodeel/test_data/mgs_profiles_test.tsv`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.2/crocodeel/test_data/results/contamination_events.pdf` & `crocodeel-1.0.3/crocodeel/test_data/results/contamination_events.pdf`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.2/crocodeel/test_data/results/contamination_events.tsv` & `crocodeel-1.0.3/crocodeel/test_data/results/contamination_events.tsv`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.2/crocodeel/test_install.py` & `crocodeel-1.0.3/crocodeel/test_install.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 import logging
 from tempfile import NamedTemporaryFile
 import filecmp
 import sys
 from typing import Final
 from crocodeel.easy_wf import run_easy_wf
 
+
 class TestData:
     SPECIES_ABUNDANCE_TABLE: Final[Path] = Path(
         importlib.resources.files().joinpath("test_data", "mgs_profiles_test.tsv")
     )
 
     EXPECTED_CONTA_EVENTS_FILE: Final[Path] = Path(
         importlib.resources.files().joinpath("test_data", "results", "contamination_events.tsv")
     )
 
     EXPECTED_PDF_REPORT_FILE: Final[Path] = Path(
         importlib.resources.files().joinpath("test_data", "results", "contamination_events.pdf")
     )
 
+
 def run_test_install(keep_results: bool) -> None:
     with (
         open(TestData.SPECIES_ABUNDANCE_TABLE, "r", encoding="utf-8") as species_ab_table_fh,
         NamedTemporaryFile(
             mode="w+",
             prefix="contamination_events_",
             suffix=".tsv",
@@ -35,25 +37,26 @@
             prefix="contamination_events_",
             suffix=".pdf",
             delete=not keep_results,
             delete_on_close=False,
         ) as pdf_report_fh,
     ):
         easy_wf_args = {
-            "species_ab_table_fh" : species_ab_table_fh,
-            "conta_events_fh" : conta_events_fh,
-            "pdf_report_fh" : pdf_report_fh,
-            "nproc" : 1
+            "species_ab_table_fh": species_ab_table_fh,
+            "conta_events_fh": conta_events_fh,
+            "pdf_report_fh": pdf_report_fh,
+            "nproc": 1,
         }
 
         logging.info("Tests on the toy dataset started")
         run_easy_wf(easy_wf_args)
-        logging.info("Tests completed successfully")
 
         if filecmp.cmp(TestData.EXPECTED_CONTA_EVENTS_FILE, conta_events_fh.name):
             logging.info("All contamination events with expected rates and probabilities found")
         else:
             logging.error("Contamination events found are not those expected")
             sys.exit(1)
 
     if not keep_results:
         logging.info("Temporary result files deleted")
+    
+    logging.info("Tests completed successfully")
```

### Comparing `crocodeel-1.0.2/pyproject.toml` & `crocodeel-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crocodeel"
-version = "1.0.2"
+version = "1.0.3"
 description = "CroCoDeEL is a tool that detects cross-sample (aka well-to-well) contamination in shotgun metagenomic data"
 authors = [
     "Lindsay Goulet <lindsay.goulet@inrae.fr>",
     "Florian Plaza Oñate <florian.plaza-onate@inrae.fr>",
     "Edi Prifti <edi.prifti@ird.fr>",
     "Eugeni Belda <eugeni.belda@ird.fr>",
     "Emmanuelle Le Chatelier <emmanuelle.le-chatelier@inrae.fr>",
```

### Comparing `crocodeel-1.0.2/PKG-INFO` & `crocodeel-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crocodeel
-Version: 1.0.2
+Version: 1.0.3
 Summary: CroCoDeEL is a tool that detects cross-sample (aka well-to-well) contamination in shotgun metagenomic data
 Home-page: https://github.com/metagenopolis/CroCoDeEL
 License: GPL-3.0-or-later
 Keywords: Metagenomics
 Author: Lindsay Goulet
 Author-email: lindsay.goulet@inrae.fr
 Requires-Python: >=3.12
@@ -23,28 +23,28 @@
 Requires-Dist: scipy (>=1.13,<2.0)
 Requires-Dist: tqdm (>=4.66,<5.0)
 Project-URL: Repository, https://github.com/metagenopolis/CroCoDeEL
 Description-Content-Type: text/markdown
 
 #  CroCoDeEL : **CRO**ss-sample **CO**ntamination **DE**tection and **E**stimation of its **L**evels 🐊
 
-[![install with conda](https://img.shields.io/conda/vn/fplazaonate/crocodeel?color=green&label=fplazaonate%2Fcrocodeel&logo=anaconda)](https://anaconda.org/fplazaonate/crocodeel)
+[![install with conda](https://img.shields.io/conda/vn/bioconda/crocodeel?color=green&label=bioconda%2Fcrocodeel&logo=anaconda)](https://anaconda.org/bioconda/crocodeel)
 [![PyPI](https://img.shields.io/pypi/v/crocodeel?label=pypi%20package)](https://pypi.org/project/crocodeel/)
 
 ## Introduction
 
 CroCoDeEL is a tool that detects cross-sample (aka well-to-well) contamination in shotgun metagenomic data.\
 It accurately identifies contaminated samples but also pinpoints contamination sources and estimates contamination rates.\
 CroCoDeEL relies only on species abundance tables and does not need negative controls.
 
 ## Installation
 
-CroCoDeEL can be easily installed with conda:
+CroCoDeEL is available on bioconda:
 ```
-conda create --name crocodeel_env -c conda-forge -c fplazaonate crocodeel
+conda create --name crocodeel_env -c conda-forge -c bioconda crocodeel
 conda activate crocodeel_env
 ```
 
 Alternatively, you can use pip:
 ```
 pip install crocodeel
 ```
```

