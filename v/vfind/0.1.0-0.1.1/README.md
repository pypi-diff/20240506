# Comparing `tmp/vfind-0.1.0-cp311-cp311-macosx_11_0_arm64.whl.zip` & `tmp/vfind-0.1.1-cp312-cp312-manylinux_2_34_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3008631 bytes, number of entries: 6
--rw-r--r--  4.6 unx     7891 b- defN 24-Apr-15 20:49 vfind-0.1.0.dist-info/METADATA
--rw-r--r--  4.6 unx      104 b- defN 24-Apr-15 20:49 vfind-0.1.0.dist-info/WHEEL
--rw-r--r--  4.6 unx     1077 b- defN 24-Apr-15 20:49 vfind-0.1.0.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx      103 b- defN 24-Apr-15 20:49 vfind/__init__.py
--rwxr-xr-x  4.6 unx 14949712 b- defN 24-Apr-15 20:49 vfind/vfind.cpython-311-darwin.so
--rw-r--r--  4.6 unx      468 b- defN 24-Apr-15 20:49 vfind-0.1.0.dist-info/RECORD
-6 files, 14959355 bytes uncompressed, 3007797 bytes compressed:  79.9%
+Zip file size: 7600060 bytes, number of entries: 6
+-rw-r--r--  4.6 unx     7748 b- defN 24-May-06 05:13 vfind-0.1.1.dist-info/METADATA
+-rw-r--r--  4.6 unx      108 b- defN 24-May-06 05:13 vfind-0.1.1.dist-info/WHEEL
+-rw-r--r--  4.6 unx     1077 b- defN 24-May-06 05:13 vfind-0.1.1.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx      103 b- defN 24-May-06 05:13 vfind/__init__.py
+-rwxr-xr-x  4.6 unx 30228792 b- defN 24-May-06 05:13 vfind/vfind.cpython-312-x86_64-linux-gnu.so
+-rw-r--r--  4.6 unx      478 b- defN 24-May-06 05:13 vfind-0.1.1.dist-info/RECORD
+6 files, 30238306 bytes uncompressed, 7599206 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: vfind-0.1.0.dist-info/METADATA
+Filename: vfind-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: vfind-0.1.0.dist-info/WHEEL
+Filename: vfind-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: vfind-0.1.0.dist-info/license_files/LICENSE
+Filename: vfind-0.1.1.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: vfind/__init__.py
 Comment: 
 
-Filename: vfind/vfind.cpython-311-darwin.so
+Filename: vfind/vfind.cpython-312-x86_64-linux-gnu.so
 Comment: 
 
