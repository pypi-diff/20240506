# Comparing `tmp/fluidimage-0.5.0.tar.gz` & `tmp/fluidimage-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluidimage-0.5.0.tar", last modified: Thu May  2 10:24:20 2024, max compression
+gzip compressed data, was "fluidimage-0.5.1.tar", last modified: Mon May  6 09:04:16 2024, max compression
```

## Comparing `fluidimage-0.5.0.tar` & `fluidimage-0.5.1.tar`

### file list

```diff
@@ -1,263 +1,263 @@
--rw-r--r--   0        0        0       58 2024-05-02 10:23:27.000000 fluidimage-0.5.0/.flake8
--rw-r--r--   0        0        0     1166 2024-05-02 10:23:27.000000 fluidimage-0.5.0/.github/workflows/ci-linux.yml
--rw-r--r--   0        0        0      554 2024-05-02 10:23:27.000000 fluidimage-0.5.0/.github/workflows/ci-pixi.yml
--rw-r--r--   0        0        0     3919 2024-05-02 10:23:27.000000 fluidimage-0.5.0/.github/workflows/wheels.yml
--rw-r--r--   0        0        0     3223 2024-05-02 10:23:27.000000 fluidimage-0.5.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     1104 2024-05-02 10:23:27.000000 fluidimage-0.5.0/.hgtags
--rw-r--r--   0        0        0       43 2024-05-02 10:23:27.000000 fluidimage-0.5.0/.mdformat.toml
--rw-r--r--   0        0        0      376 2024-05-02 10:23:27.000000 fluidimage-0.5.0/.readthedocs.yml
--rw-r--r--   0        0        0      210 2024-05-02 10:23:27.000000 fluidimage-0.5.0/AUTHORS.md
--rw-r--r--   0        0        0     7457 2024-05-02 10:23:27.000000 fluidimage-0.5.0/CHANGES.md
--rw-r--r--   0        0        0     1266 2024-05-02 10:23:27.000000 fluidimage-0.5.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    21781 2024-05-02 10:23:27.000000 fluidimage-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0      205 2024-05-02 10:23:27.000000 fluidimage-0.5.0/MANIFEST.in
--rw-r--r--   0        0        0      309 2024-05-02 10:23:27.000000 fluidimage-0.5.0/Makefile
--rw-r--r--   0        0        0     3151 2024-05-02 10:23:27.000000 fluidimage-0.5.0/README.md
--rw-r--r--   0        0        0     1266 2024-05-02 10:24:19.935472 fluidimage-0.5.0/doc/CONTRIBUTING.md
--rw-r--r--   0        0        0     5780 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/Makefile
--rw-r--r--   0        0        0      210 2024-05-02 10:24:19.935472 fluidimage-0.5.0/doc/authors.md
--rw-r--r--   0        0        0      748 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/autosum.rst
--rw-r--r--   0        0        0     8443 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/build-from-source.md
--rw-r--r--   0        0        0     7457 2024-05-02 10:24:19.935472 fluidimage-0.5.0/doc/changes.md
--rw-r--r--   0        0        0     9545 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/conf.py
--rw-r--r--   0        0        0       36 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/Makefile
--rw-r--r--   0        0        0      275 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/bos_parallel.md
--rw-r--r--   0        0        0      708 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/bos_parallel.py
--rw-r--r--   0        0        0      914 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/im2im_parallel.py
--rw-r--r--   0        0        0      442 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/im2im_try_params.py
--rw-r--r--   0        0        0      217 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/my_example_im2im.py
--rw-r--r--   0        0        0      370 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/my_example_im2im_class.py
--rw-r--r--   0        0        0      375 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/optflow_parallel.md
--rw-r--r--   0        0        0      864 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/optflow_parallel.py
--rw-r--r--   0        0        0      645 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/optflow_try_params.md
--rw-r--r--   0        0        0      675 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/optflow_try_params.py
--rw-r--r--   0        0        0     2124 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_as_real/README.md
--rw-r--r--   0        0        0        0 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_as_real/__init__.py
--rw-r--r--   0        0        0     1386 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_as_real/args.py
--rwxr-xr-x   0        0        0      779 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_as_real/job_piv.py
--rwxr-xr-x   0        0        0     1095 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_as_real/job_pre.py
--rwxr-xr-x   0        0        0     2087 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_as_real/params_piv.py
--rwxr-xr-x   0        0        0     1811 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_as_real/params_pre.py
--rwxr-xr-x   0        0        0      672 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_as_real/submit_piv.py
--rwxr-xr-x   0        0        0      787 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_as_real/submit_pre.py
--rw-r--r--   0        0        0      896 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_as_real/test_piv_as_real.py
--rwxr-xr-x   0        0        0      724 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_as_real/try_piv.py
--rwxr-xr-x   0        0        0      538 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_as_real/try_pre.py
--rw-r--r--   0        0        0      457 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_cluster.md
--rw-r--r--   0        0        0      918 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_parallel.md
--rw-r--r--   0        0        0      827 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_parallel.py
--rw-r--r--   0        0        0      536 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_parallel_complete.py
--rw-r--r--   0        0        0      953 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_parallel_im2im.py
--rw-r--r--   0        0        0      989 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_parallel_im2im_class.py
--rw-r--r--   0        0        0      863 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_try_params.md
--rw-r--r--   0        0        0      614 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_try_params.py
--rw-r--r--   0        0        0      747 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_try_params_Karman.py
--rw-r--r--   0        0        0      814 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/piv_try_params_with_im2im_preproc.py
--rw-r--r--   0        0        0      380 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/pivchallenge/README.md
--rw-r--r--   0        0        0      908 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/pivchallenge/bench_piv_2005C.py
--rw-r--r--   0        0        0     1419 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/pivchallenge/download.py
--rw-r--r--   0        0        0      744 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/pivchallenge/path_images.py
--rw-r--r--   0        0        0      437 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/pivchallenge/piv_2001A_topology.py
--rw-r--r--   0        0        0      496 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/pivchallenge/piv_2001A_work.py
--rw-r--r--   0        0        0      622 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/pivchallenge/piv_2005C_topology.py
--rw-r--r--   0        0        0      682 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/pivchallenge/piv_2005C_work.py
--rw-r--r--   0        0        0      117 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/pivchallenge/possible_paths.txt
--rw-r--r--   0        0        0     1413 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/preproc.md
--rw-r--r--   0        0        0     1061 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/preproc_parallel.py
--rw-r--r--   0        0        0      816 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/preproc_sback1_filter.py
--rw-r--r--   0        0        0     1037 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/preproc_sback2_rescale.py
--rw-r--r--   0        0        0      544 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/preproc_try_params.py
--rw-r--r--   0        0        0      364 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/preproc_try_params_opencv.py
--rw-r--r--   0        0        0     1553 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/profile_piv_work.py
--rw-r--r--   0        0        0      448 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/submit_job_legi.py
--rw-r--r--   0        0        0      711 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/surface_tracking.py
--rw-r--r--   0        0        0     1201 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples/test_run_examples.py
--rw-r--r--   0        0        0      357 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/examples.md
--rw-r--r--   0        0        0      238 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/for_dev.md
--rw-r--r--   0        0        0      673 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/index.md
--rw-r--r--   0        0        0     1686 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/install.md
--rw-r--r--   0        0        0      405 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/ipynbslides/README.txt
--rw-r--r--   0        0        0   493343 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/ipynbslides/fluidimage_legi_20170403.ipynb
--rw-r--r--   0        0        0     2094 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/overview.md
--rw-r--r--   0        0        0     1424 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/overview_orga_package.md
--rw-r--r--   0        0        0     1857 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/related_codes.md
--rw-r--r--   0        0        0       77 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/to_do.md
--rw-r--r--   0        0        0      432 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/tutorial.md
--rw-r--r--   0        0        0     3116 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/tutorials/tuto_calibration2dsimple.md
--rw-r--r--   0        0        0     2412 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/tutorials/tuto_direct_calibration.md
--rw-r--r--   0        0        0     7352 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/tutorials/tuto_opencv_calibration.md
--rw-r--r--   0        0        0     4407 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/tutorials/tuto_opencv_tomo_reconstruct.md
--rw-r--r--   0        0        0     8785 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/tutorials/tuto_piv.md
--rw-r--r--   0        0        0     2950 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/tutorials/tuto_stereo_reconstruction.md
--rw-r--r--   0        0        0     1367 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/tutorials/tuto_tsai_calibration.md
--rw-r--r--   0        0        0     8971 2024-05-02 10:23:27.000000 fluidimage-0.5.0/doc/uvmat.md
--rw-r--r--   0        0        0     1252 2024-05-02 10:23:27.000000 fluidimage-0.5.0/docker/Dockerfile
--rw-r--r--   0        0        0     1147 2024-05-02 10:23:27.000000 fluidimage-0.5.0/docker/Makefile
--rw-r--r--   0        0        0      618 2024-05-02 10:23:27.000000 fluidimage-0.5.0/docker/hgrc
--rw-r--r--   0        0        0       77 2024-05-02 10:23:27.000000 fluidimage-0.5.0/docker/pythranrc
--rw-r--r--   0        0        0     1803 2024-05-02 10:23:27.000000 fluidimage-0.5.0/meson.build
--rw-r--r--   0        0        0      655 2024-05-02 10:23:27.000000 fluidimage-0.5.0/meson.options
--rw-r--r--   0        0        0     4888 2024-05-02 10:23:27.000000 fluidimage-0.5.0/noxfile.py
--rw-r--r--   0        0        0   310844 2024-05-02 10:23:27.000000 fluidimage-0.5.0/pdm.lock
--rw-r--r--   0        0        0   782153 2024-05-02 10:23:27.000000 fluidimage-0.5.0/pixi.lock
--rw-r--r--   0        0        0     1009 2024-05-02 10:23:27.000000 fluidimage-0.5.0/pixi.toml
--rw-r--r--   0        0        0    21630 2024-05-02 10:23:27.000000 fluidimage-0.5.0/pylintrc
--rw-r--r--   0        0        0     4483 2024-05-02 10:23:27.000000 fluidimage-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3311 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/__init__.py
--rw-r--r--   0        0        0      534 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/_opencv.py
--rw-r--r--   0        0        0      162 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/_version.py
--rw-r--r--   0        0        0      278 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/bos.py
--rw-r--r--   0        0        0      263 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/__init__.py
--rw-r--r--   0        0        0     2858 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/_evaluate_subpix.py
--rw-r--r--   0        0        0      878 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/correl.cu
--rw-r--r--   0        0        0    21039 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/correl.py
--rw-r--r--   0        0        0    10794 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/correl_pycuda.py
--rw-r--r--   0        0        0      333 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/errors.py
--rw-r--r--   0        0        0     7467 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/fft.py
--rw-r--r--   0        0        0      132 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/interpolate/__init__.py
--rw-r--r--   0        0        0      613 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/interpolate/griddata.py
--rw-r--r--   0        0        0      388 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/interpolate/meson.build
--rw-r--r--   0        0        0      867 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/interpolate/test_thin_plate_spline.py
--rw-r--r--   0        0        0     8006 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/interpolate/thin_plate_spline.py
--rw-r--r--   0        0        0    10216 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/interpolate/thin_plate_spline_subdom.py
--rw-r--r--   0        0        0     4807 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/mean_neighbors.py
--rw-r--r--   0        0        0      489 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/meson.build
--rw-r--r--   0        0        0    39595 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=1.0 _nx_ny = 64_64.png
--rw-r--r--   0        0        0    37615 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=2.0 _nx_ny = 64_64.png
--rw-r--r--   0        0        0    36317 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=3.0 _nx_ny = 64_64.png
--rw-r--r--   0        0        0    35832 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=4.0 _nx_ny = 64_64.png
--rw-r--r--   0        0        0    37828 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=1.0 _nx_ny = 64_64.png
--rw-r--r--   0        0        0    38146 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=2.0 _nx_ny = 64_64.png
--rw-r--r--   0        0        0    36451 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=3.0 _nx_ny = 64_64.png
--rw-r--r--   0        0        0    34562 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=4.0 _nx_ny = 64_64.png
--rw-r--r--   0        0        0     1188 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/reduction_kernel.cu
--rw-r--r--   0        0        0     6180 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/subpix.py
--rw-r--r--   0        0        0     6544 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/test_correl.py
--rw-r--r--   0        0        0     2519 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calcul/test_fft.py
--rw-r--r--   0        0        0      465 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calibration/__init__.py
--rw-r--r--   0        0        0     3587 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calibration/calib2d_simple.py
--rw-r--r--   0        0        0     9318 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calibration/calib_cv.py
--rw-r--r--   0        0        0    23798 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calibration/calib_direct.py
--rw-r--r--   0        0        0     7528 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calibration/calib_tsai.py
--rw-r--r--   0        0        0      302 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calibration/meson.build
--rw-r--r--   0        0        0     2033 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calibration/test_calib_cv.py
--rw-r--r--   0        0        0     2609 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calibration/test_direct_stereo_reconstruction.py
--rw-r--r--   0        0        0     1302 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calibration/test_tsai_calibration.py
--rw-r--r--   0        0        0     4272 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/calibration/util.py
--rw-r--r--   0        0        0      739 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/config.py
--rw-r--r--   0        0        0     1434 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/conftest.py
--rw-r--r--   0        0        0      274 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/data_objects/__init__.py
--rw-r--r--   0        0        0    13511 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/data_objects/display_piv.py
--rw-r--r--   0        0        0     4822 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/data_objects/display_pre.py
--rw-r--r--   0        0        0      214 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/data_objects/meson.build
--rw-r--r--   0        0        0    26293 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/data_objects/piv.py
--rw-r--r--   0        0        0     4457 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/data_objects/preproc.py
--rw-r--r--   0        0        0      425 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/data_objects/test_piv.py
--rw-r--r--   0        0        0     9009 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/data_objects/tomo.py
--rw-r--r--   0        0        0     3376 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/executors/__init__.py
--rw-r--r--   0        0        0    17837 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/executors/base.py
--rw-r--r--   0        0        0    10536 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/executors/exec_async.py
--rw-r--r--   0        0        0     4054 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/executors/exec_async_multiproc.py
--rw-r--r--   0        0        0     3892 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/executors/exec_async_seq_for_multi.py
--rw-r--r--   0        0        0     2106 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/executors/exec_async_sequential.py
--rw-r--r--   0        0        0     8058 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/executors/exec_async_servers.py
--rw-r--r--   0        0        0      396 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/executors/exec_async_servers_threading.py
--rw-r--r--   0        0        0     2210 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/executors/exec_sequential.py
--rw-r--r--   0        0        0      393 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/executors/meson.build
--rw-r--r--   0        0        0     7358 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/executors/multi_exec_async.py
--rw-r--r--   0        0        0     3668 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/executors/multi_exec_subproc.py
--rw-r--r--   0        0        0     7661 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/executors/servers.py
--rw-r--r--   0        0        0      338 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/__init__.py
--rw-r--r--   0        0        0      769 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/base_matplotlib.py
--rw-r--r--   0        0        0     8981 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/imviewer.py
--rw-r--r--   0        0        0      228 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/launcher/Makefile
--rw-r--r--   0        0        0      153 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/launcher/__init__.py
--rw-r--r--   0        0        0     2659 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/launcher/main.py
--rw-r--r--   0        0        0     3750 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/launcher/mainwindow.py
--rw-r--r--   0        0        0     1671 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/launcher/mainwindow.ui
--rw-r--r--   0        0        0      170 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/launcher/meson.build
--rw-r--r--   0        0        0      568 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/launcher/test_launcher.py
--rw-r--r--   0        0        0      348 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/meson.build
--rw-r--r--   0        0        0    10703 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/monitor.py
--rw-r--r--   0        0        0       67 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/monitor.tcss
--rw-r--r--   0        0        0     2459 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/pg_main.py
--rw-r--r--   0        0        0     5903 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/pg_wrapper.py
--rw-r--r--   0        0        0     6018 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/piv_viewer.py
--rw-r--r--   0        0        0     1093 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/test_imviewer.py
--rw-r--r--   0        0        0      965 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/test_imviewer_pg.py
--rw-r--r--   0        0        0     2727 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/test_monitor.py
--rw-r--r--   0        0        0     1132 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/gui/test_piv_viewer.py
--rw-r--r--   0        0        0     2612 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/image2image.py
--rw-r--r--   0        0        0      543 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/meson.build
--rw-r--r--   0        0        0      337 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/optical_flow.py
--rw-r--r--   0        0        0      278 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/piv.py
--rw-r--r--   0        0        0      104 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/postproc/__init__.py
--rw-r--r--   0        0        0      210 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/postproc/meson.build
--rw-r--r--   0        0        0     2412 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/postproc/piv.py
--rw-r--r--   0        0        0    14134 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/postproc/postproc.py
--rw-r--r--   0        0        0     2927 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/postproc/test_piv.py
--rw-r--r--   0        0        0     3771 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/postproc/test_util.py
--rw-r--r--   0        0        0     4070 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/postproc/util.py
--rw-r--r--   0        0        0    24145 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/postproc/vector_field.py
--rw-r--r--   0        0        0      580 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/preproc.py
--rw-r--r--   0        0        0      351 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/reconstruct/__init__.py
--rw-r--r--   0        0        0      131 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/reconstruct/meson.build
--rw-r--r--   0        0        0      230 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/reconstruct/tomo/__init__.py
--rw-r--r--   0        0        0      151 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/reconstruct/tomo/meson.build
--rw-r--r--   0        0        0     7578 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/reconstruct/tomo/mlos.py
--rw-r--r--   0        0        0     1362 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/reconstruct/tomo/test_mlos.py
--rw-r--r--   0        0        0     2730 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/run_from_xml.py
--rw-r--r--   0        0        0     1605 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/synthetic.py
--rw-r--r--   0        0        0      521 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/test_image2image.py
--rw-r--r--   0        0        0     2259 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/test_run_from_xml.py
--rw-r--r--   0        0        0     2874 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/__init__.py
--rw-r--r--   0        0        0    17551 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/base.py
--rw-r--r--   0        0        0     6355 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/bos.py
--rw-r--r--   0        0        0     5706 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/example.py
--rw-r--r--   0        0        0     3999 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/image2image.py
--rw-r--r--   0        0        0     2497 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/launcher.py
--rw-r--r--   0        0        0    10341 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/log.py
--rw-r--r--   0        0        0      642 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/meson.build
--rw-r--r--   0        0        0     1422 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/nb_cpu_cores.py
--rw-r--r--   0        0        0     1020 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/optical_flow.py
--rw-r--r--   0        0        0     8851 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/piv.py
--rw-r--r--   0        0        0    10337 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/preproc.py
--rw-r--r--   0        0        0     8772 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/splitters.py
--rw-r--r--   0        0        0    10745 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/surface_tracking.py
--rw-r--r--   0        0        0     1347 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/test_bos.py
--rw-r--r--   0        0        0     1993 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/test_example.py
--rw-r--r--   0        0        0     1628 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/test_image2image.py
--rw-r--r--   0        0        0     1220 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/test_optical_flow.py
--rw-r--r--   0        0        0     2578 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/test_piv.py
--rw-r--r--   0        0        0     1773 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/test_preproc.py
--rw-r--r--   0        0        0     1919 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/test_splitters.py
--rw-r--r--   0        0        0     2251 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/topologies/test_surftracking.py
--rw-r--r--   0        0        0      741 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/util/__init__.py
--rw-r--r--   0        0        0     1318 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/util/log.py
--rw-r--r--   0        0        0      151 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/util/meson.build
--rw-r--r--   0        0        0      398 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/util/test_util.py
--rw-r--r--   0        0        0     3154 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/util/util.py
--rw-r--r--   0        0        0     7306 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/uvmat.py
--rw-r--r--   0        0        0     6699 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/__init__.py
--rw-r--r--   0        0        0     2662 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/bos.py
--rw-r--r--   0        0        0     2687 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/image2image.py
--rw-r--r--   0        0        0      301 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/meson.build
--rw-r--r--   0        0        0     6651 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/optical_flow.py
--rw-r--r--   0        0        0      198 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/piv/__init__.py
--rw-r--r--   0        0        0     7836 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/piv/fix.py
--rw-r--r--   0        0        0      179 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/piv/meson.build
--rw-r--r--   0        0        0     6418 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/piv/multipass.py
--rw-r--r--   0        0        0    26467 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/piv/singlepass.py
--rw-r--r--   0        0        0     2492 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/piv/test_piv.py
--rw-r--r--   0        0        0     4587 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/preproc/__init__.py
--rw-r--r--   0        0        0     3844 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/preproc/_toolbox_cv.py
--rw-r--r--   0        0        0    14387 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/preproc/_toolbox_py.py
--rw-r--r--   0        0        0     2213 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/preproc/io.py
--rw-r--r--   0        0        0      184 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/preproc/meson.build
--rw-r--r--   0        0        0     3977 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/preproc/toolbox.py
--rw-r--r--   0        0        0    22183 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/surface_tracking.py
--rw-r--r--   0        0        0      776 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/test_bos.py
--rw-r--r--   0        0        0      542 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/test_image2image.py
--rw-r--r--   0        0        0     1815 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/test_preproc.py
--rw-r--r--   0        0        0     1307 2024-05-02 10:23:27.000000 fluidimage-0.5.0/src/fluidimage/works/with_mask.py
--rw-r--r--   0        0        0     4742 2024-05-02 10:24:20.412518 fluidimage-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0       58 2024-05-06 08:54:34.000000 fluidimage-0.5.1/.flake8
+-rw-r--r--   0        0        0     1166 2024-05-06 08:54:34.000000 fluidimage-0.5.1/.github/workflows/ci-linux.yml
+-rw-r--r--   0        0        0      554 2024-05-06 08:54:34.000000 fluidimage-0.5.1/.github/workflows/ci-pixi.yml
+-rw-r--r--   0        0        0     3919 2024-05-06 08:54:34.000000 fluidimage-0.5.1/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0     3223 2024-05-06 08:54:34.000000 fluidimage-0.5.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1151 2024-05-06 08:54:34.000000 fluidimage-0.5.1/.hgtags
+-rw-r--r--   0        0        0       43 2024-05-06 08:54:34.000000 fluidimage-0.5.1/.mdformat.toml
+-rw-r--r--   0        0        0      376 2024-05-06 08:54:34.000000 fluidimage-0.5.1/.readthedocs.yml
+-rw-r--r--   0        0        0      210 2024-05-06 08:54:34.000000 fluidimage-0.5.1/AUTHORS.md
+-rw-r--r--   0        0        0     7668 2024-05-06 08:54:34.000000 fluidimage-0.5.1/CHANGES.md
+-rw-r--r--   0        0        0     1266 2024-05-06 08:54:34.000000 fluidimage-0.5.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    21781 2024-05-06 08:54:34.000000 fluidimage-0.5.1/LICENSE.txt
+-rw-r--r--   0        0        0      205 2024-05-06 08:54:34.000000 fluidimage-0.5.1/MANIFEST.in
+-rw-r--r--   0        0        0      309 2024-05-06 08:54:34.000000 fluidimage-0.5.1/Makefile
+-rw-r--r--   0        0        0     3151 2024-05-06 08:54:34.000000 fluidimage-0.5.1/README.md
+-rw-r--r--   0        0        0     1266 2024-05-06 09:04:15.958915 fluidimage-0.5.1/doc/CONTRIBUTING.md
+-rw-r--r--   0        0        0     5780 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/Makefile
+-rw-r--r--   0        0        0      210 2024-05-06 09:04:15.958915 fluidimage-0.5.1/doc/authors.md
+-rw-r--r--   0        0        0      748 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/autosum.rst
+-rw-r--r--   0        0        0     8443 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/build-from-source.md
+-rw-r--r--   0        0        0     7668 2024-05-06 09:04:15.958915 fluidimage-0.5.1/doc/changes.md
+-rw-r--r--   0        0        0     9545 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/conf.py
+-rw-r--r--   0        0        0       36 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/Makefile
+-rw-r--r--   0        0        0      275 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/bos_parallel.md
+-rw-r--r--   0        0        0      708 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/bos_parallel.py
+-rw-r--r--   0        0        0      914 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/im2im_parallel.py
+-rw-r--r--   0        0        0      442 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/im2im_try_params.py
+-rw-r--r--   0        0        0      217 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/my_example_im2im.py
+-rw-r--r--   0        0        0      370 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/my_example_im2im_class.py
+-rw-r--r--   0        0        0      375 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/optflow_parallel.md
+-rw-r--r--   0        0        0      864 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/optflow_parallel.py
+-rw-r--r--   0        0        0      645 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/optflow_try_params.md
+-rw-r--r--   0        0        0      675 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/optflow_try_params.py
+-rw-r--r--   0        0        0     2124 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_as_real/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_as_real/__init__.py
+-rw-r--r--   0        0        0     1386 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_as_real/args.py
+-rwxr-xr-x   0        0        0      779 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_as_real/job_piv.py
+-rwxr-xr-x   0        0        0     1095 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_as_real/job_pre.py
+-rwxr-xr-x   0        0        0     2086 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_as_real/params_piv.py
+-rwxr-xr-x   0        0        0     1811 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_as_real/params_pre.py
+-rwxr-xr-x   0        0        0      672 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_as_real/submit_piv.py
+-rwxr-xr-x   0        0        0      787 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_as_real/submit_pre.py
+-rw-r--r--   0        0        0      896 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_as_real/test_piv_as_real.py
+-rwxr-xr-x   0        0        0      724 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_as_real/try_piv.py
+-rwxr-xr-x   0        0        0      538 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_as_real/try_pre.py
+-rw-r--r--   0        0        0      457 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_cluster.md
+-rw-r--r--   0        0        0      918 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_parallel.md
+-rw-r--r--   0        0        0      827 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_parallel.py
+-rw-r--r--   0        0        0      536 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_parallel_complete.py
+-rw-r--r--   0        0        0      953 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_parallel_im2im.py
+-rw-r--r--   0        0        0      989 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_parallel_im2im_class.py
+-rw-r--r--   0        0        0      863 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_try_params.md
+-rw-r--r--   0        0        0      614 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_try_params.py
+-rw-r--r--   0        0        0      747 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_try_params_Karman.py
+-rw-r--r--   0        0        0      814 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/piv_try_params_with_im2im_preproc.py
+-rw-r--r--   0        0        0      380 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/pivchallenge/README.md
+-rw-r--r--   0        0        0      908 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/pivchallenge/bench_piv_2005C.py
+-rw-r--r--   0        0        0     1419 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/pivchallenge/download.py
+-rw-r--r--   0        0        0      744 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/pivchallenge/path_images.py
+-rw-r--r--   0        0        0      437 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/pivchallenge/piv_2001A_topology.py
+-rw-r--r--   0        0        0      496 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/pivchallenge/piv_2001A_work.py
+-rw-r--r--   0        0        0      622 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/pivchallenge/piv_2005C_topology.py
+-rw-r--r--   0        0        0      682 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/pivchallenge/piv_2005C_work.py
+-rw-r--r--   0        0        0      117 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/pivchallenge/possible_paths.txt
+-rw-r--r--   0        0        0     1413 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/preproc.md
+-rw-r--r--   0        0        0     1061 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/preproc_parallel.py
+-rw-r--r--   0        0        0      816 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/preproc_sback1_filter.py
+-rw-r--r--   0        0        0     1037 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/preproc_sback2_rescale.py
+-rw-r--r--   0        0        0      544 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/preproc_try_params.py
+-rw-r--r--   0        0        0      364 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/preproc_try_params_opencv.py
+-rw-r--r--   0        0        0     1552 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/profile_piv_work.py
+-rw-r--r--   0        0        0      448 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/submit_job_legi.py
+-rw-r--r--   0        0        0      711 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/surface_tracking.py
+-rw-r--r--   0        0        0     1201 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples/test_run_examples.py
+-rw-r--r--   0        0        0      357 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/examples.md
+-rw-r--r--   0        0        0      238 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/for_dev.md
+-rw-r--r--   0        0        0      673 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/index.md
+-rw-r--r--   0        0        0     1686 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/install.md
+-rw-r--r--   0        0        0      405 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/ipynbslides/README.txt
+-rw-r--r--   0        0        0   493343 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/ipynbslides/fluidimage_legi_20170403.ipynb
+-rw-r--r--   0        0        0     2094 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/overview.md
+-rw-r--r--   0        0        0     1424 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/overview_orga_package.md
+-rw-r--r--   0        0        0     1857 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/related_codes.md
+-rw-r--r--   0        0        0       77 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/to_do.md
+-rw-r--r--   0        0        0      432 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/tutorial.md
+-rw-r--r--   0        0        0     3116 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/tutorials/tuto_calibration2dsimple.md
+-rw-r--r--   0        0        0     2412 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/tutorials/tuto_direct_calibration.md
+-rw-r--r--   0        0        0     7352 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/tutorials/tuto_opencv_calibration.md
+-rw-r--r--   0        0        0     4407 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/tutorials/tuto_opencv_tomo_reconstruct.md
+-rw-r--r--   0        0        0     8785 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/tutorials/tuto_piv.md
+-rw-r--r--   0        0        0     2950 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/tutorials/tuto_stereo_reconstruction.md
+-rw-r--r--   0        0        0     1367 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/tutorials/tuto_tsai_calibration.md
+-rw-r--r--   0        0        0     8971 2024-05-06 08:54:34.000000 fluidimage-0.5.1/doc/uvmat.md
+-rw-r--r--   0        0        0     1252 2024-05-06 08:54:34.000000 fluidimage-0.5.1/docker/Dockerfile
+-rw-r--r--   0        0        0     1147 2024-05-06 08:54:34.000000 fluidimage-0.5.1/docker/Makefile
+-rw-r--r--   0        0        0      618 2024-05-06 08:54:34.000000 fluidimage-0.5.1/docker/hgrc
+-rw-r--r--   0        0        0       77 2024-05-06 08:54:34.000000 fluidimage-0.5.1/docker/pythranrc
+-rw-r--r--   0        0        0     1803 2024-05-06 08:54:34.000000 fluidimage-0.5.1/meson.build
+-rw-r--r--   0        0        0      655 2024-05-06 08:54:34.000000 fluidimage-0.5.1/meson.options
+-rw-r--r--   0        0        0     4888 2024-05-06 08:54:34.000000 fluidimage-0.5.1/noxfile.py
+-rw-r--r--   0        0        0   310844 2024-05-06 08:54:34.000000 fluidimage-0.5.1/pdm.lock
+-rw-r--r--   0        0        0   782153 2024-05-06 08:54:34.000000 fluidimage-0.5.1/pixi.lock
+-rw-r--r--   0        0        0     1009 2024-05-06 08:54:34.000000 fluidimage-0.5.1/pixi.toml
+-rw-r--r--   0        0        0    21630 2024-05-06 08:54:34.000000 fluidimage-0.5.1/pylintrc
+-rw-r--r--   0        0        0     4483 2024-05-06 08:54:34.000000 fluidimage-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3311 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/__init__.py
+-rw-r--r--   0        0        0      534 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/_opencv.py
+-rw-r--r--   0        0        0      162 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/_version.py
+-rw-r--r--   0        0        0      278 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/bos.py
+-rw-r--r--   0        0        0      263 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/__init__.py
+-rw-r--r--   0        0        0     2858 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/_evaluate_subpix.py
+-rw-r--r--   0        0        0      878 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/correl.cu
+-rw-r--r--   0        0        0    21039 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/correl.py
+-rw-r--r--   0        0        0    10794 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/correl_pycuda.py
+-rw-r--r--   0        0        0      333 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/errors.py
+-rw-r--r--   0        0        0     7467 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/fft.py
+-rw-r--r--   0        0        0      132 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/interpolate/__init__.py
+-rw-r--r--   0        0        0      613 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/interpolate/griddata.py
+-rw-r--r--   0        0        0      388 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/interpolate/meson.build
+-rw-r--r--   0        0        0      867 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/interpolate/test_thin_plate_spline.py
+-rw-r--r--   0        0        0     8006 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/interpolate/thin_plate_spline.py
+-rw-r--r--   0        0        0    10312 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/interpolate/thin_plate_spline_subdom.py
+-rw-r--r--   0        0        0     4807 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/mean_neighbors.py
+-rw-r--r--   0        0        0      489 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/meson.build
+-rw-r--r--   0        0        0    39595 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=1.0 _nx_ny = 64_64.png
+-rw-r--r--   0        0        0    37615 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=2.0 _nx_ny = 64_64.png
+-rw-r--r--   0        0        0    36317 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=3.0 _nx_ny = 64_64.png
+-rw-r--r--   0        0        0    35832 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=4.0 _nx_ny = 64_64.png
+-rw-r--r--   0        0        0    37828 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=1.0 _nx_ny = 64_64.png
+-rw-r--r--   0        0        0    38146 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=2.0 _nx_ny = 64_64.png
+-rw-r--r--   0        0        0    36451 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=3.0 _nx_ny = 64_64.png
+-rw-r--r--   0        0        0    34562 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=4.0 _nx_ny = 64_64.png
+-rw-r--r--   0        0        0     1188 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/reduction_kernel.cu
+-rw-r--r--   0        0        0     6180 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/subpix.py
+-rw-r--r--   0        0        0     6544 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/test_correl.py
+-rw-r--r--   0        0        0     2519 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calcul/test_fft.py
+-rw-r--r--   0        0        0      465 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calibration/__init__.py
+-rw-r--r--   0        0        0     3587 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calibration/calib2d_simple.py
+-rw-r--r--   0        0        0     9318 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calibration/calib_cv.py
+-rw-r--r--   0        0        0    23798 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calibration/calib_direct.py
+-rw-r--r--   0        0        0     7528 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calibration/calib_tsai.py
+-rw-r--r--   0        0        0      302 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calibration/meson.build
+-rw-r--r--   0        0        0     2033 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calibration/test_calib_cv.py
+-rw-r--r--   0        0        0     2609 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calibration/test_direct_stereo_reconstruction.py
+-rw-r--r--   0        0        0     1302 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calibration/test_tsai_calibration.py
+-rw-r--r--   0        0        0     4272 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/calibration/util.py
+-rw-r--r--   0        0        0      739 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/config.py
+-rw-r--r--   0        0        0     1434 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/conftest.py
+-rw-r--r--   0        0        0      274 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/data_objects/__init__.py
+-rw-r--r--   0        0        0    13511 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/data_objects/display_piv.py
+-rw-r--r--   0        0        0     4822 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/data_objects/display_pre.py
+-rw-r--r--   0        0        0      214 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/data_objects/meson.build
+-rw-r--r--   0        0        0    26293 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/data_objects/piv.py
+-rw-r--r--   0        0        0     4457 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/data_objects/preproc.py
+-rw-r--r--   0        0        0      425 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/data_objects/test_piv.py
+-rw-r--r--   0        0        0     9009 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/data_objects/tomo.py
+-rw-r--r--   0        0        0     3376 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/executors/__init__.py
+-rw-r--r--   0        0        0    17837 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/executors/base.py
+-rw-r--r--   0        0        0    10536 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/executors/exec_async.py
+-rw-r--r--   0        0        0     4054 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/executors/exec_async_multiproc.py
+-rw-r--r--   0        0        0     3892 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/executors/exec_async_seq_for_multi.py
+-rw-r--r--   0        0        0     2106 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/executors/exec_async_sequential.py
+-rw-r--r--   0        0        0     8058 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/executors/exec_async_servers.py
+-rw-r--r--   0        0        0      396 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/executors/exec_async_servers_threading.py
+-rw-r--r--   0        0        0     2210 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/executors/exec_sequential.py
+-rw-r--r--   0        0        0      393 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/executors/meson.build
+-rw-r--r--   0        0        0     7358 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/executors/multi_exec_async.py
+-rw-r--r--   0        0        0     3668 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/executors/multi_exec_subproc.py
+-rw-r--r--   0        0        0     7661 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/executors/servers.py
+-rw-r--r--   0        0        0      338 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/__init__.py
+-rw-r--r--   0        0        0      769 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/base_matplotlib.py
+-rw-r--r--   0        0        0     8981 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/imviewer.py
+-rw-r--r--   0        0        0      228 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/launcher/Makefile
+-rw-r--r--   0        0        0      153 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/launcher/__init__.py
+-rw-r--r--   0        0        0     2659 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/launcher/main.py
+-rw-r--r--   0        0        0     3750 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/launcher/mainwindow.py
+-rw-r--r--   0        0        0     1671 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/launcher/mainwindow.ui
+-rw-r--r--   0        0        0      170 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/launcher/meson.build
+-rw-r--r--   0        0        0      568 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/launcher/test_launcher.py
+-rw-r--r--   0        0        0      348 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/meson.build
+-rw-r--r--   0        0        0    10703 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/monitor.py
+-rw-r--r--   0        0        0       67 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/monitor.tcss
+-rw-r--r--   0        0        0     2459 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/pg_main.py
+-rw-r--r--   0        0        0     5903 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/pg_wrapper.py
+-rw-r--r--   0        0        0     6018 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/piv_viewer.py
+-rw-r--r--   0        0        0     1093 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/test_imviewer.py
+-rw-r--r--   0        0        0      965 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/test_imviewer_pg.py
+-rw-r--r--   0        0        0     2727 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/test_monitor.py
+-rw-r--r--   0        0        0     1132 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/gui/test_piv_viewer.py
+-rw-r--r--   0        0        0     2612 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/image2image.py
+-rw-r--r--   0        0        0      543 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/meson.build
+-rw-r--r--   0        0        0      337 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/optical_flow.py
+-rw-r--r--   0        0        0      278 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/piv.py
+-rw-r--r--   0        0        0      104 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/postproc/__init__.py
+-rw-r--r--   0        0        0      210 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/postproc/meson.build
+-rw-r--r--   0        0        0     2412 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/postproc/piv.py
+-rw-r--r--   0        0        0    14134 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/postproc/postproc.py
+-rw-r--r--   0        0        0     2927 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/postproc/test_piv.py
+-rw-r--r--   0        0        0     3771 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/postproc/test_util.py
+-rw-r--r--   0        0        0     4070 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/postproc/util.py
+-rw-r--r--   0        0        0    24145 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/postproc/vector_field.py
+-rw-r--r--   0        0        0      580 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/preproc.py
+-rw-r--r--   0        0        0      351 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/reconstruct/__init__.py
+-rw-r--r--   0        0        0      131 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/reconstruct/meson.build
+-rw-r--r--   0        0        0      230 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/reconstruct/tomo/__init__.py
+-rw-r--r--   0        0        0      151 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/reconstruct/tomo/meson.build
+-rw-r--r--   0        0        0     7578 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/reconstruct/tomo/mlos.py
+-rw-r--r--   0        0        0     1362 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/reconstruct/tomo/test_mlos.py
+-rw-r--r--   0        0        0     2730 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/run_from_xml.py
+-rw-r--r--   0        0        0     1605 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/synthetic.py
+-rw-r--r--   0        0        0      521 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/test_image2image.py
+-rw-r--r--   0        0        0     2259 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/test_run_from_xml.py
+-rw-r--r--   0        0        0     2874 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/__init__.py
+-rw-r--r--   0        0        0    17551 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/base.py
+-rw-r--r--   0        0        0     6355 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/bos.py
+-rw-r--r--   0        0        0     5706 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/example.py
+-rw-r--r--   0        0        0     3999 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/image2image.py
+-rw-r--r--   0        0        0     2497 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/launcher.py
+-rw-r--r--   0        0        0    10341 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/log.py
+-rw-r--r--   0        0        0      642 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/meson.build
+-rw-r--r--   0        0        0     1422 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/nb_cpu_cores.py
+-rw-r--r--   0        0        0     1020 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/optical_flow.py
+-rw-r--r--   0        0        0     8851 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/piv.py
+-rw-r--r--   0        0        0    10337 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/preproc.py
+-rw-r--r--   0        0        0     8772 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/splitters.py
+-rw-r--r--   0        0        0    10745 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/surface_tracking.py
+-rw-r--r--   0        0        0     1347 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/test_bos.py
+-rw-r--r--   0        0        0     1993 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/test_example.py
+-rw-r--r--   0        0        0     1628 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/test_image2image.py
+-rw-r--r--   0        0        0     1220 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/test_optical_flow.py
+-rw-r--r--   0        0        0     2578 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/test_piv.py
+-rw-r--r--   0        0        0     1773 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/test_preproc.py
+-rw-r--r--   0        0        0     1919 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/test_splitters.py
+-rw-r--r--   0        0        0     2251 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/topologies/test_surftracking.py
+-rw-r--r--   0        0        0      741 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/util/__init__.py
+-rw-r--r--   0        0        0     1318 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/util/log.py
+-rw-r--r--   0        0        0      151 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/util/meson.build
+-rw-r--r--   0        0        0      398 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/util/test_util.py
+-rw-r--r--   0        0        0     3154 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/util/util.py
+-rw-r--r--   0        0        0     7306 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/uvmat.py
+-rw-r--r--   0        0        0     6699 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/__init__.py
+-rw-r--r--   0        0        0     2662 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/bos.py
+-rw-r--r--   0        0        0     2687 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/image2image.py
+-rw-r--r--   0        0        0      301 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/meson.build
+-rw-r--r--   0        0        0     6651 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/optical_flow.py
+-rw-r--r--   0        0        0      198 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/piv/__init__.py
+-rw-r--r--   0        0        0     7836 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/piv/fix.py
+-rw-r--r--   0        0        0      179 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/piv/meson.build
+-rw-r--r--   0        0        0     6418 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/piv/multipass.py
+-rw-r--r--   0        0        0    26467 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/piv/singlepass.py
+-rw-r--r--   0        0        0     2492 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/piv/test_piv.py
+-rw-r--r--   0        0        0     4587 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/preproc/__init__.py
+-rw-r--r--   0        0        0     3844 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/preproc/_toolbox_cv.py
+-rw-r--r--   0        0        0    14387 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/preproc/_toolbox_py.py
+-rw-r--r--   0        0        0     2213 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/preproc/io.py
+-rw-r--r--   0        0        0      184 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/preproc/meson.build
+-rw-r--r--   0        0        0     3977 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/preproc/toolbox.py
+-rw-r--r--   0        0        0    22183 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/surface_tracking.py
+-rw-r--r--   0        0        0      776 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/test_bos.py
+-rw-r--r--   0        0        0      542 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/test_image2image.py
+-rw-r--r--   0        0        0     1815 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/test_preproc.py
+-rw-r--r--   0        0        0     1307 2024-05-06 08:54:34.000000 fluidimage-0.5.1/src/fluidimage/works/with_mask.py
+-rw-r--r--   0        0        0     4742 2024-05-06 09:04:16.440784 fluidimage-0.5.1/PKG-INFO
```

### Comparing `fluidimage-0.5.0/.github/workflows/ci-linux.yml` & `fluidimage-0.5.1/.github/workflows/ci-linux.yml`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/.github/workflows/ci-pixi.yml` & `fluidimage-0.5.1/.github/workflows/ci-pixi.yml`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/.github/workflows/wheels.yml` & `fluidimage-0.5.1/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/.gitlab-ci.yml` & `fluidimage-0.5.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/.hgtags` & `fluidimage-0.5.1/.hgtags`

 * *Files 19% similar despite different names*

```diff
@@ -17,7 +17,8 @@
 4bb44f739762f5fffbd2a8b0e7b759bd63709c03 0.4.1
 bb6f0ccc21452f0e1aa5caa5e058c8a163556c0d 0.4.2
 d1026b6b03c5e9ef8d0f23b60158684ed3d9e936 0.4.3
 f615cec0efdc3377cb9c7dfa96926fc2100d8c02 0.4.3.post0
 e66f70954560bbccdde36c76eac0a12f82ada45d 0.4.4
 80b7c7a51553b4ff08206a336e3e5d4795ffe306 0.4.5
 15eedfa330603df0403c6d8d6fc49ec468536e9b 0.4.6
