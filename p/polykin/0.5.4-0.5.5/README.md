# Comparing `tmp/polykin-0.5.4.tar.gz` & `tmp/polykin-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polykin-0.5.4.tar", max compression
+gzip compressed data, was "polykin-0.5.5.tar", max compression
```

## Comparing `polykin-0.5.4.tar` & `polykin-0.5.5.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0     1066 2024-04-22 20:38:40.869225 polykin-0.5.4/LICENSE
--rw-r--r--   0        0        0     3034 2024-04-22 20:38:40.869225 polykin-0.5.4/README.md
--rw-r--r--   0        0        0     1801 2024-04-22 20:38:40.885225 polykin-0.5.4/pyproject.toml
--rw-r--r--   0        0        0      701 2024-04-22 20:38:40.885225 polykin-0.5.4/src/polykin/__init__.py
--rw-r--r--   0        0        0      366 2024-04-22 20:38:40.885225 polykin-0.5.4/src/polykin/copolymerization/__init__.py
--rw-r--r--   0        0        0     7689 2024-04-22 20:38:40.885225 polykin-0.5.4/src/polykin/copolymerization/binary.py
--rw-r--r--   0        0        0     6932 2024-04-22 20:38:40.885225 polykin-0.5.4/src/polykin/copolymerization/copodataset.py
--rw-r--r--   0        0        0    13055 2024-04-22 20:38:40.885225 polykin-0.5.4/src/polykin/copolymerization/fitting.py
--rw-r--r--   0        0        0     4236 2024-04-22 20:38:40.885225 polykin-0.5.4/src/polykin/copolymerization/fitting_experimental.py
--rw-r--r--   0        0        0    19770 2024-04-22 20:38:40.885225 polykin-0.5.4/src/polykin/copolymerization/multicomponent.py
--rw-r--r--   0        0        0    17038 2024-04-22 20:38:40.885225 polykin-0.5.4/src/polykin/copolymerization/penultimate.py
--rw-r--r--   0        0        0    24342 2024-04-22 20:38:40.885225 polykin-0.5.4/src/polykin/copolymerization/terminal.py
--rw-r--r--   0        0        0      362 2024-04-22 20:38:40.885225 polykin-0.5.4/src/polykin/distributions/__init__.py
--rw-r--r--   0        0        0    11409 2024-04-22 20:38:40.885225 polykin-0.5.4/src/polykin/distributions/analyticaldistributions.py
--rw-r--r--   0        0        0    27758 2024-04-22 20:38:40.885225 polykin-0.5.4/src/polykin/distributions/base.py
--rw-r--r--   0        0        0     7334 2024-04-22 20:38:40.885225 polykin-0.5.4/src/polykin/distributions/datadistribution.py
--rw-r--r--   0        0        0    30255 2024-04-22 20:38:40.885225 polykin-0.5.4/src/polykin/distributions/sampledata.py
--rw-r--r--   0        0        0      335 2024-04-22 20:38:40.885225 polykin-0.5.4/src/polykin/kinetics/__init__.py
--rw-r--r--   0        0        0     9448 2024-04-22 20:38:40.885225 polykin-0.5.4/src/polykin/kinetics/arrhenius.py
--rw-r--r--   0        0        0      846 2024-04-22 20:38:40.885225 polykin-0.5.4/src/polykin/kinetics/base.py
--rw-r--r--   0        0        0     4078 2024-04-22 20:38:40.885225 polykin-0.5.4/src/polykin/kinetics/cldpropagation.py
--rw-r--r--   0        0        0     4936 2024-04-22 20:38:40.885225 polykin-0.5.4/src/polykin/kinetics/cldtermination.py
--rw-r--r--   0        0        0     3692 2024-04-22 20:38:40.885225 polykin-0.5.4/src/polykin/kinetics/eyring.py
--rw-r--r--   0        0        0      198 2024-04-22 20:38:40.885225 polykin-0.5.4/src/polykin/math/__init__.py
--rw-r--r--   0        0        0     2885 2024-04-22 20:38:40.885225 polykin-0.5.4/src/polykin/math/derivatives.py
--rw-r--r--   0        0        0    11145 2024-04-22 20:38:40.885225 polykin-0.5.4/src/polykin/math/jcr.py
--rw-r--r--   0        0        0      281 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/properties/__init__.py
--rw-r--r--   0        0        0      284 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/properties/diffusion/__init__.py
--rw-r--r--   0        0        0     4645 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/properties/diffusion/liquid.py
--rw-r--r--   0        0        0     3759 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/properties/diffusion/vapor.py
--rw-r--r--   0        0        0    11866 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/properties/diffusion/vrentasduda.py
--rw-r--r--   0        0        0      323 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/properties/equations/__init__.py
--rw-r--r--   0        0        0    10887 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/properties/equations/base.py
--rw-r--r--   0        0        0    14174 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/properties/equations/dippr.py
--rw-r--r--   0        0        0     6410 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/properties/equations/vapor_pressure.py
--rw-r--r--   0        0        0     3070 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/properties/equations/viscosity.py
--rw-r--r--   0        0        0     4274 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/properties/mixing_rules.py
--rw-r--r--   0        0        0     3348 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/properties/pvt_polymer/Flory_parameters.tsv
--rw-r--r--   0        0        0     3722 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/properties/pvt_polymer/HartmannHaque_parameters.tsv
--rw-r--r--   0        0        0     3298 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/properties/pvt_polymer/SanchezLacombe_parameters.tsv
--rw-r--r--   0        0        0     2954 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/properties/pvt_polymer/Tait_parameters.tsv
--rw-r--r--   0        0        0      213 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/properties/pvt_polymer/__init__.py
--rw-r--r--   0        0        0     6555 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/properties/pvt_polymer/base.py
--rw-r--r--   0        0        0    10277 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/properties/pvt_polymer/eos.py
--rw-r--r--   0        0        0     5566 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/properties/pvt_polymer/tait.py
--rw-r--r--   0        0        0      272 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/properties/thermal_conductivity/__init__.py
--rw-r--r--   0        0        0     2159 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/properties/thermal_conductivity/liquid.py
--rw-r--r--   0        0        0     7252 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/properties/thermal_conductivity/vapor.py
--rw-r--r--   0        0        0     7619 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/properties/vaporization_enthalpy.py
--rw-r--r--   0        0        0      247 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/properties/viscosity/__init__.py
--rw-r--r--   0        0        0     1802 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/properties/viscosity/liquid.py
--rw-r--r--   0        0        0    12768 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/properties/viscosity/vapor.py
--rw-r--r--   0        0        0      215 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/stepgrowth/__init__.py
--rw-r--r--   0        0        0    34496 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/stepgrowth/solutions.py
--rw-r--r--   0        0        0      195 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/thermo/__init__.py
--rw-r--r--   0        0        0      287 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/thermo/acm/__init__.py
--rw-r--r--   0        0        0    12659 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/thermo/acm/base.py
--rw-r--r--   0        0        0    12628 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/thermo/acm/floryhuggins.py
--rw-r--r--   0        0        0      886 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/thermo/acm/ideal.py
--rw-r--r--   0        0        0     7598 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/thermo/acm/nrtl.py
--rw-r--r--   0        0        0     9363 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/thermo/acm/polynrtl.py
--rw-r--r--   0        0        0     7479 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/thermo/acm/uniquac.py
--rw-r--r--   0        0        0     4926 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/thermo/acm/wilson.py
--rw-r--r--   0        0        0      260 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/thermo/eos/__init__.py
--rw-r--r--   0        0        0     6544 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/thermo/eos/base.py
--rw-r--r--   0        0        0    15285 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/thermo/eos/cubic.py
--rw-r--r--   0        0        0     1976 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/thermo/eos/idealgas.py
--rw-r--r--   0        0        0     9579 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/thermo/eos/virial.py
--rw-r--r--   0        0        0       86 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/utils/__init__.py
--rw-r--r--   0        0        0      356 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/utils/exceptions.py
--rw-r--r--   0        0        0     3082 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/utils/math.py
--rw-r--r--   0        0        0     9976 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/utils/tools.py
--rw-r--r--   0        0        0     1088 2024-04-22 20:38:40.889225 polykin-0.5.4/src/polykin/utils/types.py
--rw-r--r--   0        0        0     4143 1970-01-01 00:00:00.000000 polykin-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-06 18:45:33.396371 polykin-0.5.5/LICENSE
+-rw-r--r--   0        0        0     3034 2024-05-06 18:45:33.396371 polykin-0.5.5/README.md
+-rw-r--r--   0        0        0     1799 2024-05-06 18:45:33.416370 polykin-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0      701 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/__init__.py
+-rw-r--r--   0        0        0      366 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/copolymerization/__init__.py
+-rw-r--r--   0        0        0     8303 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/copolymerization/binary.py
+-rw-r--r--   0        0        0     7976 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/copolymerization/copodataset.py
+-rw-r--r--   0        0        0    17469 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/copolymerization/fitting.py
+-rw-r--r--   0        0        0    19890 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/copolymerization/multicomponent.py
+-rw-r--r--   0        0        0    17038 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/copolymerization/penultimate.py
+-rw-r--r--   0        0        0    24342 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/copolymerization/terminal.py
+-rw-r--r--   0        0        0      362 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/distributions/__init__.py
+-rw-r--r--   0        0        0    11409 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/distributions/analyticaldistributions.py
+-rw-r--r--   0        0        0    27758 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/distributions/base.py
+-rw-r--r--   0        0        0     7334 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/distributions/datadistribution.py
+-rw-r--r--   0        0        0    30255 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/distributions/sampledata.py
+-rw-r--r--   0        0        0      335 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/kinetics/__init__.py
+-rw-r--r--   0        0        0     9886 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/kinetics/arrhenius.py
+-rw-r--r--   0        0        0      846 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/kinetics/base.py
+-rw-r--r--   0        0        0     4850 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/kinetics/cldpropagation.py
+-rw-r--r--   0        0        0     5666 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/kinetics/cldtermination.py
+-rw-r--r--   0        0        0     4064 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/kinetics/eyring.py
+-rw-r--r--   0        0        0      221 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/math/__init__.py
+-rw-r--r--   0        0        0     5564 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/math/derivatives.py
+-rw-r--r--   0        0        0    10372 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/math/jcr.py
+-rw-r--r--   0        0        0     4722 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/math/solvers.py
+-rw-r--r--   0        0        0      281 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/properties/__init__.py
+-rw-r--r--   0        0        0      284 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/properties/diffusion/__init__.py
+-rw-r--r--   0        0        0     4645 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/properties/diffusion/liquid.py
+-rw-r--r--   0        0        0     3759 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/properties/diffusion/vapor.py
+-rw-r--r--   0        0        0    11866 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/properties/diffusion/vrentasduda.py
+-rw-r--r--   0        0        0      323 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/properties/equations/__init__.py
+-rw-r--r--   0        0        0    10887 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/properties/equations/base.py
+-rw-r--r--   0        0        0    14174 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/properties/equations/dippr.py
+-rw-r--r--   0        0        0     6410 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/properties/equations/vapor_pressure.py
+-rw-r--r--   0        0        0     3070 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/properties/equations/viscosity.py
+-rw-r--r--   0        0        0     4274 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/properties/mixing_rules.py
+-rw-r--r--   0        0        0     3348 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/properties/pvt_polymer/Flory_parameters.tsv
+-rw-r--r--   0        0        0     3722 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/properties/pvt_polymer/HartmannHaque_parameters.tsv
+-rw-r--r--   0        0        0     3298 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/properties/pvt_polymer/SanchezLacombe_parameters.tsv
+-rw-r--r--   0        0        0     2954 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/properties/pvt_polymer/Tait_parameters.tsv
+-rw-r--r--   0        0        0      213 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/properties/pvt_polymer/__init__.py
+-rw-r--r--   0        0        0     6555 2024-05-06 18:45:33.416370 polykin-0.5.5/src/polykin/properties/pvt_polymer/base.py
+-rw-r--r--   0        0        0    10277 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/properties/pvt_polymer/eos.py
+-rw-r--r--   0        0        0     5788 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/properties/pvt_polymer/tait.py
+-rw-r--r--   0        0        0      272 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/properties/thermal_conductivity/__init__.py
+-rw-r--r--   0        0        0     2159 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/properties/thermal_conductivity/liquid.py
+-rw-r--r--   0        0        0     7252 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/properties/thermal_conductivity/vapor.py
+-rw-r--r--   0        0        0     7619 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/properties/vaporization_enthalpy.py
+-rw-r--r--   0        0        0      247 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/properties/viscosity/__init__.py
+-rw-r--r--   0        0        0     1802 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/properties/viscosity/liquid.py
+-rw-r--r--   0        0        0    12768 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/properties/viscosity/vapor.py
+-rw-r--r--   0        0        0      215 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/stepgrowth/__init__.py
+-rw-r--r--   0        0        0    34496 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/stepgrowth/solutions.py
+-rw-r--r--   0        0        0      195 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/thermo/__init__.py
+-rw-r--r--   0        0        0      287 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/thermo/acm/__init__.py
+-rw-r--r--   0        0        0    12659 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/thermo/acm/base.py
+-rw-r--r--   0        0        0    12628 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/thermo/acm/floryhuggins.py
+-rw-r--r--   0        0        0      886 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/thermo/acm/ideal.py
+-rw-r--r--   0        0        0     7598 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/thermo/acm/nrtl.py
+-rw-r--r--   0        0        0     9363 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/thermo/acm/polynrtl.py
+-rw-r--r--   0        0        0     7479 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/thermo/acm/uniquac.py
+-rw-r--r--   0        0        0     4926 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/thermo/acm/wilson.py
+-rw-r--r--   0        0        0      260 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/thermo/eos/__init__.py
+-rw-r--r--   0        0        0     6544 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/thermo/eos/base.py
+-rw-r--r--   0        0        0    15285 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/thermo/eos/cubic.py
+-rw-r--r--   0        0        0     1976 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/thermo/eos/idealgas.py
+-rw-r--r--   0        0        0     9579 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/thermo/eos/virial.py
+-rw-r--r--   0        0        0       86 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/utils/__init__.py
+-rw-r--r--   0        0        0      356 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/utils/exceptions.py
+-rw-r--r--   0        0        0     3082 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/utils/math.py
+-rw-r--r--   0        0        0    10697 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/utils/tools.py
+-rw-r--r--   0        0        0     1012 2024-05-06 18:45:33.420370 polykin-0.5.5/src/polykin/utils/types.py
+-rw-r--r--   0        0        0     4183 1970-01-01 00:00:00.000000 polykin-0.5.5/PKG-INFO
```

### Comparing `polykin-0.5.4/LICENSE` & `polykin-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/README.md` & `polykin-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/pyproject.toml` & `polykin-0.5.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polykin"
-version = "0.5.4"
+version = "0.5.5"
 description = "A polymerization kinetics library."
 authors = ["HugoMVale <57530119+HugoMVale@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://hugomvale.github.io/polykin/"
 repository = "https://github.com/HugoMVale/polykin"
 documentation = "https://hugomvale.github.io/polykin/"
@@ -25,15 +25,15 @@
 pydantic = "^1.10.13"
 numpy = "^1.23.5"
 scipy = "^1.11.4"
 matplotlib = "^3.7.1"
 nptyping = "^2.5.0"
 pandas = ">=1.5.3"
 # sqlalchemy = "^2.0.22"
-# numba = "^0.58.1"
+numba = "^0.59.1"
 
 [tool.poetry.group.docs]
 optional = true
 [tool.poetry.group.docs.dependencies]
 ipykernel = "^6.20.0"
 mkdocs = "^1.4.2"
 mkdocs-material = "^9.5.3"
```

### Comparing `polykin-0.5.4/src/polykin/__init__.py` & `polykin-0.5.5/src/polykin/__init__.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/copolymerization/binary.py` & `polykin-0.5.5/src/polykin/copolymerization/binary.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # PolyKin: A polymerization kinetics library for Python.
 #
 # Copyright Hugo Vale 2023
 
-from typing import Union
+from typing import Literal, Union
 
 import numpy as np
+from numba import jit
 from scipy.integrate import solve_ivp
 
 from polykin.utils.exceptions import ODESolverError
 from polykin.utils.math import eps
 from polykin.utils.types import (FloatArray, FloatArrayLike, FloatMatrix,
-                                 FloatVector, FloatVectorLike)
+                                 FloatVectorLike)
 
 __all__ = ['inst_copolymer_binary',
            'kp_average_binary',
            'monomer_drift_binary']
 
 
