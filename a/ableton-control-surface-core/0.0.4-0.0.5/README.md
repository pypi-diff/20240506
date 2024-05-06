# Comparing `tmp/ableton-control-surface-core-0.0.4.tar.gz` & `tmp/ableton-control-surface-core-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/sahlen/repositories/oslo1989/ableton-controlsurface-toolkit/ableton-control-surface-core/dist/.tmp-njjfi_ew/ableton-cont", last modified: Sun May  5 19:37:07 2024, max compression
+gzip compressed data, was "/Users/sahlen/repositories/oslo1989/ableton-controlsurface-toolkit/ableton-control-surface-core/dist/.tmp-v1z596ec/ableton-cont", last modified: Sun May  5 19:48:50 2024, max compression
```

## Comparing `ableton-control-surface-core-0.0.4.tar` & `ableton-control-surface-core-0.0.5.tar`

### file list

```diff
@@ -1,407 +1,471 @@
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/
--rw-r--r--   0 sahlen     (501) staff       (20)       23 2024-05-05 19:32:49.000000 ableton-control-surface-core-0.0.4/MANIFEST.in
--rw-r--r--   0 sahlen     (501) staff       (20)      677 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/PKG-INFO
--rw-r--r--   0 sahlen     (501) staff       (20)      784 2024-05-05 19:36:58.000000 ableton-control-surface-core-0.0.4/pyproject.toml
--rw-r--r--   0 sahlen     (501) staff       (20)       38 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/setup.cfg
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/Application/
--rw-r--r--   0 sahlen     (501) staff       (20)    33998 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/Application/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/Base/
--rw-r--r--   0 sahlen     (501) staff       (20)     7902 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/Base/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/Browser/
--rw-r--r--   0 sahlen     (501) staff       (20)    12899 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/Browser/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/CcControlDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)    32941 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/CcControlDevice/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/Chain/
--rw-r--r--   0 sahlen     (501) staff       (20)    13722 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/Chain/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/ChainMixerDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)     3237 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/ChainMixerDevice/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/Clip/
--rw-r--r--   0 sahlen     (501) staff       (20)    77137 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/Clip/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/ClipSlot/
--rw-r--r--   0 sahlen     (501) staff       (20)    15636 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/ClipSlot/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/CompressorDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)    17945 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/CompressorDevice/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/Conversions/
--rw-r--r--   0 sahlen     (501) staff       (20)     5053 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/Conversions/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/Device/
--rw-r--r--   0 sahlen     (501) staff       (20)    12155 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/Device/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/DeviceIO/
--rw-r--r--   0 sahlen     (501) staff       (20)     7742 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/DeviceIO/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/DeviceParameter/
--rw-r--r--   0 sahlen     (501) staff       (20)    11899 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/DeviceParameter/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/DriftDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)    36356 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/DriftDevice/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/DrumChain/
--rw-r--r--   0 sahlen     (501) staff       (20)    16427 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/DrumChain/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/DrumPad/
--rw-r--r--   0 sahlen     (501) staff       (20)     7070 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/DrumPad/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/Eq8Device/
--rw-r--r--   0 sahlen     (501) staff       (20)    18335 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/Eq8Device/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/Groove/
--rw-r--r--   0 sahlen     (501) staff       (20)     9819 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/Groove/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/GroovePool/
--rw-r--r--   0 sahlen     (501) staff       (20)     2695 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/GroovePool/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/HybridReverbDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)    21543 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/HybridReverbDevice/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/Listener/
--rw-r--r--   0 sahlen     (501) staff       (20)     2671 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/Listener/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/LomObject/
--rw-r--r--   0 sahlen     (501) staff       (20)     1273 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/LomObject/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/MaxDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)    19811 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/MaxDevice/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/MeldDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)    16732 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/MeldDevice/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/MidiMap/
--rw-r--r--   0 sahlen     (501) staff       (20)     7319 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/MidiMap/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/MixerDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)     8527 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/MixerDevice/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/PluginDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)    14632 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/PluginDevice/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/RackDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)    35755 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/RackDevice/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/RoarDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)    14175 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/RoarDevice/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/Sample/
--rw-r--r--   0 sahlen     (501) staff       (20)    35677 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/Sample/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/Live/Scene/
--rw-r--r--   0 sahlen     (501) staff       (20)    17944 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/Scene/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/Live/ShifterDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)    14278 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/ShifterDevice/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/Live/SimplerDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)    48147 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/SimplerDevice/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/Live/Song/
--rw-r--r--   0 sahlen     (501) staff       (20)   107534 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/Song/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/Live/SpectralResonatorDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)    28621 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/SpectralResonatorDevice/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/Live/Track/
--rw-r--r--   0 sahlen     (501) staff       (20)    83720 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/Track/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/Live/WavetableDevice/
--rw-r--r--   0 sahlen     (501) staff       (20)    42891 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/WavetableDevice/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)      917 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/Live/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/MidiRemoteScript/
--rw-r--r--   0 sahlen     (501) staff       (20)    32839 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.4/src/MidiRemoteScript/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/_Framework/
--rw-r--r--   0 sahlen     (501) staff       (20)     1833 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.4/src/_Framework/BackgroundComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3300 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/_Framework/ButtonElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3616 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/_Framework/ButtonMatrixElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4089 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.4/src/_Framework/ButtonSliderElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1761 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/_Framework/Capabilities.py
--rw-r--r--   0 sahlen     (501) staff       (20)    14782 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/_Framework/ChannelStripComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1472 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/_Framework/ChannelTranslationSelector.py
--rw-r--r--   0 sahlen     (501) staff       (20)      888 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.4/src/_Framework/ClipCreator.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9996 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/_Framework/ClipSlotComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)    10819 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.4/src/_Framework/ComboElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1728 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/_Framework/CompoundComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7910 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/_Framework/CompoundElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)    32374 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/_Framework/Control.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4548 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/_Framework/ControlElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)    23782 2024-01-08 19:11:24.000000 ableton-control-surface-core-0.0.4/src/_Framework/ControlSurface.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4675 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/_Framework/ControlSurfaceComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      490 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.4/src/_Framework/Defaults.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3273 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.4/src/_Framework/Dependency.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1377 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/_Framework/DeviceBankRegistry.py
--rw-r--r--   0 sahlen     (501) staff       (20)    17045 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/_Framework/DeviceComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1843 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/_Framework/Disconnectable.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3030 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/_Framework/DisplayDataSource.py
--rw-r--r--   0 sahlen     (501) staff       (20)    12883 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/_Framework/DrumGroupComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2055 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/_Framework/DrumRackComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6553 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/_Framework/EncoderElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2152 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/_Framework/IdentifiableControlSurface.py
--rw-r--r--   0 sahlen     (501) staff       (20)    14136 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/_Framework/InputControlElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4367 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.4/src/_Framework/Layer.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2234 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/_Framework/LogicalDisplaySegment.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6158 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/_Framework/MessageScheduler.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1904 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.4/src/_Framework/MidiMap.py
--rw-r--r--   0 sahlen     (501) staff       (20)    12255 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/_Framework/MixerComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4571 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/_Framework/ModeSelectorComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)    20978 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/_Framework/ModesComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1724 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.4/src/_Framework/MomentaryModeObserver.py
--rw-r--r--   0 sahlen     (501) staff       (20)      729 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.4/src/_Framework/NotifyingControlElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1072 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/_Framework/OptionalElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)    11654 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.4/src/_Framework/PhysicalDisplayElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1160 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/_Framework/Profile.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2293 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/_Framework/Proxy.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7708 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/_Framework/Resource.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7057 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.4/src/_Framework/SceneComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4412 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/_Framework/ScrollComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)    24427 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/_Framework/SessionComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)    11946 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.4/src/_Framework/SessionRecordingComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)    13213 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/_Framework/SessionZoomingComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2258 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/_Framework/Signal.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1456 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/_Framework/Skin.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3749 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.4/src/_Framework/SlideComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      622 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.4/src/_Framework/SliderElement.py
--rw-r--r--   0 sahlen     (501) staff       (20)    11114 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/_Framework/SubjectSlot.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1063 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/_Framework/SysexValueControl.py
--rw-r--r--   0 sahlen     (501) staff       (20)    11460 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.4/src/_Framework/Task.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2889 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.4/src/_Framework/ToggleComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1708 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.4/src/_Framework/TrackArmState.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9300 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.4/src/_Framework/TransportComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)    11558 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/_Framework/Util.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5769 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/_Framework/ViewControlComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      351 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.4/src/_Framework/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/_Generic/
--rw-r--r--   0 sahlen     (501) staff       (20)    37606 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/_Generic/Devices.py
--rw-r--r--   0 sahlen     (501) staff       (20)    16384 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/_Generic/GenericScript.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1089 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/_Generic/SelectChanStripComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      792 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/_Generic/SpecialMixerComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)      349 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.4/src/_Generic/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1908 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/_Generic/util.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/_MxDCore/
--rw-r--r--   0 sahlen     (501) staff       (20)    10569 2024-01-08 19:11:24.000000 ableton-control-surface-core-0.0.4/src/_MxDCore/ControlSurfaceWrapper.py
--rw-r--r--   0 sahlen     (501) staff       (20)    39976 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/_MxDCore/LomTypes.py
--rw-r--r--   0 sahlen     (501) staff       (20)    14199 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/_MxDCore/LomUtils.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6675 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/_MxDCore/MxDControlSurfaceAPI.py
--rw-r--r--   0 sahlen     (501) staff       (20)    61272 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/_MxDCore/MxDCore.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6601 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/_MxDCore/MxDUtils.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1504 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.4/src/_MxDCore/NotesAPIUtils.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1512 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.4/src/_MxDCore/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/_Tools/
--rw-r--r--   0 sahlen     (501) staff       (20)      347 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.4/src/_Tools/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/_Userscript/
--rw-r--r--   0 sahlen     (501) staff       (20)     4827 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/_Userscript/DeviceComponent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9889 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/_Userscript/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-01-13 16:36:43.000000 ableton-control-surface-core-0.0.4/src/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/ableton/
--rw-r--r--   0 sahlen     (501) staff       (20)      348 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.4/src/ableton/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/
--rw-r--r--   0 sahlen     (501) staff       (20)      351 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/base/
--rw-r--r--   0 sahlen     (501) staff       (20)     3343 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/base/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2330 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/base/abl_signal.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/base/collection/
--rw-r--r--   0 sahlen     (501) staff       (20)      433 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/base/collection/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1551 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/base/collection/indexed_dict.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3336 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/base/dependency.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2042 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/base/disconnectable.py
--rw-r--r--   0 sahlen     (501) staff       (20)    14794 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/base/event.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1340 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/base/gcutil.py
--rw-r--r--   0 sahlen     (501) staff       (20)      732 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/base/isclose.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1042 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/base/live_api_utils.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2295 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/base/proxy.py
--rw-r--r--   0 sahlen     (501) staff       (20)    11401 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/base/task.py
--rw-r--r--   0 sahlen     (501) staff       (20)    12775 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/base/util.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/
--rw-r--r--   0 sahlen     (501) staff       (20)     4994 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4084 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/banking_util.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1779 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/capabilities.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1203 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/clip_creator.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4633 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/component.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/
--rw-r--r--   0 sahlen     (501) staff       (20)     3574 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1391 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/accent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4234 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/auto_arm.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2028 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/background.py
--rw-r--r--   0 sahlen     (501) staff       (20)    15153 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/channel_strip.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3304 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/clip_actions.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9748 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/clip_slot.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5506 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/device.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7407 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/device_navigation.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5791 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/device_parameters.py
--rw-r--r--   0 sahlen     (501) staff       (20)    11832 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/drum_group.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9005 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/item_lister.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8917 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/mixer.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4324 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/playable.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8193 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/scene.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4225 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/scroll.py
--rw-r--r--   0 sahlen     (501) staff       (20)    11420 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/session.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5917 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/session_navigation.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6813 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/session_overview.py
--rw-r--r--   0 sahlen     (501) staff       (20)    13211 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/session_recording.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5390 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/session_ring.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3749 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/slide.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2966 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/target_track.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2838 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/toggle.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8721 2024-01-27 16:20:11.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/transport.py
--rw-r--r--   0 sahlen     (501) staff       (20)      874 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/undo_redo.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6121 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/view_control.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8705 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/compound_element.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/control/
--rw-r--r--   0 sahlen     (501) staff       (20)     2012 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/control/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)    10270 2024-01-08 19:05:13.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/control/button.py
--rw-r--r--   0 sahlen     (501) staff       (20)    10181 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/control/control.py
--rw-r--r--   0 sahlen     (501) staff       (20)    10908 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/control/control_list.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8999 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/control/encoder.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5216 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/control/mapped.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1991 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/control/radio_button.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1259 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/control/sysex.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1726 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/control/text_display.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2147 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/control/toggle_button.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5527 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/control_element.py
--rw-r--r--   0 sahlen     (501) staff       (20)    23210 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/control_surface.py
--rw-r--r--   0 sahlen     (501) staff       (20)    12340 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/decoration.py
--rw-r--r--   0 sahlen     (501) staff       (20)   244847 2024-01-08 19:05:13.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/default_bank_definitions.py
--rw-r--r--   0 sahlen     (501) staff       (20)      531 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/defaults.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4579 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/delay_decoration.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1479 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/device_bank_registry.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1564 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/device_chain_utils.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1779 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/device_decorator_factory.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6493 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/device_parameter_bank.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4720 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/device_provider.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2208 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/drift_decoration.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/
--rw-r--r--   0 sahlen     (501) staff       (20)     2902 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4179 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/button.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3805 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/button_matrix.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4134 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/button_slider.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3399 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/color.py
--rw-r--r--   0 sahlen     (501) staff       (20)    10979 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/combo.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3025 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/display_data_source.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8383 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/encoder.py
--rw-r--r--   0 sahlen     (501) staff       (20)      666 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/full_velocity_element.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2261 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/logical_display_segment.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1077 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/optional.py
--rw-r--r--   0 sahlen     (501) staff       (20)    11781 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/physical_display.py
--rw-r--r--   0 sahlen     (501) staff       (20)      857 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/playhead_element.py
--rw-r--r--   0 sahlen     (501) staff       (20)      630 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/proxy_element.py
--rw-r--r--   0 sahlen     (501) staff       (20)      633 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/slider.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2094 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/sysex_element.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1041 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/velocity_levels_element.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2403 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/identifiable_control_surface.py
--rw-r--r--   0 sahlen     (501) staff       (20)    15040 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/input_control_element.py
--rw-r--r--   0 sahlen     (501) staff       (20)    12427 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/internal_parameter.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4936 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/layer.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6506 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/message_scheduler.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1683 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/midi.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1831 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/midi_map.py
--rw-r--r--   0 sahlen     (501) staff       (20)    16494 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/mode.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1924 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/parameter_provider.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5089 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/parameter_slot_description.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3683 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/percussion_instrument_finder.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1176 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/profile.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7737 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/resource.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1215 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/roar_decoration.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1893 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/session_ring_selection_linking.py
--rw-r--r--   0 sahlen     (501) staff       (20)    14536 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/simpler_decoration.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4010 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/simpler_slice_nudging.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2582 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/skin.py
--rw-r--r--   0 sahlen     (501) staff       (20)    11861 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/wavetable_decoration.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/
--rw-r--r--   0 sahlen     (501) staff       (20)      351 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/__init__.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/base/
--rw-r--r--   0 sahlen     (501) staff       (20)     1791 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/base/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1674 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/base/util.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/
--rw-r--r--   0 sahlen     (501) staff       (20)     4373 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4680 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/banking_util.py
--rw-r--r--   0 sahlen     (501) staff       (20)      746 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/capabilities.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4179 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/colors.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4762 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/component.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3333 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/component_map.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/
--rw-r--r--   0 sahlen     (501) staff       (20)     4190 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1359 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/accent.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3465 2024-01-08 19:12:03.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/active_parameter.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3417 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/auto_arm.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3113 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/background.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8425 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/channel_strip.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5020 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/clip_actions.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7637 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/clip_slot.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2417 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/clipboard.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9053 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/device.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5354 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/device_bank_navigation.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2336 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/device_parameters.py
--rw-r--r--   0 sahlen     (501) staff       (20)    14802 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/drum_group.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2087 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/drum_group_scroll.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2987 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/grid_resolution.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7049 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/loop_selector.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9585 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/mixer.py
--rw-r--r--   0 sahlen     (501) staff       (20)    17858 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/note_editor.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3459 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/page.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2116 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/paginator.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4144 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/playable.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2733 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/playhead.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6702 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/recording.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4613 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/scene.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4560 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/scroll.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9303 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/session.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5580 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/session_navigation.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4777 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/session_overview.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6395 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/session_ring.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2104 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/simple_device_navigation.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8492 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/sliced_simpler.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5588 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/step_sequence.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6721 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/target_track.py
--rw-r--r--   0 sahlen     (501) staff       (20)     9883 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/transport.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1358 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/undo_redo.py
--rw-r--r--   0 sahlen     (501) staff       (20)     5696 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/view_control.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2748 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/view_toggle.py
--rw-r--r--   0 sahlen     (501) staff       (20)      582 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/consts.py
--rw-r--r--   0 sahlen     (501) staff       (20)    14932 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/control_surface.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3959 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/control_surface_mapping.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2384 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/control_surface_specification.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/controls/
--rw-r--r--   0 sahlen     (501) staff       (20)     1775 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/controls/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2304 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/controls/button.py
--rw-r--r--   0 sahlen     (501) staff       (20)      662 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/controls/control.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2021 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/controls/control_list.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3614 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/controls/mapped.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1071 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/controls/toggle_button.py
--rw-r--r--   0 sahlen     (501) staff       (20)   110010 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/default_bank_definitions.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6838 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/default_skin.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2569 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/device_decorators.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/
--rw-r--r--   0 sahlen     (501) staff       (20)      913 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     4884 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/display_specification.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/event_signal/
--rw-r--r--   0 sahlen     (501) staff       (20)      507 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/event_signal/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)      771 2024-01-08 19:25:27.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/event_signal/core.py
--rw-r--r--   0 sahlen     (501) staff       (20)      601 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/event_signal/type_decl.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/notifications/
--rw-r--r--   0 sahlen     (501) staff       (20)      515 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/notifications/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8662 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/notifications/all.py
--rw-r--r--   0 sahlen     (501) staff       (20)      552 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/notifications/default.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2117 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/notifications/meta.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1219 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/notifications/type_decl.py
--rw-r--r--   0 sahlen     (501) staff       (20)      767 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/notifications/util.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3710 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/renderable.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2339 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/state.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1819 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/text.py
--rw-r--r--   0 sahlen     (501) staff       (20)      736 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/type_decl.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1433 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/util.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/view/
--rw-r--r--   0 sahlen     (501) staff       (20)      618 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/view/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3422 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/view/notification.py
--rw-r--r--   0 sahlen     (501) staff       (20)      613 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/view/type_decl.py
--rw-r--r--   0 sahlen     (501) staff       (20)      686 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/view/util.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2799 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/view/view.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/elements/
--rw-r--r--   0 sahlen     (501) staff       (20)     1573 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/elements/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2709 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/elements/button.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1374 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/elements/button_matrix.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2154 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/elements/color.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1547 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/elements/discrete_values.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2261 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/elements/display_line.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7540 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/elements/encoder.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2216 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/elements/lockable_button.py
--rw-r--r--   0 sahlen     (501) staff       (20)      646 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/elements/lockable_combo.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3723 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/elements/sysex.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1493 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/elements/touch.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8328 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/elements_base.py
--rw-r--r--   0 sahlen     (501) staff       (20)     6039 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/identification.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3490 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/instrument_finder.py
--rw-r--r--   0 sahlen     (501) staff       (20)      675 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/layer.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1160 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/legacy_bank_definitions.py
--rw-r--r--   0 sahlen     (501) staff       (20)     1030 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/midi.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/mode/
--rw-r--r--   0 sahlen     (501) staff       (20)     1648 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/mode/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2180 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/mode/behaviour.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2531 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/mode/mode.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8685 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/mode/modes.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2584 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/mode/selector.py
--rw-r--r--   0 sahlen     (501) staff       (20)      918 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/parameter_info.py
--rw-r--r--   0 sahlen     (501) staff       (20)     3521 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/parameter_mapping_sensitivities.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2617 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/session_ring_selection_linking.py
--rw-r--r--   0 sahlen     (501) staff       (20)     2215 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/skin.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/live/
--rw-r--r--   0 sahlen     (501) staff       (20)     1986 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/live/__init__.py
--rw-r--r--   0 sahlen     (501) staff       (20)     7661 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/live/action.py
--rw-r--r--   0 sahlen     (501) staff       (20)     8160 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.4/src/ableton/v3/live/util.py
-drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:37:07.000000 ableton-control-surface-core-0.0.4/src/ableton_control_surface_core.egg-info/
--rw-r--r--   0 sahlen     (501) staff       (20)      677 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/ableton_control_surface_core.egg-info/PKG-INFO
--rw-r--r--   0 sahlen     (501) staff       (20)    15139 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/ableton_control_surface_core.egg-info/SOURCES.txt
--rw-r--r--   0 sahlen     (501) staff       (20)        1 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/ableton_control_surface_core.egg-info/dependency_links.txt
--rw-r--r--   0 sahlen     (501) staff       (20)       87 2024-05-05 19:37:06.000000 ableton-control-surface-core-0.0.4/src/ableton_control_surface_core.egg-info/top_level.txt
--rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:32:58.000000 ableton-control-surface-core-0.0.4/src/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/
+-rw-r--r--   0 sahlen     (501) staff       (20)       23 2024-05-05 19:32:49.000000 ableton-control-surface-core-0.0.5/MANIFEST.in
+-rw-r--r--   0 sahlen     (501) staff       (20)      677 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/PKG-INFO
+-rw-r--r--   0 sahlen     (501) staff       (20)      784 2024-05-05 19:48:34.000000 ableton-control-surface-core-0.0.5/pyproject.toml
+-rw-r--r--   0 sahlen     (501) staff       (20)       38 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/setup.cfg
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/Application/
+-rw-r--r--   0 sahlen     (501) staff       (20)    33998 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/Application/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/Application/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/Base/
+-rw-r--r--   0 sahlen     (501) staff       (20)     7902 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/Base/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/Base/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/Browser/
+-rw-r--r--   0 sahlen     (501) staff       (20)    12899 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/Browser/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/Browser/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/CcControlDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)    32941 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/CcControlDevice/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/CcControlDevice/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/Chain/
+-rw-r--r--   0 sahlen     (501) staff       (20)    13722 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/Chain/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/Chain/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/ChainMixerDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)     3237 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/ChainMixerDevice/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/ChainMixerDevice/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/Clip/
+-rw-r--r--   0 sahlen     (501) staff       (20)    77137 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/Clip/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/Clip/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/ClipSlot/
+-rw-r--r--   0 sahlen     (501) staff       (20)    15636 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/ClipSlot/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/ClipSlot/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/CompressorDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)    17945 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/CompressorDevice/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/CompressorDevice/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/Conversions/
+-rw-r--r--   0 sahlen     (501) staff       (20)     5053 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/Conversions/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/Conversions/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/Device/
+-rw-r--r--   0 sahlen     (501) staff       (20)    12155 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/Device/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/Device/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/DeviceIO/
+-rw-r--r--   0 sahlen     (501) staff       (20)     7742 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/DeviceIO/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/DeviceIO/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/DeviceParameter/
+-rw-r--r--   0 sahlen     (501) staff       (20)    11899 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/DeviceParameter/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/DeviceParameter/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/DriftDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)    36356 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/DriftDevice/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/DriftDevice/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/DrumChain/
+-rw-r--r--   0 sahlen     (501) staff       (20)    16427 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/DrumChain/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/DrumChain/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/DrumPad/
+-rw-r--r--   0 sahlen     (501) staff       (20)     7070 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/DrumPad/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/DrumPad/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/Eq8Device/
+-rw-r--r--   0 sahlen     (501) staff       (20)    18335 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/Eq8Device/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/Eq8Device/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/Groove/
+-rw-r--r--   0 sahlen     (501) staff       (20)     9819 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/Groove/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/Groove/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/GroovePool/
+-rw-r--r--   0 sahlen     (501) staff       (20)     2695 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/GroovePool/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/GroovePool/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/HybridReverbDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)    21543 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/HybridReverbDevice/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/HybridReverbDevice/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/Listener/
+-rw-r--r--   0 sahlen     (501) staff       (20)     2671 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/Listener/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/Listener/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/LomObject/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1273 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/LomObject/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/LomObject/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/MaxDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)    19811 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/MaxDevice/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/MaxDevice/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/MeldDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)    16732 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/MeldDevice/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/MeldDevice/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/MidiMap/
+-rw-r--r--   0 sahlen     (501) staff       (20)     7319 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/MidiMap/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/MidiMap/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/MixerDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)     8527 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/MixerDevice/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/MixerDevice/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/PluginDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)    14632 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/PluginDevice/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/PluginDevice/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/RackDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)    35755 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/RackDevice/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/RackDevice/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/RoarDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)    14175 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/RoarDevice/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/RoarDevice/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/Sample/
+-rw-r--r--   0 sahlen     (501) staff       (20)    35677 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/Sample/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/Sample/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/Scene/
+-rw-r--r--   0 sahlen     (501) staff       (20)    17944 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/Scene/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/Scene/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/ShifterDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)    14278 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/ShifterDevice/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/ShifterDevice/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/SimplerDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)    48147 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/SimplerDevice/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/SimplerDevice/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/Song/
+-rw-r--r--   0 sahlen     (501) staff       (20)   107534 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/Song/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/Song/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/SpectralResonatorDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)    28621 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/SpectralResonatorDevice/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/SpectralResonatorDevice/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/Track/
+-rw-r--r--   0 sahlen     (501) staff       (20)    83720 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/Track/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/Track/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/Live/WavetableDevice/
+-rw-r--r--   0 sahlen     (501) staff       (20)    42891 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/WavetableDevice/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/WavetableDevice/py.typed
+-rw-r--r--   0 sahlen     (501) staff       (20)      917 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/Live/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/Live/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/MidiRemoteScript/
+-rw-r--r--   0 sahlen     (501) staff       (20)    32839 2024-01-20 22:36:35.000000 ableton-control-surface-core-0.0.5/src/MidiRemoteScript/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/MidiRemoteScript/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/_Framework/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1833 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.5/src/_Framework/BackgroundComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3300 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/_Framework/ButtonElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3616 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/_Framework/ButtonMatrixElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4089 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.5/src/_Framework/ButtonSliderElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1761 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/_Framework/Capabilities.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    14782 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/_Framework/ChannelStripComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1472 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/_Framework/ChannelTranslationSelector.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      888 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.5/src/_Framework/ClipCreator.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9996 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/_Framework/ClipSlotComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    10819 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.5/src/_Framework/ComboElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1728 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/_Framework/CompoundComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7910 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/_Framework/CompoundElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    32374 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/_Framework/Control.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4548 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/_Framework/ControlElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    23782 2024-01-08 19:11:24.000000 ableton-control-surface-core-0.0.5/src/_Framework/ControlSurface.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4675 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/_Framework/ControlSurfaceComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      490 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.5/src/_Framework/Defaults.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3273 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.5/src/_Framework/Dependency.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1377 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/_Framework/DeviceBankRegistry.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    17045 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/_Framework/DeviceComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1843 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/_Framework/Disconnectable.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3030 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/_Framework/DisplayDataSource.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    12883 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/_Framework/DrumGroupComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2055 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/_Framework/DrumRackComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6553 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/_Framework/EncoderElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2152 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/_Framework/IdentifiableControlSurface.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    14136 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/_Framework/InputControlElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4367 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.5/src/_Framework/Layer.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2234 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/_Framework/LogicalDisplaySegment.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6158 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/_Framework/MessageScheduler.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1904 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.5/src/_Framework/MidiMap.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    12255 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/_Framework/MixerComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4571 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/_Framework/ModeSelectorComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    20978 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/_Framework/ModesComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1724 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.5/src/_Framework/MomentaryModeObserver.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      729 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.5/src/_Framework/NotifyingControlElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1072 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/_Framework/OptionalElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    11654 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.5/src/_Framework/PhysicalDisplayElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1160 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/_Framework/Profile.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2293 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/_Framework/Proxy.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7708 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/_Framework/Resource.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7057 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.5/src/_Framework/SceneComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4412 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/_Framework/ScrollComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    24427 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/_Framework/SessionComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    11946 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.5/src/_Framework/SessionRecordingComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    13213 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/_Framework/SessionZoomingComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2258 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/_Framework/Signal.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1456 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/_Framework/Skin.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3749 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.5/src/_Framework/SlideComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      622 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.5/src/_Framework/SliderElement.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    11114 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/_Framework/SubjectSlot.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1063 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/_Framework/SysexValueControl.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    11460 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.5/src/_Framework/Task.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2889 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.5/src/_Framework/ToggleComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1708 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.5/src/_Framework/TrackArmState.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9300 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.5/src/_Framework/TransportComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    11558 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/_Framework/Util.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5769 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/_Framework/ViewControlComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      351 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.5/src/_Framework/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/_Framework/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/_Generic/
+-rw-r--r--   0 sahlen     (501) staff       (20)    37606 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/_Generic/Devices.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    16384 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/_Generic/GenericScript.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1089 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/_Generic/SelectChanStripComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      792 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/_Generic/SpecialMixerComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      349 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.5/src/_Generic/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/_Generic/py.typed
+-rw-r--r--   0 sahlen     (501) staff       (20)     1908 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/_Generic/util.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/_MxDCore/
+-rw-r--r--   0 sahlen     (501) staff       (20)    10569 2024-01-08 19:11:24.000000 ableton-control-surface-core-0.0.5/src/_MxDCore/ControlSurfaceWrapper.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    39976 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/_MxDCore/LomTypes.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    14199 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/_MxDCore/LomUtils.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6675 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/_MxDCore/MxDControlSurfaceAPI.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    61272 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/_MxDCore/MxDCore.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6601 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/_MxDCore/MxDUtils.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1504 2024-01-08 18:49:34.000000 ableton-control-surface-core-0.0.5/src/_MxDCore/NotesAPIUtils.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1512 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.5/src/_MxDCore/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/_MxDCore/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/_Tools/
+-rw-r--r--   0 sahlen     (501) staff       (20)      347 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.5/src/_Tools/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/_Tools/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/_Userscript/
+-rw-r--r--   0 sahlen     (501) staff       (20)     4827 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/_Userscript/DeviceComponent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9889 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/_Userscript/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/_Userscript/py.typed
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-01-13 16:36:43.000000 ableton-control-surface-core-0.0.5/src/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/ableton/
+-rw-r--r--   0 sahlen     (501) staff       (20)      348 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.5/src/ableton/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/ableton/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/
+-rw-r--r--   0 sahlen     (501) staff       (20)      351 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/base/
+-rw-r--r--   0 sahlen     (501) staff       (20)     3343 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/base/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2330 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/base/abl_signal.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/base/collection/
+-rw-r--r--   0 sahlen     (501) staff       (20)      433 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/base/collection/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1551 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/base/collection/indexed_dict.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/base/collection/py.typed
+-rw-r--r--   0 sahlen     (501) staff       (20)     3336 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/base/dependency.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2042 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/base/disconnectable.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    14794 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/base/event.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1340 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/base/gcutil.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      732 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/base/isclose.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1042 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/base/live_api_utils.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2295 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/base/proxy.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/base/py.typed
+-rw-r--r--   0 sahlen     (501) staff       (20)    11401 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/base/task.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    12775 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/base/util.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/
+-rw-r--r--   0 sahlen     (501) staff       (20)     4994 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4084 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/banking_util.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1779 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/capabilities.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1203 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/clip_creator.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4633 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/component.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/
+-rw-r--r--   0 sahlen     (501) staff       (20)     3574 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1391 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/accent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4234 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/auto_arm.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2028 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/background.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    15153 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/channel_strip.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3304 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/clip_actions.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9748 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/clip_slot.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5506 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/device.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7407 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/device_navigation.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5791 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/device_parameters.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    11832 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/drum_group.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9005 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/item_lister.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8917 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/mixer.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4324 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/playable.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/py.typed
+-rw-r--r--   0 sahlen     (501) staff       (20)     8193 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/scene.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4225 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/scroll.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    11420 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/session.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5917 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/session_navigation.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6813 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/session_overview.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    13211 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/session_recording.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5390 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/session_ring.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3749 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/slide.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2966 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/target_track.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2838 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/toggle.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8721 2024-01-27 16:20:11.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/transport.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      874 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/undo_redo.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6121 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/view_control.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8705 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/compound_element.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/control/
+-rw-r--r--   0 sahlen     (501) staff       (20)     2012 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/control/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    10270 2024-01-08 19:05:13.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/control/button.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    10181 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/control/control.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    10908 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/control/control_list.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8999 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/control/encoder.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5216 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/control/mapped.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/control/py.typed
+-rw-r--r--   0 sahlen     (501) staff       (20)     1991 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/control/radio_button.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1259 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/control/sysex.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1726 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/control/text_display.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2147 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/control/toggle_button.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5527 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/control_element.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    23210 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/control_surface.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    12340 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/decoration.py
+-rw-r--r--   0 sahlen     (501) staff       (20)   244847 2024-01-08 19:05:13.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/default_bank_definitions.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      531 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/defaults.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4579 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/delay_decoration.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1479 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/device_bank_registry.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1564 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/device_chain_utils.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1779 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/device_decorator_factory.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6493 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/device_parameter_bank.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4720 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/device_provider.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2208 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/drift_decoration.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/
+-rw-r--r--   0 sahlen     (501) staff       (20)     2902 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4179 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/button.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3805 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/button_matrix.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4134 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/button_slider.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3399 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/color.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    10979 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/combo.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3025 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/display_data_source.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8383 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/encoder.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      666 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/full_velocity_element.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2261 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/logical_display_segment.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1077 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/optional.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    11781 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/physical_display.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      857 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/playhead_element.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      630 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/proxy_element.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/py.typed
+-rw-r--r--   0 sahlen     (501) staff       (20)      633 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/slider.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2094 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/sysex_element.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1041 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/velocity_levels_element.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2403 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/identifiable_control_surface.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    15040 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/input_control_element.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    12427 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/internal_parameter.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4936 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/layer.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6506 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/message_scheduler.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1683 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/midi.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1831 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/midi_map.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    16494 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/mode.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1924 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/parameter_provider.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5089 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/parameter_slot_description.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3683 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/percussion_instrument_finder.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1176 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/profile.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/py.typed
+-rw-r--r--   0 sahlen     (501) staff       (20)     7737 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/resource.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1215 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/roar_decoration.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1893 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/session_ring_selection_linking.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    14536 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/simpler_decoration.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4010 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/simpler_slice_nudging.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2582 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/skin.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    11861 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/wavetable_decoration.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/ableton/v2/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/
+-rw-r--r--   0 sahlen     (501) staff       (20)      351 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/__init__.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/base/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1791 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/base/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/base/py.typed
+-rw-r--r--   0 sahlen     (501) staff       (20)     1674 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/base/util.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/
+-rw-r--r--   0 sahlen     (501) staff       (20)     4373 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4680 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/banking_util.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      746 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/capabilities.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4179 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/colors.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4762 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/component.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3333 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/component_map.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/
+-rw-r--r--   0 sahlen     (501) staff       (20)     4190 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1359 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/accent.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3465 2024-01-08 19:12:03.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/active_parameter.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3417 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/auto_arm.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3113 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/background.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8425 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/channel_strip.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5020 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/clip_actions.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7637 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/clip_slot.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2417 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/clipboard.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9053 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/device.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5354 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/device_bank_navigation.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2336 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/device_parameters.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    14802 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/drum_group.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2087 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/drum_group_scroll.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2987 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/grid_resolution.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7049 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/loop_selector.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9585 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/mixer.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    17858 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/note_editor.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3459 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/page.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2116 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/paginator.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4144 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/playable.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2733 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/playhead.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/py.typed
+-rw-r--r--   0 sahlen     (501) staff       (20)     6702 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/recording.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4613 2024-01-08 18:43:23.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/scene.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4560 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/scroll.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9303 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/session.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5580 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/session_navigation.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4777 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/session_overview.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6395 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/session_ring.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2104 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/simple_device_navigation.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8492 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/sliced_simpler.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5588 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/step_sequence.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6721 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/target_track.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     9883 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/transport.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1358 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/undo_redo.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     5696 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/view_control.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2748 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/view_toggle.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      582 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/consts.py
+-rw-r--r--   0 sahlen     (501) staff       (20)    14932 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/control_surface.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3959 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/control_surface_mapping.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2384 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/control_surface_specification.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/controls/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1775 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/controls/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2304 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/controls/button.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      662 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/controls/control.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2021 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/controls/control_list.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3614 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/controls/mapped.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/controls/py.typed
+-rw-r--r--   0 sahlen     (501) staff       (20)     1071 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/controls/toggle_button.py
+-rw-r--r--   0 sahlen     (501) staff       (20)   110010 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/default_bank_definitions.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6838 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/default_skin.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2569 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/device_decorators.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/
+-rw-r--r--   0 sahlen     (501) staff       (20)      913 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     4884 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/display_specification.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/event_signal/
+-rw-r--r--   0 sahlen     (501) staff       (20)      507 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/event_signal/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      771 2024-01-08 19:25:27.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/event_signal/core.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/event_signal/py.typed
+-rw-r--r--   0 sahlen     (501) staff       (20)      601 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/event_signal/type_decl.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/notifications/
+-rw-r--r--   0 sahlen     (501) staff       (20)      515 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/notifications/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8662 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/notifications/all.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      552 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/notifications/default.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2117 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/notifications/meta.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/notifications/py.typed
+-rw-r--r--   0 sahlen     (501) staff       (20)     1219 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/notifications/type_decl.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      767 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/notifications/util.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/py.typed
+-rw-r--r--   0 sahlen     (501) staff       (20)     3710 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/renderable.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2339 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/state.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1819 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/text.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      736 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/type_decl.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1433 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/util.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/view/
+-rw-r--r--   0 sahlen     (501) staff       (20)      618 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/view/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3422 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/view/notification.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/view/py.typed
+-rw-r--r--   0 sahlen     (501) staff       (20)      613 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/view/type_decl.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      686 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/view/util.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2799 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/view/view.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/elements/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1573 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/elements/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2709 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/elements/button.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1374 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/elements/button_matrix.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2154 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/elements/color.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1547 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/elements/discrete_values.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2261 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/elements/display_line.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7540 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/elements/encoder.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2216 2024-01-08 18:43:24.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/elements/lockable_button.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      646 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/elements/lockable_combo.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/elements/py.typed
+-rw-r--r--   0 sahlen     (501) staff       (20)     3723 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/elements/sysex.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1493 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/elements/touch.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8328 2024-01-08 19:11:02.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/elements_base.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     6039 2024-01-08 19:05:12.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/identification.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3490 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/instrument_finder.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      675 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/layer.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1160 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/legacy_bank_definitions.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     1030 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/midi.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/mode/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1648 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/mode/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2180 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/mode/behaviour.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2531 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/mode/mode.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     8685 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/mode/modes.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/mode/py.typed
+-rw-r--r--   0 sahlen     (501) staff       (20)     2584 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/mode/selector.py
+-rw-r--r--   0 sahlen     (501) staff       (20)      918 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/parameter_info.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     3521 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/parameter_mapping_sensitivities.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/py.typed
+-rw-r--r--   0 sahlen     (501) staff       (20)     2617 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/session_ring_selection_linking.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     2215 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/skin.py
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/live/
+-rw-r--r--   0 sahlen     (501) staff       (20)     1986 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/live/__init__.py
+-rw-r--r--   0 sahlen     (501) staff       (20)     7661 2024-01-08 18:49:35.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/live/action.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/live/py.typed
+-rw-r--r--   0 sahlen     (501) staff       (20)     8160 2024-05-05 18:23:11.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/live/util.py
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/ableton/v3/py.typed
+drwxr-xr-x   0 sahlen     (501) staff       (20)        0 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/ableton_control_surface_core.egg-info/
+-rw-r--r--   0 sahlen     (501) staff       (20)      677 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/ableton_control_surface_core.egg-info/PKG-INFO
+-rw-r--r--   0 sahlen     (501) staff       (20)    17249 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/ableton_control_surface_core.egg-info/SOURCES.txt
+-rw-r--r--   0 sahlen     (501) staff       (20)        1 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/ableton_control_surface_core.egg-info/dependency_links.txt
+-rw-r--r--   0 sahlen     (501) staff       (20)        0 2024-05-05 19:46:58.000000 ableton-control-surface-core-0.0.5/src/ableton_control_surface_core.egg-info/py.typed
+-rw-r--r--   0 sahlen     (501) staff       (20)       87 2024-05-05 19:48:50.000000 ableton-control-surface-core-0.0.5/src/ableton_control_surface_core.egg-info/top_level.txt
```

### Comparing `ableton-control-surface-core-0.0.4/PKG-INFO` & `ableton-control-surface-core-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ableton-control-surface-core
-Version: 0.0.4
+Version: 0.0.5
 Summary: Decompiled core packages from Ableton Live's Python API to help developers build custom control surfaces.
 Author-email: Martin Sahlen <martin8900@gmail.com>
 Project-URL: Homepage, https://github.com/oslo1989/ableton-control-surface-toolkit
 Project-URL: Issues, https://github.com/oslo1989/ableton-control-surface-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ableton-control-surface-core-0.0.4/pyproject.toml` & `ableton-control-surface-core-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools ~=68.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ableton-control-surface-core"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     {name = "Martin Sahlen", email = "martin8900@gmail.com"}
 ]
 description = "Decompiled core packages from Ableton Live's Python API to help developers build custom control surfaces."
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `ableton-control-surface-core-0.0.4/src/Live/Application/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/Application/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/Base/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/Base/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/Browser/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/Browser/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/CcControlDevice/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/CcControlDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/Chain/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/Chain/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/ChainMixerDevice/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/ChainMixerDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/Clip/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/Clip/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/ClipSlot/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/ClipSlot/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/CompressorDevice/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/CompressorDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/Conversions/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/Conversions/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/Device/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/Device/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/DeviceIO/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/DeviceIO/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/DeviceParameter/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/DeviceParameter/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/DriftDevice/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/DriftDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/DrumChain/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/DrumChain/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/DrumPad/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/DrumPad/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/Eq8Device/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/Eq8Device/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/Groove/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/Groove/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/GroovePool/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/GroovePool/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/HybridReverbDevice/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/HybridReverbDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/Listener/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/Listener/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/LomObject/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/LomObject/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/MaxDevice/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/MaxDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/MeldDevice/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/MeldDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/MidiMap/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/MidiMap/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/MixerDevice/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/MixerDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/PluginDevice/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/PluginDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/RackDevice/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/RackDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/RoarDevice/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/RoarDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/Sample/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/Sample/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/Scene/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/Scene/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/ShifterDevice/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/ShifterDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/SimplerDevice/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/SimplerDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/Song/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/Song/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/SpectralResonatorDevice/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/SpectralResonatorDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/Track/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/Track/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/WavetableDevice/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/WavetableDevice/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/Live/__init__.py` & `ableton-control-surface-core-0.0.5/src/Live/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/MidiRemoteScript/__init__.py` & `ableton-control-surface-core-0.0.5/src/MidiRemoteScript/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/BackgroundComponent.py` & `ableton-control-surface-core-0.0.5/src/_Framework/BackgroundComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/ButtonElement.py` & `ableton-control-surface-core-0.0.5/src/_Framework/ButtonElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/ButtonMatrixElement.py` & `ableton-control-surface-core-0.0.5/src/_Framework/ButtonMatrixElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/ButtonSliderElement.py` & `ableton-control-surface-core-0.0.5/src/_Framework/ButtonSliderElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/Capabilities.py` & `ableton-control-surface-core-0.0.5/src/_Framework/Capabilities.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/ChannelStripComponent.py` & `ableton-control-surface-core-0.0.5/src/_Framework/ChannelStripComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/ChannelTranslationSelector.py` & `ableton-control-surface-core-0.0.5/src/_Framework/ChannelTranslationSelector.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/ClipCreator.py` & `ableton-control-surface-core-0.0.5/src/_Framework/ClipCreator.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/ClipSlotComponent.py` & `ableton-control-surface-core-0.0.5/src/_Framework/ClipSlotComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/ComboElement.py` & `ableton-control-surface-core-0.0.5/src/_Framework/ComboElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/CompoundComponent.py` & `ableton-control-surface-core-0.0.5/src/_Framework/CompoundComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/CompoundElement.py` & `ableton-control-surface-core-0.0.5/src/_Framework/CompoundElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/Control.py` & `ableton-control-surface-core-0.0.5/src/_Framework/Control.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/ControlElement.py` & `ableton-control-surface-core-0.0.5/src/_Framework/ControlElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/ControlSurface.py` & `ableton-control-surface-core-0.0.5/src/_Framework/ControlSurface.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/ControlSurfaceComponent.py` & `ableton-control-surface-core-0.0.5/src/_Framework/ControlSurfaceComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/Dependency.py` & `ableton-control-surface-core-0.0.5/src/_Framework/Dependency.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/DeviceBankRegistry.py` & `ableton-control-surface-core-0.0.5/src/_Framework/DeviceBankRegistry.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/DeviceComponent.py` & `ableton-control-surface-core-0.0.5/src/_Framework/DeviceComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/Disconnectable.py` & `ableton-control-surface-core-0.0.5/src/_Framework/Disconnectable.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/DisplayDataSource.py` & `ableton-control-surface-core-0.0.5/src/_Framework/DisplayDataSource.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/DrumGroupComponent.py` & `ableton-control-surface-core-0.0.5/src/_Framework/DrumGroupComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/DrumRackComponent.py` & `ableton-control-surface-core-0.0.5/src/_Framework/DrumRackComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/EncoderElement.py` & `ableton-control-surface-core-0.0.5/src/_Framework/EncoderElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/IdentifiableControlSurface.py` & `ableton-control-surface-core-0.0.5/src/_Framework/IdentifiableControlSurface.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/InputControlElement.py` & `ableton-control-surface-core-0.0.5/src/_Framework/InputControlElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/Layer.py` & `ableton-control-surface-core-0.0.5/src/_Framework/Layer.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/LogicalDisplaySegment.py` & `ableton-control-surface-core-0.0.5/src/_Framework/LogicalDisplaySegment.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/MessageScheduler.py` & `ableton-control-surface-core-0.0.5/src/_Framework/MessageScheduler.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/MidiMap.py` & `ableton-control-surface-core-0.0.5/src/_Framework/MidiMap.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/MixerComponent.py` & `ableton-control-surface-core-0.0.5/src/_Framework/MixerComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/ModeSelectorComponent.py` & `ableton-control-surface-core-0.0.5/src/_Framework/ModeSelectorComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/ModesComponent.py` & `ableton-control-surface-core-0.0.5/src/_Framework/ModesComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/MomentaryModeObserver.py` & `ableton-control-surface-core-0.0.5/src/_Framework/MomentaryModeObserver.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/NotifyingControlElement.py` & `ableton-control-surface-core-0.0.5/src/_Framework/NotifyingControlElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/OptionalElement.py` & `ableton-control-surface-core-0.0.5/src/_Framework/OptionalElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/PhysicalDisplayElement.py` & `ableton-control-surface-core-0.0.5/src/_Framework/PhysicalDisplayElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/Profile.py` & `ableton-control-surface-core-0.0.5/src/_Framework/Profile.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/Proxy.py` & `ableton-control-surface-core-0.0.5/src/_Framework/Proxy.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/Resource.py` & `ableton-control-surface-core-0.0.5/src/_Framework/Resource.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/SceneComponent.py` & `ableton-control-surface-core-0.0.5/src/_Framework/SceneComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/ScrollComponent.py` & `ableton-control-surface-core-0.0.5/src/_Framework/ScrollComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/SessionComponent.py` & `ableton-control-surface-core-0.0.5/src/_Framework/SessionComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/SessionRecordingComponent.py` & `ableton-control-surface-core-0.0.5/src/_Framework/SessionRecordingComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/SessionZoomingComponent.py` & `ableton-control-surface-core-0.0.5/src/_Framework/SessionZoomingComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/Signal.py` & `ableton-control-surface-core-0.0.5/src/_Framework/Signal.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/Skin.py` & `ableton-control-surface-core-0.0.5/src/_Framework/Skin.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/SlideComponent.py` & `ableton-control-surface-core-0.0.5/src/_Framework/SlideComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/SliderElement.py` & `ableton-control-surface-core-0.0.5/src/_Framework/SliderElement.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/SubjectSlot.py` & `ableton-control-surface-core-0.0.5/src/_Framework/SubjectSlot.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/SysexValueControl.py` & `ableton-control-surface-core-0.0.5/src/_Framework/SysexValueControl.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/Task.py` & `ableton-control-surface-core-0.0.5/src/_Framework/Task.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/ToggleComponent.py` & `ableton-control-surface-core-0.0.5/src/_Framework/ToggleComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/TrackArmState.py` & `ableton-control-surface-core-0.0.5/src/_Framework/TrackArmState.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/TransportComponent.py` & `ableton-control-surface-core-0.0.5/src/_Framework/TransportComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/Util.py` & `ableton-control-surface-core-0.0.5/src/_Framework/Util.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Framework/ViewControlComponent.py` & `ableton-control-surface-core-0.0.5/src/_Framework/ViewControlComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Generic/Devices.py` & `ableton-control-surface-core-0.0.5/src/_Generic/Devices.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Generic/GenericScript.py` & `ableton-control-surface-core-0.0.5/src/_Generic/GenericScript.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Generic/SelectChanStripComponent.py` & `ableton-control-surface-core-0.0.5/src/_Generic/SelectChanStripComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Generic/SpecialMixerComponent.py` & `ableton-control-surface-core-0.0.5/src/_Generic/SpecialMixerComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Generic/util.py` & `ableton-control-surface-core-0.0.5/src/_Generic/util.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_MxDCore/ControlSurfaceWrapper.py` & `ableton-control-surface-core-0.0.5/src/_MxDCore/ControlSurfaceWrapper.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_MxDCore/LomTypes.py` & `ableton-control-surface-core-0.0.5/src/_MxDCore/LomTypes.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_MxDCore/LomUtils.py` & `ableton-control-surface-core-0.0.5/src/_MxDCore/LomUtils.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_MxDCore/MxDControlSurfaceAPI.py` & `ableton-control-surface-core-0.0.5/src/_MxDCore/MxDControlSurfaceAPI.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_MxDCore/MxDCore.py` & `ableton-control-surface-core-0.0.5/src/_MxDCore/MxDCore.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_MxDCore/MxDUtils.py` & `ableton-control-surface-core-0.0.5/src/_MxDCore/MxDUtils.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_MxDCore/NotesAPIUtils.py` & `ableton-control-surface-core-0.0.5/src/_MxDCore/NotesAPIUtils.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_MxDCore/__init__.py` & `ableton-control-surface-core-0.0.5/src/_MxDCore/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Userscript/DeviceComponent.py` & `ableton-control-surface-core-0.0.5/src/_Userscript/DeviceComponent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/_Userscript/__init__.py` & `ableton-control-surface-core-0.0.5/src/_Userscript/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/base/__init__.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/base/abl_signal.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/base/abl_signal.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/base/collection/indexed_dict.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/base/collection/indexed_dict.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/base/dependency.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/base/dependency.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/base/disconnectable.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/base/disconnectable.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/base/event.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/base/event.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/base/gcutil.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/base/gcutil.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/base/isclose.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/base/isclose.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/base/live_api_utils.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/base/live_api_utils.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/base/proxy.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/base/proxy.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/base/task.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/base/task.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/base/util.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/base/util.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/__init__.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/banking_util.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/banking_util.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/capabilities.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/capabilities.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/clip_creator.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/clip_creator.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/component.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/__init__.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/accent.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/accent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/auto_arm.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/auto_arm.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/background.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/background.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/channel_strip.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/channel_strip.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/clip_actions.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/clip_actions.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/clip_slot.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/clip_slot.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/device.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/device.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/device_navigation.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/device_navigation.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/device_parameters.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/device_parameters.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/drum_group.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/drum_group.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/item_lister.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/item_lister.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/mixer.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/mixer.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/playable.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/playable.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/scene.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/scene.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/scroll.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/scroll.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/session.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/session.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/session_navigation.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/session_navigation.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/session_overview.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/session_overview.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/session_recording.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/session_recording.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/session_ring.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/session_ring.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/slide.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/slide.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/target_track.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/target_track.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/toggle.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/toggle.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/transport.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/transport.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/undo_redo.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/undo_redo.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/components/view_control.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/components/view_control.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/compound_element.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/compound_element.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/control/__init__.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/control/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/control/button.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/control/button.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/control/control.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/control/control.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/control/control_list.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/control/control_list.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/control/encoder.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/control/encoder.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/control/mapped.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/control/mapped.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/control/radio_button.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/control/radio_button.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/control/sysex.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/control/sysex.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/control/text_display.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/control/text_display.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/control/toggle_button.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/control/toggle_button.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/control_element.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/control_element.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/control_surface.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/control_surface.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/decoration.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/decoration.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/default_bank_definitions.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/default_bank_definitions.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/defaults.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/defaults.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/delay_decoration.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/delay_decoration.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/device_bank_registry.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/device_bank_registry.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/device_chain_utils.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/device_chain_utils.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/device_decorator_factory.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/device_decorator_factory.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/device_parameter_bank.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/device_parameter_bank.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/device_provider.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/device_provider.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/drift_decoration.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/drift_decoration.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/__init__.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/button.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/button.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/button_matrix.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/button_matrix.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/button_slider.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/button_slider.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/color.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/color.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/combo.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/combo.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/display_data_source.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/display_data_source.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/encoder.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/encoder.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/full_velocity_element.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/full_velocity_element.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/logical_display_segment.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/logical_display_segment.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/optional.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/optional.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/physical_display.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/physical_display.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/playhead_element.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/playhead_element.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/proxy_element.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/proxy_element.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/slider.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/slider.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/sysex_element.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/sysex_element.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/elements/velocity_levels_element.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/elements/velocity_levels_element.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/identifiable_control_surface.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/identifiable_control_surface.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/input_control_element.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/input_control_element.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/internal_parameter.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/internal_parameter.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/layer.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/layer.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/message_scheduler.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/message_scheduler.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/midi.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/midi.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/midi_map.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/midi_map.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/mode.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/mode.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/parameter_provider.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/parameter_provider.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/parameter_slot_description.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/parameter_slot_description.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/percussion_instrument_finder.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/percussion_instrument_finder.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/profile.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/profile.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/resource.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/resource.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/roar_decoration.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/roar_decoration.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/session_ring_selection_linking.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/session_ring_selection_linking.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/simpler_decoration.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/simpler_decoration.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/simpler_slice_nudging.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/simpler_slice_nudging.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/skin.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/skin.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v2/control_surface/wavetable_decoration.py` & `ableton-control-surface-core-0.0.5/src/ableton/v2/control_surface/wavetable_decoration.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/base/__init__.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/base/util.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/base/util.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/__init__.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/banking_util.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/banking_util.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/capabilities.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/capabilities.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/colors.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/colors.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/component.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/component.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/component_map.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/component_map.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/__init__.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/accent.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/accent.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/active_parameter.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/active_parameter.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/auto_arm.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/auto_arm.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/background.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/background.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/channel_strip.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/channel_strip.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/clip_actions.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/clip_actions.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/clip_slot.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/clip_slot.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/clipboard.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/clipboard.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/device.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/device.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/device_bank_navigation.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/device_bank_navigation.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/device_parameters.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/device_parameters.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/drum_group.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/drum_group.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/drum_group_scroll.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/drum_group_scroll.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/grid_resolution.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/grid_resolution.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/loop_selector.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/loop_selector.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/mixer.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/mixer.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/note_editor.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/note_editor.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/page.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/page.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/paginator.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/paginator.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/playable.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/playable.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/playhead.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/playhead.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/recording.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/recording.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/scene.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/scene.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/scroll.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/scroll.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/session.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/session.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/session_navigation.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/session_navigation.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/session_overview.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/session_overview.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/session_ring.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/session_ring.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/simple_device_navigation.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/simple_device_navigation.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/sliced_simpler.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/sliced_simpler.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/step_sequence.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/step_sequence.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/target_track.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/target_track.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/transport.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/transport.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/undo_redo.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/undo_redo.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/view_control.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/view_control.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/components/view_toggle.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/components/view_toggle.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/consts.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/consts.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/control_surface.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/control_surface.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/control_surface_mapping.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/control_surface_mapping.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/control_surface_specification.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/control_surface_specification.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/controls/__init__.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/controls/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/controls/button.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/controls/button.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/controls/control.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/controls/control.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/controls/control_list.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/controls/control_list.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/controls/mapped.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/controls/mapped.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/controls/toggle_button.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/controls/toggle_button.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/default_bank_definitions.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/default_bank_definitions.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/default_skin.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/default_skin.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/device_decorators.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/device_decorators.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/__init__.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/display_specification.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/display_specification.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/event_signal/core.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/event_signal/core.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/event_signal/type_decl.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/event_signal/type_decl.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/notifications/__init__.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/notifications/all.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/notifications/all.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/notifications/default.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/notifications/default.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/notifications/meta.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/notifications/meta.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/notifications/type_decl.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/notifications/type_decl.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/notifications/util.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/notifications/util.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/renderable.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/renderable.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/state.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/state.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/text.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/text.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/type_decl.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/type_decl.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/util.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/util.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/view/__init__.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/view/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/view/notification.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/view/notification.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/view/type_decl.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/view/type_decl.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/view/util.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/view/util.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/display/view/view.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/display/view/view.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/elements/__init__.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/elements/button.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/elements/button.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/elements/button_matrix.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/elements/button_matrix.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/elements/color.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/elements/color.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/elements/discrete_values.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/elements/discrete_values.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/elements/display_line.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/elements/display_line.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/elements/encoder.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/elements/encoder.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/elements/lockable_button.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/elements/lockable_button.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/elements/lockable_combo.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/elements/lockable_combo.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/elements/sysex.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/elements/sysex.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/elements/touch.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/elements/touch.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/elements_base.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/elements_base.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/identification.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/identification.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/instrument_finder.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/instrument_finder.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/layer.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/layer.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/legacy_bank_definitions.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/legacy_bank_definitions.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/midi.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/midi.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/mode/__init__.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/mode/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/mode/behaviour.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/mode/behaviour.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/mode/mode.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/mode/mode.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/mode/modes.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/mode/modes.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/mode/selector.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/mode/selector.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/parameter_info.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/parameter_info.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/parameter_mapping_sensitivities.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/parameter_mapping_sensitivities.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/session_ring_selection_linking.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/session_ring_selection_linking.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/control_surface/skin.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/control_surface/skin.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/live/__init__.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/live/__init__.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/live/action.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/live/action.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton/v3/live/util.py` & `ableton-control-surface-core-0.0.5/src/ableton/v3/live/util.py`

 * *Files identical despite different names*