+2c46b012bb330adfdac0d3c636af579e6b22426f 0.5.0
```

### Comparing `fluidimage-0.5.0/CHANGES.md` & `fluidimage-0.5.1/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # Release notes
 
 See also the
-[unreleased changes](https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.5.0...branch%2Fdefault).
+[unreleased changes](https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.5.1...branch%2Fdefault).
+
+## [0.5.1] (2024-05-06)
+
+- Follow UVmat: change defaults and exact meaning for parameter
+  `params.multipass.smoothing_coef` (=2).
 
 ## [0.5.0] (2024-05-02)
 
 - UVmat compatibility (launching in "local" mode).
 - Change defaults and exact meaning for parameters. `params.multipass.smoothing_coef`
   (=2) and `params.multipass.threshold_tps` (=1.5).
 - PIV saving: use float32 and save "smooth" displacement fields.
@@ -207,7 +212,8 @@
 [0.4.1]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.0...0.4.1
 [0.4.2]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.1...0.4.2
 [0.4.3]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.2...0.4.3
 [0.4.4]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.3...0.4.4
 [0.4.5]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.4...0.4.5
 [0.4.6]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.5...0.4.6
 [0.5.0]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.6...0.5.0
+[0.5.1]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.5.0...0.5.1
```

### Comparing `fluidimage-0.5.0/CONTRIBUTING.md` & `fluidimage-0.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/LICENSE.txt` & `fluidimage-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/README.md` & `fluidimage-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/CONTRIBUTING.md` & `fluidimage-0.5.1/doc/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/Makefile` & `fluidimage-0.5.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/autosum.rst` & `fluidimage-0.5.1/doc/autosum.rst`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/build-from-source.md` & `fluidimage-0.5.1/doc/build-from-source.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/changes.md` & `fluidimage-0.5.1/doc/changes.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # Release notes
 
 See also the
-[unreleased changes](https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.5.0...branch%2Fdefault).
+[unreleased changes](https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.5.1...branch%2Fdefault).
+
+## [0.5.1] (2024-05-06)
+
+- Follow UVmat: change defaults and exact meaning for parameter
+  `params.multipass.smoothing_coef` (=2).
 
 ## [0.5.0] (2024-05-02)
 
 - UVmat compatibility (launching in "local" mode).
 - Change defaults and exact meaning for parameters. `params.multipass.smoothing_coef`
   (=2) and `params.multipass.threshold_tps` (=1.5).
 - PIV saving: use float32 and save "smooth" displacement fields.
@@ -207,7 +212,8 @@
 [0.4.1]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.0...0.4.1
 [0.4.2]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.1...0.4.2
 [0.4.3]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.2...0.4.3
 [0.4.4]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.3...0.4.4
 [0.4.5]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.4...0.4.5
 [0.4.6]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.5...0.4.6
 [0.5.0]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.4.6...0.5.0
+[0.5.1]: https://foss.heptapod.net/fluiddyn/fluidimage/-/compare/0.5.0...0.5.1
```