+@jit
 def inst_copolymer_binary(f1: Union[float, FloatArrayLike],
                           r1: Union[float, FloatArray],
                           r2: Union[float, FloatArray]
                           ) -> Union[float, FloatArray]:
     r"""Calculate the instantaneous copolymer composition using the
     [Mayo-Lewis](https://en.wikipedia.org/wiki/Mayo%E2%80%93Lewis_equation)
      equation.
@@ -141,15 +143,17 @@
     return (r1*f1**2 + r2*f2**2 + 2*f1*f2)/((r1*f1/k11) + (r2*f2/k22))
 
 
 def monomer_drift_binary(f10: Union[float, FloatVectorLike],
                          x: FloatVectorLike,
                          r1: float,
                          r2: float,
-                         atol: float = 1e-4
+                         atol: float = 1e-4,
+                         rtol: float = 1e-4,
+                         method: Literal['LSODA', 'RK45'] = 'LSODA'
                          ) -> FloatMatrix:
     r"""Compute the monomer composition drift for a binary system.
 
     In a closed binary system, the drift in monomer composition is given by
     the solution of the following differential equation:
 
     $$ \frac{\textup{d} f_1}{\textup{d}x} = \frac{f_1 - F_1}{1 - x} $$
@@ -166,14 +170,18 @@
         Total monomer conversion values where the drift is to be evaluated.
     r1 : float | FloatArray
         Reactivity ratio of M1.
     r2 : float | FloatArray
         Reactivity ratio of M2.
     atol : float
         Absolute tolerance of ODE solver.