### Comparing `ableton-control-surface-core-0.0.4/src/ableton_control_surface_core.egg-info/PKG-INFO` & `ableton-control-surface-core-0.0.5/src/ableton_control_surface_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ableton-control-surface-core
-Version: 0.0.4
+Version: 0.0.5
 Summary: Decompiled core packages from Ableton Live's Python API to help developers build custom control surfaces.
 Author-email: Martin Sahlen <martin8900@gmail.com>
 Project-URL: Homepage, https://github.com/oslo1989/ableton-control-surface-toolkit
 Project-URL: Issues, https://github.com/oslo1989/ableton-control-surface-toolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ableton-control-surface-core-0.0.4/src/ableton_control_surface_core.egg-info/SOURCES.txt` & `ableton-control-surface-core-0.0.5/src/ableton_control_surface_core.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,88 @@
 MANIFEST.in
 pyproject.toml
 src/__init__.py
-src/py.typed
 src/Live/__init__.py
+src/Live/py.typed
 src/Live/Application/__init__.py
+src/Live/Application/py.typed
 src/Live/Base/__init__.py
+src/Live/Base/py.typed
 src/Live/Browser/__init__.py
+src/Live/Browser/py.typed
 src/Live/CcControlDevice/__init__.py
+src/Live/CcControlDevice/py.typed
 src/Live/Chain/__init__.py