### Comparing `fluidimage-0.5.0/doc/conf.py` & `fluidimage-0.5.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/bos_parallel.py` & `fluidimage-0.5.1/doc/examples/bos_parallel.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/im2im_parallel.py` & `fluidimage-0.5.1/doc/examples/im2im_parallel.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/optflow_parallel.py` & `fluidimage-0.5.1/doc/examples/optflow_parallel.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/optflow_try_params.md` & `fluidimage-0.5.1/doc/examples/optflow_try_params.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/optflow_try_params.py` & `fluidimage-0.5.1/doc/examples/optflow_try_params.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/piv_as_real/README.md` & `fluidimage-0.5.1/doc/examples/piv_as_real/README.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/piv_as_real/args.py` & `fluidimage-0.5.1/doc/examples/piv_as_real/args.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/piv_as_real/job_piv.py` & `fluidimage-0.5.1/doc/examples/piv_as_real/job_piv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/piv_as_real/job_pre.py` & `fluidimage-0.5.1/doc/examples/piv_as_real/job_pre.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/piv_as_real/params_piv.py` & `fluidimage-0.5.1/doc/examples/piv_as_real/params_piv.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     params.piv0.nb_peaks_to_search = 2
     params.piv0.particle_radius = 3
 
     params.mask.strcrop = ":, 50:"
 
     params.multipass.number = 2
     params.multipass.use_tps = "last"