-Filename: vfind-0.1.0.dist-info/RECORD
+Filename: vfind-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `vfind-0.1.0.dist-info/METADATA` & `vfind-0.1.1.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: vfind
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: polars
 License-File: LICENSE
 Summary: A simple variant finder for NGS data
 Keywords: bioinformatics,sequence analysis,NGS,variant finding
@@ -12,14 +12,16 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Repository, https://github.com/nsbuitrago/vfind
 Project-URL: Issues, https://github.com/nsbuitrago/vfind/issues
 
 # vFind
 
+[![PyPI - Version](https://img.shields.io/pypi/v/vfind)](https://pypi.org/project/vfind/)
+
 *A simple variant finder for NGS data.*
 
 1. [Introduction](#introduction)
 2. [Installation](#installation)
 3. [Examples](#examples)
 4. [Contributing](#contributing)
 5. [License](#license)
@@ -27,76 +29,77 @@
 ## Introduction
 
 vFind is unlike a traditional [*variant caller*](https://gencore.bio.nyu.edu/variant-calling-pipeline-gatk4/).
 It is actually using a simpler algorithm which is *usually* sufficient for 
 screening experiments. The main use case is finding variants from a library that
 has constant adapter sequences flanking a variable region.
 
-The workflow can be described generally by these steps:
+This simple algorithm is summarized as:
 
-1. define a set of constant adapter sequences that immediately flank a variable region of interest.
-2. for each fastq read, search for exact matches of these adapters.
-3. in case of no exact match for either adapter, perform a semi-global alignment of
-the adapter sequence on the fastq read.
-4. if the alignment is produces a score that is above a set threshold, recover the variable region.
-To adjust the thresholds for accepting alignments, see the [alignment parameters](#using-custom-alignment-parameters) section
-
-Alignments are accepted if they produce a score above a set threshold.
-These thresholds correspond to the fraction of the max theoretical alignment score
-that can be produced from a given adapter sequence and fastq read. Thus, thresholds
-are values between 0 and 1. By default, thresholds for both adapter sequences are
-set to 0.75. In some cases, you may want to change these values to be more or less
-stringent. 
+1. Define a pair of adapter sequences that flank the variable region.
+2. For each fastq read, search for exact matches of these adapters.
+3. If both adapters are found exactly, recover the variable region.
+4. For each adapter without an exact match, perform semi-global alignment between the given adapter and read (optional see the [alignment parameters](#using-custom-alignment-parameters) section).
+5. If the alignment score meets a set threshold, that adapter is considered to match.
+6. If both adapters are exactly or partially matched, recover the variable region.
+7. For exact matches of both adapters, recover the variable region. Otherwise, continue to the next read.
+8. Finally, translate the variable region to its amino acid sequence and filter out any sequences with partial codons (Optional, see the [miscellaneuous](#miscellaneuous) section).
 
 > [!WARNING]
-> Note that vFind doesn't do any kind of fastq preprocessing. For initial quality
+> Note that vFind doesn't do any kind of preprocessing. For initial quality
 > filtering, merging, and other common preprocessing operations, you might be
-> interested in something like [fastp]() or [ngmerge](). We generally recommend
-> using fastp for quality filtering and merging fastq files before using vFind.
+> interested in something like [fastp](https://github.com/OpenGene/fastp) or
+> [ngmerge](https://github.com/jsh58/NGmerge). We generally recommend using
+> fastp for quality filtering and merging fastq files before using vFind.
+
+Installation details and usage examples are given below. For more usage details,
+please see the [API reference](docs/api-reference.md)
 
 ## Installation
 
+vFind is a Python package and can be installed via pip or nix. For a CLI version,
+see the [vFind-cli](https://github.com/nsbuitrago/vfind-cli) repository.
+
 ### PyPI (Recommended for most)
 
-vFind is available on [PyPI](https://pypi.org/) and can be installed via pip (or alternatives like
-[uv](https://github.com/astral-sh/uv)).
+The package is available on [PyPI](https://pypi.org/project/vfind) and can be installed via pip (or alternatives like [uv](https://github.com/astral-sh/uv)).
 
 Below is an example using pip with Python3 in a new project.
 
 ```bash
 # create a new virtual env
 python3 -m venv .venv # create a new virtual env if haven't already
 source .venv/bin/activate # activate the virtual env
 
 python3 -m pip install vfind # install vfind
 ```
 
 ### Nix
 
-vFind is also available as a Python package on [NixPkgs](https://search.nixos.org/packages?). You can declare new
-development enviroments using [nix flakes](https://wiki.nixos.org/wiki/Flakes).
+vFind is also available on [NixPkgs](https://search.nixos.org/packages?). You can declare new
+enviroments using [nix flakes](https://wiki.nixos.org/wiki/Flakes).
 
-For something quick, you can use nix-shell,
+For something quick, you can use nix-shell. For example, the following will
+create a new shell with Python 3.11, vFind, and polars installed.
 
 ```bash
-nix-shell -p python311 python3Packages.vfind
+nix-shell -p python311 python3Packages.vfind python3Packages.polars
 ```
 
 ## Examples
 
 ### Basic Usage
 
 ```python
 from vfind import find_variants
 import polars as pl # variants are returned in a polars dataframe
 
-adapters = ("GGG", "CCC") # define the Adapters
-fq_path = "./path/to/your/fastq/file.fq.gz" # path fo fq file
+adapters = ("GGG", "CCC") # define the adapters
+fq_path = "./path/to/your/fastq/file.fq.gz" # path to fq file
 
-# now, let's find some variants
 variants = find_variants(fq_path, adapters)
 
 # print the number of unique sequences 
 print(variants.n_unique())
 ```
 
 `find_variants` returns a polars dataframe with `sequence` and `count` columns.
@@ -111,15 +114,15 @@
 variants.sort("count", descending=True) # sort by the counts in descending order
 print(variants.head(5)) # print the first 5 (most frequent) variants
 
 # filter out sequences with less than 10 read counts
 # also any sequences that have a pre-mature stop codon (i.e., * before the last residue)
 
 filtered_variants = variants.filter(
-    ~variants["counts"] < 10,
+    variants["count"] > 10,
     ~variants["sequence"][::-2].str.contains("*")
 )
 
 # write the filtered variants to a csv file
 filtered_variants.write_csv("filtered_variants.csv")
 ```
 
@@ -128,16 +131,19 @@
 By default, vFind uses semi-global alignment with the following parameters:
 
 - match score = 3
 - mismatch score = -2
 - gap open penalty = 5
 - gap extend penalty = 2
 