+src/Live/Chain/py.typed
 src/Live/ChainMixerDevice/__init__.py
+src/Live/ChainMixerDevice/py.typed
 src/Live/Clip/__init__.py
+src/Live/Clip/py.typed
 src/Live/ClipSlot/__init__.py
+src/Live/ClipSlot/py.typed
 src/Live/CompressorDevice/__init__.py
+src/Live/CompressorDevice/py.typed
 src/Live/Conversions/__init__.py
+src/Live/Conversions/py.typed
 src/Live/Device/__init__.py
+src/Live/Device/py.typed
 src/Live/DeviceIO/__init__.py
+src/Live/DeviceIO/py.typed
 src/Live/DeviceParameter/__init__.py
+src/Live/DeviceParameter/py.typed
 src/Live/DriftDevice/__init__.py
+src/Live/DriftDevice/py.typed
 src/Live/DrumChain/__init__.py
+src/Live/DrumChain/py.typed
 src/Live/DrumPad/__init__.py
+src/Live/DrumPad/py.typed
 src/Live/Eq8Device/__init__.py
+src/Live/Eq8Device/py.typed
 src/Live/Groove/__init__.py
+src/Live/Groove/py.typed
 src/Live/GroovePool/__init__.py
+src/Live/GroovePool/py.typed
 src/Live/HybridReverbDevice/__init__.py