-    params.multipass.smoothing_coef = 10.0
+    params.multipass.smoothing_coef = 5.0
     params.multipass.threshold_tps = 0.1
 
     params.fix.correl_min = 0.2
     params.fix.threshold_diff_neighbour = 2
 
     params.saving.how = savinghow
     params.saving.postfix = postfix_out
```

### Comparing `fluidimage-0.5.0/doc/examples/piv_as_real/params_pre.py` & `fluidimage-0.5.1/doc/examples/piv_as_real/params_pre.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/piv_as_real/submit_piv.py` & `fluidimage-0.5.1/doc/examples/piv_as_real/submit_piv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/piv_as_real/submit_pre.py` & `fluidimage-0.5.1/doc/examples/piv_as_real/submit_pre.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/piv_as_real/test_piv_as_real.py` & `fluidimage-0.5.1/doc/examples/piv_as_real/test_piv_as_real.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/piv_as_real/try_piv.py` & `fluidimage-0.5.1/doc/examples/piv_as_real/try_piv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/piv_as_real/try_pre.py` & `fluidimage-0.5.1/doc/examples/piv_as_real/try_pre.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/piv_parallel.md` & `fluidimage-0.5.1/doc/examples/piv_parallel.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/piv_parallel.py` & `fluidimage-0.5.1/doc/examples/piv_parallel.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/piv_parallel_complete.py` & `fluidimage-0.5.1/doc/examples/piv_parallel_complete.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/piv_parallel_im2im.py` & `fluidimage-0.5.1/doc/examples/piv_parallel_im2im.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/piv_parallel_im2im_class.py` & `fluidimage-0.5.1/doc/examples/piv_parallel_im2im_class.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/piv_try_params.md` & `fluidimage-0.5.1/doc/examples/piv_try_params.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/piv_try_params.py` & `fluidimage-0.5.1/doc/examples/piv_try_params.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/piv_try_params_Karman.py` & `fluidimage-0.5.1/doc/examples/piv_try_params_Karman.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 params.piv0.shape_crop_im0 = 32
 params.piv0.displacement_max = 5
 params.piv0.nb_peaks_to_search = 2
 
 params.multipass.number = 2
 params.multipass.use_tps = "last"
 params.multipass.subdom_size = 400