+    rtol : float
+        Relative tolerance of ODE solver.
+    method : Literal['LSODA', 'RK45']
+        ODE solver.
 
     Returns
     -------
     FloatMatrix (M, N)
         Monomer fraction of M1 at a given conversion, $f_1(x)$.
 
     See also
@@ -194,40 +202,61 @@
     >>> f1 = monomer_drift_binary(f10=[0.2, 0.8], x=[0.1, 0.5, 0.9],
     ...                           r1=0.16, r2=0.70)
     >>> f1
     array([[0.19841009, 0.18898084, 0.15854395],
            [0.82315475, 0.94379024, 0.99996457]])
     """
 
-    def df1dx(x: float, f1: FloatVector) -> FloatVector:
-        return (f1 - inst_copolymer_binary(f1, r1, r2))/(1 - x + eps)
-
     if isinstance(f10, (int, float)):
         f10 = [f10]
 
     sol = solve_ivp(df1dx,
                     (0., max(x)),
                     f10,
+                    args=(r1, r2),
                     t_eval=x,
-                    method='LSODA',  # LSODA is by far the fastest solver
+                    method=method,
                     vectorized=True,
                     atol=atol,
-                    rtol=1e-4)
+                    rtol=rtol)
 
     if sol.success:
         result = sol.y
         result = np.maximum(0., result)
         if result.shape[0] == 1:
             result = result[0]
     else:
         raise ODESolverError(sol.message)
 
     return result
 
+
+@jit
+def df1dx(x: float, f1: FloatArray, r1: float, r2: float) -> FloatArray:
+    """Skeist equation for a binary system.
+
+    Parameters
+    ----------
+    x : float
+        Total monomer conversion.
+    f1 : FloatArray
+        Molar fraction of M1.
+    r1 : float
+        Reactivity ratio of M1.
+    r2 : float
+        Reactivity ratio of M2.
+
+    Returns
+    -------
+    FloatVector
+        df1/dx.
+    """
+    return (f1 - inst_copolymer_binary(f1, r1, r2))/(1 - x + eps)
+
 # %% Jacobian for monomer_drift_binary
 # Tried, but does not really accelerate computation
-
-# def jac(x: float, f1: FloatVector) -> FloatVector:
+# @jit
+# def jac(x: float, f1: FloatVector, r1, r2) -> FloatVector:
 #     f2 = 1 - f1
 #     dF1df1 = (r1*f1**2 + r2*f2*(1 + (-1 + 2*r1)*f1)) / \
 #         (r2*f2**2 + f1*(2 + (-2 + r1)*f1))**2
 #     return (1 - dF1df1)/(1 - x + eps)
```

### Comparing `polykin-0.5.4/src/polykin/copolymerization/copodataset.py` & `polykin-0.5.5/src/polykin/copolymerization/copodataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 # PolyKin: A polymerization kinetics library for Python.
 #
 # Copyright Hugo Vale 2023
 
 from abc import ABC
+from dataclasses import dataclass
 from typing import Any, Literal, Union
 
 from polykin.utils.math import convert_FloatOrVectorLike_to_FloatOrVector
 from polykin.utils.tools import check_shapes
-from polykin.utils.types import FloatVectorLike
+from polykin.utils.types import FloatVector, FloatVectorLike
 
 # from dataclasses import dataclass
 
 
 __all__ = ['MayoDataset',
            'DriftDataset',
-           'kpDataset']
+           'kpDataset',
+           'CopoDataset_Ff',
+           'CopoDataset_fx',
+           'CopoDataset_Fx']
 
 
 class CopoDataset(ABC):
 
     varmap: dict[str, str]
 
     def __init__(self,
@@ -226,7 +230,42 @@
                  Tunit: Literal['C', 'K'] = 'K',
                  name: str = '',
                  source: str = '',
                  ) -> None:
         """Construct `DriftDataset` with the given parameters."""
         super().__init__(M1, M2, f1, kp, sigma_f1, sigma_kp, weight, T, Tunit,
                          name, source)
+
+
+@dataclass(frozen=True)
+class CopoDataset_Ff():
+    """Dataclass for instantaneous copolymerization data of the form F(f)."""
+    name: str
+    f1: FloatVector
+    F1: FloatVector
+    scale_f1: Union[FloatVector, float] = 1.0
+    scale_F1: Union[FloatVector, float] = 1.0
+    weight: float = 1.0
+
+
+@dataclass(frozen=True)
+class CopoDataset_fx():
+    """Dataclass for drift copolymerization data of the form f1(x)."""
+    name: str
+    f10: float
+    x: FloatVector
+    f1: FloatVector
+    # scale_x: Union[FloatVector, float] = 1.0
+    scale_f1: Union[FloatVector, float] = 1.0
+    weight: float = 1.0
+
+
+@dataclass(frozen=True)
+class CopoDataset_Fx():
+    """Dataclass for drift copolymerization data of the form F1(x)."""
+    name: str
+    f10: float
+    x: FloatVector
+    F1: FloatVector
+    # scale_x: Union[FloatVector, float] = 1.0
+    scale_F1: Union[FloatVector, float] = 1.0
+    weight: float = 1.0
```

### Comparing `polykin-0.5.4/src/polykin/copolymerization/multicomponent.py` & `polykin-0.5.5/src/polykin/copolymerization/multicomponent.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,15 +231,16 @@
 
     return F
 
 
 def monomer_drift_multi(f0: FloatVectorLike,
                         x: FloatVectorLike,
                         r: FloatSquareMatrix,
-                        atol: float = 1e-4
+                        atol: float = 1e-4,
+                        rtol: float = 1e-4
                         ) -> FloatMatrix:
     r"""Compute the monomer composition drift for a multicomponent system.
 
     In a closed system, the drift in monomer composition is given by
     the solution of the following system of differential equations:
 
     $$ \frac{\textup{d} f_i}{\textup{d}x} = \frac{f_i - F_i}{1 - x} $$