+src/Live/HybridReverbDevice/py.typed
 src/Live/Listener/__init__.py
+src/Live/Listener/py.typed
 src/Live/LomObject/__init__.py
+src/Live/LomObject/py.typed
 src/Live/MaxDevice/__init__.py
+src/Live/MaxDevice/py.typed
 src/Live/MeldDevice/__init__.py
+src/Live/MeldDevice/py.typed
 src/Live/MidiMap/__init__.py
+src/Live/MidiMap/py.typed
 src/Live/MixerDevice/__init__.py
+src/Live/MixerDevice/py.typed
 src/Live/PluginDevice/__init__.py
+src/Live/PluginDevice/py.typed
 src/Live/RackDevice/__init__.py
+src/Live/RackDevice/py.typed
 src/Live/RoarDevice/__init__.py
+src/Live/RoarDevice/py.typed
 src/Live/Sample/__init__.py
+src/Live/Sample/py.typed
 src/Live/Scene/__init__.py
+src/Live/Scene/py.typed
 src/Live/ShifterDevice/__init__.py
+src/Live/ShifterDevice/py.typed
 src/Live/SimplerDevice/__init__.py
+src/Live/SimplerDevice/py.typed
 src/Live/Song/__init__.py
+src/Live/Song/py.typed
 src/Live/SpectralResonatorDevice/__init__.py