-params.multipass.smoothing_coef = 2.0
+params.multipass.smoothing_coef = 5.0
 
 work = Work(params=params)
 
 piv = work.process_1_serie()
 
 piv.display(show_interp=True, scale=0.3, show_error=False, show_correl=False)
 # piv.display(show_interp=False, scale=1, show_error=True)
```

### Comparing `fluidimage-0.5.0/doc/examples/piv_try_params_with_im2im_preproc.py` & `fluidimage-0.5.1/doc/examples/piv_try_params_with_im2im_preproc.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/pivchallenge/bench_piv_2005C.py` & `fluidimage-0.5.1/doc/examples/pivchallenge/bench_piv_2005C.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/pivchallenge/download.py` & `fluidimage-0.5.1/doc/examples/pivchallenge/download.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/pivchallenge/path_images.py` & `fluidimage-0.5.1/doc/examples/pivchallenge/path_images.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/pivchallenge/piv_2005C_topology.py` & `fluidimage-0.5.1/doc/examples/pivchallenge/piv_2005C_topology.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/pivchallenge/piv_2005C_work.py` & `fluidimage-0.5.1/doc/examples/pivchallenge/piv_2005C_work.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/preproc.md` & `fluidimage-0.5.1/doc/examples/preproc.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/preproc_parallel.py` & `fluidimage-0.5.1/doc/examples/preproc_parallel.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/preproc_sback1_filter.py` & `fluidimage-0.5.1/doc/examples/preproc_sback1_filter.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/preproc_sback2_rescale.py` & `fluidimage-0.5.1/doc/examples/preproc_sback2_rescale.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/preproc_try_params.py` & `fluidimage-0.5.1/doc/examples/preproc_try_params.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/profile_piv_work.py` & `fluidimage-0.5.1/doc/examples/profile_piv_work.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 params.mask.strcrop = ":, :1500"
 
 params.multipass.number = 2
 
 # params.multipass.use_tps = "last"
 params.multipass.use_tps = False
 params.multipass.subdom_size = 200