@@ -255,14 +256,16 @@
     x : FloatVectorLike (M)
         Vector of total monomer conversion values where the drift is to be
         evaluated.
     r : FloatSquareMatrix (N, N)
         Matrix of reactivity ratios, $r_{ij}=k_{ii}/k_{ij}$.
     atol : float
         Absolute tolerance of the ODE solver.
+    rtol : float
+        Relative tolerance of the ODE solver.
 
     Returns
     -------
     FloatMatrix (M, N)
         Matrix of monomer fraction of monomer $i$ at the specified total
         monomer conversions, $f_i(x_j)$.
 
@@ -308,15 +311,15 @@
         return (f - F[:-1]) / (1. - x + eps)
 
     sol = solve_ivp(dfdx,
                     t_span=(0., max(x)),
                     y0=f0[:-1],
                     t_eval=x,
                     atol=atol,
-                    rtol=1e-4,
+                    rtol=rtol,
                     method='LSODA')
 
     if sol.success:
         f = np.empty((len(x), N))
         f[:, :-1] = np.transpose(sol.y)
         f[:, -1] = 1. - np.sum(f[:, :-1], axis=1)
     else:
@@ -517,15 +520,15 @@
         process modeling, Wiley, 1996, p. 179.
 
     Parameters
     ----------
     P : FloatSquareMatrix (N, N)
         Matrix of transition probabilities, $P_{ij}$.
     n : int
-        Tuple length,.e.g monads (1), diads (2), triads (3), etc.
+        Tuple length, e.g. monads (1), diads (2), triads (3), etc.
     F : FloatVectorLike (N) | None
         Vector of instantaneous copolymer composition, $F_i$. If `None`,
         the value will be computed internally. When calculating tuples of
         various lengths, it is more efficient to precompute $F$ and use it in
         all tuple cases.
 
     Returns
@@ -575,18 +578,18 @@
     # Generate all tuple combinations
     N = P.shape[0]
     indexes = list(itertools.product(range(N), repeat=n))
 
     result = {}
     for idx in indexes:
         # Compute tuple probability
-        Pprod = 1.
+        P_product = 1.
         for j in range(n-1):
-            Pprod *= P[idx[j], idx[j+1]]
-        A = F[idx[0]]*Pprod
+            P_product *= P[idx[j], idx[j+1]]
+        A = F[idx[0]]*P_product
         # Add probability to dict, but combine symmetric tuples: 12 <- 12 + 21
         reversed_idx = idx[::-1]
         if reversed_idx in result.keys():
             result[reversed_idx] += A
         else:
             result[idx] = A
```

### Comparing `polykin-0.5.4/src/polykin/copolymerization/penultimate.py` & `polykin-0.5.5/src/polykin/copolymerization/penultimate.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/copolymerization/terminal.py` & `polykin-0.5.5/src/polykin/copolymerization/terminal.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/distributions/analyticaldistributions.py` & `polykin-0.5.5/src/polykin/distributions/analyticaldistributions.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/distributions/base.py` & `polykin-0.5.5/src/polykin/distributions/base.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/distributions/datadistribution.py` & `polykin-0.5.5/src/polykin/distributions/datadistribution.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/distributions/sampledata.py` & `polykin-0.5.5/src/polykin/distributions/sampledata.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/kinetics/arrhenius.py` & `polykin-0.5.5/src/polykin/kinetics/arrhenius.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,21 +5,20 @@
 from __future__ import annotations
 
 from typing import Union
 
 import numpy as np
 from numpy import exp
 
+from polykin.kinetics.base import KineticCoefficientT
 from polykin.utils.exceptions import ShapeError
 from polykin.utils.math import convert_FloatOrArrayLike_to_FloatOrArray
 from polykin.utils.tools import check_bounds, check_shapes
 from polykin.utils.types import FloatArray, FloatArrayLike
 