+src/Live/SpectralResonatorDevice/py.typed
 src/Live/Track/__init__.py
+src/Live/Track/py.typed
 src/Live/WavetableDevice/__init__.py
+src/Live/WavetableDevice/py.typed
 src/MidiRemoteScript/__init__.py
+src/MidiRemoteScript/py.typed
 src/_Framework/BackgroundComponent.py
 src/_Framework/ButtonElement.py
 src/_Framework/ButtonMatrixElement.py
 src/_Framework/ButtonSliderElement.py
 src/_Framework/Capabilities.py
 src/_Framework/ChannelStripComponent.py
 src/_Framework/ChannelTranslationSelector.py
@@ -96,46 +134,55 @@
 src/_Framework/Task.py
 src/_Framework/ToggleComponent.py
 src/_Framework/TrackArmState.py
 src/_Framework/TransportComponent.py
 src/_Framework/Util.py
 src/_Framework/ViewControlComponent.py
 src/_Framework/__init__.py
+src/_Framework/py.typed
 src/_Generic/Devices.py
 src/_Generic/GenericScript.py
 src/_Generic/SelectChanStripComponent.py
 src/_Generic/SpecialMixerComponent.py
 src/_Generic/__init__.py
+src/_Generic/py.typed
 src/_Generic/util.py
 src/_MxDCore/ControlSurfaceWrapper.py
 src/_MxDCore/LomTypes.py
 src/_MxDCore/LomUtils.py
 src/_MxDCore/MxDControlSurfaceAPI.py
 src/_MxDCore/MxDCore.py
 src/_MxDCore/MxDUtils.py
 src/_MxDCore/NotesAPIUtils.py
 src/_MxDCore/__init__.py