-Note that the gap penalties are represented as positive integers. This is largely due to the underlying
-alignment library.
+Note that the gap penalties are represented as positive integers. This is largely due to how the underlying
+alignment library works.
+
+To adjust these alignment parameters, use the `match_score`, `mismatch_score`,
+`gap_open_penalty`, and `gap_extend_penalty` keyword arguments:
 
 ```python
 from vfind import find_variants
 
 # ... define adapters and fq_path
 
 # use identity scoring with no gap penalties for alignments
@@ -147,24 +153,23 @@
     match_score = 1,
     mismatch_score = -1,
     gap_open_penalty: 0,
     gap_extend_penalty: 0,
 )
 ```
 
-Only alignments that produce scores meeting a threshold will be considered accepted. 
-The threshold for considering an acceptable alignment can be adjusted with the
-`accept_prefix_alignment` and `accept_suffix_alignment` arguments. By default,
-both thresholds are set to 0.75.
-
-The thresholds represent a fraction of the maximum alignment score. So, a value of 0.75
-means alignments producing scores that are greater than 75% the maximum theoretical score
-will be accepted.
+Alignments are accepted if they produce a score above a set threshold. The threshold
+for considering an acceptable alignment can be adjusted with the `accept_prefix_alignment`
+and `accept_suffix_alignment` arguments. By default, both thresholds are set to 0.75.
+
+The thresholds are represent a percentage of the maximum alignment score. So, a value of 0.75
+means alignments producing scores that are greater than 75% the maximum theoretical score will be accepted. Thus, valid values are between 0 and 1.
 
 Either an exact match or partial match (accepted alignment) must be made for both adapter sequences to recover a variant. 
+In order to skip alignment and only look for exact matches, set the `skip_alignment` argument to `True`.
 
 ### Miscellaneous
 
 **Q:** I don't need the amino acid sequence. Can I just get the DNA sequence?
 
 **A:** Yes. Just set `skip_translation` to True.
 
@@ -177,62 +182,29 @@
 
 **Q:** I don't want to use polars. Can I use pandas instead?
 
 **A:** Yes. Use the [`to_pandas`](https://docs.pola.rs/py-polars/html/reference/dataframe/api/polars.DataFrame.to_pandas.html#polars.DataFrame.to_pandas) method on the dataframe.
 
 ---
 
-**Q:** `find_variants` is slow. Is there anything I can do to speed it up?
+**Q:** I have a lot of data and `find_variants` is slow. Is there anything I can do to speed it up?
 
-**A:** Maybe? Try changing the number of threads or queue length the function uses.
+**A:** Maybe. Try changing the number of threads or queue length the function uses.
 
 ```python
 # ...
 variants = find_variants(fq_path, adapters, n_threads=6, queue_len=4)
 ```
 
-## Contributing
-
-Contributions are welcome. Please submit an issue or pull request for any bugs,
-suggestions, or feedback.
-
-### Developing
-
-vFind is written in Rust and uses [PyO3](https://pyo3.rs/v0.21.1/) and [Maturin](https://github.com/PyO3/maturin)
-to generate the Python module. To get started, you will need to have the
-[rust toolchain](https://www.rust-lang.org/tools/install) and [Python >= 3.10](https://www.python.org/downloads/).
+For more usage details, see the [API reference](docs/api-reference.md).
 
-Below are some general steps to get up and running. Note that these examples
-use [uv]). However, you could do this with standard pip or your preferred method.
-
-1. clone the repository to your machine
-
-```bash
-git clone git@github.com:nsbuitrago/vfind.git
-cd vfind
-```
-
-2. Create a new Python virtual environment and install dev dependencies.
-
-```bash
-uv venv
-source .venv/bin/activate
-
-# this will intsall maturin, polars, and any other required packages.
-uv pip install -r dev-requirements.txt
-```
-
-3. Build and install the vFind package in your virtual environment with maturin. 
-
-```bash
-# in the root project directory
-maturin develop
-```
+## Contributing
 
-4. From here, you can make changes to the Rust lib and run `maturin` develop
-to rebuild the package with those changes.
+Feedback is a gift and contributions are more than welcome. Please submit an
+issue or pull request for any bugs, suggestions, or feedback. Please see the 
+[developing](docs/developing) guide for more details on how to work on vFind.
 
 ## License
 
 vFind is licensed under the [MIT license](LICENSE)
```

## Comparing `vfind-0.1.0.dist-info/license_files/LICENSE` & `vfind-0.1.1.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