-from .base import KineticCoefficientT
-
 __all__ = ['Arrhenius']
 
 
 class Arrhenius(KineticCoefficientT):
     r"""[Arrhenius](https://en.wikipedia.org/wiki/Arrhenius_equation) kinetic
     rate coefficient.
 
@@ -58,14 +57,27 @@
     name : str
         Name.
 
     See also
     --------
     * [`Eyring`](Eyring.md): alternative method.
 
+    Examples
+    --------
+    Define and evaluate the propagation rate coefficient of styrene.
+    >>> from polykin.kinetics import Arrhenius 
+    >>> kp = Arrhenius(
+    ...     10**7.63,       # pre-exponential factor
+    ...     32.5e3/8.314,   # Ea/R, K
+    ...     Tmin=261., Tmax=366.,
+    ...     symbol='k_p',
+    ...     unit='L/mol/s',
+    ...     name='kp of styrene')
+    >>> kp(25.,'C') 
+    86.28385101961442
     """
 
     _pinfo = {'k0': ('#', True), 'EaR': ('K', True), 'T0': ('K', False)}
 
     def __init__(self,
                  k0: Union[float, FloatArrayLike],
                  EaR: Union[float, FloatArrayLike],
```

### Comparing `polykin-0.5.4/src/polykin/kinetics/base.py` & `polykin-0.5.5/src/polykin/kinetics/base.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/kinetics/cldpropagation.py` & `polykin-0.5.5/src/polykin/kinetics/cldpropagation.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,23 +3,22 @@
 # Copyright Hugo Vale 2023
 
 from typing import Literal, Union
 
 import numpy as np
 from numpy import exp, log
 
+from polykin.kinetics.arrhenius import Arrhenius
+from polykin.kinetics.base import KineticCoefficientCLD
+from polykin.kinetics.eyring import Eyring
 from polykin.utils.tools import (check_bounds, check_type,
                                  convert_check_temperature, custom_repr)
 from polykin.utils.types import (FloatArray, FloatArrayLike, IntArray,
                                  IntArrayLike)
 
-from .arrhenius import Arrhenius
-from .base import KineticCoefficientCLD
-from .eyring import Eyring
-
 __all__ = ['PropagationHalfLength']
 
 
 class PropagationHalfLength(KineticCoefficientCLD):
     r"""Half-length model for the decay of the propagation rate coefficient
     with chain length.
 
@@ -46,24 +45,49 @@
     C : float
         Ratio of the propagation coefficients of a monomeric radical and a
         long-chain radical, $C$.
     ihalf : float
         Half-length, $i_{1/2}$.
     name : str
         Name.
+
+    Examples
+    --------
+    >>> from polykin.kinetics import PropagationHalfLength, Arrhenius
+    >>> kp = Arrhenius(
+    ...    10**7.63, 32.5e3/8.314, Tmin=261., Tmax=366.,
+    ...    symbol='k_p', unit='L/mol/s', name='kp of styrene')
+
+    >>> kpi = PropagationHalfLength(kp, C=10, ihalf=0.5,
+    ...    name='kp(T,i) of styrene')
+    >>> kpi
+    name:    kp(T,i) of styrene
+    C:       10
+    ihalf:   0.5
+    kp:
+      name:            kp of styrene
+      symbol:          k_p
+      unit:            L/mol/s
+      Trange [K]:      (261.0, 366.0)
+      k0 [L/mol/s]:    42657951.88015926
+      EaR [K]:         3909.0690401732018
+      T0 [K]:          inf
+
+    >>> kpi(T=50., i=3, Tunit='C')
+    371.75986615653215
     """
 
     kp: Union[Arrhenius, Eyring]
     C: float
     ihalf: float
     symbol: str = 'k_p(i)'
 
     def __init__(self,
                  kp: Union[Arrhenius, Eyring],
-                 C: float = 10.,
+                 C: float = 10.0,
                  ihalf: float = 1.0,
                  name: str = ''
                  ) -> None:
 
         check_type(kp, (Arrhenius, Eyring), 'kp')
         check_bounds(C, 1., 100., 'C')
         check_bounds(ihalf, 0.1, 10, 'ihalf')
```

### Comparing `polykin-0.5.4/src/polykin/kinetics/eyring.py` & `polykin-0.5.5/src/polykin/kinetics/eyring.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,20 +7,19 @@
 from typing import Union
 
 import numpy as np
 from numpy import exp
 from scipy.constants import Boltzmann as kB
 from scipy.constants import R, h
 
+from polykin.kinetics.base import KineticCoefficientT
 from polykin.utils.math import convert_FloatOrArrayLike_to_FloatOrArray
 from polykin.utils.tools import check_bounds, check_shapes
 from polykin.utils.types import FloatArray, FloatArrayLike
 
-from .base import KineticCoefficientT
-
 __all__ = ['Eyring']
 
 
 class Eyring(KineticCoefficientT):
     r"""[Eyring](https://en.wikipedia.org/wiki/Eyring_equation) kinetic rate
     coefficient.
 
@@ -57,14 +56,27 @@
     name : str
         Name.
 
     See also
     --------
     * [`Arrhenius`](Arrhenius.md): alternative method.
 
+    Examples
+    --------
+    Define and evaluate a rate coefficient from transition state properties.
+    >>> from polykin.kinetics import Eyring 
+    >>> k = Eyring(
+    ...     DSa=20.,
+    ...     DHa=5e4,
+    ...     kappa=0.8,
+    ...     Tmin=273., Tmax=373.,
+    ...     symbol='k',
+    ...     name='A->B')
+    >>> k(25.,'C')
+    95808.36742009166
     """
 
     _pinfo = {'DSa': ('J/(mol·K)', True),
               'DHa': ('J/mol', True), 'kappa': ('', False)}
 
     def __init__(self,
                  DSa: Union[float, FloatArrayLike],
```

### Comparing `polykin-0.5.4/src/polykin/math/jcr.py` & `polykin-0.5.5/src/polykin/math/jcr.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # PolyKin: A polymerization kinetics library for Python.
 #
 # Copyright Hugo Vale 2024
 
+import functools
 from typing import Callable, Optional
 
 import numpy as np
 from matplotlib.axes._axes import Axes
 from matplotlib.patches import Ellipse
 from numpy import arctan, cos, exp, log, sin, sqrt
-from scipy.integrate import solve_ivp
-from scipy.optimize import root_scalar
 from scipy.stats.distributions import f as Fdist
 from scipy.stats.distributions import t as tdist
 
-from polykin.utils.exceptions import (ODESolverError, RootSolverError,
-                                      ShapeError)
+from polykin.math.solvers import RootResult, root_secant
+from polykin.utils.exceptions import ShapeError
 from polykin.utils.math import eps
 from polykin.utils.tools import check_bounds
 from polykin.utils.types import Float2x2Matrix, FloatVector
 
 __all__ = ['confidence_ellipse',
            'confidence_region']
 
@@ -97,15 +96,15 @@
     Examples
     --------
     >>> from polykin.math.jcr import confidence_ellipse
     >>> import matplotlib.pyplot as plt
     >>> import numpy as np
     >>> fig, ax = plt.subplots()
     >>> confidence_ellipse(ax=ax, center=(0.3,0.8),
-    ...                    cov=np.array([[2e-4, 3e-4], [3e-4, 2e-3]]), ndata=9)
+    ...     cov=np.array([[2e-4, 3e-4], [3e-4, 2e-3]]), ndata=9)
     """
 
     # Method implementation is specific for 2D
     npar = 2
     if len(center) != npar:
         raise ShapeError(f"`center` must be a vector of length {npar}.")
 
@@ -147,19 +146,20 @@
         ci = sqrt(np.diag(cov))*tdist.ppf(1. - alpha/2, ndata - npar)
         ax.errorbar(*center, xerr=ci[0], yerr=ci[1], color=color)
 
     return None
 
 
 def confidence_region(center: tuple[float, float],
-                      sse: Callable[[float, float], float],
+                      sse: Callable[[tuple[float, float]], float],
                       ndata: int,
                       alpha: float = 0.05,
                       width: Optional[float] = None,
-                      rtol: float = 1e-4
+                      npoints: int = 200,
+                      rtol: float = 1e-2
                       ) -> tuple[FloatVector, FloatVector]:
     r"""Generate a confidence region for 2 jointly estimated parameters
     using a rigorous method.
 
     The joint $100(1-\alpha)\%$ confidence region (JCR) for the parameters
     $\beta=(\beta_1, \beta_2)$ is represented by the domain of values that
     satisfy the following condition:
@@ -173,47 +173,47 @@
     $\alpha$ is the significance level, and $F$ is the Fisher-Snedecor
     distribution.
 
     !!! note
 
         This method is suitable for arbitrary models (linear or non-linear in
         the parameters), without making assumptions about the shape of the JCR.
-        The algorithm used to compute the JCR is very efficient in comparison
+        The algorithm used to compute the JCR is efficient in comparison
         to naive 2D mesh screening approaches, but the number of $S(\beta)$
         evaluations remains large (typically several hundreds). Therefore, the
         applicability of this method depends on the cost of evaluating
         $S(\beta)$.
 
     **References**
 
-    * Arutjunjan, R., Schaefer, B. M., Kreutz, C., Constructing Exact
-    Confidence Regions on Parameter Manifolds of Non-Linear Models, 2022.
-
     *   Vugrin, K. W., L. P. Swiler, R. M. Roberts, N. J. Stucky-Mack, and
     S. P. Sullivan (2007), Confidence region estimation techniques for
     nonlinear regression in groundwater flow: Three case studies, Water
     Resour. Res., 43.
 
     Parameters
     ----------
     center : tuple[float, float]
         Point estimate of the model parameters, $\hat{\beta}$.
-    sse : Callable[[float, float], float]
+    sse : Callable[[tuple[float, float]], float]
         Error sum of squares function, $S(\beta_1, \beta_2)$.
     ndata : int
         Number of data points.
     alpha : float
         Significance level, $\alpha$.
     width : float | None
         Initial guess of the width of the joint confidence region at its
         center. If `None`, it is assumed that `width=0.5*center[0]`.
+    npoints : int
+        Number of points where the JCR is evaluated. The computational effort
+        increases linearly with `npoints`.
     rtol : float
-        Relative tolerance of ODE solver. The default value may be decreased
-        by one or more orders of magnitude if the resolution of the JCR appears
-        insufficient.
+        Relative tolerance for the determination of the JCR. The default value
+        (1e-2) should be adequate in most cases, as it implies a 1% accuracy in
+        the JCR coordinates. 
 
     Returns
     -------
     tuple[FloatVector, FloatVector]
         Coordinates (x, y) of the confidence region.
 
     See also
@@ -222,96 +222,75 @@
       on a linear approximation.
 
     Examples
     --------
     Let's generate a confidence region for a non-quadratic sse function.
     >>> from polykin.math import confidence_region
     >>> import matplotlib.pyplot as plt
-    >>> def sse(x, y):
-    ...     return 1. + ((x-10)**2 + (y-20)**2 + (x-10)*np.sin((y-20)**2))
+    >>> def sse(x):
+    ...     return 1. + ((x[0]-10)**2 + (x[1]-20)**2 + (x[0]-10)*np.sin((x[1]-20)**2))
     >>> x, y = confidence_region(center=(10, 20.), sse=sse, ndata=10, alpha=0.10)
     >>> fig, ax = plt.subplots()
     >>> ax.plot(x,y)
     """
 
     # Method implementation is specific for 2D
     npar = 2
     if len(center) != npar:
         raise ShapeError(f"`center` must be a vector of length {npar}.")
 
     # Check inputs
     check_bounds(alpha, 0.001, 0.99, 'alpha')
     check_bounds(ndata, npar + 1, np.inf, 'ndata')
+    if width is not None:
+        check_bounds(width, eps, np.inf, 'width')
+    check_bounds(npoints, 1, 500, 'npoints')
+    check_bounds(rtol, 1e-4, 1e-1, 'rtol')
 
-    # Boundary
-    sse_center = sse(*center)
+    # Get 'sse' at center
+    sse_center = sse(center)
     if abs(sse_center) < eps:
         raise ValueError(
             "`sse(center)` is close to zero. Without residual error, there is no JCR.")
-    Fval = Fdist.ppf(1. - alpha, npar, ndata - npar)
-    sse_boundary = sse_center*(1. + npar/(ndata - npar)*Fval)
 
-    # Find boundary radius at 3 o'clock
-    sol = root_scalar(
-        f=lambda r: sse(center[0] + r, center[1]) - sse_boundary,
-        method='secant',
-        x0=0,
-        x1=width/2 if width is not None else 0.25*center[0])
-    if not sol.converged:
-        raise RootSolverError(sol.flag)
-    else:
-        r0 = sol.root
-
-    # Transform 'sse' to log-radial coordinates
-    def f(s: float, q: float) -> float:
-        r = exp(s)
-        x = center[0] + r*cos(q)
-        y = center[1] + r*sin(q)
-        return sse(x, y)
-
-    # Move along boundary using radial coordinates
-    # Imagine a particle transported by a velocity field orthogonal to 'sse'
-    def dydt(t: float, y: np.ndarray) -> np.ndarray:
-        s = y[0]
-        q = y[1]
-        h = 2*sqrt(eps)
-        f_s = (f(s + h, q) - f(s - h, q))/h
-        f_q = (f(s, q + h) - f(s, q - h))/h
-        ydot = np.empty_like(y)
-        ydot[0] = -f_q
-        ydot[1] = f_s
-        return ydot
-
-    # Stop the trajectory after one revolution
-    def event(t: float, y: np.ndarray) -> float:
-        return y[1] - 2*np.pi
-    event.terminal = True
-
-    sol = solve_ivp(dydt, (0., 1e10), (log(r0), 0.),
-                    method='LSODA',
-                    events=event,
-                    atol=[0, 1*rtol], rtol=rtol)
-    if not sol.success:
-        raise ODESolverError(sol.message)
-    else:
-        r = exp(sol.y[0, :])
-        theta = sol.y[1, :]
-        if not np.isclose(r[0], r[-1], atol=min(*center), rtol=10*rtol):
-            print("Warning: offset between start and end positions of JCR > 10*rtol.")
-
-    # Interpolate in radial coordinates, without loosing the original points
-    dim = theta.shape[0]
-    npoints = 1000
-    if dim < npoints:
-        theta_interp = np.linspace(0, 2*np.pi, npoints)
-        r_interp = np.interp(theta_interp, theta, r)
-        theta = np.concatenate((theta, theta_interp))
-        r = np.concatenate((r, r_interp))
-        idx_sorted = np.argsort(theta)
-        theta[:] = theta[idx_sorted]
-        r[:] = r[idx_sorted]
+    @functools.cache
+    def nsse(lnr: float, θ: float) -> float:
+        "Normalized 'sse' in log-radial coordinates"
+        r = exp(lnr)
+        x = center[0] + r*cos(θ)
+        y = center[1] + r*sin(θ)
+        return sse((x, y))/sse_center
+
+    # Boundary value
+    Fval = float(Fdist.ppf(1. - alpha, npar, ndata - npar))
+    nsse_boundary = (1. + npar/(ndata - npar)*Fval)
+
+    def find_radius(θ: float, r0: float) -> RootResult:
+        "Find boundary ln(radius) at given angle θ."
+        solution = root_secant(
+            f=lambda x: nsse(x, θ)/nsse_boundary - 1.0,
+            x0=log(r0*1.02),
+            x1=log(r0),
+            xtol=abs(log(1 + rtol)),
+            ftol=1e-4,
+            maxiter=100)
+        return solution
+
+    # Find radius at each angle using previous solution as initial guess
+    angles = np.linspace(0., 2*np.pi, npoints)
+    r = np.zeros_like(angles)
+    r_guess_0 = abs(width/2) if width is not None else 0.25*center[0]
+    r_guess = r_guess_0
+    for i, θ in enumerate(angles):
+        sol = find_radius(θ, r_guess)
+        if sol.success:
+            r[i] = exp(sol.x)
+            r_guess = r[i]
+        else:
+            r[i] = np.nan
+            r_guess = r_guess_0
 
     # Convert to cartesian coordinates
-    x = center[0] + r*cos(theta)
-    y = center[1] + r*sin(theta)
+    x = center[0] + r*cos(angles)
+    y = center[1] + r*sin(angles)
 
     return (x, y)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `polykin-0.5.4/src/polykin/properties/diffusion/liquid.py` & `polykin-0.5.5/src/polykin/properties/diffusion/liquid.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/properties/diffusion/vapor.py` & `polykin-0.5.5/src/polykin/properties/diffusion/vapor.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/properties/diffusion/vrentasduda.py` & `polykin-0.5.5/src/polykin/properties/diffusion/vrentasduda.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/properties/equations/base.py` & `polykin-0.5.5/src/polykin/properties/equations/base.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/properties/equations/dippr.py` & `polykin-0.5.5/src/polykin/properties/equations/dippr.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/properties/equations/vapor_pressure.py` & `polykin-0.5.5/src/polykin/properties/equations/vapor_pressure.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/properties/equations/viscosity.py` & `polykin-0.5.5/src/polykin/properties/equations/viscosity.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/properties/mixing_rules.py` & `polykin-0.5.5/src/polykin/properties/mixing_rules.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/properties/pvt_polymer/Flory_parameters.tsv` & `polykin-0.5.5/src/polykin/properties/pvt_polymer/Flory_parameters.tsv`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/properties/pvt_polymer/HartmannHaque_parameters.tsv` & `polykin-0.5.5/src/polykin/properties/pvt_polymer/HartmannHaque_parameters.tsv`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/properties/pvt_polymer/SanchezLacombe_parameters.tsv` & `polykin-0.5.5/src/polykin/properties/pvt_polymer/SanchezLacombe_parameters.tsv`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/properties/pvt_polymer/Tait_parameters.tsv` & `polykin-0.5.5/src/polykin/properties/pvt_polymer/Tait_parameters.tsv`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/properties/pvt_polymer/base.py` & `polykin-0.5.5/src/polykin/properties/pvt_polymer/base.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/properties/pvt_polymer/eos.py` & `polykin-0.5.5/src/polykin/properties/pvt_polymer/eos.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/properties/pvt_polymer/tait.py` & `polykin-0.5.5/src/polykin/properties/pvt_polymer/tait.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # PolyKin: A polymerization kinetics library for Python.
 #
 # Copyright Hugo Vale 2023
 
+from typing import Union
+
 import numpy as np
 from numpy import exp, log
 
-from polykin.utils.types import FloatOrArray
 from polykin.utils.tools import check_bounds
+from polykin.utils.types import FloatArray
 
 from .base import PolymerPVTEquation
 
 __all__ = ['Tait']
 
 
 class Tait(PolymerPVTEquation):
@@ -115,108 +117,108 @@
             f"A1 [m³/kg.K]:  {self.A1}\n"
             f"A2 [m³/kg.K²]: {self.A2}\n"
             f"B0 [Pa]:       {self.B0}\n"
             f"B1 [1/K]:      {self.B1}"
         )
 
     def eval(self,
-             T: FloatOrArray,
-             P: FloatOrArray
-             ) -> FloatOrArray:
+             T: Union[float, FloatArray],
+             P: Union[float, FloatArray]
+             ) -> Union[float, FloatArray]:
         r"""Evaluate specific volume, $\hat{V}$, at given SI conditions without
         unit conversions or checks.
 
         Parameters
         ----------
-        T : FloatOrArray
+        T : float | FloatArray
             Temperature.
             Unit = K.
-        P : FloatOrArray
+        P : float | FloatArray
             Pressure.
             Unit = Pa.
 
         Returns
         -------
-        FloatOrArray
+        float | FloatArray
             Specific volume.
             Unit = m³/kg.
         """
         TC = T - 273.15
         V0 = self.A0 + self.A1*TC + self.A2*TC**2
         B = self._B(T)
         V = V0*(1 - self._C*log(1 + P/B))
         return V
 
     def _B(self,
-           T: FloatOrArray
-           ) -> FloatOrArray:
+           T: Union[float, FloatArray]
+           ) -> Union[float, FloatArray]:
         r"""Parameter B(T).
 
         Parameters
         ----------
-        T : FloatOrArray
+        T : float | FloatArray
             Temperature.
             Unit = K.
 
         Returns
         -------
-        FloatOrArray
+        float | FloatArray
             B(T).
             Unit = Pa.
         """
         return self.B0*exp(-self.B1*(T - 273.15))
 
     def alpha(self,
-              T: FloatOrArray,
-              P: FloatOrArray
-              ) -> FloatOrArray:
+              T: Union[float, FloatArray],
+              P: Union[float, FloatArray]
+              ) -> Union[float, FloatArray]:
         r"""Calculate thermal expansion coefficient, $\alpha$.
 
         $$\alpha=\frac{1}{V}\left(\frac{\partial V}{\partial T}\right)_{P}$$
 
         Parameters
         ----------
-        T : FloatOrArray
+        T : float | FloatArray
             Temperature.
             Unit = K.
-        P : FloatOrArray
+        P : float | FloatArray
             Pressure.
             Unit = Pa.
 
         Returns
         -------
-        FloatOrArray
+        float | FloatArray
             Thermal expansion coefficient, $\alpha$.
             Unit = 1/K.
         """
         A0 = self.A0
         A1 = self.A1
         A2 = self.A2
         TC = T - 273.15
         alpha0 = (A1 + 2*A2*TC)/(A0 + A1*TC + A2*TC**2)
         return alpha0 - P*self.B1*self.beta(T, P)
 
     def beta(self,
-             T: FloatOrArray,
-             P: FloatOrArray
-             ) -> FloatOrArray:
+             T: Union[float, FloatArray],
+             P: Union[float, FloatArray]
+             ) -> Union[float, FloatArray]:
         r"""Calculate isothermal compressibility coefficient, $\beta$.
 
         $$\beta=-\frac{1}{V}\left(\frac{\partial V}{\partial P}\right)_{T}$$
 
         Parameters
         ----------
-        T : FloatOrArray
+        T : float | FloatArray
             Temperature.
             Unit = K.
-        P : FloatOrArray
+        P : float | FloatArray
             Pressure.
             Unit = Pa.
 
         Returns
         -------
-        FloatOrArray
+        float | FloatArray
             Isothermal compressibility coefficient, $\beta$.
             Unit = 1/Pa.
         """
         B = self._B(T)
         return (self._C/(P + B))/(1 - self._C*log(1 + P/B))
```

### Comparing `polykin-0.5.4/src/polykin/properties/thermal_conductivity/liquid.py` & `polykin-0.5.5/src/polykin/properties/thermal_conductivity/liquid.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/properties/thermal_conductivity/vapor.py` & `polykin-0.5.5/src/polykin/properties/thermal_conductivity/vapor.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/properties/vaporization_enthalpy.py` & `polykin-0.5.5/src/polykin/properties/vaporization_enthalpy.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/properties/viscosity/liquid.py` & `polykin-0.5.5/src/polykin/properties/viscosity/liquid.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/properties/viscosity/vapor.py` & `polykin-0.5.5/src/polykin/properties/viscosity/vapor.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/stepgrowth/solutions.py` & `polykin-0.5.5/src/polykin/stepgrowth/solutions.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/thermo/acm/base.py` & `polykin-0.5.5/src/polykin/thermo/acm/base.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/thermo/acm/floryhuggins.py` & `polykin-0.5.5/src/polykin/thermo/acm/floryhuggins.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/thermo/acm/ideal.py` & `polykin-0.5.5/src/polykin/thermo/acm/ideal.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/thermo/acm/nrtl.py` & `polykin-0.5.5/src/polykin/thermo/acm/nrtl.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/thermo/acm/polynrtl.py` & `polykin-0.5.5/src/polykin/thermo/acm/polynrtl.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/thermo/acm/uniquac.py` & `polykin-0.5.5/src/polykin/thermo/acm/uniquac.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/thermo/acm/wilson.py` & `polykin-0.5.5/src/polykin/thermo/acm/wilson.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/thermo/eos/base.py` & `polykin-0.5.5/src/polykin/thermo/eos/base.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/thermo/eos/cubic.py` & `polykin-0.5.5/src/polykin/thermo/eos/cubic.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/thermo/eos/idealgas.py` & `polykin-0.5.5/src/polykin/thermo/eos/idealgas.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/thermo/eos/virial.py` & `polykin-0.5.5/src/polykin/thermo/eos/virial.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/utils/math.py` & `polykin-0.5.5/src/polykin/utils/math.py`

 * *Files identical despite different names*

### Comparing `polykin-0.5.4/src/polykin/utils/tools.py` & `polykin-0.5.5/src/polykin/utils/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from numbers import Number
 from typing import Any, Iterable, Literal, Union
 
 import numpy as np
 
 from .exceptions import RangeError, ShapeError
-from .types import FloatOrArray, FloatOrArrayLike
+from .types import FloatOrArray, FloatOrArrayLike, FloatMatrix
 
 # %% Check tools
 
 
 def custom_error(var_name: str,
                  var_value: Any,
                  kind: type,
@@ -379,7 +379,31 @@
         rows = attr_str.split("\n")
         if len(rows) == 1:
             item = f"{attr_name}:" + " "*(nspaces - len(attr_name)) + attr_str
         else:
             item = "\n  ".join([attr_name + ":"] + rows)
         items.append(item)
     return "\n".join(items)
+
+
+def pprint_matrix(matrix: FloatMatrix,
+                  format_specifier="{:.2e}",
+                  nspaces: int = 0) -> str:
+    """Pretty print a matrix.
+
+    Parameters
+    ----------
+    matrix : FloatMatrix
+        Matrix to print.
+    format_specifier : str
+        Format specifier, e.g "{:.2f}".
+    nspaces : int
+        Number of white spaces placed before 2nd row and following.
+    """
+    nrows = matrix.shape[0]
+    result = ""
+    for i, row in enumerate(matrix):
+        line = "[[" if i == 0 else (" "*nspaces + " [")
+        line += " ".join(format_specifier.format(element) for element in row)
+        line += "]]\n" if i == nrows-1 else "]\n"
+        result += line
+    return result
```

### Comparing `polykin-0.5.4/src/polykin/utils/types.py` & `polykin-0.5.5/src/polykin/utils/types.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 
 from nptyping import Float64, Int32, NDArray, Shape
 
 Number = TypeVar("Number", float, complex)
 
 IntArray = NDArray[Any, Int32]
 IntArrayLike = Union[list[int], tuple[int, ...], IntArray]
-IntOrArray = Union[int, IntArray]
-IntOrArrayLike = Union[int, IntArrayLike]
 
 IntVector = NDArray[Shape['*'], Int32]
 IntVectorLike = Union[list[int], tuple[int, ...], IntVector]
 
 FloatArray = NDArray[Any, Float64]
 FloatArrayLike = Union[list[float], tuple[float, ...], FloatArray]
 FloatOrArray = Union[float, FloatArray]
```

### Comparing `polykin-0.5.4/PKG-INFO` & `polykin-0.5.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polykin
-Version: 0.5.4
+Version: 0.5.5
 Summary: A polymerization kinetics library.
 Home-page: https://hugomvale.github.io/polykin/
 License: MIT
 Keywords: polymer,polymerization,kinetics,reaction
 Author: HugoMVale
 Author-email: 57530119+HugoMVale@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: mpmath (>=1.3.0,<2.0.0)
 Requires-Dist: nptyping (>=2.5.0,<3.0.0)
+Requires-Dist: numba (>=0.59.1,<0.60.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Requires-Dist: pandas (>=1.5.3)
 Requires-Dist: pydantic (>=1.10.13,<2.0.0)
 Requires-Dist: scipy (>=1.11.4,<2.0.0)
 Project-URL: Documentation, https://hugomvale.github.io/polykin/
 Project-URL: Repository, https://github.com/HugoMVale/polykin
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,50 +1,50 @@
-Metadata-Version: 2.1 Name: polykin Version: 0.5.4 Summary: A polymerization
+Metadata-Version: 2.1 Name: polykin Version: 0.5.5 Summary: A polymerization
 kinetics library. Home-page: https://hugomvale.github.io/polykin/ License: MIT
 Keywords: polymer,polymerization,kinetics,reaction Author: HugoMVale Author-
 email: 57530119+HugoMVale@users.noreply.github.com Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Topic :: Scientific/
 Engineering Classifier: Topic :: Scientific/Engineering :: Chemistry Requires-
 Dist: matplotlib (>=3.7.1,<4.0.0) Requires-Dist: mpmath (>=1.3.0,<2.0.0)
-Requires-Dist: nptyping (>=2.5.0,<3.0.0) Requires-Dist: numpy (>=1.23.5,<2.0.0)
-Requires-Dist: pandas (>=1.5.3) Requires-Dist: pydantic (>=1.10.13,<2.0.0)
-Requires-Dist: scipy (>=1.11.4,<2.0.0) Project-URL: Documentation, https://
-hugomvale.github.io/polykin/ Project-URL: Repository, https://github.com/
-HugoMVale/polykin Description-Content-Type: text/markdown # PolyKin [![Test]
-(https://github.com/HugoMVale/polykin/actions/workflows/test.yml/badge.svg)]
-(https://github.com/HugoMVale/polykin/actions) [![codecov](https://codecov.io/
-gh/HugoMVale/polykin/branch/main/graph/badge.svg?token=QfqQLX2rHx)](https://
-codecov.io/gh/HugoMVale/polykin) [![Latest Commit](https://img.shields.io/
-github/last-commit/HugoMVale/polykin)](https://img.shields.io/github/last-
-commit/HugoMVale/polykin) PolyKin is an open-source polymerization kinetics
-library for Python. It is still at an early development stage, but the
-following modules can already be used: - Activity coefficient models - [x]
-Ideal solution - [x] Flory-Huggins - [x] NRTL - [ ] Poly-NRTL - [x] UNIQUAC -
-[x] Wilson - Copolymerization - [x] Implicit penultimate model - [x]
-Penultimate model - [x] Terminal model - [x] Mayo-Lewis equation (binary,
-ternary and multicomponent) - [x] Monomer drift equation (binary and
-multicomponent) - [ ] Fitting methods - Equations of state - [50%] Cubic
-(Redlich-Kwong, Soave, Peng-Robinson) - [x] Ideal gas - [ ] Sanchez-Lacombe -
-[x] Virial equation - [ ] Database - Distributions - [x] Flory - [ ] Gold - [x]
-Log-normal - [x] Poison - [x] Schulz-Zimm - Kinetics - [x] Arrhenius - [x]
-Eyring - [x] Propagation half-length - [x] Termination composite model - Math -
-[x] Joint confidence regions - [ ] Models - Physical property correlations -
-[x] Antoine - [x] DIPPR - [x] Wagner - [x] Yaws - Step-growth polymerization -
-[x] Analytical solutions for $M_n$ and $M_w$ - Transport properties (estimation
-methods, mixing rules, etc.) - Diffusivity - [x] Binary gas mixtures - [x]
-Binary liquid mixtures - [x] Binary polymer solutions - [ ] Multicomponent
-polymer solutions - Thermal conductivity - [x] Gases - [x] Liquids - [ ]
-Polymer solutions - Viscosity - [x] Gases - [x] Liquids - [ ] Polymer solutions
-## Documentation Please refer to the package [homepage](https://
-hugomvale.github.io/polykin/). ## Tutorials The main features of PolyKin are
-explained and illustrated through a series of [tutorials](https://
+Requires-Dist: nptyping (>=2.5.0,<3.0.0) Requires-Dist: numba
+(>=0.59.1,<0.60.0) Requires-Dist: numpy (>=1.23.5,<2.0.0) Requires-Dist: pandas
+(>=1.5.3) Requires-Dist: pydantic (>=1.10.13,<2.0.0) Requires-Dist: scipy
+(>=1.11.4,<2.0.0) Project-URL: Documentation, https://hugomvale.github.io/
+polykin/ Project-URL: Repository, https://github.com/HugoMVale/polykin
+Description-Content-Type: text/markdown # PolyKin [![Test](https://github.com/
+HugoMVale/polykin/actions/workflows/test.yml/badge.svg)](https://github.com/
+HugoMVale/polykin/actions) [![codecov](https://codecov.io/gh/HugoMVale/polykin/
+branch/main/graph/badge.svg?token=QfqQLX2rHx)](https://codecov.io/gh/HugoMVale/
+polykin) [![Latest Commit](https://img.shields.io/github/last-commit/HugoMVale/
+polykin)](https://img.shields.io/github/last-commit/HugoMVale/polykin) PolyKin
+is an open-source polymerization kinetics library for Python. It is still at an
+early development stage, but the following modules can already be used: -
+Activity coefficient models - [x] Ideal solution - [x] Flory-Huggins - [x] NRTL
+- [ ] Poly-NRTL - [x] UNIQUAC - [x] Wilson - Copolymerization - [x] Implicit
+penultimate model - [x] Penultimate model - [x] Terminal model - [x] Mayo-Lewis
+equation (binary, ternary and multicomponent) - [x] Monomer drift equation
+(binary and multicomponent) - [ ] Fitting methods - Equations of state - [50%]
+Cubic (Redlich-Kwong, Soave, Peng-Robinson) - [x] Ideal gas - [ ] Sanchez-
+Lacombe - [x] Virial equation - [ ] Database - Distributions - [x] Flory - [ ]
+Gold - [x] Log-normal - [x] Poison - [x] Schulz-Zimm - Kinetics - [x] Arrhenius
+- [x] Eyring - [x] Propagation half-length - [x] Termination composite model -
+Math - [x] Joint confidence regions - [ ] Models - Physical property
+correlations - [x] Antoine - [x] DIPPR - [x] Wagner - [x] Yaws - Step-growth
+polymerization - [x] Analytical solutions for $M_n$ and $M_w$ - Transport
+properties (estimation methods, mixing rules, etc.) - Diffusivity - [x] Binary
+gas mixtures - [x] Binary liquid mixtures - [x] Binary polymer solutions - [ ]
+Multicomponent polymer solutions - Thermal conductivity - [x] Gases - [x]
+Liquids - [ ] Polymer solutions - Viscosity - [x] Gases - [x] Liquids - [ ]
+Polymer solutions ## Documentation Please refer to the package [homepage]
+(https://hugomvale.github.io/polykin/). ## Tutorials The main features of
+PolyKin are explained and illustrated through a series of [tutorials](https://
 hugomvale.github.io/polykin/tutorials/) based on Jupyter [notebooks](https://
 github.com/HugoMVale/polykin/tree/main/docs/tutorials), which can be launched
 online via Binder.
                            _[_M_W_D_ _o_f_ _a_ _p_o_l_y_m_e_r_ _b_l_e_n_d_]
 ## Installation PolyKin currently runs on Python 3.9+. You can install it from
 PyPI via `pip` (or `poetry`): ```console pip install polykin # poetry add
 polykin ``` Alternatively, you may install it directly from the source code
```