+src/_MxDCore/py.typed
 src/_Tools/__init__.py
+src/_Tools/py.typed
 src/_Userscript/DeviceComponent.py
 src/_Userscript/__init__.py
+src/_Userscript/py.typed
 src/ableton/__init__.py
+src/ableton/py.typed
 src/ableton/v2/__init__.py
+src/ableton/v2/py.typed
 src/ableton/v2/base/__init__.py
 src/ableton/v2/base/abl_signal.py
 src/ableton/v2/base/dependency.py
 src/ableton/v2/base/disconnectable.py
 src/ableton/v2/base/event.py
 src/ableton/v2/base/gcutil.py
 src/ableton/v2/base/isclose.py
 src/ableton/v2/base/live_api_utils.py
 src/ableton/v2/base/proxy.py
+src/ableton/v2/base/py.typed
 src/ableton/v2/base/task.py
 src/ableton/v2/base/util.py
 src/ableton/v2/base/collection/__init__.py
 src/ableton/v2/base/collection/indexed_dict.py
+src/ableton/v2/base/collection/py.typed
 src/ableton/v2/control_surface/__init__.py
 src/ableton/v2/control_surface/banking_util.py
 src/ableton/v2/control_surface/capabilities.py
 src/ableton/v2/control_surface/clip_creator.py
 src/ableton/v2/control_surface/component.py
 src/ableton/v2/control_surface/compound_element.py
 src/ableton/v2/control_surface/control_element.py