-params.multipass.smoothing_coef = 10.0
+params.multipass.smoothing_coef = 5.0
 params.multipass.threshold_tps = 1.5
 
 params.fix.correl_min = 0.15
 params.fix.threshold_diff_neighbour = 3
 
 work = Work(params=params)
```

### Comparing `fluidimage-0.5.0/doc/examples/surface_tracking.py` & `fluidimage-0.5.1/doc/examples/surface_tracking.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/examples/test_run_examples.py` & `fluidimage-0.5.1/doc/examples/test_run_examples.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/index.md` & `fluidimage-0.5.1/doc/index.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/install.md` & `fluidimage-0.5.1/doc/install.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/ipynbslides/fluidimage_legi_20170403.ipynb` & `fluidimage-0.5.1/doc/ipynbslides/fluidimage_legi_20170403.ipynb`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/overview.md` & `fluidimage-0.5.1/doc/overview.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/overview_orga_package.md` & `fluidimage-0.5.1/doc/overview_orga_package.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/related_codes.md` & `fluidimage-0.5.1/doc/related_codes.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/tutorials/tuto_calibration2dsimple.md` & `fluidimage-0.5.1/doc/tutorials/tuto_calibration2dsimple.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/tutorials/tuto_direct_calibration.md` & `fluidimage-0.5.1/doc/tutorials/tuto_direct_calibration.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/tutorials/tuto_opencv_calibration.md` & `fluidimage-0.5.1/doc/tutorials/tuto_opencv_calibration.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/tutorials/tuto_opencv_tomo_reconstruct.md` & `fluidimage-0.5.1/doc/tutorials/tuto_opencv_tomo_reconstruct.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/tutorials/tuto_piv.md` & `fluidimage-0.5.1/doc/tutorials/tuto_piv.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/tutorials/tuto_stereo_reconstruction.md` & `fluidimage-0.5.1/doc/tutorials/tuto_stereo_reconstruction.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/tutorials/tuto_tsai_calibration.md` & `fluidimage-0.5.1/doc/tutorials/tuto_tsai_calibration.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/doc/uvmat.md` & `fluidimage-0.5.1/doc/uvmat.md`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/docker/Dockerfile` & `fluidimage-0.5.1/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/docker/Makefile` & `fluidimage-0.5.1/docker/Makefile`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/docker/hgrc` & `fluidimage-0.5.1/docker/hgrc`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/meson.build` & `fluidimage-0.5.1/meson.build`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/meson.options` & `fluidimage-0.5.1/meson.options`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/noxfile.py` & `fluidimage-0.5.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/pdm.lock` & `fluidimage-0.5.1/pdm.lock`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/pixi.lock` & `fluidimage-0.5.1/pixi.lock`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/pixi.toml` & `fluidimage-0.5.1/pixi.toml`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/pylintrc` & `fluidimage-0.5.1/pylintrc`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/pyproject.toml` & `fluidimage-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "transonic>=0.6.2",
     "pythran>=0.9.7",
 ]
 build-backend = 'mesonpy'
 
 [project]
 name = "fluidimage"