@@ -158,14 +205,15 @@
 src/ableton/v2/control_surface/midi.py
 src/ableton/v2/control_surface/midi_map.py
 src/ableton/v2/control_surface/mode.py
 src/ableton/v2/control_surface/parameter_provider.py
 src/ableton/v2/control_surface/parameter_slot_description.py
 src/ableton/v2/control_surface/percussion_instrument_finder.py
 src/ableton/v2/control_surface/profile.py
+src/ableton/v2/control_surface/py.typed
 src/ableton/v2/control_surface/resource.py
 src/ableton/v2/control_surface/roar_decoration.py
 src/ableton/v2/control_surface/session_ring_selection_linking.py
 src/ableton/v2/control_surface/simpler_decoration.py
 src/ableton/v2/control_surface/simpler_slice_nudging.py
 src/ableton/v2/control_surface/skin.py
 src/ableton/v2/control_surface/wavetable_decoration.py
@@ -179,14 +227,15 @@
 src/ableton/v2/control_surface/components/device.py
 src/ableton/v2/control_surface/components/device_navigation.py
 src/ableton/v2/control_surface/components/device_parameters.py
 src/ableton/v2/control_surface/components/drum_group.py
 src/ableton/v2/control_surface/components/item_lister.py
 src/ableton/v2/control_surface/components/mixer.py
 src/ableton/v2/control_surface/components/playable.py