-version = "0.5.0"
+version = "0.5.1"
 description = "Fluid image processing with Python."
 authors = [
     {name = "Pierre Augier", email = "pierre.augier@legi.cnrs.fr"},
 ]
 dependencies = [
     "numpy >= 1.8",
     "matplotlib >= 3.5",
```

### Comparing `fluidimage-0.5.0/src/fluidimage/__init__.py` & `fluidimage-0.5.1/src/fluidimage/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/_opencv.py` & `fluidimage-0.5.1/src/fluidimage/_opencv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calcul/_evaluate_subpix.py` & `fluidimage-0.5.1/src/fluidimage/calcul/_evaluate_subpix.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calcul/correl.cu` & `fluidimage-0.5.1/src/fluidimage/calcul/correl.cu`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calcul/correl.py` & `fluidimage-0.5.1/src/fluidimage/calcul/correl.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calcul/correl_pycuda.py` & `fluidimage-0.5.1/src/fluidimage/calcul/correl_pycuda.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calcul/fft.py` & `fluidimage-0.5.1/src/fluidimage/calcul/fft.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calcul/interpolate/griddata.py` & `fluidimage-0.5.1/src/fluidimage/calcul/interpolate/griddata.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calcul/interpolate/test_thin_plate_spline.py` & `fluidimage-0.5.1/src/fluidimage/calcul/interpolate/test_thin_plate_spline.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calcul/interpolate/thin_plate_spline.py` & `fluidimage-0.5.1/src/fluidimage/calcul/interpolate/thin_plate_spline.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calcul/interpolate/thin_plate_spline_subdom.py` & `fluidimage-0.5.1/src/fluidimage/calcul/interpolate/thin_plate_spline_subdom.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 .. autoclass:: ThinPlateSplineSubdom
    :members:
 
 """
 
 from logging import debug
+from math import sqrt
 from typing import List
 
 import numpy as np
 from transonic import Array
 
 from .thin_plate_spline import compute_tps_matrix, compute_tps_weights
 
@@ -53,32 +54,33 @@
         x_min, x_max = xs.min(), xs.max()
         y_min, y_max = ys.min(), ys.max()
         range_x = x_max - x_min
         range_y = y_max - y_min
         aspect_ratio = range_y / range_x
 
         nb_subdom = xs.size / self.subdom_size
-        nb_subdomx = int(np.floor(np.sqrt(nb_subdom / aspect_ratio)))
+        nb_subdomx = int(np.floor(sqrt(nb_subdom / aspect_ratio)))
         nb_subdomx = nb_subdomx or 1
-        nb_subdomy = int(np.ceil(np.sqrt(nb_subdom * aspect_ratio)))
+        nb_subdomy = int(np.ceil(sqrt(nb_subdom * aspect_ratio)))
         nb_subdomy = nb_subdomy or 1
 
         debug(f"nb_subdomx: {nb_subdomx} ; nb_subdomy: {nb_subdomy}")
 
         self.nb_subdomx = nb_subdomx
         self.nb_subdomy = nb_subdomy
         self.nb_subdom = nb_subdomx * nb_subdomy
 
         x_dom = np.linspace(x_min, x_max, nb_subdomx + 1)
         y_dom = np.linspace(y_min, y_max, nb_subdomy + 1)
 
         # normalization as UVmat so that the effect of the filter do not depends
         # too much on the size of the domains
-        self.smoothing_coef = (
-            smoothing_coef * (x_dom[1] - x_dom[0]) * (y_dom[1] - y_dom[0]) / 1000
+        num_vectors_per_subdom = xs.size / self.nb_subdom
+        self.smoothing_coef = smoothing_coef * sqrt(
+            (x_dom[1] - x_dom[0]) * (y_dom[1] - y_dom[0]) / num_vectors_per_subdom
         )
 
         coef_buffer = percent_buffer_area / 100
         buffer_length_x = coef_buffer * range_x / nb_subdomx
         buffer_length_y = coef_buffer * range_y / nb_subdomy
 
         self.limits_min_x = x_dom[:-1] - buffer_length_x
```

### Comparing `fluidimage-0.5.0/src/fluidimage/calcul/mean_neighbors.py` & `fluidimage-0.5.1/src/fluidimage/calcul/mean_neighbors.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=1.0 _nx_ny = 64_64.png` & `fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=1.0 _nx_ny = 64_64.png`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=2.0 _nx_ny = 64_64.png` & `fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=2.0 _nx_ny = 64_64.png`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=3.0 _nx_ny = 64_64.png` & `fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=3.0 _nx_ny = 64_64.png`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=4.0 _nx_ny = 64_64.png` & `fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/2d_gaussian _part_size=4.0 _nx_ny = 64_64.png`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=1.0 _nx_ny = 64_64.png` & `fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=1.0 _nx_ny = 64_64.png`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=2.0 _nx_ny = 64_64.png` & `fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=2.0 _nx_ny = 64_64.png`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=3.0 _nx_ny = 64_64.png` & `fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=3.0 _nx_ny = 64_64.png`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=4.0 _nx_ny = 64_64.png` & `fluidimage-0.5.1/src/fluidimage/calcul/plot_evaluate_subpix/centroid _part_size=4.0 _nx_ny = 64_64.png`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calcul/reduction_kernel.cu` & `fluidimage-0.5.1/src/fluidimage/calcul/reduction_kernel.cu`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calcul/subpix.py` & `fluidimage-0.5.1/src/fluidimage/calcul/subpix.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calcul/test_correl.py` & `fluidimage-0.5.1/src/fluidimage/calcul/test_correl.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calcul/test_fft.py` & `fluidimage-0.5.1/src/fluidimage/calcul/test_fft.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calibration/calib2d_simple.py` & `fluidimage-0.5.1/src/fluidimage/calibration/calib2d_simple.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calibration/calib_cv.py` & `fluidimage-0.5.1/src/fluidimage/calibration/calib_cv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calibration/calib_direct.py` & `fluidimage-0.5.1/src/fluidimage/calibration/calib_direct.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calibration/calib_tsai.py` & `fluidimage-0.5.1/src/fluidimage/calibration/calib_tsai.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calibration/test_calib_cv.py` & `fluidimage-0.5.1/src/fluidimage/calibration/test_calib_cv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calibration/test_direct_stereo_reconstruction.py` & `fluidimage-0.5.1/src/fluidimage/calibration/test_direct_stereo_reconstruction.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calibration/test_tsai_calibration.py` & `fluidimage-0.5.1/src/fluidimage/calibration/test_tsai_calibration.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/calibration/util.py` & `fluidimage-0.5.1/src/fluidimage/calibration/util.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/config.py` & `fluidimage-0.5.1/src/fluidimage/config.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/conftest.py` & `fluidimage-0.5.1/src/fluidimage/conftest.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/data_objects/display_piv.py` & `fluidimage-0.5.1/src/fluidimage/data_objects/display_piv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/data_objects/display_pre.py` & `fluidimage-0.5.1/src/fluidimage/data_objects/display_pre.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/data_objects/piv.py` & `fluidimage-0.5.1/src/fluidimage/data_objects/piv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/data_objects/preproc.py` & `fluidimage-0.5.1/src/fluidimage/data_objects/preproc.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/data_objects/tomo.py` & `fluidimage-0.5.1/src/fluidimage/data_objects/tomo.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/executors/__init__.py` & `fluidimage-0.5.1/src/fluidimage/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/executors/base.py` & `fluidimage-0.5.1/src/fluidimage/executors/base.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/executors/exec_async.py` & `fluidimage-0.5.1/src/fluidimage/executors/exec_async.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/executors/exec_async_multiproc.py` & `fluidimage-0.5.1/src/fluidimage/executors/exec_async_multiproc.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/executors/exec_async_seq_for_multi.py` & `fluidimage-0.5.1/src/fluidimage/executors/exec_async_seq_for_multi.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/executors/exec_async_sequential.py` & `fluidimage-0.5.1/src/fluidimage/executors/exec_async_sequential.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/executors/exec_async_servers.py` & `fluidimage-0.5.1/src/fluidimage/executors/exec_async_servers.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/executors/exec_sequential.py` & `fluidimage-0.5.1/src/fluidimage/executors/exec_sequential.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/executors/multi_exec_async.py` & `fluidimage-0.5.1/src/fluidimage/executors/multi_exec_async.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/executors/multi_exec_subproc.py` & `fluidimage-0.5.1/src/fluidimage/executors/multi_exec_subproc.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/executors/servers.py` & `fluidimage-0.5.1/src/fluidimage/executors/servers.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/gui/base_matplotlib.py` & `fluidimage-0.5.1/src/fluidimage/gui/base_matplotlib.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/gui/imviewer.py` & `fluidimage-0.5.1/src/fluidimage/gui/imviewer.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/gui/launcher/main.py` & `fluidimage-0.5.1/src/fluidimage/gui/launcher/main.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/gui/launcher/mainwindow.py` & `fluidimage-0.5.1/src/fluidimage/gui/launcher/mainwindow.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/gui/launcher/mainwindow.ui` & `fluidimage-0.5.1/src/fluidimage/gui/launcher/mainwindow.ui`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/gui/launcher/test_launcher.py` & `fluidimage-0.5.1/src/fluidimage/gui/launcher/test_launcher.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/gui/monitor.py` & `fluidimage-0.5.1/src/fluidimage/gui/monitor.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/gui/pg_main.py` & `fluidimage-0.5.1/src/fluidimage/gui/pg_main.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/gui/pg_wrapper.py` & `fluidimage-0.5.1/src/fluidimage/gui/pg_wrapper.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/gui/piv_viewer.py` & `fluidimage-0.5.1/src/fluidimage/gui/piv_viewer.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/gui/test_imviewer.py` & `fluidimage-0.5.1/src/fluidimage/gui/test_imviewer.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/gui/test_imviewer_pg.py` & `fluidimage-0.5.1/src/fluidimage/gui/test_imviewer_pg.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/gui/test_monitor.py` & `fluidimage-0.5.1/src/fluidimage/gui/test_monitor.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/gui/test_piv_viewer.py` & `fluidimage-0.5.1/src/fluidimage/gui/test_piv_viewer.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/image2image.py` & `fluidimage-0.5.1/src/fluidimage/image2image.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/meson.build` & `fluidimage-0.5.1/src/fluidimage/meson.build`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/postproc/piv.py` & `fluidimage-0.5.1/src/fluidimage/postproc/piv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/postproc/postproc.py` & `fluidimage-0.5.1/src/fluidimage/postproc/postproc.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/postproc/test_piv.py` & `fluidimage-0.5.1/src/fluidimage/postproc/test_piv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/postproc/test_util.py` & `fluidimage-0.5.1/src/fluidimage/postproc/test_util.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/postproc/util.py` & `fluidimage-0.5.1/src/fluidimage/postproc/util.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/postproc/vector_field.py` & `fluidimage-0.5.1/src/fluidimage/postproc/vector_field.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/preproc.py` & `fluidimage-0.5.1/src/fluidimage/preproc.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/reconstruct/tomo/mlos.py` & `fluidimage-0.5.1/src/fluidimage/reconstruct/tomo/mlos.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/reconstruct/tomo/test_mlos.py` & `fluidimage-0.5.1/src/fluidimage/reconstruct/tomo/test_mlos.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/run_from_xml.py` & `fluidimage-0.5.1/src/fluidimage/run_from_xml.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/synthetic.py` & `fluidimage-0.5.1/src/fluidimage/synthetic.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/test_image2image.py` & `fluidimage-0.5.1/src/fluidimage/test_image2image.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/test_run_from_xml.py` & `fluidimage-0.5.1/src/fluidimage/test_run_from_xml.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/topologies/__init__.py` & `fluidimage-0.5.1/src/fluidimage/topologies/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/topologies/base.py` & `fluidimage-0.5.1/src/fluidimage/topologies/base.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/topologies/bos.py` & `fluidimage-0.5.1/src/fluidimage/topologies/bos.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/topologies/example.py` & `fluidimage-0.5.1/src/fluidimage/topologies/example.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/topologies/image2image.py` & `fluidimage-0.5.1/src/fluidimage/topologies/image2image.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/topologies/launcher.py` & `fluidimage-0.5.1/src/fluidimage/topologies/launcher.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/topologies/log.py` & `fluidimage-0.5.1/src/fluidimage/topologies/log.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/topologies/meson.build` & `fluidimage-0.5.1/src/fluidimage/topologies/meson.build`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/topologies/nb_cpu_cores.py` & `fluidimage-0.5.1/src/fluidimage/topologies/nb_cpu_cores.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/topologies/optical_flow.py` & `fluidimage-0.5.1/src/fluidimage/topologies/optical_flow.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/topologies/piv.py` & `fluidimage-0.5.1/src/fluidimage/topologies/piv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/topologies/preproc.py` & `fluidimage-0.5.1/src/fluidimage/topologies/preproc.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/topologies/splitters.py` & `fluidimage-0.5.1/src/fluidimage/topologies/splitters.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/topologies/surface_tracking.py` & `fluidimage-0.5.1/src/fluidimage/topologies/surface_tracking.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/topologies/test_bos.py` & `fluidimage-0.5.1/src/fluidimage/topologies/test_bos.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/topologies/test_example.py` & `fluidimage-0.5.1/src/fluidimage/topologies/test_example.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/topologies/test_image2image.py` & `fluidimage-0.5.1/src/fluidimage/topologies/test_image2image.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/topologies/test_optical_flow.py` & `fluidimage-0.5.1/src/fluidimage/topologies/test_optical_flow.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/topologies/test_piv.py` & `fluidimage-0.5.1/src/fluidimage/topologies/test_piv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/topologies/test_preproc.py` & `fluidimage-0.5.1/src/fluidimage/topologies/test_preproc.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/topologies/test_splitters.py` & `fluidimage-0.5.1/src/fluidimage/topologies/test_splitters.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/topologies/test_surftracking.py` & `fluidimage-0.5.1/src/fluidimage/topologies/test_surftracking.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/util/__init__.py` & `fluidimage-0.5.1/src/fluidimage/util/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/util/log.py` & `fluidimage-0.5.1/src/fluidimage/util/log.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/util/util.py` & `fluidimage-0.5.1/src/fluidimage/util/util.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/uvmat.py` & `fluidimage-0.5.1/src/fluidimage/uvmat.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/works/__init__.py` & `fluidimage-0.5.1/src/fluidimage/works/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/works/bos.py` & `fluidimage-0.5.1/src/fluidimage/works/bos.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/works/image2image.py` & `fluidimage-0.5.1/src/fluidimage/works/image2image.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/works/optical_flow.py` & `fluidimage-0.5.1/src/fluidimage/works/optical_flow.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/works/piv/fix.py` & `fluidimage-0.5.1/src/fluidimage/works/piv/fix.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/works/piv/multipass.py` & `fluidimage-0.5.1/src/fluidimage/works/piv/multipass.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         params._set_child(
             "multipass",
             attribs={
                 "number": 1,
                 "coeff_zoom": 2,
                 "use_tps": "last",
                 "subdom_size": 200,
-                "smoothing_coef": 2.0,
+                "smoothing_coef": 5.0,
                 "threshold_tps": 1.5,
             },
         )
 
         params.multipass._set_doc(
             """Multipass PIV parameters:
 
@@ -89,15 +89,15 @@
 - subdom_size : int
 
   Number of vectors in the subdomains used for the TPS method.
 
 - smoothing_coef : float
 
   Coefficient used for the TPS method. The result is smoother for larger
-  smoothing_coef. 2 is often reasonable. Can typically be between 0 to 40.
+  smoothing_coef. 5 is often reasonable. Can typically be between 0 to 40.
 
 - threshold_tps :  float
 
   Allowed difference of displacement (in pixels) between smoothed and input
   field for TPS filter used in an iterative filtering method. Vectors too far
   from the corresponding interpolated vector are removed.
```

### Comparing `fluidimage-0.5.0/src/fluidimage/works/piv/singlepass.py` & `fluidimage-0.5.1/src/fluidimage/works/piv/singlepass.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/works/piv/test_piv.py` & `fluidimage-0.5.1/src/fluidimage/works/piv/test_piv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/works/preproc/__init__.py` & `fluidimage-0.5.1/src/fluidimage/works/preproc/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/works/preproc/_toolbox_cv.py` & `fluidimage-0.5.1/src/fluidimage/works/preproc/_toolbox_cv.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/works/preproc/_toolbox_py.py` & `fluidimage-0.5.1/src/fluidimage/works/preproc/_toolbox_py.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/works/preproc/io.py` & `fluidimage-0.5.1/src/fluidimage/works/preproc/io.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/works/preproc/toolbox.py` & `fluidimage-0.5.1/src/fluidimage/works/preproc/toolbox.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/works/surface_tracking.py` & `fluidimage-0.5.1/src/fluidimage/works/surface_tracking.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/works/test_bos.py` & `fluidimage-0.5.1/src/fluidimage/works/test_bos.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/works/test_image2image.py` & `fluidimage-0.5.1/src/fluidimage/works/test_image2image.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/works/test_preproc.py` & `fluidimage-0.5.1/src/fluidimage/works/test_preproc.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/src/fluidimage/works/with_mask.py` & `fluidimage-0.5.1/src/fluidimage/works/with_mask.py`

 * *Files identical despite different names*

### Comparing `fluidimage-0.5.0/PKG-INFO` & `fluidimage-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluidimage
-Version: 0.5.0
+Version: 0.5.1
 Summary: Fluid image processing with Python.
 Keywords: PIV
 Author-Email: Pierre Augier <pierre.augier@legi.cnrs.fr>
 License: CeCILL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