+src/ableton/v2/control_surface/components/py.typed
 src/ableton/v2/control_surface/components/scene.py
 src/ableton/v2/control_surface/components/scroll.py
 src/ableton/v2/control_surface/components/session.py
 src/ableton/v2/control_surface/components/session_navigation.py
 src/ableton/v2/control_surface/components/session_overview.py
 src/ableton/v2/control_surface/components/session_recording.py
 src/ableton/v2/control_surface/components/session_ring.py
@@ -198,14 +247,15 @@
 src/ableton/v2/control_surface/components/view_control.py
 src/ableton/v2/control_surface/control/__init__.py
 src/ableton/v2/control_surface/control/button.py
 src/ableton/v2/control_surface/control/control.py
 src/ableton/v2/control_surface/control/control_list.py
 src/ableton/v2/control_surface/control/encoder.py
 src/ableton/v2/control_surface/control/mapped.py
+src/ableton/v2/control_surface/control/py.typed
 src/ableton/v2/control_surface/control/radio_button.py
 src/ableton/v2/control_surface/control/sysex.py
 src/ableton/v2/control_surface/control/text_display.py
 src/ableton/v2/control_surface/control/toggle_button.py
 src/ableton/v2/control_surface/elements/__init__.py
 src/ableton/v2/control_surface/elements/button.py
 src/ableton/v2/control_surface/elements/button_matrix.py
@@ -216,19 +266,22 @@
 src/ableton/v2/control_surface/elements/encoder.py
 src/ableton/v2/control_surface/elements/full_velocity_element.py
 src/ableton/v2/control_surface/elements/logical_display_segment.py
 src/ableton/v2/control_surface/elements/optional.py
 src/ableton/v2/control_surface/elements/physical_display.py
 src/ableton/v2/control_surface/elements/playhead_element.py
 src/ableton/v2/control_surface/elements/proxy_element.py
+src/ableton/v2/control_surface/elements/py.typed
 src/ableton/v2/control_surface/elements/slider.py
 src/ableton/v2/control_surface/elements/sysex_element.py
 src/ableton/v2/control_surface/elements/velocity_levels_element.py
 src/ableton/v3/__init__.py
+src/ableton/v3/py.typed
 src/ableton/v3/base/__init__.py
+src/ableton/v3/base/py.typed
 src/ableton/v3/base/util.py
 src/ableton/v3/control_surface/__init__.py
 src/ableton/v3/control_surface/banking_util.py
 src/ableton/v3/control_surface/capabilities.py
 src/ableton/v3/control_surface/colors.py
 src/ableton/v3/control_surface/component.py
 src/ableton/v3/control_surface/component_map.py
@@ -243,14 +296,15 @@
 src/ableton/v3/control_surface/identification.py
 src/ableton/v3/control_surface/instrument_finder.py
 src/ableton/v3/control_surface/layer.py
 src/ableton/v3/control_surface/legacy_bank_definitions.py
 src/ableton/v3/control_surface/midi.py
 src/ableton/v3/control_surface/parameter_info.py
 src/ableton/v3/control_surface/parameter_mapping_sensitivities.py
+src/ableton/v3/control_surface/py.typed
 src/ableton/v3/control_surface/session_ring_selection_linking.py
 src/ableton/v3/control_surface/skin.py
 src/ableton/v3/control_surface/components/__init__.py
 src/ableton/v3/control_surface/components/accent.py
 src/ableton/v3/control_surface/components/active_parameter.py
 src/ableton/v3/control_surface/components/auto_arm.py
 src/ableton/v3/control_surface/components/background.py
@@ -267,14 +321,15 @@
 src/ableton/v3/control_surface/components/loop_selector.py
 src/ableton/v3/control_surface/components/mixer.py
 src/ableton/v3/control_surface/components/note_editor.py
 src/ableton/v3/control_surface/components/page.py
 src/ableton/v3/control_surface/components/paginator.py
 src/ableton/v3/control_surface/components/playable.py
 src/ableton/v3/control_surface/components/playhead.py
+src/ableton/v3/control_surface/components/py.typed
 src/ableton/v3/control_surface/components/recording.py
 src/ableton/v3/control_surface/components/scene.py
 src/ableton/v3/control_surface/components/scroll.py
 src/ableton/v3/control_surface/components/session.py
 src/ableton/v3/control_surface/components/session_navigation.py
 src/ableton/v3/control_surface/components/session_overview.py
 src/ableton/v3/control_surface/components/session_ring.py
@@ -287,52 +342,61 @@
 src/ableton/v3/control_surface/components/view_control.py
 src/ableton/v3/control_surface/components/view_toggle.py
 src/ableton/v3/control_surface/controls/__init__.py
 src/ableton/v3/control_surface/controls/button.py
 src/ableton/v3/control_surface/controls/control.py
 src/ableton/v3/control_surface/controls/control_list.py
 src/ableton/v3/control_surface/controls/mapped.py
+src/ableton/v3/control_surface/controls/py.typed
 src/ableton/v3/control_surface/controls/toggle_button.py
 src/ableton/v3/control_surface/display/__init__.py
 src/ableton/v3/control_surface/display/display_specification.py
+src/ableton/v3/control_surface/display/py.typed
 src/ableton/v3/control_surface/display/renderable.py
 src/ableton/v3/control_surface/display/state.py
 src/ableton/v3/control_surface/display/text.py
 src/ableton/v3/control_surface/display/type_decl.py
 src/ableton/v3/control_surface/display/util.py
 src/ableton/v3/control_surface/display/event_signal/__init__.py
 src/ableton/v3/control_surface/display/event_signal/core.py
+src/ableton/v3/control_surface/display/event_signal/py.typed
 src/ableton/v3/control_surface/display/event_signal/type_decl.py
 src/ableton/v3/control_surface/display/notifications/__init__.py
 src/ableton/v3/control_surface/display/notifications/all.py
 src/ableton/v3/control_surface/display/notifications/default.py
 src/ableton/v3/control_surface/display/notifications/meta.py
+src/ableton/v3/control_surface/display/notifications/py.typed
 src/ableton/v3/control_surface/display/notifications/type_decl.py
 src/ableton/v3/control_surface/display/notifications/util.py
 src/ableton/v3/control_surface/display/view/__init__.py
 src/ableton/v3/control_surface/display/view/notification.py
+src/ableton/v3/control_surface/display/view/py.typed
 src/ableton/v3/control_surface/display/view/type_decl.py
 src/ableton/v3/control_surface/display/view/util.py
 src/ableton/v3/control_surface/display/view/view.py
 src/ableton/v3/control_surface/elements/__init__.py
 src/ableton/v3/control_surface/elements/button.py
 src/ableton/v3/control_surface/elements/button_matrix.py
 src/ableton/v3/control_surface/elements/color.py
 src/ableton/v3/control_surface/elements/discrete_values.py
 src/ableton/v3/control_surface/elements/display_line.py
 src/ableton/v3/control_surface/elements/encoder.py
 src/ableton/v3/control_surface/elements/lockable_button.py
 src/ableton/v3/control_surface/elements/lockable_combo.py
+src/ableton/v3/control_surface/elements/py.typed
 src/ableton/v3/control_surface/elements/sysex.py
 src/ableton/v3/control_surface/elements/touch.py
 src/ableton/v3/control_surface/mode/__init__.py
 src/ableton/v3/control_surface/mode/behaviour.py
 src/ableton/v3/control_surface/mode/mode.py
 src/ableton/v3/control_surface/mode/modes.py
+src/ableton/v3/control_surface/mode/py.typed
 src/ableton/v3/control_surface/mode/selector.py
 src/ableton/v3/live/__init__.py
 src/ableton/v3/live/action.py
+src/ableton/v3/live/py.typed
 src/ableton/v3/live/util.py
 src/ableton_control_surface_core.egg-info/PKG-INFO
 src/ableton_control_surface_core.egg-info/SOURCES.txt
 src/ableton_control_surface_core.egg-info/dependency_links.txt
+src/ableton_control_surface_core.egg-info/py.typed
 src/ableton_control_surface_core.egg-info/top_level.txt
```

