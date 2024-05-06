# Comparing `tmp/tm_devices-1.4.0.tar.gz` & `tmp/tm_devices-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tm_devices-1.4.0.tar", max compression
+gzip compressed data, was "tm_devices-1.4.1.tar", max compression
```

## Comparing `tm_devices-1.4.0.tar` & `tm_devices-1.4.1.tar`

### file list

```diff
@@ -1,903 +1,903 @@
--rw-r--r--   0        0        0    10262 2024-05-03 19:10:04.445310 tm_devices-1.4.0/LICENSE.md
--rw-r--r--   0        0        0    18641 2024-05-03 19:10:04.445310 tm_devices-1.4.0/README.md
--rw-r--r--   0        0        0    15316 2024-05-03 19:10:04.453310 tm_devices-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      858 2024-05-03 19:10:04.453310 tm_devices-1.4.0/src/tm_devices/__init__.py
--rw-r--r--   0        0        0    10643 2024-05-03 19:10:04.453310 tm_devices-1.4.0/src/tm_devices/commands/__init__.py
--rw-r--r--   0        0        0    35404 2024-05-03 19:10:04.453310 tm_devices-1.4.0/src/tm_devices/commands/afg3k_commands.py
--rw-r--r--   0        0        0    35423 2024-05-03 19:10:04.453310 tm_devices-1.4.0/src/tm_devices/commands/afg3kb_commands.py
--rw-r--r--   0        0        0    35423 2024-05-03 19:10:04.453310 tm_devices-1.4.0/src/tm_devices/commands/afg3kc_commands.py
--rw-r--r--   0        0        0    40196 2024-05-03 19:10:04.453310 tm_devices-1.4.0/src/tm_devices/commands/awg5200_commands.py
--rw-r--r--   0        0        0    31702 2024-05-03 19:10:04.453310 tm_devices-1.4.0/src/tm_devices/commands/awg5k_commands.py
--rw-r--r--   0        0        0    31721 2024-05-03 19:10:04.453310 tm_devices-1.4.0/src/tm_devices/commands/awg5kc_commands.py
--rw-r--r--   0        0        0    40082 2024-05-03 19:10:04.453310 tm_devices-1.4.0/src/tm_devices/commands/awg70ka_commands.py
--rw-r--r--   0        0        0    40082 2024-05-03 19:10:04.453310 tm_devices-1.4.0/src/tm_devices/commands/awg70kb_commands.py
--rw-r--r--   0        0        0    31702 2024-05-03 19:10:04.453310 tm_devices-1.4.0/src/tm_devices/commands/awg7k_commands.py
--rw-r--r--   0        0        0    31721 2024-05-03 19:10:04.453310 tm_devices-1.4.0/src/tm_devices/commands/awg7kc_commands.py
--rw-r--r--   0        0        0   110433 2024-05-03 19:10:04.453310 tm_devices-1.4.0/src/tm_devices/commands/daq6510_commands.py
--rw-r--r--   0        0        0    72918 2024-05-03 19:10:04.453310 tm_devices-1.4.0/src/tm_devices/commands/dmm6500_commands.py
--rw-r--r--   0        0        0    70438 2024-05-03 19:10:04.453310 tm_devices-1.4.0/src/tm_devices/commands/dmm7510_commands.py
--rw-r--r--   0        0        0   105183 2024-05-03 19:10:04.453310 tm_devices-1.4.0/src/tm_devices/commands/dpo2k_commands.py
--rw-r--r--   0        0        0   105202 2024-05-03 19:10:04.453310 tm_devices-1.4.0/src/tm_devices/commands/dpo2kb_commands.py
--rw-r--r--   0        0        0   130739 2024-05-03 19:10:04.457310 tm_devices-1.4.0/src/tm_devices/commands/dpo4k_commands.py
--rw-r--r--   0        0        0   131028 2024-05-03 19:10:04.457310 tm_devices-1.4.0/src/tm_devices/commands/dpo4kb_commands.py
--rw-r--r--   0        0        0   154860 2024-05-03 19:10:04.457310 tm_devices-1.4.0/src/tm_devices/commands/dpo5k_commands.py
--rw-r--r--   0        0        0   159820 2024-05-03 19:10:04.457310 tm_devices-1.4.0/src/tm_devices/commands/dpo5kb_commands.py
--rw-r--r--   0        0        0   159061 2024-05-03 19:10:04.457310 tm_devices-1.4.0/src/tm_devices/commands/dpo70kc_commands.py
--rw-r--r--   0        0        0   159061 2024-05-03 19:10:04.457310 tm_devices-1.4.0/src/tm_devices/commands/dpo70kd_commands.py
--rw-r--r--   0        0        0   159080 2024-05-03 19:10:04.457310 tm_devices-1.4.0/src/tm_devices/commands/dpo70kdx_commands.py
--rw-r--r--   0        0        0   163875 2024-05-03 19:10:04.457310 tm_devices-1.4.0/src/tm_devices/commands/dpo70ksx_commands.py
--rw-r--r--   0        0        0   154860 2024-05-03 19:10:04.457310 tm_devices-1.4.0/src/tm_devices/commands/dpo7k_commands.py
--rw-r--r--   0        0        0   159062 2024-05-03 19:10:04.457310 tm_devices-1.4.0/src/tm_devices/commands/dpo7kc_commands.py
--rw-r--r--   0        0        0   159061 2024-05-03 19:10:04.457310 tm_devices-1.4.0/src/tm_devices/commands/dsa70kc_commands.py
--rw-r--r--   0        0        0   159061 2024-05-03 19:10:04.457310 tm_devices-1.4.0/src/tm_devices/commands/dsa70kd_commands.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.457310 tm_devices-1.4.0/src/tm_devices/commands/gen_163n04_mdo/__init__.py
--rw-r--r--   0        0        0   904180 2024-05-03 19:10:04.465310 tm_devices-1.4.0/src/tm_devices/commands/gen_163n04_mdo/search.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.465310 tm_devices-1.4.0/src/tm_devices/commands/gen_16x4xq_mdo/__init__.py
--rw-r--r--   0        0        0   797746 2024-05-03 19:10:04.469310 tm_devices-1.4.0/src/tm_devices/commands/gen_16x4xq_mdo/search.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.469310 tm_devices-1.4.0/src/tm_devices/commands/gen_1jzp7o_mdodpo/__init__.py
--rw-r--r--   0        0        0   738804 2024-05-03 19:10:04.469310 tm_devices-1.4.0/src/tm_devices/commands/gen_1jzp7o_mdodpo/trigger.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.469310 tm_devices-1.4.0/src/tm_devices/commands/gen_1kdqwg_mdo/__init__.py
--rw-r--r--   0        0        0   916756 2024-05-03 19:10:04.469310 tm_devices-1.4.0/src/tm_devices/commands/gen_1kdqwg_mdo/search.py
--rw-r--r--   0        0        0   832335 2024-05-03 19:10:04.473310 tm_devices-1.4.0/src/tm_devices/commands/gen_1kdqwg_mdo/trigger.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.473310 tm_devices-1.4.0/src/tm_devices/commands/gen_1kjd62_mdo/__init__.py
--rw-r--r--   0        0        0   203791 2024-05-03 19:10:04.473310 tm_devices-1.4.0/src/tm_devices/commands/gen_1kjd62_mdo/rf.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.473310 tm_devices-1.4.0/src/tm_devices/commands/gen_1kozfv_dpo/__init__.py
--rw-r--r--   0        0        0   759094 2024-05-03 19:10:04.473310 tm_devices-1.4.0/src/tm_devices/commands/gen_1kozfv_dpo/search.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.473310 tm_devices-1.4.0/src/tm_devices/commands/gen_1l4fot_mdomso/__init__.py
--rw-r--r--   0        0        0    82893 2024-05-03 19:10:04.477310 tm_devices-1.4.0/src/tm_devices/commands/gen_1l4fot_mdomso/cursor.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.477310 tm_devices-1.4.0/src/tm_devices/commands/gen_1la1ym_msomdodpo/__init__.py
--rw-r--r--   0        0        0   821454 2024-05-03 19:10:04.477310 tm_devices-1.4.0/src/tm_devices/commands/gen_1la1ym_msomdodpo/trigger.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.477310 tm_devices-1.4.0/src/tm_devices/commands/gen_1lcv3a_msodpomdo/__init__.py
--rw-r--r--   0        0        0    10809 2024-05-03 19:10:04.477310 tm_devices-1.4.0/src/tm_devices/commands/gen_1lcv3a_msodpomdo/message.py
--rw-r--r--   0        0        0     5278 2024-05-03 19:10:04.477310 tm_devices-1.4.0/src/tm_devices/commands/gen_1lcv3a_msodpomdo/setup_1.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.477310 tm_devices-1.4.0/src/tm_devices/commands/gen_1lh2st_msodpo/__init__.py
--rw-r--r--   0        0        0   865545 2024-05-03 19:10:04.477310 tm_devices-1.4.0/src/tm_devices/commands/gen_1lh2st_msodpo/search.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.477310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/__init__.py
--rw-r--r--   0        0        0    45151 2024-05-03 19:10:04.477310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/actonevent.py
--rw-r--r--   0        0        0    69457 2024-05-03 19:10:04.477310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/afg.py
--rw-r--r--   0        0        0     9715 2024-05-03 19:10:04.477310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/alias.py
--rw-r--r--   0        0        0    13357 2024-05-03 19:10:04.477310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/application.py
--rw-r--r--   0        0        0     3625 2024-05-03 19:10:04.477310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/autoset.py
--rw-r--r--   0        0        0    26008 2024-05-03 19:10:04.477310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/auxin.py
--rw-r--r--   0        0        0     3780 2024-05-03 19:10:04.477310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/auxout.py
--rw-r--r--   0        0        0   319685 2024-05-03 19:10:04.481310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/bus.py
--rw-r--r--   0        0        0    41940 2024-05-03 19:10:04.481310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/calibrate.py
--rw-r--r--   0        0        0    74577 2024-05-03 19:10:04.481310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/ch.py
--rw-r--r--   0        0        0     7842 2024-05-03 19:10:04.481310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/d.py
--rw-r--r--   0        0        0    27302 2024-05-03 19:10:04.481310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/data.py
--rw-r--r--   0        0        0    18170 2024-05-03 19:10:04.481310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/diag.py
--rw-r--r--   0        0        0    22847 2024-05-03 19:10:04.481310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/dvm.py
--rw-r--r--   0        0        0    14675 2024-05-03 19:10:04.481310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/email.py
--rw-r--r--   0        0        0    42390 2024-05-03 19:10:04.481310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/ethernet.py
--rw-r--r--   0        0        0    33557 2024-05-03 19:10:04.481310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/filesystem.py
--rw-r--r--   0        0        0    10959 2024-05-03 19:10:04.481310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/fpanel.py
--rw-r--r--   0        0        0     3733 2024-05-03 19:10:04.481310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/gpibusb.py
--rw-r--r--   0        0        0    20948 2024-05-03 19:10:04.481310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/hardcopy.py
--rw-r--r--   0        0        0    24507 2024-05-03 19:10:04.481310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/histogram.py
--rw-r--r--   0        0        0    26671 2024-05-03 19:10:04.481310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/horizontal.py
--rw-r--r--   0        0        0    28374 2024-05-03 19:10:04.481310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/mark.py
--rw-r--r--   0        0        0    43937 2024-05-03 19:10:04.481310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/marker.py
--rw-r--r--   0        0        0    39214 2024-05-03 19:10:04.481310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/math1.py
--rw-r--r--   0        0        0    20522 2024-05-03 19:10:04.481310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/pictbridge.py
--rw-r--r--   0        0        0   348440 2024-05-03 19:10:04.485310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/power.py
--rw-r--r--   0        0        0     1021 2024-05-03 19:10:04.485310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/reboot.py
--rw-r--r--   0        0        0    19812 2024-05-03 19:10:04.485310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/ref.py
--rw-r--r--   0        0        0    37418 2024-05-03 19:10:04.485310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/save.py
--rw-r--r--   0        0        0     7694 2024-05-03 19:10:04.485310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/socketserver.py
--rw-r--r--   0        0        0     1501 2024-05-03 19:10:04.485310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/time.py
--rw-r--r--   0        0        0    32867 2024-05-03 19:10:04.485310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/vidpic.py
--rw-r--r--   0        0        0    54903 2024-05-03 19:10:04.485310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/wfminpre.py
--rw-r--r--   0        0        0    45499 2024-05-03 19:10:04.485310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/wfmoutpre.py
--rw-r--r--   0        0        0    20895 2024-05-03 19:10:04.485310 tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/zoom.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.485310 tm_devices-1.4.0/src/tm_devices/commands/gen_1lwj1r_msomdodpo/__init__.py
--rw-r--r--   0        0        0     4839 2024-05-03 19:10:04.485310 tm_devices-1.4.0/src/tm_devices/commands/gen_1lwj1r_msomdodpo/rosc.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.485310 tm_devices-1.4.0/src/tm_devices/commands/gen_1lxxm9_msomdodpo/__init__.py
--rw-r--r--   0        0        0    77140 2024-05-03 19:10:04.485310 tm_devices-1.4.0/src/tm_devices/commands/gen_1lxxm9_msomdodpo/cursor.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.485310 tm_devices-1.4.0/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/__init__.py
--rw-r--r--   0        0        0    29207 2024-05-03 19:10:04.485310 tm_devices-1.4.0/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/acquire.py
--rw-r--r--   0        0        0    84211 2024-05-03 19:10:04.485310 tm_devices-1.4.0/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/configuration.py
--rw-r--r--   0        0        0     3065 2024-05-03 19:10:04.489310 tm_devices-1.4.0/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/deskew.py
--rw-r--r--   0        0        0    44570 2024-05-03 19:10:04.489310 tm_devices-1.4.0/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/display.py
--rw-r--r--   0        0        0   148268 2024-05-03 19:10:04.489310 tm_devices-1.4.0/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/mask.py
--rw-r--r--   0        0        0   194267 2024-05-03 19:10:04.489310 tm_devices-1.4.0/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/measurement.py
--rw-r--r--   0        0        0    10398 2024-05-03 19:10:04.489310 tm_devices-1.4.0/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/recall.py
--rw-r--r--   0        0        0    38664 2024-05-03 19:10:04.489310 tm_devices-1.4.0/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/select.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.489310 tm_devices-1.4.0/src/tm_devices/commands/gen_1mq0z9_msodpo/__init__.py
--rw-r--r--   0        0        0   182231 2024-05-03 19:10:04.489310 tm_devices-1.4.0/src/tm_devices/commands/gen_1mq0z9_msodpo/rf.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.489310 tm_devices-1.4.0/src/tm_devices/commands/gen_1nmc1o_msodpomdo/__init__.py
--rw-r--r--   0        0        0     1040 2024-05-03 19:10:04.489310 tm_devices-1.4.0/src/tm_devices/commands/gen_1nmc1o_msodpomdo/clearmenu.py
--rw-r--r--   0        0        0     4740 2024-05-03 19:10:04.489310 tm_devices-1.4.0/src/tm_devices/commands/gen_1nmc1o_msodpomdo/errlog.py
--rw-r--r--   0        0        0     1892 2024-05-03 19:10:04.489310 tm_devices-1.4.0/src/tm_devices/commands/gen_1nmc1o_msodpomdo/header.py
--rw-r--r--   0        0        0     1694 2024-05-03 19:10:04.489310 tm_devices-1.4.0/src/tm_devices/commands/gen_1nmc1o_msodpomdo/language.py
--rw-r--r--   0        0        0     2138 2024-05-03 19:10:04.489310 tm_devices-1.4.0/src/tm_devices/commands/gen_1nmc1o_msodpomdo/status_and_error.py
--rw-r--r--   0        0        0     3152 2024-05-03 19:10:04.489310 tm_devices-1.4.0/src/tm_devices/commands/gen_1nmc1o_msodpomdo/usbdevice.py
--rw-r--r--   0        0        0    12816 2024-05-03 19:10:04.489310 tm_devices-1.4.0/src/tm_devices/commands/gen_1nmc1o_msodpomdo/usbtmc.py
--rw-r--r--   0        0        0     1492 2024-05-03 19:10:04.489310 tm_devices-1.4.0/src/tm_devices/commands/gen_1nmc1o_msodpomdo/verbose.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.489310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/__init__.py
--rw-r--r--   0        0        0    24124 2024-05-03 19:10:04.489310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/acquire.py
--rw-r--r--   0        0        0   130490 2024-05-03 19:10:04.489310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/actonevent.py
--rw-r--r--   0        0        0     5035 2024-05-03 19:10:04.489310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/auxout.py
--rw-r--r--   0        0        0    11020 2024-05-03 19:10:04.489310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/battery.py
--rw-r--r--   0        0        0   243616 2024-05-03 19:10:04.493310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/bus.py
--rw-r--r--   0        0        0    36323 2024-05-03 19:10:04.493310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/callouts.py
--rw-r--r--   0        0        0    63363 2024-05-03 19:10:04.493310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/ch.py
--rw-r--r--   0        0        0    29416 2024-05-03 19:10:04.493310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/data.py
--rw-r--r--   0        0        0    26913 2024-05-03 19:10:04.493310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/dch.py
--rw-r--r--   0        0        0    16876 2024-05-03 19:10:04.493310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/diag.py
--rw-r--r--   0        0        0   580922 2024-05-03 19:10:04.493310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/display.py
--rw-r--r--   0        0        0     7079 2024-05-03 19:10:04.497310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/fpanel.py
--rw-r--r--   0        0        0    44079 2024-05-03 19:10:04.497310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/horizontal.py
--rw-r--r--   0        0        0     3165 2024-05-03 19:10:04.497310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/lic.py
--rw-r--r--   0        0        0    14641 2024-05-03 19:10:04.497310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/license.py
--rw-r--r--   0        0        0    41868 2024-05-03 19:10:04.497310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/mask.py
--rw-r--r--   0        0        0    89876 2024-05-03 19:10:04.497310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/math.py
--rw-r--r--   0        0        0   555657 2024-05-03 19:10:04.497310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/measurement.py
--rw-r--r--   0        0        0    28636 2024-05-03 19:10:04.497310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/pg.py
--rw-r--r--   0        0        0     9116 2024-05-03 19:10:04.497310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/plot.py
--rw-r--r--   0        0        0    62601 2024-05-03 19:10:04.497310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/power.py
--rw-r--r--   0        0        0    32565 2024-05-03 19:10:04.497310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/ref.py
--rw-r--r--   0        0        0    37873 2024-05-03 19:10:04.497310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/save.py
--rw-r--r--   0        0        0    23156 2024-05-03 19:10:04.497310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/saveon.py
--rw-r--r--   0        0        0    16637 2024-05-03 19:10:04.497310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/saveonevent.py
--rw-r--r--   0        0        0   419529 2024-05-03 19:10:04.501310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/search.py
--rw-r--r--   0        0        0     7641 2024-05-03 19:10:04.501310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/select.py
--rw-r--r--   0        0        0     3357 2024-05-03 19:10:04.501310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/touchscreen.py
--rw-r--r--   0        0        0   319248 2024-05-03 19:10:04.501310 tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/trigger.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.501310 tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/__init__.py
--rw-r--r--   0        0        0     2192 2024-05-03 19:10:04.501310 tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/afgcontrol.py
--rw-r--r--   0        0        0    21587 2024-05-03 19:10:04.501310 tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/data.py
--rw-r--r--   0        0        0     2627 2024-05-03 19:10:04.501310 tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/diagnostic.py
--rw-r--r--   0        0        0    14155 2024-05-03 19:10:04.501310 tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/display.py
--rw-r--r--   0        0        0     3447 2024-05-03 19:10:04.501310 tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/hcopy.py
--rw-r--r--   0        0        0    11509 2024-05-03 19:10:04.501310 tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/memory.py
--rw-r--r--   0        0        0    17547 2024-05-03 19:10:04.501310 tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/mmemory.py
--rw-r--r--   0        0        0     4782 2024-05-03 19:10:04.501310 tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/output.py
--rw-r--r--   0        0        0     7071 2024-05-03 19:10:04.501310 tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/output1.py
--rw-r--r--   0        0        0     7071 2024-05-03 19:10:04.501310 tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/output2.py
--rw-r--r--   0        0        0     3963 2024-05-03 19:10:04.501310 tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/source.py
--rw-r--r--   0        0        0   190576 2024-05-03 19:10:04.501310 tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/source1.py
--rw-r--r--   0        0        0   190576 2024-05-03 19:10:04.501310 tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/source2.py
--rw-r--r--   0        0        0     7600 2024-05-03 19:10:04.501310 tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/source3.py
--rw-r--r--   0        0        0     7600 2024-05-03 19:10:04.501310 tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/source4.py
--rw-r--r--   0        0        0    17014 2024-05-03 19:10:04.501310 tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/status.py
--rw-r--r--   0        0        0    26993 2024-05-03 19:10:04.501310 tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/system.py
--rw-r--r--   0        0        0     9281 2024-05-03 19:10:04.501310 tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/trigger.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.501310 tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/__init__.py
--rw-r--r--   0        0        0     1043 2024-05-03 19:10:04.501310 tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/abort.py
--rw-r--r--   0        0        0     4919 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/auxoutput.py
--rw-r--r--   0        0        0    34829 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/awgcontrol.py
--rw-r--r--   0        0        0    28178 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/bwaveform.py
--rw-r--r--   0        0        0    38773 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/clock.py
--rw-r--r--   0        0        0    42644 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/cplayback.py
--rw-r--r--   0        0        0    28829 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/fgen.py
--rw-r--r--   0        0        0     6748 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/instrument.py
--rw-r--r--   0        0        0    49454 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/mmemory.py
--rw-r--r--   0        0        0    23340 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/output.py
--rw-r--r--   0        0        0    83750 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/source.py
--rw-r--r--   0        0        0     4606 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/synchronize.py
--rw-r--r--   0        0        0    16556 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/system.py
--rw-r--r--   0        0        0    14179 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/trigger.py
--rw-r--r--   0        0        0   163247 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/wlist.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/__init__.py
--rw-r--r--   0        0        0    90242 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/awgcontrol.py
--rw-r--r--   0        0        0     9092 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/diagnostic.py
--rw-r--r--   0        0        0     8411 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/display.py
--rw-r--r--   0        0        0    10230 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/event.py
--rw-r--r--   0        0        0     4266 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/instrument.py
--rw-r--r--   0        0        0    44926 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/mmemory.py
--rw-r--r--   0        0        0     8026 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/output.py
--rw-r--r--   0        0        0    35563 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/sequence.py
--rw-r--r--   0        0        0    17757 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/slist.py
--rw-r--r--   0        0        0   114889 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/source.py
--rw-r--r--   0        0        0    14353 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/status.py
--rw-r--r--   0        0        0    10476 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/system.py
--rw-r--r--   0        0        0    21093 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/trigger.py
--rw-r--r--   0        0        0    23571 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/wlist.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_33ijgq_afgawg/__init__.py
--rw-r--r--   0        0        0      940 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_33ijgq_afgawg/abort.py
--rw-r--r--   0        0        0     2821 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_33ijgq_afgawg/calibration.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_3n9auv_awg/__init__.py
--rw-r--r--   0        0        0     6308 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_3n9auv_awg/active.py
--rw-r--r--   0        0        0    29075 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_3n9auv_awg/calibration.py
--rw-r--r--   0        0        0    49372 2024-05-03 19:10:04.505310 tm_devices-1.4.0/src/tm_devices/commands/gen_3n9auv_awg/diagnostic.py
--rw-r--r--   0        0        0     4206 2024-05-03 19:10:04.509310 tm_devices-1.4.0/src/tm_devices/commands/gen_3n9auv_awg/display.py
--rw-r--r--   0        0        0     3890 2024-05-03 19:10:04.509310 tm_devices-1.4.0/src/tm_devices/commands/gen_3n9auv_awg/output.py
--rw-r--r--   0        0        0    76706 2024-05-03 19:10:04.509310 tm_devices-1.4.0/src/tm_devices/commands/gen_3n9auv_awg/slist.py
--rw-r--r--   0        0        0    23034 2024-05-03 19:10:04.509310 tm_devices-1.4.0/src/tm_devices/commands/gen_3n9auv_awg/status.py
--rw-r--r--   0        0        0     3386 2024-05-03 19:10:04.509310 tm_devices-1.4.0/src/tm_devices/commands/gen_3n9auv_awg/wplugin.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.509310 tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/__init__.py
--rw-r--r--   0        0        0     4946 2024-05-03 19:10:04.509310 tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/auxoutput.py
--rw-r--r--   0        0        0    68357 2024-05-03 19:10:04.509310 tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/awgcontrol.py
--rw-r--r--   0        0        0    28271 2024-05-03 19:10:04.509310 tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/bwaveform.py
--rw-r--r--   0        0        0    40671 2024-05-03 19:10:04.509310 tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/clock.py
--rw-r--r--   0        0        0    44230 2024-05-03 19:10:04.509310 tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/cplayback.py
--rw-r--r--   0        0        0    27950 2024-05-03 19:10:04.509310 tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/fgen.py
--rw-r--r--   0        0        0     6670 2024-05-03 19:10:04.509310 tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/instrument.py
--rw-r--r--   0        0        0    49463 2024-05-03 19:10:04.509310 tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/mmemory.py
--rw-r--r--   0        0        0    40589 2024-05-03 19:10:04.509310 tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/output.py
--rw-r--r--   0        0        0    70630 2024-05-03 19:10:04.509310 tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/source.py
--rw-r--r--   0        0        0    13005 2024-05-03 19:10:04.509310 tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/synchronize.py
--rw-r--r--   0        0        0    22277 2024-05-03 19:10:04.509310 tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/system.py
--rw-r--r--   0        0        0    14385 2024-05-03 19:10:04.509310 tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/trigger.py
--rw-r--r--   0        0        0   168016 2024-05-03 19:10:04.509310 tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/wlist.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.509310 tm_devices-1.4.0/src/tm_devices/commands/gen_3skc3w_dpo/__init__.py
--rw-r--r--   0        0        0  1609205 2024-05-03 19:10:04.517310 tm_devices-1.4.0/src/tm_devices/commands/gen_3skc3w_dpo/trigger.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.517310 tm_devices-1.4.0/src/tm_devices/commands/gen_3tjgb2_dpo/__init__.py
--rw-r--r--   0        0        0  1648252 2024-05-03 19:10:04.517310 tm_devices-1.4.0/src/tm_devices/commands/gen_3tjgb2_dpo/trigger.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.521310 tm_devices-1.4.0/src/tm_devices/commands/gen_4jiykk_dpo/__init__.py
--rw-r--r--   0        0        0     1159 2024-05-03 19:10:04.521310 tm_devices-1.4.0/src/tm_devices/commands/gen_4jiykk_dpo/channelmapping.py
--rw-r--r--   0        0        0    55974 2024-05-03 19:10:04.521310 tm_devices-1.4.0/src/tm_devices/commands/gen_4jiykk_dpo/counter.py
--rw-r--r--   0        0        0   239239 2024-05-03 19:10:04.521310 tm_devices-1.4.0/src/tm_devices/commands/gen_4jiykk_dpo/errordetector.py
--rw-r--r--   0        0        0     7734 2024-05-03 19:10:04.521310 tm_devices-1.4.0/src/tm_devices/commands/gen_4jiykk_dpo/idnmultiscope.py
--rw-r--r--   0        0        0    45422 2024-05-03 19:10:04.521310 tm_devices-1.4.0/src/tm_devices/commands/gen_4jiykk_dpo/linktraining.py
--rw-r--r--   0        0        0    13504 2024-05-03 19:10:04.521310 tm_devices-1.4.0/src/tm_devices/commands/gen_4jiykk_dpo/rosc.py
--rw-r--r--   0        0        0  1559854 2024-05-03 19:10:04.525310 tm_devices-1.4.0/src/tm_devices/commands/gen_4jiykk_dpo/trigger.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.525310 tm_devices-1.4.0/src/tm_devices/commands/gen_53md2e_dpomso/__init__.py
--rw-r--r--   0        0        0     2033 2024-05-03 19:10:04.525310 tm_devices-1.4.0/src/tm_devices/commands/gen_53md2e_dpomso/fpanel.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.525310 tm_devices-1.4.0/src/tm_devices/commands/gen_561g9r_mso/__init__.py
--rw-r--r--   0        0        0  1655550 2024-05-03 19:10:04.525310 tm_devices-1.4.0/src/tm_devices/commands/gen_561g9r_mso/trigger.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.525310 tm_devices-1.4.0/src/tm_devices/commands/gen_5ri0nj_dpomso/__init__.py
--rw-r--r--   0        0        0   289056 2024-05-03 19:10:04.529310 tm_devices-1.4.0/src/tm_devices/commands/gen_5ri0nj_dpomso/bus.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.529310 tm_devices-1.4.0/src/tm_devices/commands/gen_5vmwut_dpodsamso/__init__.py
--rw-r--r--   0        0        0  1559999 2024-05-03 19:10:04.529310 tm_devices-1.4.0/src/tm_devices/commands/gen_5vmwut_dpodsamso/trigger.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.529310 tm_devices-1.4.0/src/tm_devices/commands/gen_5xwdsk_dpodsamso/__init__.py
--rw-r--r--   0        0        0   293039 2024-05-03 19:10:04.529310 tm_devices-1.4.0/src/tm_devices/commands/gen_5xwdsk_dpodsamso/errordetector.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.529310 tm_devices-1.4.0/src/tm_devices/commands/gen_5y90wx_dpodsamso/__init__.py
--rw-r--r--   0        0        0   931776 2024-05-03 19:10:04.533310 tm_devices-1.4.0/src/tm_devices/commands/gen_5y90wx_dpodsamso/dpojet.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.533310 tm_devices-1.4.0/src/tm_devices/commands/gen_5yyb4r_mso/__init__.py
--rw-r--r--   0        0        0  1567252 2024-05-03 19:10:04.533310 tm_devices-1.4.0/src/tm_devices/commands/gen_5yyb4r_mso/trigger.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.533310 tm_devices-1.4.0/src/tm_devices/commands/gen_60xy3r_smu/__init__.py
--rw-r--r--   0        0        0    27630 2024-05-03 19:10:04.533310 tm_devices-1.4.0/src/tm_devices/commands/gen_60xy3r_smu/buffer.py
--rw-r--r--   0        0        0     2837 2024-05-03 19:10:04.533310 tm_devices-1.4.0/src/tm_devices/commands/gen_60xy3r_smu/script.py
--rw-r--r--   0        0        0   204886 2024-05-03 19:10:04.537310 tm_devices-1.4.0/src/tm_devices/commands/gen_60xy3r_smu/smu.py
--rw-r--r--   0        0        0     2467 2024-05-03 19:10:04.537310 tm_devices-1.4.0/src/tm_devices/commands/gen_60xy3r_smu/upgrade.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.537310 tm_devices-1.4.0/src/tm_devices/commands/gen_6ocqvh_smu/__init__.py
--rw-r--r--   0        0        0    33084 2024-05-03 19:10:04.537310 tm_devices-1.4.0/src/tm_devices/commands/gen_6ocqvh_smu/buffer.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.537310 tm_devices-1.4.0/src/tm_devices/commands/gen_6srh1x_smu/__init__.py
--rw-r--r--   0        0        0   204889 2024-05-03 19:10:04.537310 tm_devices-1.4.0/src/tm_devices/commands/gen_6srh1x_smu/smu.py
--rw-r--r--   0        0        0     2467 2024-05-03 19:10:04.537310 tm_devices-1.4.0/src/tm_devices/commands/gen_6srh1x_smu/upgrade.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.537310 tm_devices-1.4.0/src/tm_devices/commands/gen_6vynmi_smu/__init__.py
--rw-r--r--   0        0        0     6822 2024-05-03 19:10:04.537310 tm_devices-1.4.0/src/tm_devices/commands/gen_6vynmi_smu/acal.py
--rw-r--r--   0        0        0   317011 2024-05-03 19:10:04.537310 tm_devices-1.4.0/src/tm_devices/commands/gen_6vynmi_smu/smu.py
--rw-r--r--   0        0        0   205369 2024-05-03 19:10:04.537310 tm_devices-1.4.0/src/tm_devices/commands/gen_6vynmi_smu/trigger.py
--rw-r--r--   0        0        0     2467 2024-05-03 19:10:04.537310 tm_devices-1.4.0/src/tm_devices/commands/gen_6vynmi_smu/upgrade.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.537310 tm_devices-1.4.0/src/tm_devices/commands/gen_6w7311_smu/__init__.py
--rw-r--r--   0        0        0   204760 2024-05-03 19:10:04.537310 tm_devices-1.4.0/src/tm_devices/commands/gen_6w7311_smu/trigger.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.537310 tm_devices-1.4.0/src/tm_devices/commands/gen_6xiuc2_smu/__init__.py
--rw-r--r--   0        0        0    27548 2024-05-03 19:10:04.537310 tm_devices-1.4.0/src/tm_devices/commands/gen_6xiuc2_smu/buffer.py
--rw-r--r--   0        0        0   208019 2024-05-03 19:10:04.537310 tm_devices-1.4.0/src/tm_devices/commands/gen_6xiuc2_smu/smu.py
--rw-r--r--   0        0        0     2467 2024-05-03 19:10:04.537310 tm_devices-1.4.0/src/tm_devices/commands/gen_6xiuc2_smu/upgrade.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.537310 tm_devices-1.4.0/src/tm_devices/commands/gen_7kqm9p_smu/__init__.py
--rw-r--r--   0        0        0    39420 2024-05-03 19:10:04.537310 tm_devices-1.4.0/src/tm_devices/commands/gen_7kqm9p_smu/buffervar.py
--rw-r--r--   0        0        0    30303 2024-05-03 19:10:04.537310 tm_devices-1.4.0/src/tm_devices/commands/gen_7kqm9p_smu/display.py
--rw-r--r--   0        0        0    19620 2024-05-03 19:10:04.537310 tm_devices-1.4.0/src/tm_devices/commands/gen_7kqm9p_smu/tsplink.py
--rw-r--r--   0        0        0    23820 2024-05-03 19:10:04.537310 tm_devices-1.4.0/src/tm_devices/commands/gen_7kqm9p_smu/tspnet.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.537310 tm_devices-1.4.0/src/tm_devices/commands/gen_7ryhce_smu/__init__.py
--rw-r--r--   0        0        0   582496 2024-05-03 19:10:04.541310 tm_devices-1.4.0/src/tm_devices/commands/gen_7ryhce_smu/status.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.541310 tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/__init__.py
--rw-r--r--   0        0        0      966 2024-05-03 19:10:04.541310 tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/beeper.py
--rw-r--r--   0        0        0     3589 2024-05-03 19:10:04.541310 tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/buffervar.py
--rw-r--r--   0        0        0      939 2024-05-03 19:10:04.541310 tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/dataqueue.py
--rw-r--r--   0        0        0     7748 2024-05-03 19:10:04.541310 tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/digio.py
--rw-r--r--   0        0        0    27457 2024-05-03 19:10:04.541310 tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/display.py
--rw-r--r--   0        0        0     1720 2024-05-03 19:10:04.541310 tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/errorqueue.py
--rw-r--r--   0        0        0     1302 2024-05-03 19:10:04.541310 tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/eventlog.py
--rw-r--r--   0        0        0     4790 2024-05-03 19:10:04.541310 tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/format.py
--rw-r--r--   0        0        0    10117 2024-05-03 19:10:04.541310 tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/lan.py
--rw-r--r--   0        0        0     2601 2024-05-03 19:10:04.541310 tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/localnode.py
--rw-r--r--   0        0        0     8531 2024-05-03 19:10:04.541310 tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/serial.py
--rw-r--r--   0        0        0   301954 2024-05-03 19:10:04.541310 tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/smux.py
--rw-r--r--   0        0        0   370965 2024-05-03 19:10:04.545310 tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/status.py
--rw-r--r--   0        0        0     5013 2024-05-03 19:10:04.545310 tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/trigger.py
--rw-r--r--   0        0        0     5479 2024-05-03 19:10:04.545310 tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/tsplink.py
--rw-r--r--   0        0        0     1399 2024-05-03 19:10:04.545310 tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/tspnet.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.545310 tm_devices-1.4.0/src/tm_devices/commands/gen_7s43m8_smu/__init__.py
--rw-r--r--   0        0        0   627134 2024-05-03 19:10:04.545310 tm_devices-1.4.0/src/tm_devices/commands/gen_7s43m8_smu/status.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.545310 tm_devices-1.4.0/src/tm_devices/commands/gen_7s6wr5_smu/__init__.py
--rw-r--r--   0        0        0   613433 2024-05-03 19:10:04.545310 tm_devices-1.4.0/src/tm_devices/commands/gen_7s6wr5_smu/status.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.545310 tm_devices-1.4.0/src/tm_devices/commands/gen_8ojdkz_smu/__init__.py
--rw-r--r--   0        0        0    55384 2024-05-03 19:10:04.545310 tm_devices-1.4.0/src/tm_devices/commands/gen_8ojdkz_smu/display.py
--rw-r--r--   0        0        0     3812 2024-05-03 19:10:04.545310 tm_devices-1.4.0/src/tm_devices/commands/gen_8ojdkz_smu/node.py
--rw-r--r--   0        0        0   297756 2024-05-03 19:10:04.545310 tm_devices-1.4.0/src/tm_devices/commands/gen_8ojdkz_smu/smux.py
--rw-r--r--   0        0        0   618736 2024-05-03 19:10:04.545310 tm_devices-1.4.0/src/tm_devices/commands/gen_8ojdkz_smu/status.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.545310 tm_devices-1.4.0/src/tm_devices/commands/gen_8wm55i_smu/__init__.py
--rw-r--r--   0        0        0   304522 2024-05-03 19:10:04.545310 tm_devices-1.4.0/src/tm_devices/commands/gen_8wm55i_smu/smux.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.549310 tm_devices-1.4.0/src/tm_devices/commands/gen_9kezla_smu/__init__.py
--rw-r--r--   0        0        0   303892 2024-05-03 19:10:04.549310 tm_devices-1.4.0/src/tm_devices/commands/gen_9kezla_smu/smux.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.549310 tm_devices-1.4.0/src/tm_devices/commands/gen_9mzp2j_smu/__init__.py
--rw-r--r--   0        0        0    25789 2024-05-03 19:10:04.549310 tm_devices-1.4.0/src/tm_devices/commands/gen_9mzp2j_smu/digio.py
--rw-r--r--   0        0        0    55526 2024-05-03 19:10:04.549310 tm_devices-1.4.0/src/tm_devices/commands/gen_9mzp2j_smu/display.py
--rw-r--r--   0        0        0    34661 2024-05-03 19:10:04.549310 tm_devices-1.4.0/src/tm_devices/commands/gen_9mzp2j_smu/tsplink.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.549310 tm_devices-1.4.0/src/tm_devices/commands/gen_9ncc6e_smu/__init__.py
--rw-r--r--   0        0        0    50411 2024-05-03 19:10:04.549310 tm_devices-1.4.0/src/tm_devices/commands/gen_9ncc6e_smu/display.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.549310 tm_devices-1.4.0/src/tm_devices/commands/gen_9nnkq7_smu/__init__.py
--rw-r--r--   0        0        0   583623 2024-05-03 19:10:04.549310 tm_devices-1.4.0/src/tm_devices/commands/gen_9nnkq7_smu/status.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.549310 tm_devices-1.4.0/src/tm_devices/commands/gen_9slyux_smu/__init__.py
--rw-r--r--   0        0        0   614560 2024-05-03 19:10:04.549310 tm_devices-1.4.0/src/tm_devices/commands/gen_9slyux_smu/status.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.549310 tm_devices-1.4.0/src/tm_devices/commands/gen_ahkybr_smu/__init__.py
--rw-r--r--   0        0        0     4640 2024-05-03 19:10:04.549310 tm_devices-1.4.0/src/tm_devices/commands/gen_ahkybr_smu/beeper.py
--rw-r--r--   0        0        0    41300 2024-05-03 19:10:04.549310 tm_devices-1.4.0/src/tm_devices/commands/gen_ahkybr_smu/buffervar.py
--rw-r--r--   0        0        0    11124 2024-05-03 19:10:04.549310 tm_devices-1.4.0/src/tm_devices/commands/gen_ahkybr_smu/eventlog.py
--rw-r--r--   0        0        0    90987 2024-05-03 19:10:04.549310 tm_devices-1.4.0/src/tm_devices/commands/gen_ahkybr_smu/lan.py
--rw-r--r--   0        0        0     4062 2024-05-03 19:10:04.549310 tm_devices-1.4.0/src/tm_devices/commands/gen_ahkybr_smu/os.py
--rw-r--r--   0        0        0     8610 2024-05-03 19:10:04.549310 tm_devices-1.4.0/src/tm_devices/commands/gen_ahkybr_smu/script.py
--rw-r--r--   0        0        0    12291 2024-05-03 19:10:04.549310 tm_devices-1.4.0/src/tm_devices/commands/gen_ahkybr_smu/scriptvar.py
--rw-r--r--   0        0        0     5290 2024-05-03 19:10:04.549310 tm_devices-1.4.0/src/tm_devices/commands/gen_ahkybr_smu/setup_1.py
--rw-r--r--   0        0        0    23587 2024-05-03 19:10:04.549310 tm_devices-1.4.0/src/tm_devices/commands/gen_ahkybr_smu/tspnet.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.549310 tm_devices-1.4.0/src/tm_devices/commands/gen_aih9e2_smu/__init__.py
--rw-r--r--   0        0        0    36289 2024-05-03 19:10:04.549310 tm_devices-1.4.0/src/tm_devices/commands/gen_aih9e2_smu/trigger.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.549310 tm_devices-1.4.0/src/tm_devices/commands/gen_ak4990_smu/__init__.py
--rw-r--r--   0        0        0   304272 2024-05-03 19:10:04.549310 tm_devices-1.4.0/src/tm_devices/commands/gen_ak4990_smu/smux.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_am6pcr_smu/__init__.py
--rw-r--r--   0        0        0   278566 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_am6pcr_smu/smux.py
--rw-r--r--   0        0        0   623556 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_am6pcr_smu/status.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_amm5lc_smu/__init__.py
--rw-r--r--   0        0        0    31321 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_amm5lc_smu/digio.py
--rw-r--r--   0        0        0    37909 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_amm5lc_smu/tsplink.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_aostep_smu/__init__.py
--rw-r--r--   0        0        0    13800 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_aostep_smu/serial.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_aqr1t1_smu/__init__.py
--rw-r--r--   0        0        0    27960 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_aqr1t1_smu/localnode.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_as1ejq_smu/__init__.py
--rw-r--r--   0        0        0    25146 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_as1ejq_smu/localnode.py
--rw-r--r--   0        0        0   275978 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_as1ejq_smu/smux.py
--rw-r--r--   0        0        0   635702 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_as1ejq_smu/status.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_at7jl1_smu/__init__.py
--rw-r--r--   0        0        0    55816 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_at7jl1_smu/display.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_au597k_smu/__init__.py
--rw-r--r--   0        0        0    29997 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_au597k_smu/digio.py
--rw-r--r--   0        0        0    14069 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_au597k_smu/format.py
--rw-r--r--   0        0        0    36102 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_au597k_smu/tsplink.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_auyr50_smu/__init__.py
--rw-r--r--   0        0        0    13354 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_auyr50_smu/format.py
--rw-r--r--   0        0        0    28034 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_auyr50_smu/localnode.py
--rw-r--r--   0        0        0     4117 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_auyr50_smu/node.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_avh0iw_smu/__init__.py
--rw-r--r--   0        0        0    51741 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_avh0iw_smu/display.py
--rw-r--r--   0        0        0    35047 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_avh0iw_smu/trigger.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_awhjao_smu/__init__.py
--rw-r--r--   0        0        0   628261 2024-05-03 19:10:04.553310 tm_devices-1.4.0/src/tm_devices/commands/gen_awhjao_smu/status.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.557310 tm_devices-1.4.0/src/tm_devices/commands/gen_by991s_smudaq/__init__.py
--rw-r--r--   0        0        0    12283 2024-05-03 19:10:04.557310 tm_devices-1.4.0/src/tm_devices/commands/gen_by991s_smudaq/digio.py
--rw-r--r--   0        0        0    31576 2024-05-03 19:10:04.557310 tm_devices-1.4.0/src/tm_devices/commands/gen_by991s_smudaq/status.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.557310 tm_devices-1.4.0/src/tm_devices/commands/gen_canxny_daq/__init__.py
--rw-r--r--   0        0        0    36287 2024-05-03 19:10:04.557310 tm_devices-1.4.0/src/tm_devices/commands/gen_canxny_daq/buffer.py
--rw-r--r--   0        0        0    34903 2024-05-03 19:10:04.557310 tm_devices-1.4.0/src/tm_devices/commands/gen_canxny_daq/buffervar.py
--rw-r--r--   0        0        0    38415 2024-05-03 19:10:04.557310 tm_devices-1.4.0/src/tm_devices/commands/gen_canxny_daq/channel.py
--rw-r--r--   0        0        0    35222 2024-05-03 19:10:04.557310 tm_devices-1.4.0/src/tm_devices/commands/gen_canxny_daq/display.py
--rw-r--r--   0        0        0   318520 2024-05-03 19:10:04.557310 tm_devices-1.4.0/src/tm_devices/commands/gen_canxny_daq/dmm.py
--rw-r--r--   0        0        0    57952 2024-05-03 19:10:04.557310 tm_devices-1.4.0/src/tm_devices/commands/gen_canxny_daq/scan.py
--rw-r--r--   0        0        0    32594 2024-05-03 19:10:04.557310 tm_devices-1.4.0/src/tm_devices/commands/gen_canxny_daq/slot.py
--rw-r--r--   0        0        0   201599 2024-05-03 19:10:04.557310 tm_devices-1.4.0/src/tm_devices/commands/gen_canxny_daq/trigger.py
--rw-r--r--   0        0        0    16778 2024-05-03 19:10:04.557310 tm_devices-1.4.0/src/tm_devices/commands/gen_canxny_daq/tsplink.py
--rw-r--r--   0        0        0     2473 2024-05-03 19:10:04.557310 tm_devices-1.4.0/src/tm_devices/commands/gen_canxny_daq/upgrade.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.557310 tm_devices-1.4.0/src/tm_devices/commands/gen_d6b496_dmm/__init__.py
--rw-r--r--   0        0        0    11150 2024-05-03 19:10:04.557310 tm_devices-1.4.0/src/tm_devices/commands/gen_d6b496_dmm/acal.py
--rw-r--r--   0        0        0    28019 2024-05-03 19:10:04.557310 tm_devices-1.4.0/src/tm_devices/commands/gen_d6b496_dmm/buffer.py
--rw-r--r--   0        0        0    32622 2024-05-03 19:10:04.557310 tm_devices-1.4.0/src/tm_devices/commands/gen_d6b496_dmm/buffervar.py
--rw-r--r--   0        0        0    30425 2024-05-03 19:10:04.557310 tm_devices-1.4.0/src/tm_devices/commands/gen_d6b496_dmm/display.py
--rw-r--r--   0        0        0   250833 2024-05-03 19:10:04.557310 tm_devices-1.4.0/src/tm_devices/commands/gen_d6b496_dmm/dmm.py
--rw-r--r--   0        0        0     3182 2024-05-03 19:10:04.557310 tm_devices-1.4.0/src/tm_devices/commands/gen_d6b496_dmm/fan.py
--rw-r--r--   0        0        0    23204 2024-05-03 19:10:04.557310 tm_devices-1.4.0/src/tm_devices/commands/gen_d6b496_dmm/localnode.py
--rw-r--r--   0        0        0   195016 2024-05-03 19:10:04.557310 tm_devices-1.4.0/src/tm_devices/commands/gen_d6b496_dmm/trigger.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.557310 tm_devices-1.4.0/src/tm_devices/commands/gen_d83qe0_dmm/__init__.py
--rw-r--r--   0        0        0    31410 2024-05-03 19:10:04.557310 tm_devices-1.4.0/src/tm_devices/commands/gen_d83qe0_dmm/buffer.py
--rw-r--r--   0        0        0    34053 2024-05-03 19:10:04.557310 tm_devices-1.4.0/src/tm_devices/commands/gen_d83qe0_dmm/buffervar.py
--rw-r--r--   0        0        0    17456 2024-05-03 19:10:04.557310 tm_devices-1.4.0/src/tm_devices/commands/gen_d83qe0_dmm/channel.py
--rw-r--r--   0        0        0    33229 2024-05-03 19:10:04.557310 tm_devices-1.4.0/src/tm_devices/commands/gen_d83qe0_dmm/display.py
--rw-r--r--   0        0        0   196568 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_d83qe0_dmm/dmm.py
--rw-r--r--   0        0        0    51560 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_d83qe0_dmm/scan.py
--rw-r--r--   0        0        0     8718 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_d83qe0_dmm/slot.py
--rw-r--r--   0        0        0   192379 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_d83qe0_dmm/trigger.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_dawv9y_smudaqdmm/__init__.py
--rw-r--r--   0        0        0    22079 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_dawv9y_smudaqdmm/localnode.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/__init__.py
--rw-r--r--   0        0        0     1803 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/beeper.py
--rw-r--r--   0        0        0     7528 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/eventlog.py
--rw-r--r--   0        0        0     9275 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/file.py
--rw-r--r--   0        0        0    11990 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/format.py
--rw-r--r--   0        0        0     8492 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/lan.py
--rw-r--r--   0        0        0     4238 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/scriptvar.py
--rw-r--r--   0        0        0     2547 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/timer.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_dbqd7k_dmm/__init__.py
--rw-r--r--   0        0        0    11902 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_dbqd7k_dmm/digio.py
--rw-r--r--   0        0        0     3837 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_dbqd7k_dmm/node.py
--rw-r--r--   0        0        0    28175 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_dbqd7k_dmm/status.py
--rw-r--r--   0        0        0    16823 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_dbqd7k_dmm/tsplink.py
--rw-r--r--   0        0        0    22886 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_dbqd7k_dmm/tspnet.py
--rw-r--r--   0        0        0     2466 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_dbqd7k_dmm/upgrade.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_dcpheg_daqdmm/__init__.py
--rw-r--r--   0        0        0     1493 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_dcpheg_daqdmm/smu.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_dd4xnb_smudaqdmm/__init__.py
--rw-r--r--   0        0        0     2881 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_dd4xnb_smudaqdmm/script.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/__init__.py
--rw-r--r--   0        0        0    41892 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/acquire.py
--rw-r--r--   0        0        0   130167 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/actonevent.py
--rw-r--r--   0        0        0     2689 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/application.py
--rw-r--r--   0        0        0     5019 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/auxout.py
--rw-r--r--   0        0        0   949605 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/bus.py
--rw-r--r--   0        0        0    35014 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/callouts.py
--rw-r--r--   0        0        0   162423 2024-05-03 19:10:04.561310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/ch.py
--rw-r--r--   0        0        0    37622 2024-05-03 19:10:04.565310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/data.py
--rw-r--r--   0        0        0    16839 2024-05-03 19:10:04.565310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/diag.py
--rw-r--r--   0        0        0     5110 2024-05-03 19:10:04.565310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/diggrp.py
--rw-r--r--   0        0        0   685976 2024-05-03 19:10:04.565310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/display.py
--rw-r--r--   0        0        0    25348 2024-05-03 19:10:04.565310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/dvm.py
--rw-r--r--   0        0        0    28233 2024-05-03 19:10:04.565310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/eyemask.py
--rw-r--r--   0        0        0     8919 2024-05-03 19:10:04.565310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/fpanel.py
--rw-r--r--   0        0        0    74061 2024-05-03 19:10:04.565310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/histogram.py
--rw-r--r--   0        0        0   124292 2024-05-03 19:10:04.565310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/horizontal.py
--rw-r--r--   0        0        0    17319 2024-05-03 19:10:04.565310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/license.py
--rw-r--r--   0        0        0    53760 2024-05-03 19:10:04.565310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/mask.py
--rw-r--r--   0        0        0   229865 2024-05-03 19:10:04.565310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/math.py
--rw-r--r--   0        0        0     3469 2024-05-03 19:10:04.565310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/matharbflt.py
--rw-r--r--   0        0        0  1409304 2024-05-03 19:10:04.565310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/measurement.py
--rw-r--r--   0        0        0     8831 2024-05-03 19:10:04.565310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/peakstable.py
--rw-r--r--   0        0        0     5944 2024-05-03 19:10:04.565310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/pilogger.py
--rw-r--r--   0        0        0    99309 2024-05-03 19:10:04.565310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/plot.py
--rw-r--r--   0        0        0   842344 2024-05-03 19:10:04.569310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/power.py
--rw-r--r--   0        0        0    80340 2024-05-03 19:10:04.569310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/ref.py
--rw-r--r--   0        0        0     5139 2024-05-03 19:10:04.569310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/rosc.py
--rw-r--r--   0        0        0    53395 2024-05-03 19:10:04.569310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/save.py
--rw-r--r--   0        0        0    22709 2024-05-03 19:10:04.569310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/saveon.py
--rw-r--r--   0        0        0    15515 2024-05-03 19:10:04.569310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/saveonevent.py
--rw-r--r--   0        0        0  2492066 2024-05-03 19:10:04.569310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/search.py
--rw-r--r--   0        0        0     5403 2024-05-03 19:10:04.573310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/searchtable.py
--rw-r--r--   0        0        0     3863 2024-05-03 19:10:04.573310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/select.py
--rw-r--r--   0        0        0   135335 2024-05-03 19:10:04.573310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/sv.py
--rw-r--r--   0        0        0     4879 2024-05-03 19:10:04.573310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/touchscreen.py
--rw-r--r--   0        0        0  1714107 2024-05-03 19:10:04.573310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/trigger.py
--rw-r--r--   0        0        0     4743 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/tstamptable.py
--rw-r--r--   0        0        0    47508 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/visual.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/__init__.py
--rw-r--r--   0        0        0    43920 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/afg.py
--rw-r--r--   0        0        0     1437 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/autosavepitimeout.py
--rw-r--r--   0        0        0     1429 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/autosaveuitimeout.py
--rw-r--r--   0        0        0    20778 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/autoset.py
--rw-r--r--   0        0        0     4738 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/bustable.py
--rw-r--r--   0        0        0     7206 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/calibrate.py
--rw-r--r--   0        0        0     3708 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/configuration.py
--rw-r--r--   0        0        0    13730 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/connected.py
--rw-r--r--   0        0        0     4367 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/curve.py
--rw-r--r--   0        0        0     2854 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/curvestream.py
--rw-r--r--   0        0        0     4916 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/customtable.py
--rw-r--r--   0        0        0     1050 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/date.py
--rw-r--r--   0        0        0    32195 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/ethernet.py
--rw-r--r--   0        0        0    40419 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/filesystem.py
--rw-r--r--   0        0        0     6444 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/mainwindow.py
--rw-r--r--   0        0        0     3716 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/meastable.py
--rw-r--r--   0        0        0     8484 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/recall.py
--rw-r--r--   0        0        0     8465 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/socketserver.py
--rw-r--r--   0        0        0     6072 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/time.py
--rw-r--r--   0        0        0      958 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/undo.py
--rw-r--r--   0        0        0     3627 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/usbdevice.py
--rw-r--r--   0        0        0    15172 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/vertical.py
--rw-r--r--   0        0        0    48263 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/wfmoutpre.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/__init__.py
--rw-r--r--   0        0        0     4266 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/beeper.py
--rw-r--r--   0        0        0    36070 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/buffervar.py
--rw-r--r--   0        0        0    69159 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/channel.py
--rw-r--r--   0        0        0    20278 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/comm.py
--rw-r--r--   0        0        0    24474 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/digio.py
--rw-r--r--   0        0        0    25306 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/display.py
--rw-r--r--   0        0        0   152544 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/dmm.py
--rw-r--r--   0        0        0    10688 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/eventlog.py
--rw-r--r--   0        0        0    10200 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/format.py
--rw-r--r--   0        0        0    73653 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/lan.py
--rw-r--r--   0        0        0    25565 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/localnode.py
--rw-r--r--   0        0        0     2816 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/memory.py
--rw-r--r--   0        0        0     1817 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/os.py
--rw-r--r--   0        0        0    15065 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/ptp.py
--rw-r--r--   0        0        0    48486 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/scan.py
--rw-r--r--   0        0        0    21067 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/schedule.py
--rw-r--r--   0        0        0     8315 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/script.py
--rw-r--r--   0        0        0    10591 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/scriptvar.py
--rw-r--r--   0        0        0     5436 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/setup_1.py
--rw-r--r--   0        0        0    30730 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/slot.py
--rw-r--r--   0        0        0   125084 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/status.py
--rw-r--r--   0        0        0    33767 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/trigger.py
--rw-r--r--   0        0        0    32863 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/tsplink.py
--rw-r--r--   0        0        0     2483 2024-05-03 19:10:04.577310 tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/upgrade.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_e4de2d_lpdmsomdo/__init__.py
--rw-r--r--   0        0        0      928 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_e4de2d_lpdmsomdo/clear.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_e6606z_lpdmsomdodpo/__init__.py
--rw-r--r--   0        0        0     1296 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_e6606z_lpdmsomdodpo/pause.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_e6lgg1_lpdmsodpomdo/__init__.py
--rw-r--r--   0        0        0     1313 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_e6lgg1_lpdmsodpomdo/totaluptime.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_e7aqno_smudaqss/__init__.py
--rw-r--r--   0        0        0     3893 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_e7aqno_smudaqss/node.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_eat5s3_smudaqdmmss/__init__.py
--rw-r--r--   0        0        0     5522 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_eat5s3_smudaqdmmss/dataqueue.py
--rw-r--r--   0        0        0     7625 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_eat5s3_smudaqdmmss/fs.py
--rw-r--r--   0        0        0     3970 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_eat5s3_smudaqdmmss/userstring.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_ed9nkc_daqss/__init__.py
--rw-r--r--   0        0        0    23101 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_ed9nkc_daqss/tspnet.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_efap3f_smuss/__init__.py
--rw-r--r--   0        0        0    11856 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_efap3f_smuss/bit.py
--rw-r--r--   0        0        0     3765 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_efap3f_smuss/errorqueue.py
--rw-r--r--   0        0        0     9696 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_efap3f_smuss/io.py
--rw-r--r--   0        0        0     3063 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_efap3f_smuss/timer.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_eg5ll2_smudaqdmmss/__init__.py
--rw-r--r--   0        0        0     3409 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_eg5ll2_smudaqdmmss/gpib.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_ffz2xs_dpodsamso/__init__.py
--rw-r--r--   0        0        0   286772 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_ffz2xs_dpodsamso/bus.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_fhrp27_msodpomdodsa/__init__.py
--rw-r--r--   0        0        0     3441 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_fhrp27_msodpomdodsa/curve.py
--rw-r--r--   0        0        0     1641 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_fhrp27_msodpomdodsa/date.py
--rw-r--r--   0        0        0     4241 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_fhrp27_msodpomdodsa/mathvar.py
--rw-r--r--   0        0        0     2201 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_fhrp27_msodpomdodsa/save_and_recall.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/__init__.py
--rw-r--r--   0        0        0    41898 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/acquire.py
--rw-r--r--   0        0        0     4042 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/allocate.py
--rw-r--r--   0        0        0     6660 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/application.py
--rw-r--r--   0        0        0     4703 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/autoset.py
--rw-r--r--   0        0        0    67957 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/auxin.py
--rw-r--r--   0        0        0     6172 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/auxout.py
--rw-r--r--   0        0        0     1026 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/bell.py
--rw-r--r--   0        0        0    16111 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/calibrate.py
--rw-r--r--   0        0        0   143892 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/ch.py
--rw-r--r--   0        0        0      983 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/clear.py
--rw-r--r--   0        0        0     1992 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/cmdbatch.py
--rw-r--r--   0        0        0     2987 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/cq.py
--rw-r--r--   0        0        0    86089 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/cursor.py
--rw-r--r--   0        0        0     1636 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/curvenext.py
--rw-r--r--   0        0        0     3015 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/curvestream.py
--rw-r--r--   0        0        0     8707 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/custom.py
--rw-r--r--   0        0        0    12219 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/d.py
--rw-r--r--   0        0        0    30249 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/data.py
--rw-r--r--   0        0        0     5294 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/delete.py
--rw-r--r--   0        0        0    59925 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/diag.py
--rw-r--r--   0        0        0   139335 2024-05-03 19:10:04.581310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/display.py
--rw-r--r--   0        0        0    41283 2024-05-03 19:10:04.585310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/email.py
--rw-r--r--   0        0        0    12662 2024-05-03 19:10:04.585310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/export.py
--rw-r--r--   0        0        0     6134 2024-05-03 19:10:04.585310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/fastacq.py
--rw-r--r--   0        0        0    24502 2024-05-03 19:10:04.585310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/filesystem.py
--rw-r--r--   0        0        0     5528 2024-05-03 19:10:04.585310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/gpibusb.py
--rw-r--r--   0        0        0    17838 2024-05-03 19:10:04.585310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/hardcopy.py
--rw-r--r--   0        0        0     1903 2024-05-03 19:10:04.585310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/hdr.py
--rw-r--r--   0        0        0    28803 2024-05-03 19:10:04.585310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/histogram.py
--rw-r--r--   0        0        0   233302 2024-05-03 19:10:04.585310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/horizontal.py
--rw-r--r--   0        0        0    60154 2024-05-03 19:10:04.585310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/limit.py
--rw-r--r--   0        0        0    28385 2024-05-03 19:10:04.585310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/mark.py
--rw-r--r--   0        0        0   282367 2024-05-03 19:10:04.585310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/mask.py
--rw-r--r--   0        0        0    88338 2024-05-03 19:10:04.585310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/math.py
--rw-r--r--   0        0        0     4906 2024-05-03 19:10:04.585310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/matharbflt.py
--rw-r--r--   0        0        0    21243 2024-05-03 19:10:04.585310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/mch.py
--rw-r--r--   0        0        0   240397 2024-05-03 19:10:04.585310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/measurement.py
--rw-r--r--   0        0        0     7200 2024-05-03 19:10:04.585310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/multiscope.py
--rw-r--r--   0        0        0     4110 2024-05-03 19:10:04.585310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/opcextended.py
--rw-r--r--   0        0        0     1326 2024-05-03 19:10:04.585310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/pcenable.py
--rw-r--r--   0        0        0    11013 2024-05-03 19:10:04.585310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/recall.py
--rw-r--r--   0        0        0    25927 2024-05-03 19:10:04.585310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/ref.py
--rw-r--r--   0        0        0    28115 2024-05-03 19:10:04.585310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/save.py
--rw-r--r--   0        0        0     1466 2024-05-03 19:10:04.585310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/save_and_recall.py
--rw-r--r--   0        0        0    42097 2024-05-03 19:10:04.585310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/saveon.py
--rw-r--r--   0        0        0  1314240 2024-05-03 19:10:04.585310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/search.py
--rw-r--r--   0        0        0    24294 2024-05-03 19:10:04.589310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/select.py
--rw-r--r--   0        0        0     3069 2024-05-03 19:10:04.589310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/setup_1.py
--rw-r--r--   0        0        0     2945 2024-05-03 19:10:04.589310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/system.py
--rw-r--r--   0        0        0     4521 2024-05-03 19:10:04.589310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/teklink.py
--rw-r--r--   0        0        0     6698 2024-05-03 19:10:04.589310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/test.py
--rw-r--r--   0        0        0     5298 2024-05-03 19:10:04.589310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/trig.py
--rw-r--r--   0        0        0    12636 2024-05-03 19:10:04.589310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/usbtmc.py
--rw-r--r--   0        0        0    44201 2024-05-03 19:10:04.589310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/visual.py
--rw-r--r--   0        0        0     1540 2024-05-03 19:10:04.589310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/wavfrmstream.py
--rw-r--r--   0        0        0    43700 2024-05-03 19:10:04.589310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/wfminpre.py
--rw-r--r--   0        0        0    38216 2024-05-03 19:10:04.589310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/wfmoutpre.py
--rw-r--r--   0        0        0     2344 2024-05-03 19:10:04.589310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/wfmpre.py
--rw-r--r--   0        0        0   145020 2024-05-03 19:10:04.589310 tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/zoom.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.589310 tm_devices-1.4.0/src/tm_devices/commands/gen_fkjfe8_msodpodsa/__init__.py
--rw-r--r--   0        0        0     1739 2024-05-03 19:10:04.589310 tm_devices-1.4.0/src/tm_devices/commands/gen_fkjfe8_msodpodsa/time.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.589310 tm_devices-1.4.0/src/tm_devices/commands/gen_fn2qbf_msodpo/__init__.py
--rw-r--r--   0        0        0   234734 2024-05-03 19:10:04.589310 tm_devices-1.4.0/src/tm_devices/commands/gen_fn2qbf_msodpo/errordetector.py
--rw-r--r--   0        0        0  1544101 2024-05-03 19:10:04.589310 tm_devices-1.4.0/src/tm_devices/commands/gen_fn2qbf_msodpo/trigger.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.589310 tm_devices-1.4.0/src/tm_devices/commands/gen_fpx9s1_dpodsamso/__init__.py
--rw-r--r--   0        0        0    14139 2024-05-03 19:10:04.589310 tm_devices-1.4.0/src/tm_devices/commands/gen_fpx9s1_dpodsamso/counter.py
--rw-r--r--   0        0        0    30331 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fpx9s1_dpodsamso/linktraining.py
--rw-r--r--   0        0        0    11549 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fpx9s1_dpodsamso/rosc.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_ft5uww_lpdmsodpomdoafgawgdsa/__init__.py
--rw-r--r--   0        0        0     1403 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_ft5uww_lpdmsodpomdoafgawgdsa/calibration.py
--rw-r--r--   0        0        0     2445 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_ft5uww_lpdmsodpomdoafgawgdsa/miscellaneous.py
--rw-r--r--   0        0        0     8131 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_ft5uww_lpdmsodpomdoafgawgdsa/status_and_error.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fteabn_lpdmsomdodpoafgawgdsa/__init__.py
--rw-r--r--   0        0        0     1653 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fteabn_lpdmsomdodpoafgawgdsa/status_and_error.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fug7nl_lpdmsodpomdoawgdsa/__init__.py
--rw-r--r--   0        0        0     3041 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fug7nl_lpdmsodpomdoawgdsa/status_and_error.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fuzvln_lpdmsodpodsa/__init__.py
--rw-r--r--   0        0        0    12102 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fuzvln_lpdmsodpodsa/alias.py
--rw-r--r--   0        0        0     2110 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fuzvln_lpdmsodpodsa/header.py
--rw-r--r--   0        0        0     2422 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fuzvln_lpdmsodpodsa/status_and_error.py
--rw-r--r--   0        0        0     1512 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fuzvln_lpdmsodpodsa/verbose.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/__init__.py
--rw-r--r--   0        0        0     1554 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/allev.py
--rw-r--r--   0        0        0     1380 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/busy.py
--rw-r--r--   0        0        0     2051 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/dese.py
--rw-r--r--   0        0        0     1432 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/event.py
--rw-r--r--   0        0        0     1462 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/evmsg.py
--rw-r--r--   0        0        0     1426 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/evqty.py
--rw-r--r--   0        0        0     1802 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/factory.py
--rw-r--r--   0        0        0     1424 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/id.py
--rw-r--r--   0        0        0     3148 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/miscellaneous.py
--rw-r--r--   0        0        0     1462 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/newpass.py
--rw-r--r--   0        0        0     1947 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/password.py
--rw-r--r--   0        0        0     1427 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/rem.py
--rw-r--r--   0        0        0     1880 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/set.py
--rw-r--r--   0        0        0     1783 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/status_and_error.py
--rw-r--r--   0        0        0     1438 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/teksecure.py
--rw-r--r--   0        0        0     1488 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/wavfrm.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fzn174_lpdmsodpomdodsa/__init__.py
--rw-r--r--   0        0        0     2360 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fzn174_lpdmsodpomdodsa/lock.py
--rw-r--r--   0        0        0     1403 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_fzn174_lpdmsodpomdodsa/unlock.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/__init__.py
--rw-r--r--   0        0        0    18509 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/acquire.py
--rw-r--r--   0        0        0    10925 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/alias.py
--rw-r--r--   0        0        0     2961 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/autoset.py
--rw-r--r--   0        0        0    23027 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/auxin.py
--rw-r--r--   0        0        0   179853 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/bus.py
--rw-r--r--   0        0        0    17740 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/calibrate.py
--rw-r--r--   0        0        0    53778 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/ch.py
--rw-r--r--   0        0        0    76450 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/cursor.py
--rw-r--r--   0        0        0     7660 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/d.py
--rw-r--r--   0        0        0    29317 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/data.py
--rw-r--r--   0        0        0    25433 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/diag.py
--rw-r--r--   0        0        0    31518 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/display.py
--rw-r--r--   0        0        0    26251 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/ethernet.py
--rw-r--r--   0        0        0    22162 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/filesystem.py
--rw-r--r--   0        0        0     4958 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/filtervu.py
--rw-r--r--   0        0        0     8169 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/fpanel.py
--rw-r--r--   0        0        0     2368 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/gpibusb.py
--rw-r--r--   0        0        0    20476 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/hardcopy.py
--rw-r--r--   0        0        0    43301 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/horizontal.py
--rw-r--r--   0        0        0    22328 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/mark.py
--rw-r--r--   0        0        0    44629 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/math1.py
--rw-r--r--   0        0        0   142818 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/measurement.py
--rw-r--r--   0        0        0    17180 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/pictbridge.py
--rw-r--r--   0        0        0     6558 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/recall.py
--rw-r--r--   0        0        0    23375 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/ref.py
--rw-r--r--   0        0        0    31179 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/save.py
--rw-r--r--   0        0        0   446842 2024-05-03 19:10:04.593310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/search.py
--rw-r--r--   0        0        0    16968 2024-05-03 19:10:04.597310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/select.py
--rw-r--r--   0        0        0   442210 2024-05-03 19:10:04.597310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/trigger.py
--rw-r--r--   0        0        0    44738 2024-05-03 19:10:04.597310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/wfminpre.py
--rw-r--r--   0        0        0    44636 2024-05-03 19:10:04.597310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/wfmoutpre.py
--rw-r--r--   0        0        0    18830 2024-05-03 19:10:04.597310 tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/zoom.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.597310 tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/__init__.py
--rw-r--r--   0        0        0    34225 2024-05-03 19:10:04.597310 tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/acquire.py
--rw-r--r--   0        0        0    82260 2024-05-03 19:10:04.597310 tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/configuration.py
--rw-r--r--   0        0        0    80849 2024-05-03 19:10:04.597310 tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/cursor.py
--rw-r--r--   0        0        0     3011 2024-05-03 19:10:04.597310 tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/deskew.py
--rw-r--r--   0        0        0    47590 2024-05-03 19:10:04.597310 tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/display.py
--rw-r--r--   0        0        0     7928 2024-05-03 19:10:04.597310 tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/lock.py
--rw-r--r--   0        0        0   150766 2024-05-03 19:10:04.597310 tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/mask.py
--rw-r--r--   0        0        0   193055 2024-05-03 19:10:04.597310 tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/measurement.py
--rw-r--r--   0        0        0    23425 2024-05-03 19:10:04.597310 tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/message.py
--rw-r--r--   0        0        0    10363 2024-05-03 19:10:04.597310 tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/recall.py
--rw-r--r--   0        0        0   171778 2024-05-03 19:10:04.597310 tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/rf.py
--rw-r--r--   0        0        0     2877 2024-05-03 19:10:04.597310 tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/rrb.py
--rw-r--r--   0        0        0   745139 2024-05-03 19:10:04.597310 tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/search.py
--rw-r--r--   0        0        0    32522 2024-05-03 19:10:04.597310 tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/select.py
--rw-r--r--   0        0        0     5235 2024-05-03 19:10:04.601310 tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/setup1.py
--rw-r--r--   0        0        0   716529 2024-05-03 19:10:04.601310 tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/trigger.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.601310 tm_devices-1.4.0/src/tm_devices/commands/gen_usaa3_mdo/__init__.py
--rw-r--r--   0        0        0   185741 2024-05-03 19:10:04.601310 tm_devices-1.4.0/src/tm_devices/commands/gen_usaa3_mdo/rf.py
--rw-r--r--   0        0        0   771669 2024-05-03 19:10:04.601310 tm_devices-1.4.0/src/tm_devices/commands/gen_usaa3_mdo/search.py
--rw-r--r--   0        0        0   749699 2024-05-03 19:10:04.601310 tm_devices-1.4.0/src/tm_devices/commands/gen_usaa3_mdo/trigger.py
--rw-r--r--   0        0        0      878 2024-05-03 19:10:04.601310 tm_devices-1.4.0/src/tm_devices/commands/helpers/__init__.py
--rw-r--r--   0        0        0     5009 2024-05-03 19:10:04.601310 tm_devices-1.4.0/src/tm_devices/commands/helpers/generic_commands.py
--rw-r--r--   0        0        0    14623 2024-05-03 19:10:04.601310 tm_devices-1.4.0/src/tm_devices/commands/helpers/scpi_commands.py
--rw-r--r--   0        0        0     1832 2024-05-03 19:10:04.601310 tm_devices-1.4.0/src/tm_devices/commands/helpers/tsp_commands.py
--rw-r--r--   0        0        0   150973 2024-05-03 19:10:04.601310 tm_devices-1.4.0/src/tm_devices/commands/lpd6_commands.py
--rw-r--r--   0        0        0   129766 2024-05-03 19:10:04.601310 tm_devices-1.4.0/src/tm_devices/commands/mdo3_commands.py
--rw-r--r--   0        0        0   130785 2024-05-03 19:10:04.601310 tm_devices-1.4.0/src/tm_devices/commands/mdo3k_commands.py
--rw-r--r--   0        0        0   131141 2024-05-03 19:10:04.605310 tm_devices-1.4.0/src/tm_devices/commands/mdo4k_commands.py
--rw-r--r--   0        0        0   130948 2024-05-03 19:10:04.605310 tm_devices-1.4.0/src/tm_devices/commands/mdo4kb_commands.py
--rw-r--r--   0        0        0   131209 2024-05-03 19:10:04.605310 tm_devices-1.4.0/src/tm_devices/commands/mdo4kc_commands.py
--rw-r--r--   0        0        0   116295 2024-05-03 19:10:04.605310 tm_devices-1.4.0/src/tm_devices/commands/mso2_commands.py
--rw-r--r--   0        0        0   105183 2024-05-03 19:10:04.605310 tm_devices-1.4.0/src/tm_devices/commands/mso2k_commands.py
--rw-r--r--   0        0        0   105202 2024-05-03 19:10:04.605310 tm_devices-1.4.0/src/tm_devices/commands/mso2kb_commands.py
--rw-r--r--   0        0        0   150973 2024-05-03 19:10:04.605310 tm_devices-1.4.0/src/tm_devices/commands/mso4_commands.py
--rw-r--r--   0        0        0   150992 2024-05-03 19:10:04.605310 tm_devices-1.4.0/src/tm_devices/commands/mso4b_commands.py
--rw-r--r--   0        0        0   131009 2024-05-03 19:10:04.605310 tm_devices-1.4.0/src/tm_devices/commands/mso4k_commands.py
--rw-r--r--   0        0        0   131083 2024-05-03 19:10:04.605310 tm_devices-1.4.0/src/tm_devices/commands/mso4kb_commands.py
--rw-r--r--   0        0        0   150973 2024-05-03 19:10:04.605310 tm_devices-1.4.0/src/tm_devices/commands/mso5_commands.py
--rw-r--r--   0        0        0   150992 2024-05-03 19:10:04.605310 tm_devices-1.4.0/src/tm_devices/commands/mso5b_commands.py
--rw-r--r--   0        0        0   154860 2024-05-03 19:10:04.605310 tm_devices-1.4.0/src/tm_devices/commands/mso5k_commands.py
--rw-r--r--   0        0        0   159850 2024-05-03 19:10:04.605310 tm_devices-1.4.0/src/tm_devices/commands/mso5kb_commands.py
--rw-r--r--   0        0        0   151011 2024-05-03 19:10:04.605310 tm_devices-1.4.0/src/tm_devices/commands/mso5lp_commands.py
--rw-r--r--   0        0        0   150973 2024-05-03 19:10:04.605310 tm_devices-1.4.0/src/tm_devices/commands/mso6_commands.py
--rw-r--r--   0        0        0   150992 2024-05-03 19:10:04.605310 tm_devices-1.4.0/src/tm_devices/commands/mso6b_commands.py
--rw-r--r--   0        0        0   159058 2024-05-03 19:10:04.605310 tm_devices-1.4.0/src/tm_devices/commands/mso70kc_commands.py
--rw-r--r--   0        0        0   159104 2024-05-03 19:10:04.605310 tm_devices-1.4.0/src/tm_devices/commands/mso70kdx_commands.py
--rw-r--r--   0        0        0    84668 2024-05-03 19:10:04.605310 tm_devices-1.4.0/src/tm_devices/commands/smu2450_commands.py
--rw-r--r--   0        0        0    88434 2024-05-03 19:10:04.605310 tm_devices-1.4.0/src/tm_devices/commands/smu2460_commands.py
--rw-r--r--   0        0        0    88578 2024-05-03 19:10:04.605310 tm_devices-1.4.0/src/tm_devices/commands/smu2461_commands.py
--rw-r--r--   0        0        0    84757 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/commands/smu2470_commands.py
--rw-r--r--   0        0        0   133683 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/commands/smu2601b_commands.py
--rw-r--r--   0        0        0    63551 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/commands/smu2601b_pulse_commands.py
--rw-r--r--   0        0        0   140431 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/commands/smu2602b_commands.py
--rw-r--r--   0        0        0   127767 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/commands/smu2604b_commands.py
--rw-r--r--   0        0        0   139285 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/commands/smu2606b_commands.py
--rw-r--r--   0        0        0   133503 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/commands/smu2611b_commands.py
--rw-r--r--   0        0        0   140251 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/commands/smu2612b_commands.py
--rw-r--r--   0        0        0   127587 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/commands/smu2614b_commands.py
--rw-r--r--   0        0        0   127740 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/commands/smu2634b_commands.py
--rw-r--r--   0        0        0   133656 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/commands/smu2635b_commands.py
--rw-r--r--   0        0        0   140404 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/commands/smu2636b_commands.py
--rw-r--r--   0        0        0   123159 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/commands/smu2651a_commands.py
--rw-r--r--   0        0        0   123084 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/commands/smu2657a_commands.py
--rw-r--r--   0        0        0    51307 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/commands/ss3706a_commands.py
--rw-r--r--   0        0        0      155 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/components/__init__.py
--rw-r--r--   0        0        0    18263 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/components/dm_config_parser.py
--rw-r--r--   0        0        0    53954 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/device_manager.py
--rw-r--r--   0        0        0      176 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/driver_mixins/__init__.py
--rw-r--r--   0        0        0     6579 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/driver_mixins/analysis_object_mixins.py
--rw-r--r--   0        0        0     4041 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/driver_mixins/class_extension_mixin.py
--rw-r--r--   0        0        0      943 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/driver_mixins/licensed_mixin.py
--rw-r--r--   0        0        0     3048 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/driver_mixins/signal_generator_mixin.py
--rw-r--r--   0        0        0      540 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/driver_mixins/usb_drives_mixin.py
--rw-r--r--   0        0        0     9181 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/drivers/__init__.py
--rw-r--r--   0        0        0       55 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/drivers/api/__init__.py
--rw-r--r--   0        0        0      242 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/drivers/api/api_device.py
--rw-r--r--   0        0        0       31 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/drivers/api/rest_api/__init__.py
--rw-r--r--   0        0        0      243 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/drivers/api/rest_api/margin_testers/__init__.py
--rw-r--r--   0        0        0     5891 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/drivers/api/rest_api/margin_testers/margin_tester.py
--rw-r--r--   0        0        0     6155 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/drivers/api/rest_api/margin_testers/tmt4.py
--rw-r--r--   0        0        0    22603 2024-05-03 19:10:04.609310 tm_devices-1.4.0/src/tm_devices/drivers/api/rest_api/rest_api_device.py
--rw-r--r--   0        0        0    29615 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/device.py
--rw-r--r--   0        0        0    12713 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/device_driver_mapping.py
--rw-r--r--   0        0        0     1372 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/device_type_classes.py
--rw-r--r--   0        0        0       43 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/__init__.py
--rw-r--r--   0        0        0      329 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/data_acquisition_systems/__init__.py
--rw-r--r--   0        0        0     3283 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/data_acquisition_systems/daq6510.py
--rw-r--r--   0        0        0     1095 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/data_acquisition_systems/data_acquisition_system.py
--rw-r--r--   0        0        0      362 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/digital_multimeters/__init__.py
--rw-r--r--   0        0        0     1464 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/digital_multimeters/digital_multimeter.py
--rw-r--r--   0        0        0      142 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/digital_multimeters/dmm6500/__init__.py
--rw-r--r--   0        0        0     3114 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/digital_multimeters/dmm6500/dmm6500.py
--rw-r--r--   0        0        0      328 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/digital_multimeters/dmm7500/__init__.py
--rw-r--r--   0        0        0     3135 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/digital_multimeters/dmm7500/dmm7500.py
--rw-r--r--   0        0        0     1791 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/digital_multimeters/dmm7500/dmm7510.py
--rw-r--r--   0        0        0     1777 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/digital_multimeters/dmm7500/dmm7512.py
--rw-r--r--   0        0        0    13515 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/ieee488_2_commands.py
--rw-r--r--   0        0        0    34941 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/pi_device.py
--rw-r--r--   0        0        0      245 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/power_supplies/__init__.py
--rw-r--r--   0        0        0     1603 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/power_supplies/power_supply.py
--rw-r--r--   0        0        0      668 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/power_supplies/psu2200/__init__.py
--rw-r--r--   0        0        0     2471 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/power_supplies/psu2200/psu2200.py
--rw-r--r--   0        0        0     1096 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/power_supplies/psu2200/psu2220.py
--rw-r--r--   0        0        0     1096 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/power_supplies/psu2200/psu2230.py
--rw-r--r--   0        0        0     1096 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/power_supplies/psu2200/psu2231.py
--rw-r--r--   0        0        0     1100 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/power_supplies/psu2200/psu2231a.py
--rw-r--r--   0        0        0     1316 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/power_supplies/psu2200/psu2280.py
--rw-r--r--   0        0        0     1096 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/power_supplies/psu2200/psu2281.py
--rw-r--r--   0        0        0      584 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/__init__.py
--rw-r--r--   0        0        0     4875 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/scope.py
--rw-r--r--   0        0        0      887 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope/__init__.py
--rw-r--r--   0        0        0     1083 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope/lpd6.py
--rw-r--r--   0        0        0     2290 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope/mso2.py
--rw-r--r--   0        0        0     1095 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope/mso4.py
--rw-r--r--   0        0        0     1089 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope/mso4b.py
--rw-r--r--   0        0        0     1095 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope/mso5.py
--rw-r--r--   0        0        0     1089 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope/mso5b.py
--rw-r--r--   0        0        0     1095 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope/mso5lp.py
--rw-r--r--   0        0        0     1095 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope/mso6.py
--rw-r--r--   0        0        0     1089 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope/mso6b.py
--rw-r--r--   0        0        0    27396 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope/tekscope.py
--rw-r--r--   0        0        0     2445 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope/tekscopesw.py
--rw-r--r--   0        0        0      464 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_2k/__init__.py
--rw-r--r--   0        0        0     1780 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_2k/dpo2k.py
--rw-r--r--   0        0        0     1770 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_2k/dpo2kb.py
--rw-r--r--   0        0        0     1780 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_2k/mso2k.py
--rw-r--r--   0        0        0     1770 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_2k/mso2kb.py
--rw-r--r--   0        0        0     1415 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_2k/tekscope_2k.py
--rw-r--r--   0        0        0      896 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/__init__.py
--rw-r--r--   0        0        0     1790 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/dpo4k.py
--rw-r--r--   0        0        0     1773 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/dpo4kb.py
--rw-r--r--   0        0        0     2056 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/mdo3.py
--rw-r--r--   0        0        0     1790 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/mdo3k.py
--rw-r--r--   0        0        0     1790 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/mdo4k.py
--rw-r--r--   0        0        0     1773 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/mdo4kb.py
--rw-r--r--   0        0        0     1776 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/mdo4kc.py
--rw-r--r--   0        0        0     1790 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/mso4k.py
--rw-r--r--   0        0        0     1773 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/mso4kb.py
--rw-r--r--   0        0        0     1783 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/tekscope_3k_4k.py
--rw-r--r--   0        0        0     1695 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/__init__.py
--rw-r--r--   0        0        0     1804 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo5k.py
--rw-r--r--   0        0        0     1108 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo5kb.py
--rw-r--r--   0        0        0     1798 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo70k.py
--rw-r--r--   0        0        0     1117 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo70kc.py
--rw-r--r--   0        0        0     1120 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo70kd.py
--rw-r--r--   0        0        0     1123 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo70kdx.py
--rw-r--r--   0        0        0     1123 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo70ksx.py
--rw-r--r--   0        0        0     1804 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo7k.py
--rw-r--r--   0        0        0     1108 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo7kc.py
--rw-r--r--   0        0        0     1798 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dsa70k.py
--rw-r--r--   0        0        0     1117 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dsa70kc.py
--rw-r--r--   0        0        0     1117 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dsa70kd.py
--rw-r--r--   0        0        0     1804 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/mso5k.py
--rw-r--r--   0        0        0     1108 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/mso5kb.py
--rw-r--r--   0        0        0     1798 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/mso70k.py
--rw-r--r--   0        0        0     1117 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/mso70kc.py
--rw-r--r--   0        0        0     1123 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/mso70kdx.py
--rw-r--r--   0        0        0     3037 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/tekscope_5k_7k_70k.py
--rw-r--r--   0        0        0      117 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tso/__init__.py
--rw-r--r--   0        0        0     1766 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tso/tsovu.py
--rw-r--r--   0        0        0      298 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/__init__.py
--rw-r--r--   0        0        0      443 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/afgs/__init__.py
--rw-r--r--   0        0        0     6878 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/afgs/afg.py
--rw-r--r--   0        0        0     2043 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/afgs/afg31k.py
--rw-r--r--   0        0        0     1283 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/afgs/afg3k.py
--rw-r--r--   0        0        0     1327 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/afgs/afg3kb.py
--rw-r--r--   0        0        0     1330 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/afgs/afg3kc.py
--rw-r--r--   0        0        0      859 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/awgs/__init__.py
--rw-r--r--   0        0        0     5783 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/awgs/awg.py
--rw-r--r--   0        0        0     1517 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/awgs/awg5200.py
--rw-r--r--   0        0        0     1505 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/awgs/awg5k.py
--rw-r--r--   0        0        0     1091 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/awgs/awg5kb.py
--rw-r--r--   0        0        0     1106 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/awgs/awg5kc.py
--rw-r--r--   0        0        0     1519 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/awgs/awg70ka.py
--rw-r--r--   0        0        0     1115 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/awgs/awg70kb.py
--rw-r--r--   0        0        0     1505 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/awgs/awg7k.py
--rw-r--r--   0        0        0     1091 2024-05-03 19:10:04.613310 tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/awgs/awg7kb.py
--rw-r--r--   0        0        0     1329 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/awgs/awg7kc.py
--rw-r--r--   0        0        0     5211 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/signal_source.py
--rw-r--r--   0        0        0      633 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/__init__.py
--rw-r--r--   0        0        0      963 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2400/__init__.py
--rw-r--r--   0        0        0     1141 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2400.py
--rw-r--r--   0        0        0     3358 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2400_interactive.py
--rw-r--r--   0        0        0     5707 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2400_standard.py
--rw-r--r--   0        0        0     1141 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2401.py
--rw-r--r--   0        0        0     1141 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2410.py
--rw-r--r--   0        0        0     1173 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2450.py
--rw-r--r--   0        0        0     1173 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2460.py
--rw-r--r--   0        0        0     1173 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2461.py
--rw-r--r--   0        0        0     1173 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2470.py
--rw-r--r--   0        0        0     2487 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/__init__.py
--rw-r--r--   0        0        0     3814 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2600.py
--rw-r--r--   0        0        0      216 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2600a.py
--rw-r--r--   0        0        0     1196 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2600b.py
--rw-r--r--   0        0        0     1123 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2601a.py
--rw-r--r--   0        0        0     1139 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2601b.py
--rw-r--r--   0        0        0     1172 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2601b_pulse.py
--rw-r--r--   0        0        0     1123 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2602a.py
--rw-r--r--   0        0        0     1139 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2602b.py
--rw-r--r--   0        0        0     1123 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2604a.py
--rw-r--r--   0        0        0     1139 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2604b.py
--rw-r--r--   0        0        0     1139 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2606b.py
--rw-r--r--   0        0        0     1123 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2611a.py
--rw-r--r--   0        0        0     1139 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2611b.py
--rw-r--r--   0        0        0     1123 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2612a.py
--rw-r--r--   0        0        0     1139 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2612b.py
--rw-r--r--   0        0        0     1123 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2614a.py
--rw-r--r--   0        0        0     1139 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2614b.py
--rw-r--r--   0        0        0     1123 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2634a.py
--rw-r--r--   0        0        0     1139 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2634b.py
--rw-r--r--   0        0        0     1123 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2635a.py
--rw-r--r--   0        0        0     1139 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2635b.py
--rw-r--r--   0        0        0     1123 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2636a.py
--rw-r--r--   0        0        0     1139 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2636b.py
--rw-r--r--   0        0        0      718 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2650a.py
--rw-r--r--   0        0        0     1139 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2651a.py
--rw-r--r--   0        0        0     1139 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2657a.py
--rw-r--r--   0        0        0      409 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu6000/__init__.py
--rw-r--r--   0        0        0     5922 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu6000/smu6000.py
--rw-r--r--   0        0        0     1109 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu6000/smu6430.py
--rw-r--r--   0        0        0     1109 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu6000/smu6514.py
--rw-r--r--   0        0        0     1113 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu6000/smu6517b.py
--rw-r--r--   0        0        0      587 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/source_measure_unit.py
--rw-r--r--   0        0        0      241 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/systems_switches/__init__.py
--rw-r--r--   0        0        0     3584 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/systems_switches/ss3706a.py
--rw-r--r--   0        0        0      527 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/systems_switches/systems_switch.py
--rw-r--r--   0        0        0    10612 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/drivers/pi/tsp_device.py
--rw-r--r--   0        0        0     2235 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/helpers/__init__.py
--rw-r--r--   0        0        0     3788 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/helpers/alias_dict.py
--rw-r--r--   0        0        0    29480 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/helpers/constants_and_dataclasses.py
--rw-r--r--   0        0        0     2733 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/helpers/dataclass_mixins.py
--rw-r--r--   0        0        0     6836 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/helpers/enums.py
--rw-r--r--   0        0        0    27496 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/helpers/functions.py
--rw-r--r--   0        0        0     3603 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/helpers/read_only_cached_property.py
--rw-r--r--   0        0        0     1149 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/helpers/singleton_metaclass.py
--rw-r--r--   0        0        0     1408 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/helpers/standalone_functions.py
--rw-r--r--   0        0        0     3914 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/helpers/stubgen.py
--rw-r--r--   0        0        0        0 2024-05-03 19:10:04.617310 tm_devices-1.4.0/src/tm_devices/py.typed
--rw-r--r--   0        0        0    20956 1970-01-01 00:00:00.000000 tm_devices-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    10262 2024-05-06 18:52:31.186463 tm_devices-1.4.1/LICENSE.md
+-rw-r--r--   0        0        0    18639 2024-05-06 18:52:31.186463 tm_devices-1.4.1/README.md
+-rw-r--r--   0        0        0    14815 2024-05-06 18:52:31.194463 tm_devices-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0      858 2024-05-06 18:52:31.194463 tm_devices-1.4.1/src/tm_devices/__init__.py
+-rw-r--r--   0        0        0    10643 2024-05-06 18:52:31.194463 tm_devices-1.4.1/src/tm_devices/commands/__init__.py
+-rw-r--r--   0        0        0    35404 2024-05-06 18:52:31.194463 tm_devices-1.4.1/src/tm_devices/commands/afg3k_commands.py
+-rw-r--r--   0        0        0    35423 2024-05-06 18:52:31.194463 tm_devices-1.4.1/src/tm_devices/commands/afg3kb_commands.py
+-rw-r--r--   0        0        0    35423 2024-05-06 18:52:31.194463 tm_devices-1.4.1/src/tm_devices/commands/afg3kc_commands.py
+-rw-r--r--   0        0        0    40196 2024-05-06 18:52:31.194463 tm_devices-1.4.1/src/tm_devices/commands/awg5200_commands.py
+-rw-r--r--   0        0        0    31702 2024-05-06 18:52:31.194463 tm_devices-1.4.1/src/tm_devices/commands/awg5k_commands.py
+-rw-r--r--   0        0        0    31721 2024-05-06 18:52:31.194463 tm_devices-1.4.1/src/tm_devices/commands/awg5kc_commands.py
+-rw-r--r--   0        0        0    40082 2024-05-06 18:52:31.194463 tm_devices-1.4.1/src/tm_devices/commands/awg70ka_commands.py
+-rw-r--r--   0        0        0    40082 2024-05-06 18:52:31.194463 tm_devices-1.4.1/src/tm_devices/commands/awg70kb_commands.py
+-rw-r--r--   0        0        0    31702 2024-05-06 18:52:31.194463 tm_devices-1.4.1/src/tm_devices/commands/awg7k_commands.py
+-rw-r--r--   0        0        0    31721 2024-05-06 18:52:31.194463 tm_devices-1.4.1/src/tm_devices/commands/awg7kc_commands.py
+-rw-r--r--   0        0        0   110433 2024-05-06 18:52:31.194463 tm_devices-1.4.1/src/tm_devices/commands/daq6510_commands.py
+-rw-r--r--   0        0        0    72918 2024-05-06 18:52:31.194463 tm_devices-1.4.1/src/tm_devices/commands/dmm6500_commands.py
+-rw-r--r--   0        0        0    70438 2024-05-06 18:52:31.194463 tm_devices-1.4.1/src/tm_devices/commands/dmm7510_commands.py
+-rw-r--r--   0        0        0   105183 2024-05-06 18:52:31.194463 tm_devices-1.4.1/src/tm_devices/commands/dpo2k_commands.py
+-rw-r--r--   0        0        0   105202 2024-05-06 18:52:31.194463 tm_devices-1.4.1/src/tm_devices/commands/dpo2kb_commands.py
+-rw-r--r--   0        0        0   130739 2024-05-06 18:52:31.198463 tm_devices-1.4.1/src/tm_devices/commands/dpo4k_commands.py
+-rw-r--r--   0        0        0   131028 2024-05-06 18:52:31.198463 tm_devices-1.4.1/src/tm_devices/commands/dpo4kb_commands.py
+-rw-r--r--   0        0        0   154860 2024-05-06 18:52:31.198463 tm_devices-1.4.1/src/tm_devices/commands/dpo5k_commands.py
+-rw-r--r--   0        0        0   159820 2024-05-06 18:52:31.198463 tm_devices-1.4.1/src/tm_devices/commands/dpo5kb_commands.py
+-rw-r--r--   0        0        0   159061 2024-05-06 18:52:31.198463 tm_devices-1.4.1/src/tm_devices/commands/dpo70kc_commands.py
+-rw-r--r--   0        0        0   159061 2024-05-06 18:52:31.198463 tm_devices-1.4.1/src/tm_devices/commands/dpo70kd_commands.py
+-rw-r--r--   0        0        0   159080 2024-05-06 18:52:31.198463 tm_devices-1.4.1/src/tm_devices/commands/dpo70kdx_commands.py
+-rw-r--r--   0        0        0   163875 2024-05-06 18:52:31.198463 tm_devices-1.4.1/src/tm_devices/commands/dpo70ksx_commands.py
+-rw-r--r--   0        0        0   154860 2024-05-06 18:52:31.198463 tm_devices-1.4.1/src/tm_devices/commands/dpo7k_commands.py
+-rw-r--r--   0        0        0   159062 2024-05-06 18:52:31.198463 tm_devices-1.4.1/src/tm_devices/commands/dpo7kc_commands.py
+-rw-r--r--   0        0        0   159061 2024-05-06 18:52:31.198463 tm_devices-1.4.1/src/tm_devices/commands/dsa70kc_commands.py
+-rw-r--r--   0        0        0   159061 2024-05-06 18:52:31.198463 tm_devices-1.4.1/src/tm_devices/commands/dsa70kd_commands.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.198463 tm_devices-1.4.1/src/tm_devices/commands/gen_163n04_mdo/__init__.py
+-rw-r--r--   0        0        0   904180 2024-05-06 18:52:31.206463 tm_devices-1.4.1/src/tm_devices/commands/gen_163n04_mdo/search.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.206463 tm_devices-1.4.1/src/tm_devices/commands/gen_16x4xq_mdo/__init__.py
+-rw-r--r--   0        0        0   797746 2024-05-06 18:52:31.206463 tm_devices-1.4.1/src/tm_devices/commands/gen_16x4xq_mdo/search.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.210463 tm_devices-1.4.1/src/tm_devices/commands/gen_1jzp7o_mdodpo/__init__.py
+-rw-r--r--   0        0        0   738804 2024-05-06 18:52:31.210463 tm_devices-1.4.1/src/tm_devices/commands/gen_1jzp7o_mdodpo/trigger.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.210463 tm_devices-1.4.1/src/tm_devices/commands/gen_1kdqwg_mdo/__init__.py
+-rw-r--r--   0        0        0   916756 2024-05-06 18:52:31.210463 tm_devices-1.4.1/src/tm_devices/commands/gen_1kdqwg_mdo/search.py
+-rw-r--r--   0        0        0   832335 2024-05-06 18:52:31.214463 tm_devices-1.4.1/src/tm_devices/commands/gen_1kdqwg_mdo/trigger.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.214463 tm_devices-1.4.1/src/tm_devices/commands/gen_1kjd62_mdo/__init__.py
+-rw-r--r--   0        0        0   203791 2024-05-06 18:52:31.214463 tm_devices-1.4.1/src/tm_devices/commands/gen_1kjd62_mdo/rf.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.214463 tm_devices-1.4.1/src/tm_devices/commands/gen_1kozfv_dpo/__init__.py
+-rw-r--r--   0        0        0   759094 2024-05-06 18:52:31.214463 tm_devices-1.4.1/src/tm_devices/commands/gen_1kozfv_dpo/search.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.214463 tm_devices-1.4.1/src/tm_devices/commands/gen_1l4fot_mdomso/__init__.py
+-rw-r--r--   0        0        0    82893 2024-05-06 18:52:31.218463 tm_devices-1.4.1/src/tm_devices/commands/gen_1l4fot_mdomso/cursor.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.218463 tm_devices-1.4.1/src/tm_devices/commands/gen_1la1ym_msomdodpo/__init__.py
+-rw-r--r--   0        0        0   821454 2024-05-06 18:52:31.218463 tm_devices-1.4.1/src/tm_devices/commands/gen_1la1ym_msomdodpo/trigger.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.218463 tm_devices-1.4.1/src/tm_devices/commands/gen_1lcv3a_msodpomdo/__init__.py
+-rw-r--r--   0        0        0    10809 2024-05-06 18:52:31.218463 tm_devices-1.4.1/src/tm_devices/commands/gen_1lcv3a_msodpomdo/message.py
+-rw-r--r--   0        0        0     5278 2024-05-06 18:52:31.218463 tm_devices-1.4.1/src/tm_devices/commands/gen_1lcv3a_msodpomdo/setup_1.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.218463 tm_devices-1.4.1/src/tm_devices/commands/gen_1lh2st_msodpo/__init__.py
+-rw-r--r--   0        0        0   865545 2024-05-06 18:52:31.218463 tm_devices-1.4.1/src/tm_devices/commands/gen_1lh2st_msodpo/search.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.218463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/__init__.py
+-rw-r--r--   0        0        0    45151 2024-05-06 18:52:31.218463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/actonevent.py
+-rw-r--r--   0        0        0    69457 2024-05-06 18:52:31.218463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/afg.py
+-rw-r--r--   0        0        0     9715 2024-05-06 18:52:31.218463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/alias.py
+-rw-r--r--   0        0        0    13357 2024-05-06 18:52:31.218463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/application.py
+-rw-r--r--   0        0        0     3625 2024-05-06 18:52:31.218463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/autoset.py
+-rw-r--r--   0        0        0    26008 2024-05-06 18:52:31.218463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/auxin.py
+-rw-r--r--   0        0        0     3780 2024-05-06 18:52:31.218463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/auxout.py
+-rw-r--r--   0        0        0   319685 2024-05-06 18:52:31.218463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/bus.py
+-rw-r--r--   0        0        0    41940 2024-05-06 18:52:31.222463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/calibrate.py
+-rw-r--r--   0        0        0    74577 2024-05-06 18:52:31.222463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/ch.py
+-rw-r--r--   0        0        0     7842 2024-05-06 18:52:31.222463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/d.py
+-rw-r--r--   0        0        0    27302 2024-05-06 18:52:31.222463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/data.py
+-rw-r--r--   0        0        0    18170 2024-05-06 18:52:31.222463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/diag.py
+-rw-r--r--   0        0        0    22847 2024-05-06 18:52:31.222463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/dvm.py
+-rw-r--r--   0        0        0    14675 2024-05-06 18:52:31.222463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/email.py
+-rw-r--r--   0        0        0    42390 2024-05-06 18:52:31.222463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/ethernet.py
+-rw-r--r--   0        0        0    33557 2024-05-06 18:52:31.222463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/filesystem.py
+-rw-r--r--   0        0        0    10959 2024-05-06 18:52:31.222463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/fpanel.py
+-rw-r--r--   0        0        0     3733 2024-05-06 18:52:31.222463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/gpibusb.py
+-rw-r--r--   0        0        0    20948 2024-05-06 18:52:31.222463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/hardcopy.py
+-rw-r--r--   0        0        0    24507 2024-05-06 18:52:31.222463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/histogram.py
+-rw-r--r--   0        0        0    26671 2024-05-06 18:52:31.222463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/horizontal.py
+-rw-r--r--   0        0        0    28374 2024-05-06 18:52:31.222463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/mark.py
+-rw-r--r--   0        0        0    43937 2024-05-06 18:52:31.222463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/marker.py
+-rw-r--r--   0        0        0    39214 2024-05-06 18:52:31.222463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/math1.py
+-rw-r--r--   0        0        0    20522 2024-05-06 18:52:31.222463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/pictbridge.py
+-rw-r--r--   0        0        0   348440 2024-05-06 18:52:31.226463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/power.py
+-rw-r--r--   0        0        0     1021 2024-05-06 18:52:31.226463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/reboot.py
+-rw-r--r--   0        0        0    19812 2024-05-06 18:52:31.226463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/ref.py
+-rw-r--r--   0        0        0    37418 2024-05-06 18:52:31.226463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/save.py
+-rw-r--r--   0        0        0     7694 2024-05-06 18:52:31.226463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/socketserver.py
+-rw-r--r--   0        0        0     1501 2024-05-06 18:52:31.226463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/time.py
+-rw-r--r--   0        0        0    32867 2024-05-06 18:52:31.226463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/vidpic.py
+-rw-r--r--   0        0        0    54903 2024-05-06 18:52:31.226463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/wfminpre.py
+-rw-r--r--   0        0        0    45499 2024-05-06 18:52:31.226463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/wfmoutpre.py
+-rw-r--r--   0        0        0    20895 2024-05-06 18:52:31.226463 tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/zoom.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.226463 tm_devices-1.4.1/src/tm_devices/commands/gen_1lwj1r_msomdodpo/__init__.py
+-rw-r--r--   0        0        0     4839 2024-05-06 18:52:31.226463 tm_devices-1.4.1/src/tm_devices/commands/gen_1lwj1r_msomdodpo/rosc.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.226463 tm_devices-1.4.1/src/tm_devices/commands/gen_1lxxm9_msomdodpo/__init__.py
+-rw-r--r--   0        0        0    77140 2024-05-06 18:52:31.226463 tm_devices-1.4.1/src/tm_devices/commands/gen_1lxxm9_msomdodpo/cursor.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.226463 tm_devices-1.4.1/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/__init__.py
+-rw-r--r--   0        0        0    29207 2024-05-06 18:52:31.226463 tm_devices-1.4.1/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/acquire.py
+-rw-r--r--   0        0        0    84211 2024-05-06 18:52:31.226463 tm_devices-1.4.1/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/configuration.py
+-rw-r--r--   0        0        0     3065 2024-05-06 18:52:31.226463 tm_devices-1.4.1/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/deskew.py
+-rw-r--r--   0        0        0    44570 2024-05-06 18:52:31.226463 tm_devices-1.4.1/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/display.py
+-rw-r--r--   0        0        0   148268 2024-05-06 18:52:31.230463 tm_devices-1.4.1/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/mask.py
+-rw-r--r--   0        0        0   194267 2024-05-06 18:52:31.230463 tm_devices-1.4.1/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/measurement.py
+-rw-r--r--   0        0        0    10398 2024-05-06 18:52:31.230463 tm_devices-1.4.1/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/recall.py
+-rw-r--r--   0        0        0    38664 2024-05-06 18:52:31.230463 tm_devices-1.4.1/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/select.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.230463 tm_devices-1.4.1/src/tm_devices/commands/gen_1mq0z9_msodpo/__init__.py
+-rw-r--r--   0        0        0   182231 2024-05-06 18:52:31.230463 tm_devices-1.4.1/src/tm_devices/commands/gen_1mq0z9_msodpo/rf.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.230463 tm_devices-1.4.1/src/tm_devices/commands/gen_1nmc1o_msodpomdo/__init__.py
+-rw-r--r--   0        0        0     1040 2024-05-06 18:52:31.230463 tm_devices-1.4.1/src/tm_devices/commands/gen_1nmc1o_msodpomdo/clearmenu.py
+-rw-r--r--   0        0        0     4740 2024-05-06 18:52:31.230463 tm_devices-1.4.1/src/tm_devices/commands/gen_1nmc1o_msodpomdo/errlog.py
+-rw-r--r--   0        0        0     1892 2024-05-06 18:52:31.230463 tm_devices-1.4.1/src/tm_devices/commands/gen_1nmc1o_msodpomdo/header.py
+-rw-r--r--   0        0        0     1694 2024-05-06 18:52:31.230463 tm_devices-1.4.1/src/tm_devices/commands/gen_1nmc1o_msodpomdo/language.py
+-rw-r--r--   0        0        0     2138 2024-05-06 18:52:31.230463 tm_devices-1.4.1/src/tm_devices/commands/gen_1nmc1o_msodpomdo/status_and_error.py
+-rw-r--r--   0        0        0     3152 2024-05-06 18:52:31.230463 tm_devices-1.4.1/src/tm_devices/commands/gen_1nmc1o_msodpomdo/usbdevice.py
+-rw-r--r--   0        0        0    12816 2024-05-06 18:52:31.230463 tm_devices-1.4.1/src/tm_devices/commands/gen_1nmc1o_msodpomdo/usbtmc.py
+-rw-r--r--   0        0        0     1492 2024-05-06 18:52:31.230463 tm_devices-1.4.1/src/tm_devices/commands/gen_1nmc1o_msodpomdo/verbose.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.230463 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/__init__.py
+-rw-r--r--   0        0        0    24124 2024-05-06 18:52:31.230463 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/acquire.py
+-rw-r--r--   0        0        0   130490 2024-05-06 18:52:31.230463 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/actonevent.py
+-rw-r--r--   0        0        0     5035 2024-05-06 18:52:31.230463 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/auxout.py
+-rw-r--r--   0        0        0    11020 2024-05-06 18:52:31.230463 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/battery.py
+-rw-r--r--   0        0        0   243616 2024-05-06 18:52:31.234464 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/bus.py
+-rw-r--r--   0        0        0    36323 2024-05-06 18:52:31.234464 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/callouts.py
+-rw-r--r--   0        0        0    63363 2024-05-06 18:52:31.234464 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/ch.py
+-rw-r--r--   0        0        0    29416 2024-05-06 18:52:31.234464 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/data.py
+-rw-r--r--   0        0        0    26913 2024-05-06 18:52:31.234464 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/dch.py
+-rw-r--r--   0        0        0    16876 2024-05-06 18:52:31.234464 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/diag.py
+-rw-r--r--   0        0        0   580922 2024-05-06 18:52:31.234464 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/display.py
+-rw-r--r--   0        0        0     7079 2024-05-06 18:52:31.234464 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/fpanel.py
+-rw-r--r--   0        0        0    44079 2024-05-06 18:52:31.238463 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/horizontal.py
+-rw-r--r--   0        0        0     3165 2024-05-06 18:52:31.238463 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/lic.py
+-rw-r--r--   0        0        0    14641 2024-05-06 18:52:31.238463 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/license.py
+-rw-r--r--   0        0        0    41868 2024-05-06 18:52:31.238463 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/mask.py
+-rw-r--r--   0        0        0    89876 2024-05-06 18:52:31.238463 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/math.py
+-rw-r--r--   0        0        0   555657 2024-05-06 18:52:31.238463 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/measurement.py
+-rw-r--r--   0        0        0    28636 2024-05-06 18:52:31.238463 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/pg.py
+-rw-r--r--   0        0        0     9116 2024-05-06 18:52:31.238463 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/plot.py
+-rw-r--r--   0        0        0    62601 2024-05-06 18:52:31.238463 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/power.py
+-rw-r--r--   0        0        0    32565 2024-05-06 18:52:31.238463 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/ref.py
+-rw-r--r--   0        0        0    37873 2024-05-06 18:52:31.238463 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/save.py
+-rw-r--r--   0        0        0    23156 2024-05-06 18:52:31.238463 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/saveon.py
+-rw-r--r--   0        0        0    16637 2024-05-06 18:52:31.238463 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/saveonevent.py
+-rw-r--r--   0        0        0   419529 2024-05-06 18:52:31.242464 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/search.py
+-rw-r--r--   0        0        0     7641 2024-05-06 18:52:31.242464 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/select.py
+-rw-r--r--   0        0        0     3357 2024-05-06 18:52:31.242464 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/touchscreen.py
+-rw-r--r--   0        0        0   319248 2024-05-06 18:52:31.242464 tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/trigger.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.242464 tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/__init__.py
+-rw-r--r--   0        0        0     2192 2024-05-06 18:52:31.242464 tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/afgcontrol.py
+-rw-r--r--   0        0        0    21587 2024-05-06 18:52:31.242464 tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/data.py
+-rw-r--r--   0        0        0     2627 2024-05-06 18:52:31.242464 tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/diagnostic.py
+-rw-r--r--   0        0        0    14155 2024-05-06 18:52:31.242464 tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/display.py
+-rw-r--r--   0        0        0     3447 2024-05-06 18:52:31.242464 tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/hcopy.py
+-rw-r--r--   0        0        0    11509 2024-05-06 18:52:31.242464 tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/memory.py
+-rw-r--r--   0        0        0    17547 2024-05-06 18:52:31.242464 tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/mmemory.py
+-rw-r--r--   0        0        0     4782 2024-05-06 18:52:31.242464 tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/output.py
+-rw-r--r--   0        0        0     7071 2024-05-06 18:52:31.242464 tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/output1.py
+-rw-r--r--   0        0        0     7071 2024-05-06 18:52:31.242464 tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/output2.py
+-rw-r--r--   0        0        0     3963 2024-05-06 18:52:31.242464 tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/source.py
+-rw-r--r--   0        0        0   190576 2024-05-06 18:52:31.242464 tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/source1.py
+-rw-r--r--   0        0        0   190576 2024-05-06 18:52:31.242464 tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/source2.py
+-rw-r--r--   0        0        0     7600 2024-05-06 18:52:31.242464 tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/source3.py
+-rw-r--r--   0        0        0     7600 2024-05-06 18:52:31.242464 tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/source4.py
+-rw-r--r--   0        0        0    17014 2024-05-06 18:52:31.242464 tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/status.py
+-rw-r--r--   0        0        0    26993 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/system.py
+-rw-r--r--   0        0        0     9281 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/trigger.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/__init__.py
+-rw-r--r--   0        0        0     1043 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/abort.py
+-rw-r--r--   0        0        0     4919 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/auxoutput.py
+-rw-r--r--   0        0        0    34829 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/awgcontrol.py
+-rw-r--r--   0        0        0    28178 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/bwaveform.py
+-rw-r--r--   0        0        0    38773 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/clock.py
+-rw-r--r--   0        0        0    42644 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/cplayback.py
+-rw-r--r--   0        0        0    28829 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/fgen.py
+-rw-r--r--   0        0        0     6748 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/instrument.py
+-rw-r--r--   0        0        0    49454 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/mmemory.py
+-rw-r--r--   0        0        0    23340 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/output.py
+-rw-r--r--   0        0        0    83750 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/source.py
+-rw-r--r--   0        0        0     4606 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/synchronize.py
+-rw-r--r--   0        0        0    16556 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/system.py
+-rw-r--r--   0        0        0    14179 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/trigger.py
+-rw-r--r--   0        0        0   163247 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/wlist.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/__init__.py
+-rw-r--r--   0        0        0    90242 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/awgcontrol.py
+-rw-r--r--   0        0        0     9092 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/diagnostic.py
+-rw-r--r--   0        0        0     8411 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/display.py
+-rw-r--r--   0        0        0    10230 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/event.py
+-rw-r--r--   0        0        0     4266 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/instrument.py
+-rw-r--r--   0        0        0    44926 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/mmemory.py
+-rw-r--r--   0        0        0     8026 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/output.py
+-rw-r--r--   0        0        0    35563 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/sequence.py
+-rw-r--r--   0        0        0    17757 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/slist.py
+-rw-r--r--   0        0        0   114889 2024-05-06 18:52:31.246464 tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/source.py
+-rw-r--r--   0        0        0    14353 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/status.py
+-rw-r--r--   0        0        0    10476 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/system.py
+-rw-r--r--   0        0        0    21093 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/trigger.py
+-rw-r--r--   0        0        0    23571 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/wlist.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_33ijgq_afgawg/__init__.py
+-rw-r--r--   0        0        0      940 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_33ijgq_afgawg/abort.py
+-rw-r--r--   0        0        0     2821 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_33ijgq_afgawg/calibration.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_3n9auv_awg/__init__.py
+-rw-r--r--   0        0        0     6308 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_3n9auv_awg/active.py
+-rw-r--r--   0        0        0    29075 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_3n9auv_awg/calibration.py
+-rw-r--r--   0        0        0    49372 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_3n9auv_awg/diagnostic.py
+-rw-r--r--   0        0        0     4206 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_3n9auv_awg/display.py
+-rw-r--r--   0        0        0     3890 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_3n9auv_awg/output.py
+-rw-r--r--   0        0        0    76706 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_3n9auv_awg/slist.py
+-rw-r--r--   0        0        0    23034 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_3n9auv_awg/status.py
+-rw-r--r--   0        0        0     3386 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_3n9auv_awg/wplugin.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/__init__.py
+-rw-r--r--   0        0        0     4946 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/auxoutput.py
+-rw-r--r--   0        0        0    68357 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/awgcontrol.py
+-rw-r--r--   0        0        0    28271 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/bwaveform.py
+-rw-r--r--   0        0        0    40671 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/clock.py
+-rw-r--r--   0        0        0    44230 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/cplayback.py
+-rw-r--r--   0        0        0    27950 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/fgen.py
+-rw-r--r--   0        0        0     6670 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/instrument.py
+-rw-r--r--   0        0        0    49463 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/mmemory.py
+-rw-r--r--   0        0        0    40589 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/output.py
+-rw-r--r--   0        0        0    70630 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/source.py
+-rw-r--r--   0        0        0    13005 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/synchronize.py
+-rw-r--r--   0        0        0    22277 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/system.py
+-rw-r--r--   0        0        0    14385 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/trigger.py
+-rw-r--r--   0        0        0   168016 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/wlist.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.250464 tm_devices-1.4.1/src/tm_devices/commands/gen_3skc3w_dpo/__init__.py
+-rw-r--r--   0        0        0  1609205 2024-05-06 18:52:31.258464 tm_devices-1.4.1/src/tm_devices/commands/gen_3skc3w_dpo/trigger.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.258464 tm_devices-1.4.1/src/tm_devices/commands/gen_3tjgb2_dpo/__init__.py
+-rw-r--r--   0        0        0  1648252 2024-05-06 18:52:31.262464 tm_devices-1.4.1/src/tm_devices/commands/gen_3tjgb2_dpo/trigger.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.262464 tm_devices-1.4.1/src/tm_devices/commands/gen_4jiykk_dpo/__init__.py
+-rw-r--r--   0        0        0     1159 2024-05-06 18:52:31.262464 tm_devices-1.4.1/src/tm_devices/commands/gen_4jiykk_dpo/channelmapping.py
+-rw-r--r--   0        0        0    55974 2024-05-06 18:52:31.262464 tm_devices-1.4.1/src/tm_devices/commands/gen_4jiykk_dpo/counter.py
+-rw-r--r--   0        0        0   239239 2024-05-06 18:52:31.262464 tm_devices-1.4.1/src/tm_devices/commands/gen_4jiykk_dpo/errordetector.py
+-rw-r--r--   0        0        0     7734 2024-05-06 18:52:31.262464 tm_devices-1.4.1/src/tm_devices/commands/gen_4jiykk_dpo/idnmultiscope.py
+-rw-r--r--   0        0        0    45422 2024-05-06 18:52:31.262464 tm_devices-1.4.1/src/tm_devices/commands/gen_4jiykk_dpo/linktraining.py
+-rw-r--r--   0        0        0    13504 2024-05-06 18:52:31.262464 tm_devices-1.4.1/src/tm_devices/commands/gen_4jiykk_dpo/rosc.py
+-rw-r--r--   0        0        0  1559854 2024-05-06 18:52:31.266464 tm_devices-1.4.1/src/tm_devices/commands/gen_4jiykk_dpo/trigger.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.266464 tm_devices-1.4.1/src/tm_devices/commands/gen_53md2e_dpomso/__init__.py
+-rw-r--r--   0        0        0     2033 2024-05-06 18:52:31.266464 tm_devices-1.4.1/src/tm_devices/commands/gen_53md2e_dpomso/fpanel.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.266464 tm_devices-1.4.1/src/tm_devices/commands/gen_561g9r_mso/__init__.py
+-rw-r--r--   0        0        0  1655550 2024-05-06 18:52:31.266464 tm_devices-1.4.1/src/tm_devices/commands/gen_561g9r_mso/trigger.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.266464 tm_devices-1.4.1/src/tm_devices/commands/gen_5ri0nj_dpomso/__init__.py
+-rw-r--r--   0        0        0   289056 2024-05-06 18:52:31.270464 tm_devices-1.4.1/src/tm_devices/commands/gen_5ri0nj_dpomso/bus.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.270464 tm_devices-1.4.1/src/tm_devices/commands/gen_5vmwut_dpodsamso/__init__.py
+-rw-r--r--   0        0        0  1559999 2024-05-06 18:52:31.270464 tm_devices-1.4.1/src/tm_devices/commands/gen_5vmwut_dpodsamso/trigger.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.270464 tm_devices-1.4.1/src/tm_devices/commands/gen_5xwdsk_dpodsamso/__init__.py
+-rw-r--r--   0        0        0   293039 2024-05-06 18:52:31.270464 tm_devices-1.4.1/src/tm_devices/commands/gen_5xwdsk_dpodsamso/errordetector.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.270464 tm_devices-1.4.1/src/tm_devices/commands/gen_5y90wx_dpodsamso/__init__.py
+-rw-r--r--   0        0        0   931776 2024-05-06 18:52:31.274464 tm_devices-1.4.1/src/tm_devices/commands/gen_5y90wx_dpodsamso/dpojet.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.274464 tm_devices-1.4.1/src/tm_devices/commands/gen_5yyb4r_mso/__init__.py
+-rw-r--r--   0        0        0  1567252 2024-05-06 18:52:31.274464 tm_devices-1.4.1/src/tm_devices/commands/gen_5yyb4r_mso/trigger.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.274464 tm_devices-1.4.1/src/tm_devices/commands/gen_60xy3r_smu/__init__.py
+-rw-r--r--   0        0        0    27630 2024-05-06 18:52:31.274464 tm_devices-1.4.1/src/tm_devices/commands/gen_60xy3r_smu/buffer.py
+-rw-r--r--   0        0        0     2837 2024-05-06 18:52:31.274464 tm_devices-1.4.1/src/tm_devices/commands/gen_60xy3r_smu/script.py
+-rw-r--r--   0        0        0   204886 2024-05-06 18:52:31.278464 tm_devices-1.4.1/src/tm_devices/commands/gen_60xy3r_smu/smu.py
+-rw-r--r--   0        0        0     2467 2024-05-06 18:52:31.278464 tm_devices-1.4.1/src/tm_devices/commands/gen_60xy3r_smu/upgrade.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.278464 tm_devices-1.4.1/src/tm_devices/commands/gen_6ocqvh_smu/__init__.py
+-rw-r--r--   0        0        0    33084 2024-05-06 18:52:31.278464 tm_devices-1.4.1/src/tm_devices/commands/gen_6ocqvh_smu/buffer.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.278464 tm_devices-1.4.1/src/tm_devices/commands/gen_6srh1x_smu/__init__.py
+-rw-r--r--   0        0        0   204889 2024-05-06 18:52:31.278464 tm_devices-1.4.1/src/tm_devices/commands/gen_6srh1x_smu/smu.py
+-rw-r--r--   0        0        0     2467 2024-05-06 18:52:31.278464 tm_devices-1.4.1/src/tm_devices/commands/gen_6srh1x_smu/upgrade.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.278464 tm_devices-1.4.1/src/tm_devices/commands/gen_6vynmi_smu/__init__.py
+-rw-r--r--   0        0        0     6822 2024-05-06 18:52:31.278464 tm_devices-1.4.1/src/tm_devices/commands/gen_6vynmi_smu/acal.py
+-rw-r--r--   0        0        0   317011 2024-05-06 18:52:31.278464 tm_devices-1.4.1/src/tm_devices/commands/gen_6vynmi_smu/smu.py
+-rw-r--r--   0        0        0   205369 2024-05-06 18:52:31.278464 tm_devices-1.4.1/src/tm_devices/commands/gen_6vynmi_smu/trigger.py
+-rw-r--r--   0        0        0     2467 2024-05-06 18:52:31.278464 tm_devices-1.4.1/src/tm_devices/commands/gen_6vynmi_smu/upgrade.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.278464 tm_devices-1.4.1/src/tm_devices/commands/gen_6w7311_smu/__init__.py
+-rw-r--r--   0        0        0   204760 2024-05-06 18:52:31.278464 tm_devices-1.4.1/src/tm_devices/commands/gen_6w7311_smu/trigger.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.278464 tm_devices-1.4.1/src/tm_devices/commands/gen_6xiuc2_smu/__init__.py
+-rw-r--r--   0        0        0    27548 2024-05-06 18:52:31.278464 tm_devices-1.4.1/src/tm_devices/commands/gen_6xiuc2_smu/buffer.py
+-rw-r--r--   0        0        0   208019 2024-05-06 18:52:31.278464 tm_devices-1.4.1/src/tm_devices/commands/gen_6xiuc2_smu/smu.py
+-rw-r--r--   0        0        0     2467 2024-05-06 18:52:31.278464 tm_devices-1.4.1/src/tm_devices/commands/gen_6xiuc2_smu/upgrade.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.278464 tm_devices-1.4.1/src/tm_devices/commands/gen_7kqm9p_smu/__init__.py
+-rw-r--r--   0        0        0    39420 2024-05-06 18:52:31.278464 tm_devices-1.4.1/src/tm_devices/commands/gen_7kqm9p_smu/buffervar.py
+-rw-r--r--   0        0        0    30303 2024-05-06 18:52:31.278464 tm_devices-1.4.1/src/tm_devices/commands/gen_7kqm9p_smu/display.py
+-rw-r--r--   0        0        0    19620 2024-05-06 18:52:31.278464 tm_devices-1.4.1/src/tm_devices/commands/gen_7kqm9p_smu/tsplink.py
+-rw-r--r--   0        0        0    23820 2024-05-06 18:52:31.278464 tm_devices-1.4.1/src/tm_devices/commands/gen_7kqm9p_smu/tspnet.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.278464 tm_devices-1.4.1/src/tm_devices/commands/gen_7ryhce_smu/__init__.py
+-rw-r--r--   0        0        0   582496 2024-05-06 18:52:31.282464 tm_devices-1.4.1/src/tm_devices/commands/gen_7ryhce_smu/status.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.282464 tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/__init__.py
+-rw-r--r--   0        0        0      966 2024-05-06 18:52:31.282464 tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/beeper.py
+-rw-r--r--   0        0        0     3589 2024-05-06 18:52:31.282464 tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/buffervar.py
+-rw-r--r--   0        0        0      939 2024-05-06 18:52:31.282464 tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/dataqueue.py
+-rw-r--r--   0        0        0     7748 2024-05-06 18:52:31.282464 tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/digio.py
+-rw-r--r--   0        0        0    27457 2024-05-06 18:52:31.282464 tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/display.py
+-rw-r--r--   0        0        0     1720 2024-05-06 18:52:31.282464 tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/errorqueue.py
+-rw-r--r--   0        0        0     1302 2024-05-06 18:52:31.282464 tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/eventlog.py
+-rw-r--r--   0        0        0     4790 2024-05-06 18:52:31.282464 tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/format.py
+-rw-r--r--   0        0        0    10117 2024-05-06 18:52:31.282464 tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/lan.py
+-rw-r--r--   0        0        0     2601 2024-05-06 18:52:31.282464 tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/localnode.py
+-rw-r--r--   0        0        0     8531 2024-05-06 18:52:31.282464 tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/serial.py
+-rw-r--r--   0        0        0   301954 2024-05-06 18:52:31.282464 tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/smux.py
+-rw-r--r--   0        0        0   370965 2024-05-06 18:52:31.282464 tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/status.py
+-rw-r--r--   0        0        0     5013 2024-05-06 18:52:31.286465 tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/trigger.py
+-rw-r--r--   0        0        0     5479 2024-05-06 18:52:31.286465 tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/tsplink.py
+-rw-r--r--   0        0        0     1399 2024-05-06 18:52:31.286465 tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/tspnet.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.286465 tm_devices-1.4.1/src/tm_devices/commands/gen_7s43m8_smu/__init__.py
+-rw-r--r--   0        0        0   627134 2024-05-06 18:52:31.286465 tm_devices-1.4.1/src/tm_devices/commands/gen_7s43m8_smu/status.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.286465 tm_devices-1.4.1/src/tm_devices/commands/gen_7s6wr5_smu/__init__.py
+-rw-r--r--   0        0        0   613433 2024-05-06 18:52:31.286465 tm_devices-1.4.1/src/tm_devices/commands/gen_7s6wr5_smu/status.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.286465 tm_devices-1.4.1/src/tm_devices/commands/gen_8ojdkz_smu/__init__.py
+-rw-r--r--   0        0        0    55384 2024-05-06 18:52:31.286465 tm_devices-1.4.1/src/tm_devices/commands/gen_8ojdkz_smu/display.py
+-rw-r--r--   0        0        0     3812 2024-05-06 18:52:31.286465 tm_devices-1.4.1/src/tm_devices/commands/gen_8ojdkz_smu/node.py
+-rw-r--r--   0        0        0   297756 2024-05-06 18:52:31.286465 tm_devices-1.4.1/src/tm_devices/commands/gen_8ojdkz_smu/smux.py
+-rw-r--r--   0        0        0   618736 2024-05-06 18:52:31.286465 tm_devices-1.4.1/src/tm_devices/commands/gen_8ojdkz_smu/status.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.286465 tm_devices-1.4.1/src/tm_devices/commands/gen_8wm55i_smu/__init__.py
+-rw-r--r--   0        0        0   304522 2024-05-06 18:52:31.286465 tm_devices-1.4.1/src/tm_devices/commands/gen_8wm55i_smu/smux.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.286465 tm_devices-1.4.1/src/tm_devices/commands/gen_9kezla_smu/__init__.py
+-rw-r--r--   0        0        0   303892 2024-05-06 18:52:31.286465 tm_devices-1.4.1/src/tm_devices/commands/gen_9kezla_smu/smux.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.286465 tm_devices-1.4.1/src/tm_devices/commands/gen_9mzp2j_smu/__init__.py
+-rw-r--r--   0        0        0    25789 2024-05-06 18:52:31.286465 tm_devices-1.4.1/src/tm_devices/commands/gen_9mzp2j_smu/digio.py
+-rw-r--r--   0        0        0    55526 2024-05-06 18:52:31.286465 tm_devices-1.4.1/src/tm_devices/commands/gen_9mzp2j_smu/display.py
+-rw-r--r--   0        0        0    34661 2024-05-06 18:52:31.286465 tm_devices-1.4.1/src/tm_devices/commands/gen_9mzp2j_smu/tsplink.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.286465 tm_devices-1.4.1/src/tm_devices/commands/gen_9ncc6e_smu/__init__.py
+-rw-r--r--   0        0        0    50411 2024-05-06 18:52:31.290464 tm_devices-1.4.1/src/tm_devices/commands/gen_9ncc6e_smu/display.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.290464 tm_devices-1.4.1/src/tm_devices/commands/gen_9nnkq7_smu/__init__.py
+-rw-r--r--   0        0        0   583623 2024-05-06 18:52:31.290464 tm_devices-1.4.1/src/tm_devices/commands/gen_9nnkq7_smu/status.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.290464 tm_devices-1.4.1/src/tm_devices/commands/gen_9slyux_smu/__init__.py
+-rw-r--r--   0        0        0   614560 2024-05-06 18:52:31.290464 tm_devices-1.4.1/src/tm_devices/commands/gen_9slyux_smu/status.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.290464 tm_devices-1.4.1/src/tm_devices/commands/gen_ahkybr_smu/__init__.py
+-rw-r--r--   0        0        0     4640 2024-05-06 18:52:31.290464 tm_devices-1.4.1/src/tm_devices/commands/gen_ahkybr_smu/beeper.py
+-rw-r--r--   0        0        0    41300 2024-05-06 18:52:31.290464 tm_devices-1.4.1/src/tm_devices/commands/gen_ahkybr_smu/buffervar.py
+-rw-r--r--   0        0        0    11124 2024-05-06 18:52:31.290464 tm_devices-1.4.1/src/tm_devices/commands/gen_ahkybr_smu/eventlog.py
+-rw-r--r--   0        0        0    90987 2024-05-06 18:52:31.290464 tm_devices-1.4.1/src/tm_devices/commands/gen_ahkybr_smu/lan.py
+-rw-r--r--   0        0        0     4062 2024-05-06 18:52:31.290464 tm_devices-1.4.1/src/tm_devices/commands/gen_ahkybr_smu/os.py
+-rw-r--r--   0        0        0     8610 2024-05-06 18:52:31.290464 tm_devices-1.4.1/src/tm_devices/commands/gen_ahkybr_smu/script.py
+-rw-r--r--   0        0        0    12291 2024-05-06 18:52:31.290464 tm_devices-1.4.1/src/tm_devices/commands/gen_ahkybr_smu/scriptvar.py
+-rw-r--r--   0        0        0     5290 2024-05-06 18:52:31.290464 tm_devices-1.4.1/src/tm_devices/commands/gen_ahkybr_smu/setup_1.py
+-rw-r--r--   0        0        0    23587 2024-05-06 18:52:31.290464 tm_devices-1.4.1/src/tm_devices/commands/gen_ahkybr_smu/tspnet.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.290464 tm_devices-1.4.1/src/tm_devices/commands/gen_aih9e2_smu/__init__.py
+-rw-r--r--   0        0        0    36289 2024-05-06 18:52:31.290464 tm_devices-1.4.1/src/tm_devices/commands/gen_aih9e2_smu/trigger.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.290464 tm_devices-1.4.1/src/tm_devices/commands/gen_ak4990_smu/__init__.py
+-rw-r--r--   0        0        0   304272 2024-05-06 18:52:31.290464 tm_devices-1.4.1/src/tm_devices/commands/gen_ak4990_smu/smux.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.290464 tm_devices-1.4.1/src/tm_devices/commands/gen_am6pcr_smu/__init__.py
+-rw-r--r--   0        0        0   278566 2024-05-06 18:52:31.290464 tm_devices-1.4.1/src/tm_devices/commands/gen_am6pcr_smu/smux.py
+-rw-r--r--   0        0        0   623556 2024-05-06 18:52:31.290464 tm_devices-1.4.1/src/tm_devices/commands/gen_am6pcr_smu/status.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_amm5lc_smu/__init__.py
+-rw-r--r--   0        0        0    31321 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_amm5lc_smu/digio.py
+-rw-r--r--   0        0        0    37909 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_amm5lc_smu/tsplink.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_aostep_smu/__init__.py
+-rw-r--r--   0        0        0    13800 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_aostep_smu/serial.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_aqr1t1_smu/__init__.py
+-rw-r--r--   0        0        0    27960 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_aqr1t1_smu/localnode.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_as1ejq_smu/__init__.py
+-rw-r--r--   0        0        0    25146 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_as1ejq_smu/localnode.py
+-rw-r--r--   0        0        0   275978 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_as1ejq_smu/smux.py
+-rw-r--r--   0        0        0   635702 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_as1ejq_smu/status.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_at7jl1_smu/__init__.py
+-rw-r--r--   0        0        0    55816 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_at7jl1_smu/display.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_au597k_smu/__init__.py
+-rw-r--r--   0        0        0    29997 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_au597k_smu/digio.py
+-rw-r--r--   0        0        0    14069 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_au597k_smu/format.py
+-rw-r--r--   0        0        0    36102 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_au597k_smu/tsplink.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_auyr50_smu/__init__.py
+-rw-r--r--   0        0        0    13354 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_auyr50_smu/format.py
+-rw-r--r--   0        0        0    28034 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_auyr50_smu/localnode.py
+-rw-r--r--   0        0        0     4117 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_auyr50_smu/node.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_avh0iw_smu/__init__.py
+-rw-r--r--   0        0        0    51741 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_avh0iw_smu/display.py
+-rw-r--r--   0        0        0    35047 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_avh0iw_smu/trigger.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_awhjao_smu/__init__.py
+-rw-r--r--   0        0        0   628261 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_awhjao_smu/status.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_by991s_smudaq/__init__.py
+-rw-r--r--   0        0        0    12283 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_by991s_smudaq/digio.py
+-rw-r--r--   0        0        0    31576 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_by991s_smudaq/status.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_canxny_daq/__init__.py
+-rw-r--r--   0        0        0    36287 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_canxny_daq/buffer.py
+-rw-r--r--   0        0        0    34903 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_canxny_daq/buffervar.py
+-rw-r--r--   0        0        0    38415 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_canxny_daq/channel.py
+-rw-r--r--   0        0        0    35222 2024-05-06 18:52:31.294465 tm_devices-1.4.1/src/tm_devices/commands/gen_canxny_daq/display.py
+-rw-r--r--   0        0        0   318520 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_canxny_daq/dmm.py
+-rw-r--r--   0        0        0    57952 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_canxny_daq/scan.py
+-rw-r--r--   0        0        0    32594 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_canxny_daq/slot.py
+-rw-r--r--   0        0        0   201599 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_canxny_daq/trigger.py
+-rw-r--r--   0        0        0    16778 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_canxny_daq/tsplink.py
+-rw-r--r--   0        0        0     2473 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_canxny_daq/upgrade.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_d6b496_dmm/__init__.py
+-rw-r--r--   0        0        0    11150 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_d6b496_dmm/acal.py
+-rw-r--r--   0        0        0    28019 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_d6b496_dmm/buffer.py
+-rw-r--r--   0        0        0    32622 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_d6b496_dmm/buffervar.py
+-rw-r--r--   0        0        0    30425 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_d6b496_dmm/display.py
+-rw-r--r--   0        0        0   250833 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_d6b496_dmm/dmm.py
+-rw-r--r--   0        0        0     3182 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_d6b496_dmm/fan.py
+-rw-r--r--   0        0        0    23204 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_d6b496_dmm/localnode.py
+-rw-r--r--   0        0        0   195016 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_d6b496_dmm/trigger.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_d83qe0_dmm/__init__.py
+-rw-r--r--   0        0        0    31410 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_d83qe0_dmm/buffer.py
+-rw-r--r--   0        0        0    34053 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_d83qe0_dmm/buffervar.py
+-rw-r--r--   0        0        0    17456 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_d83qe0_dmm/channel.py
+-rw-r--r--   0        0        0    33229 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_d83qe0_dmm/display.py
+-rw-r--r--   0        0        0   196568 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_d83qe0_dmm/dmm.py
+-rw-r--r--   0        0        0    51560 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_d83qe0_dmm/scan.py
+-rw-r--r--   0        0        0     8718 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_d83qe0_dmm/slot.py
+-rw-r--r--   0        0        0   192379 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_d83qe0_dmm/trigger.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_dawv9y_smudaqdmm/__init__.py
+-rw-r--r--   0        0        0    22079 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_dawv9y_smudaqdmm/localnode.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/__init__.py
+-rw-r--r--   0        0        0     1803 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/beeper.py
+-rw-r--r--   0        0        0     7528 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/eventlog.py
+-rw-r--r--   0        0        0     9275 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/file.py
+-rw-r--r--   0        0        0    11990 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/format.py
+-rw-r--r--   0        0        0     8492 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/lan.py
+-rw-r--r--   0        0        0     4238 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/scriptvar.py
+-rw-r--r--   0        0        0     2547 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/timer.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_dbqd7k_dmm/__init__.py
+-rw-r--r--   0        0        0    11902 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_dbqd7k_dmm/digio.py
+-rw-r--r--   0        0        0     3837 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_dbqd7k_dmm/node.py
+-rw-r--r--   0        0        0    28175 2024-05-06 18:52:31.298465 tm_devices-1.4.1/src/tm_devices/commands/gen_dbqd7k_dmm/status.py
+-rw-r--r--   0        0        0    16823 2024-05-06 18:52:31.302465 tm_devices-1.4.1/src/tm_devices/commands/gen_dbqd7k_dmm/tsplink.py
+-rw-r--r--   0        0        0    22886 2024-05-06 18:52:31.302465 tm_devices-1.4.1/src/tm_devices/commands/gen_dbqd7k_dmm/tspnet.py
+-rw-r--r--   0        0        0     2466 2024-05-06 18:52:31.302465 tm_devices-1.4.1/src/tm_devices/commands/gen_dbqd7k_dmm/upgrade.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.302465 tm_devices-1.4.1/src/tm_devices/commands/gen_dcpheg_daqdmm/__init__.py
+-rw-r--r--   0        0        0     1493 2024-05-06 18:52:31.302465 tm_devices-1.4.1/src/tm_devices/commands/gen_dcpheg_daqdmm/smu.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.302465 tm_devices-1.4.1/src/tm_devices/commands/gen_dd4xnb_smudaqdmm/__init__.py
+-rw-r--r--   0        0        0     2881 2024-05-06 18:52:31.302465 tm_devices-1.4.1/src/tm_devices/commands/gen_dd4xnb_smudaqdmm/script.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.302465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/__init__.py
+-rw-r--r--   0        0        0    41892 2024-05-06 18:52:31.302465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/acquire.py
+-rw-r--r--   0        0        0   130167 2024-05-06 18:52:31.302465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/actonevent.py
+-rw-r--r--   0        0        0     2689 2024-05-06 18:52:31.302465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/application.py
+-rw-r--r--   0        0        0     5019 2024-05-06 18:52:31.302465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/auxout.py
+-rw-r--r--   0        0        0   949605 2024-05-06 18:52:31.302465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/bus.py
+-rw-r--r--   0        0        0    35014 2024-05-06 18:52:31.302465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/callouts.py
+-rw-r--r--   0        0        0   162423 2024-05-06 18:52:31.302465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/ch.py
+-rw-r--r--   0        0        0    37622 2024-05-06 18:52:31.302465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/data.py
+-rw-r--r--   0        0        0    16839 2024-05-06 18:52:31.302465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/diag.py
+-rw-r--r--   0        0        0     5110 2024-05-06 18:52:31.302465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/diggrp.py
+-rw-r--r--   0        0        0   685976 2024-05-06 18:52:31.302465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/display.py
+-rw-r--r--   0        0        0    25348 2024-05-06 18:52:31.302465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/dvm.py
+-rw-r--r--   0        0        0    28233 2024-05-06 18:52:31.302465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/eyemask.py
+-rw-r--r--   0        0        0     8919 2024-05-06 18:52:31.302465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/fpanel.py
+-rw-r--r--   0        0        0    74061 2024-05-06 18:52:31.306465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/histogram.py
+-rw-r--r--   0        0        0   124292 2024-05-06 18:52:31.306465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/horizontal.py
+-rw-r--r--   0        0        0    17319 2024-05-06 18:52:31.306465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/license.py
+-rw-r--r--   0        0        0    53760 2024-05-06 18:52:31.306465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/mask.py
+-rw-r--r--   0        0        0   229865 2024-05-06 18:52:31.306465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/math.py
+-rw-r--r--   0        0        0     3469 2024-05-06 18:52:31.306465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/matharbflt.py
+-rw-r--r--   0        0        0  1409304 2024-05-06 18:52:31.306465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/measurement.py
+-rw-r--r--   0        0        0     8831 2024-05-06 18:52:31.306465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/peakstable.py
+-rw-r--r--   0        0        0     5944 2024-05-06 18:52:31.306465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/pilogger.py
+-rw-r--r--   0        0        0    99309 2024-05-06 18:52:31.306465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/plot.py
+-rw-r--r--   0        0        0   842344 2024-05-06 18:52:31.306465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/power.py
+-rw-r--r--   0        0        0    80340 2024-05-06 18:52:31.310465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/ref.py
+-rw-r--r--   0        0        0     5139 2024-05-06 18:52:31.310465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/rosc.py
+-rw-r--r--   0        0        0    53395 2024-05-06 18:52:31.310465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/save.py
+-rw-r--r--   0        0        0    22709 2024-05-06 18:52:31.310465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/saveon.py
+-rw-r--r--   0        0        0    15515 2024-05-06 18:52:31.310465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/saveonevent.py
+-rw-r--r--   0        0        0  2492066 2024-05-06 18:52:31.310465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/search.py
+-rw-r--r--   0        0        0     5403 2024-05-06 18:52:31.314465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/searchtable.py
+-rw-r--r--   0        0        0     3863 2024-05-06 18:52:31.314465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/select.py
+-rw-r--r--   0        0        0   135335 2024-05-06 18:52:31.314465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/sv.py
+-rw-r--r--   0        0        0     4879 2024-05-06 18:52:31.314465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/touchscreen.py
+-rw-r--r--   0        0        0  1714107 2024-05-06 18:52:31.314465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/trigger.py
+-rw-r--r--   0        0        0     4743 2024-05-06 18:52:31.314465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/tstamptable.py
+-rw-r--r--   0        0        0    47508 2024-05-06 18:52:31.314465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/visual.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.314465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/__init__.py
+-rw-r--r--   0        0        0    43920 2024-05-06 18:52:31.314465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/afg.py
+-rw-r--r--   0        0        0     1437 2024-05-06 18:52:31.314465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/autosavepitimeout.py
+-rw-r--r--   0        0        0     1429 2024-05-06 18:52:31.314465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/autosaveuitimeout.py
+-rw-r--r--   0        0        0    20778 2024-05-06 18:52:31.314465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/autoset.py
+-rw-r--r--   0        0        0     4738 2024-05-06 18:52:31.314465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/bustable.py
+-rw-r--r--   0        0        0     7206 2024-05-06 18:52:31.314465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/calibrate.py
+-rw-r--r--   0        0        0     3708 2024-05-06 18:52:31.314465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/configuration.py
+-rw-r--r--   0        0        0    13730 2024-05-06 18:52:31.314465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/connected.py
+-rw-r--r--   0        0        0     4367 2024-05-06 18:52:31.314465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/curve.py
+-rw-r--r--   0        0        0     2854 2024-05-06 18:52:31.314465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/curvestream.py
+-rw-r--r--   0        0        0     4916 2024-05-06 18:52:31.314465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/customtable.py
+-rw-r--r--   0        0        0     1050 2024-05-06 18:52:31.314465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/date.py
+-rw-r--r--   0        0        0    32195 2024-05-06 18:52:31.314465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/ethernet.py
+-rw-r--r--   0        0        0    40419 2024-05-06 18:52:31.314465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/filesystem.py
+-rw-r--r--   0        0        0     6444 2024-05-06 18:52:31.314465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/mainwindow.py
+-rw-r--r--   0        0        0     3716 2024-05-06 18:52:31.314465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/meastable.py
+-rw-r--r--   0        0        0     8484 2024-05-06 18:52:31.314465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/recall.py
+-rw-r--r--   0        0        0     8465 2024-05-06 18:52:31.314465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/socketserver.py
+-rw-r--r--   0        0        0     6072 2024-05-06 18:52:31.314465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/time.py
+-rw-r--r--   0        0        0      958 2024-05-06 18:52:31.314465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/undo.py
+-rw-r--r--   0        0        0     3627 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/usbdevice.py
+-rw-r--r--   0        0        0    15172 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/vertical.py
+-rw-r--r--   0        0        0    48263 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/wfmoutpre.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/__init__.py
+-rw-r--r--   0        0        0     4266 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/beeper.py
+-rw-r--r--   0        0        0    36070 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/buffervar.py
+-rw-r--r--   0        0        0    69159 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/channel.py
+-rw-r--r--   0        0        0    20278 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/comm.py
+-rw-r--r--   0        0        0    24474 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/digio.py
+-rw-r--r--   0        0        0    25306 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/display.py
+-rw-r--r--   0        0        0   152544 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/dmm.py
+-rw-r--r--   0        0        0    10688 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/eventlog.py
+-rw-r--r--   0        0        0    10200 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/format.py
+-rw-r--r--   0        0        0    73653 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/lan.py
+-rw-r--r--   0        0        0    25565 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/localnode.py
+-rw-r--r--   0        0        0     2816 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/memory.py
+-rw-r--r--   0        0        0     1817 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/os.py
+-rw-r--r--   0        0        0    15065 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/ptp.py
+-rw-r--r--   0        0        0    48486 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/scan.py
+-rw-r--r--   0        0        0    21067 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/schedule.py
+-rw-r--r--   0        0        0     8315 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/script.py
+-rw-r--r--   0        0        0    10591 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/scriptvar.py
+-rw-r--r--   0        0        0     5436 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/setup_1.py
+-rw-r--r--   0        0        0    30730 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/slot.py
+-rw-r--r--   0        0        0   125084 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/status.py
+-rw-r--r--   0        0        0    33767 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/trigger.py
+-rw-r--r--   0        0        0    32863 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/tsplink.py
+-rw-r--r--   0        0        0     2483 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/upgrade.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e4de2d_lpdmsomdo/__init__.py
+-rw-r--r--   0        0        0      928 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e4de2d_lpdmsomdo/clear.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e6606z_lpdmsomdodpo/__init__.py
+-rw-r--r--   0        0        0     1296 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e6606z_lpdmsomdodpo/pause.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e6lgg1_lpdmsodpomdo/__init__.py
+-rw-r--r--   0        0        0     1313 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e6lgg1_lpdmsodpomdo/totaluptime.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e7aqno_smudaqss/__init__.py
+-rw-r--r--   0        0        0     3893 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_e7aqno_smudaqss/node.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_eat5s3_smudaqdmmss/__init__.py
+-rw-r--r--   0        0        0     5522 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_eat5s3_smudaqdmmss/dataqueue.py
+-rw-r--r--   0        0        0     7625 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_eat5s3_smudaqdmmss/fs.py
+-rw-r--r--   0        0        0     3970 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_eat5s3_smudaqdmmss/userstring.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_ed9nkc_daqss/__init__.py
+-rw-r--r--   0        0        0    23101 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_ed9nkc_daqss/tspnet.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_efap3f_smuss/__init__.py
+-rw-r--r--   0        0        0    11856 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_efap3f_smuss/bit.py
+-rw-r--r--   0        0        0     3765 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_efap3f_smuss/errorqueue.py
+-rw-r--r--   0        0        0     9696 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_efap3f_smuss/io.py
+-rw-r--r--   0        0        0     3063 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_efap3f_smuss/timer.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_eg5ll2_smudaqdmmss/__init__.py
+-rw-r--r--   0        0        0     3409 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_eg5ll2_smudaqdmmss/gpib.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_ffz2xs_dpodsamso/__init__.py
+-rw-r--r--   0        0        0   286772 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_ffz2xs_dpodsamso/bus.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_fhrp27_msodpomdodsa/__init__.py
+-rw-r--r--   0        0        0     3441 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_fhrp27_msodpomdodsa/curve.py
+-rw-r--r--   0        0        0     1641 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_fhrp27_msodpomdodsa/date.py
+-rw-r--r--   0        0        0     4241 2024-05-06 18:52:31.318465 tm_devices-1.4.1/src/tm_devices/commands/gen_fhrp27_msodpomdodsa/mathvar.py
+-rw-r--r--   0        0        0     2201 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fhrp27_msodpomdodsa/save_and_recall.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/__init__.py
+-rw-r--r--   0        0        0    41898 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/acquire.py
+-rw-r--r--   0        0        0     4042 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/allocate.py
+-rw-r--r--   0        0        0     6660 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/application.py
+-rw-r--r--   0        0        0     4703 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/autoset.py
+-rw-r--r--   0        0        0    67957 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/auxin.py
+-rw-r--r--   0        0        0     6172 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/auxout.py
+-rw-r--r--   0        0        0     1026 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/bell.py
+-rw-r--r--   0        0        0    16111 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/calibrate.py
+-rw-r--r--   0        0        0   143892 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/ch.py
+-rw-r--r--   0        0        0      983 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/clear.py
+-rw-r--r--   0        0        0     1992 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/cmdbatch.py
+-rw-r--r--   0        0        0     2987 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/cq.py
+-rw-r--r--   0        0        0    86089 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/cursor.py
+-rw-r--r--   0        0        0     1636 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/curvenext.py
+-rw-r--r--   0        0        0     3015 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/curvestream.py
+-rw-r--r--   0        0        0     8707 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/custom.py
+-rw-r--r--   0        0        0    12219 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/d.py
+-rw-r--r--   0        0        0    30249 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/data.py
+-rw-r--r--   0        0        0     5294 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/delete.py
+-rw-r--r--   0        0        0    59925 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/diag.py
+-rw-r--r--   0        0        0   139335 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/display.py
+-rw-r--r--   0        0        0    41283 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/email.py
+-rw-r--r--   0        0        0    12662 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/export.py
+-rw-r--r--   0        0        0     6134 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/fastacq.py
+-rw-r--r--   0        0        0    24502 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/filesystem.py
+-rw-r--r--   0        0        0     5528 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/gpibusb.py
+-rw-r--r--   0        0        0    17838 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/hardcopy.py
+-rw-r--r--   0        0        0     1903 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/hdr.py
+-rw-r--r--   0        0        0    28803 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/histogram.py
+-rw-r--r--   0        0        0   233302 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/horizontal.py
+-rw-r--r--   0        0        0    60154 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/limit.py
+-rw-r--r--   0        0        0    28385 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/mark.py
+-rw-r--r--   0        0        0   282367 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/mask.py
+-rw-r--r--   0        0        0    88338 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/math.py
+-rw-r--r--   0        0        0     4906 2024-05-06 18:52:31.322465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/matharbflt.py
+-rw-r--r--   0        0        0    21243 2024-05-06 18:52:31.326465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/mch.py
+-rw-r--r--   0        0        0   240397 2024-05-06 18:52:31.326465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/measurement.py
+-rw-r--r--   0        0        0     7200 2024-05-06 18:52:31.326465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/multiscope.py
+-rw-r--r--   0        0        0     4110 2024-05-06 18:52:31.326465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/opcextended.py
+-rw-r--r--   0        0        0     1326 2024-05-06 18:52:31.326465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/pcenable.py
+-rw-r--r--   0        0        0    11013 2024-05-06 18:52:31.326465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/recall.py
+-rw-r--r--   0        0        0    25927 2024-05-06 18:52:31.326465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/ref.py
+-rw-r--r--   0        0        0    28115 2024-05-06 18:52:31.326465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/save.py
+-rw-r--r--   0        0        0     1466 2024-05-06 18:52:31.326465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/save_and_recall.py
+-rw-r--r--   0        0        0    42097 2024-05-06 18:52:31.326465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/saveon.py
+-rw-r--r--   0        0        0  1314240 2024-05-06 18:52:31.326465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/search.py
+-rw-r--r--   0        0        0    24294 2024-05-06 18:52:31.326465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/select.py
+-rw-r--r--   0        0        0     3069 2024-05-06 18:52:31.326465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/setup_1.py
+-rw-r--r--   0        0        0     2945 2024-05-06 18:52:31.326465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/system.py
+-rw-r--r--   0        0        0     4521 2024-05-06 18:52:31.326465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/teklink.py
+-rw-r--r--   0        0        0     6698 2024-05-06 18:52:31.326465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/test.py
+-rw-r--r--   0        0        0     5298 2024-05-06 18:52:31.326465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/trig.py
+-rw-r--r--   0        0        0    12636 2024-05-06 18:52:31.326465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/usbtmc.py
+-rw-r--r--   0        0        0    44201 2024-05-06 18:52:31.326465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/visual.py
+-rw-r--r--   0        0        0     1540 2024-05-06 18:52:31.326465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/wavfrmstream.py
+-rw-r--r--   0        0        0    43700 2024-05-06 18:52:31.326465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/wfminpre.py
+-rw-r--r--   0        0        0    38216 2024-05-06 18:52:31.326465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/wfmoutpre.py
+-rw-r--r--   0        0        0     2344 2024-05-06 18:52:31.326465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/wfmpre.py
+-rw-r--r--   0        0        0   145020 2024-05-06 18:52:31.326465 tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/zoom.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.326465 tm_devices-1.4.1/src/tm_devices/commands/gen_fkjfe8_msodpodsa/__init__.py
+-rw-r--r--   0        0        0     1739 2024-05-06 18:52:31.326465 tm_devices-1.4.1/src/tm_devices/commands/gen_fkjfe8_msodpodsa/time.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.326465 tm_devices-1.4.1/src/tm_devices/commands/gen_fn2qbf_msodpo/__init__.py
+-rw-r--r--   0        0        0   234734 2024-05-06 18:52:31.326465 tm_devices-1.4.1/src/tm_devices/commands/gen_fn2qbf_msodpo/errordetector.py
+-rw-r--r--   0        0        0  1544101 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fn2qbf_msodpo/trigger.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fpx9s1_dpodsamso/__init__.py
+-rw-r--r--   0        0        0    14139 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fpx9s1_dpodsamso/counter.py
+-rw-r--r--   0        0        0    30331 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fpx9s1_dpodsamso/linktraining.py
+-rw-r--r--   0        0        0    11549 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fpx9s1_dpodsamso/rosc.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_ft5uww_lpdmsodpomdoafgawgdsa/__init__.py
+-rw-r--r--   0        0        0     1403 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_ft5uww_lpdmsodpomdoafgawgdsa/calibration.py
+-rw-r--r--   0        0        0     2445 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_ft5uww_lpdmsodpomdoafgawgdsa/miscellaneous.py
+-rw-r--r--   0        0        0     8131 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_ft5uww_lpdmsodpomdoafgawgdsa/status_and_error.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fteabn_lpdmsomdodpoafgawgdsa/__init__.py
+-rw-r--r--   0        0        0     1653 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fteabn_lpdmsomdodpoafgawgdsa/status_and_error.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fug7nl_lpdmsodpomdoawgdsa/__init__.py
+-rw-r--r--   0        0        0     3041 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fug7nl_lpdmsodpomdoawgdsa/status_and_error.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fuzvln_lpdmsodpodsa/__init__.py
+-rw-r--r--   0        0        0    12102 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fuzvln_lpdmsodpodsa/alias.py
+-rw-r--r--   0        0        0     2110 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fuzvln_lpdmsodpodsa/header.py
+-rw-r--r--   0        0        0     2422 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fuzvln_lpdmsodpodsa/status_and_error.py
+-rw-r--r--   0        0        0     1512 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fuzvln_lpdmsodpodsa/verbose.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/__init__.py
+-rw-r--r--   0        0        0     1554 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/allev.py
+-rw-r--r--   0        0        0     1380 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/busy.py
+-rw-r--r--   0        0        0     2051 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/dese.py
+-rw-r--r--   0        0        0     1432 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/event.py
+-rw-r--r--   0        0        0     1462 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/evmsg.py
+-rw-r--r--   0        0        0     1426 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/evqty.py
+-rw-r--r--   0        0        0     1802 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/factory.py
+-rw-r--r--   0        0        0     1424 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/id.py
+-rw-r--r--   0        0        0     3148 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/miscellaneous.py
+-rw-r--r--   0        0        0     1462 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/newpass.py
+-rw-r--r--   0        0        0     1947 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/password.py
+-rw-r--r--   0        0        0     1427 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/rem.py
+-rw-r--r--   0        0        0     1880 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/set.py
+-rw-r--r--   0        0        0     1783 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/status_and_error.py
+-rw-r--r--   0        0        0     1438 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/teksecure.py
+-rw-r--r--   0        0        0     1488 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/wavfrm.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fzn174_lpdmsodpomdodsa/__init__.py
+-rw-r--r--   0        0        0     2360 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fzn174_lpdmsodpomdodsa/lock.py
+-rw-r--r--   0        0        0     1403 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_fzn174_lpdmsodpomdodsa/unlock.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/__init__.py
+-rw-r--r--   0        0        0    18509 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/acquire.py
+-rw-r--r--   0        0        0    10925 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/alias.py
+-rw-r--r--   0        0        0     2961 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/autoset.py
+-rw-r--r--   0        0        0    23027 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/auxin.py
+-rw-r--r--   0        0        0   179853 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/bus.py
+-rw-r--r--   0        0        0    17740 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/calibrate.py
+-rw-r--r--   0        0        0    53778 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/ch.py
+-rw-r--r--   0        0        0    76450 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/cursor.py
+-rw-r--r--   0        0        0     7660 2024-05-06 18:52:31.330465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/d.py
+-rw-r--r--   0        0        0    29317 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/data.py
+-rw-r--r--   0        0        0    25433 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/diag.py
+-rw-r--r--   0        0        0    31518 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/display.py
+-rw-r--r--   0        0        0    26251 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/ethernet.py
+-rw-r--r--   0        0        0    22162 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/filesystem.py
+-rw-r--r--   0        0        0     4958 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/filtervu.py
+-rw-r--r--   0        0        0     8169 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/fpanel.py
+-rw-r--r--   0        0        0     2368 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/gpibusb.py
+-rw-r--r--   0        0        0    20476 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/hardcopy.py
+-rw-r--r--   0        0        0    43301 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/horizontal.py
+-rw-r--r--   0        0        0    22328 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/mark.py
+-rw-r--r--   0        0        0    44629 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/math1.py
+-rw-r--r--   0        0        0   142818 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/measurement.py
+-rw-r--r--   0        0        0    17180 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/pictbridge.py
+-rw-r--r--   0        0        0     6558 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/recall.py
+-rw-r--r--   0        0        0    23375 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/ref.py
+-rw-r--r--   0        0        0    31179 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/save.py
+-rw-r--r--   0        0        0   446842 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/search.py
+-rw-r--r--   0        0        0    16968 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/select.py
+-rw-r--r--   0        0        0   442210 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/trigger.py
+-rw-r--r--   0        0        0    44738 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/wfminpre.py
+-rw-r--r--   0        0        0    44636 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/wfmoutpre.py
+-rw-r--r--   0        0        0    18830 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/zoom.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/__init__.py
+-rw-r--r--   0        0        0    34225 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/acquire.py
+-rw-r--r--   0        0        0    82260 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/configuration.py
+-rw-r--r--   0        0        0    80849 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/cursor.py
+-rw-r--r--   0        0        0     3011 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/deskew.py
+-rw-r--r--   0        0        0    47590 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/display.py
+-rw-r--r--   0        0        0     7928 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/lock.py
+-rw-r--r--   0        0        0   150766 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/mask.py
+-rw-r--r--   0        0        0   193055 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/measurement.py
+-rw-r--r--   0        0        0    23425 2024-05-06 18:52:31.334465 tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/message.py
+-rw-r--r--   0        0        0    10363 2024-05-06 18:52:31.338465 tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/recall.py
+-rw-r--r--   0        0        0   171778 2024-05-06 18:52:31.338465 tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/rf.py
+-rw-r--r--   0        0        0     2877 2024-05-06 18:52:31.338465 tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/rrb.py
+-rw-r--r--   0        0        0   745139 2024-05-06 18:52:31.338465 tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/search.py
+-rw-r--r--   0        0        0    32522 2024-05-06 18:52:31.338465 tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/select.py
+-rw-r--r--   0        0        0     5235 2024-05-06 18:52:31.338465 tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/setup1.py
+-rw-r--r--   0        0        0   716529 2024-05-06 18:52:31.338465 tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/trigger.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.338465 tm_devices-1.4.1/src/tm_devices/commands/gen_usaa3_mdo/__init__.py
+-rw-r--r--   0        0        0   185741 2024-05-06 18:52:31.338465 tm_devices-1.4.1/src/tm_devices/commands/gen_usaa3_mdo/rf.py
+-rw-r--r--   0        0        0   771669 2024-05-06 18:52:31.338465 tm_devices-1.4.1/src/tm_devices/commands/gen_usaa3_mdo/search.py
+-rw-r--r--   0        0        0   749699 2024-05-06 18:52:31.338465 tm_devices-1.4.1/src/tm_devices/commands/gen_usaa3_mdo/trigger.py
+-rw-r--r--   0        0        0      878 2024-05-06 18:52:31.342465 tm_devices-1.4.1/src/tm_devices/commands/helpers/__init__.py
+-rw-r--r--   0        0        0     5009 2024-05-06 18:52:31.342465 tm_devices-1.4.1/src/tm_devices/commands/helpers/generic_commands.py
+-rw-r--r--   0        0        0    14623 2024-05-06 18:52:31.342465 tm_devices-1.4.1/src/tm_devices/commands/helpers/scpi_commands.py
+-rw-r--r--   0        0        0     1832 2024-05-06 18:52:31.342465 tm_devices-1.4.1/src/tm_devices/commands/helpers/tsp_commands.py
+-rw-r--r--   0        0        0   150973 2024-05-06 18:52:31.342465 tm_devices-1.4.1/src/tm_devices/commands/lpd6_commands.py
+-rw-r--r--   0        0        0   129766 2024-05-06 18:52:31.342465 tm_devices-1.4.1/src/tm_devices/commands/mdo3_commands.py
+-rw-r--r--   0        0        0   130785 2024-05-06 18:52:31.342465 tm_devices-1.4.1/src/tm_devices/commands/mdo3k_commands.py
+-rw-r--r--   0        0        0   131141 2024-05-06 18:52:31.342465 tm_devices-1.4.1/src/tm_devices/commands/mdo4k_commands.py
+-rw-r--r--   0        0        0   130948 2024-05-06 18:52:31.342465 tm_devices-1.4.1/src/tm_devices/commands/mdo4kb_commands.py
+-rw-r--r--   0        0        0   131209 2024-05-06 18:52:31.342465 tm_devices-1.4.1/src/tm_devices/commands/mdo4kc_commands.py
+-rw-r--r--   0        0        0   116295 2024-05-06 18:52:31.342465 tm_devices-1.4.1/src/tm_devices/commands/mso2_commands.py
+-rw-r--r--   0        0        0   105183 2024-05-06 18:52:31.342465 tm_devices-1.4.1/src/tm_devices/commands/mso2k_commands.py
+-rw-r--r--   0        0        0   105202 2024-05-06 18:52:31.342465 tm_devices-1.4.1/src/tm_devices/commands/mso2kb_commands.py
+-rw-r--r--   0        0        0   150973 2024-05-06 18:52:31.342465 tm_devices-1.4.1/src/tm_devices/commands/mso4_commands.py
+-rw-r--r--   0        0        0   150992 2024-05-06 18:52:31.342465 tm_devices-1.4.1/src/tm_devices/commands/mso4b_commands.py
+-rw-r--r--   0        0        0   131009 2024-05-06 18:52:31.342465 tm_devices-1.4.1/src/tm_devices/commands/mso4k_commands.py
+-rw-r--r--   0        0        0   131083 2024-05-06 18:52:31.342465 tm_devices-1.4.1/src/tm_devices/commands/mso4kb_commands.py
+-rw-r--r--   0        0        0   150973 2024-05-06 18:52:31.342465 tm_devices-1.4.1/src/tm_devices/commands/mso5_commands.py
+-rw-r--r--   0        0        0   150992 2024-05-06 18:52:31.342465 tm_devices-1.4.1/src/tm_devices/commands/mso5b_commands.py
+-rw-r--r--   0        0        0   154860 2024-05-06 18:52:31.342465 tm_devices-1.4.1/src/tm_devices/commands/mso5k_commands.py
+-rw-r--r--   0        0        0   159850 2024-05-06 18:52:31.342465 tm_devices-1.4.1/src/tm_devices/commands/mso5kb_commands.py
+-rw-r--r--   0        0        0   151011 2024-05-06 18:52:31.342465 tm_devices-1.4.1/src/tm_devices/commands/mso5lp_commands.py
+-rw-r--r--   0        0        0   150973 2024-05-06 18:52:31.342465 tm_devices-1.4.1/src/tm_devices/commands/mso6_commands.py
+-rw-r--r--   0        0        0   150992 2024-05-06 18:52:31.346465 tm_devices-1.4.1/src/tm_devices/commands/mso6b_commands.py
+-rw-r--r--   0        0        0   159058 2024-05-06 18:52:31.346465 tm_devices-1.4.1/src/tm_devices/commands/mso70kc_commands.py
+-rw-r--r--   0        0        0   159104 2024-05-06 18:52:31.346465 tm_devices-1.4.1/src/tm_devices/commands/mso70kdx_commands.py
+-rw-r--r--   0        0        0    84668 2024-05-06 18:52:31.346465 tm_devices-1.4.1/src/tm_devices/commands/smu2450_commands.py
+-rw-r--r--   0        0        0    88434 2024-05-06 18:52:31.346465 tm_devices-1.4.1/src/tm_devices/commands/smu2460_commands.py
+-rw-r--r--   0        0        0    88578 2024-05-06 18:52:31.346465 tm_devices-1.4.1/src/tm_devices/commands/smu2461_commands.py
+-rw-r--r--   0        0        0    84757 2024-05-06 18:52:31.346465 tm_devices-1.4.1/src/tm_devices/commands/smu2470_commands.py
+-rw-r--r--   0        0        0   133683 2024-05-06 18:52:31.346465 tm_devices-1.4.1/src/tm_devices/commands/smu2601b_commands.py
+-rw-r--r--   0        0        0    63551 2024-05-06 18:52:31.346465 tm_devices-1.4.1/src/tm_devices/commands/smu2601b_pulse_commands.py
+-rw-r--r--   0        0        0   140431 2024-05-06 18:52:31.346465 tm_devices-1.4.1/src/tm_devices/commands/smu2602b_commands.py
+-rw-r--r--   0        0        0   127767 2024-05-06 18:52:31.346465 tm_devices-1.4.1/src/tm_devices/commands/smu2604b_commands.py
+-rw-r--r--   0        0        0   139285 2024-05-06 18:52:31.346465 tm_devices-1.4.1/src/tm_devices/commands/smu2606b_commands.py
+-rw-r--r--   0        0        0   133503 2024-05-06 18:52:31.346465 tm_devices-1.4.1/src/tm_devices/commands/smu2611b_commands.py
+-rw-r--r--   0        0        0   140251 2024-05-06 18:52:31.346465 tm_devices-1.4.1/src/tm_devices/commands/smu2612b_commands.py
+-rw-r--r--   0        0        0   127587 2024-05-06 18:52:31.346465 tm_devices-1.4.1/src/tm_devices/commands/smu2614b_commands.py
+-rw-r--r--   0        0        0   127740 2024-05-06 18:52:31.346465 tm_devices-1.4.1/src/tm_devices/commands/smu2634b_commands.py
+-rw-r--r--   0        0        0   133656 2024-05-06 18:52:31.346465 tm_devices-1.4.1/src/tm_devices/commands/smu2635b_commands.py
+-rw-r--r--   0        0        0   140404 2024-05-06 18:52:31.346465 tm_devices-1.4.1/src/tm_devices/commands/smu2636b_commands.py
+-rw-r--r--   0        0        0   123159 2024-05-06 18:52:31.346465 tm_devices-1.4.1/src/tm_devices/commands/smu2651a_commands.py
+-rw-r--r--   0        0        0   123084 2024-05-06 18:52:31.346465 tm_devices-1.4.1/src/tm_devices/commands/smu2657a_commands.py
+-rw-r--r--   0        0        0    51307 2024-05-06 18:52:31.346465 tm_devices-1.4.1/src/tm_devices/commands/ss3706a_commands.py
+-rw-r--r--   0        0        0      155 2024-05-06 18:52:31.346465 tm_devices-1.4.1/src/tm_devices/components/__init__.py
+-rw-r--r--   0        0        0    18263 2024-05-06 18:52:31.346465 tm_devices-1.4.1/src/tm_devices/components/dm_config_parser.py
+-rw-r--r--   0        0        0    53954 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/device_manager.py
+-rw-r--r--   0        0        0      176 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/driver_mixins/__init__.py
+-rw-r--r--   0        0        0     6579 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/driver_mixins/analysis_object_mixins.py
+-rw-r--r--   0        0        0     4041 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/driver_mixins/class_extension_mixin.py
+-rw-r--r--   0        0        0      943 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/driver_mixins/licensed_mixin.py
+-rw-r--r--   0        0        0     3048 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/driver_mixins/signal_generator_mixin.py
+-rw-r--r--   0        0        0      540 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/driver_mixins/usb_drives_mixin.py
+-rw-r--r--   0        0        0     9181 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/__init__.py
+-rw-r--r--   0        0        0       55 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/api/__init__.py
+-rw-r--r--   0        0        0      242 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/api/api_device.py
+-rw-r--r--   0        0        0       31 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/api/rest_api/__init__.py
+-rw-r--r--   0        0        0      243 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/api/rest_api/margin_testers/__init__.py
+-rw-r--r--   0        0        0     5891 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/api/rest_api/margin_testers/margin_tester.py
+-rw-r--r--   0        0        0     6155 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/api/rest_api/margin_testers/tmt4.py
+-rw-r--r--   0        0        0    22603 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/api/rest_api/rest_api_device.py
+-rw-r--r--   0        0        0    29615 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/device.py
+-rw-r--r--   0        0        0    12713 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/device_driver_mapping.py
+-rw-r--r--   0        0        0     1372 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/device_type_classes.py
+-rw-r--r--   0        0        0       43 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/__init__.py
+-rw-r--r--   0        0        0      329 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/data_acquisition_systems/__init__.py
+-rw-r--r--   0        0        0     3283 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/data_acquisition_systems/daq6510.py
+-rw-r--r--   0        0        0     1095 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/data_acquisition_systems/data_acquisition_system.py
+-rw-r--r--   0        0        0      362 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/digital_multimeters/__init__.py
+-rw-r--r--   0        0        0     1464 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/digital_multimeters/digital_multimeter.py
+-rw-r--r--   0        0        0      142 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/digital_multimeters/dmm6500/__init__.py
+-rw-r--r--   0        0        0     3114 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/digital_multimeters/dmm6500/dmm6500.py
+-rw-r--r--   0        0        0      328 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/digital_multimeters/dmm7500/__init__.py
+-rw-r--r--   0        0        0     3135 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/digital_multimeters/dmm7500/dmm7500.py
+-rw-r--r--   0        0        0     1791 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/digital_multimeters/dmm7500/dmm7510.py
+-rw-r--r--   0        0        0     1777 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/digital_multimeters/dmm7500/dmm7512.py
+-rw-r--r--   0        0        0    13515 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/ieee488_2_commands.py
+-rw-r--r--   0        0        0    34941 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/pi_device.py
+-rw-r--r--   0        0        0      245 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/power_supplies/__init__.py
+-rw-r--r--   0        0        0     1603 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/power_supplies/power_supply.py
+-rw-r--r--   0        0        0      668 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/power_supplies/psu2200/__init__.py
+-rw-r--r--   0        0        0     2471 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/power_supplies/psu2200/psu2200.py
+-rw-r--r--   0        0        0     1096 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/power_supplies/psu2200/psu2220.py
+-rw-r--r--   0        0        0     1096 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/power_supplies/psu2200/psu2230.py
+-rw-r--r--   0        0        0     1096 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/power_supplies/psu2200/psu2231.py
+-rw-r--r--   0        0        0     1100 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/power_supplies/psu2200/psu2231a.py
+-rw-r--r--   0        0        0     1316 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/power_supplies/psu2200/psu2280.py
+-rw-r--r--   0        0        0     1096 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/power_supplies/psu2200/psu2281.py
+-rw-r--r--   0        0        0      584 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/__init__.py
+-rw-r--r--   0        0        0     4875 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/scope.py
+-rw-r--r--   0        0        0      887 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope/__init__.py
+-rw-r--r--   0        0        0     1083 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope/lpd6.py
+-rw-r--r--   0        0        0     2290 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope/mso2.py
+-rw-r--r--   0        0        0     1095 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope/mso4.py
+-rw-r--r--   0        0        0     1089 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope/mso4b.py
+-rw-r--r--   0        0        0     1095 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope/mso5.py
+-rw-r--r--   0        0        0     1089 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope/mso5b.py
+-rw-r--r--   0        0        0     1095 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope/mso5lp.py
+-rw-r--r--   0        0        0     1095 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope/mso6.py
+-rw-r--r--   0        0        0     1089 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope/mso6b.py
+-rw-r--r--   0        0        0    27396 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope/tekscope.py
+-rw-r--r--   0        0        0     2445 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope/tekscopesw.py
+-rw-r--r--   0        0        0      464 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_2k/__init__.py
+-rw-r--r--   0        0        0     1780 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_2k/dpo2k.py
+-rw-r--r--   0        0        0     1770 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_2k/dpo2kb.py
+-rw-r--r--   0        0        0     1780 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_2k/mso2k.py
+-rw-r--r--   0        0        0     1770 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_2k/mso2kb.py
+-rw-r--r--   0        0        0     1415 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_2k/tekscope_2k.py
+-rw-r--r--   0        0        0      896 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/__init__.py
+-rw-r--r--   0        0        0     1790 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/dpo4k.py
+-rw-r--r--   0        0        0     1773 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/dpo4kb.py
+-rw-r--r--   0        0        0     2056 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/mdo3.py
+-rw-r--r--   0        0        0     1790 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/mdo3k.py
+-rw-r--r--   0        0        0     1790 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/mdo4k.py
+-rw-r--r--   0        0        0     1773 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/mdo4kb.py
+-rw-r--r--   0        0        0     1776 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/mdo4kc.py
+-rw-r--r--   0        0        0     1790 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/mso4k.py
+-rw-r--r--   0        0        0     1773 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/mso4kb.py
+-rw-r--r--   0        0        0     1783 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/tekscope_3k_4k.py
+-rw-r--r--   0        0        0     1695 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/__init__.py
+-rw-r--r--   0        0        0     1804 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo5k.py
+-rw-r--r--   0        0        0     1108 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo5kb.py
+-rw-r--r--   0        0        0     1798 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo70k.py
+-rw-r--r--   0        0        0     1117 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo70kc.py
+-rw-r--r--   0        0        0     1120 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo70kd.py
+-rw-r--r--   0        0        0     1123 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo70kdx.py
+-rw-r--r--   0        0        0     1123 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo70ksx.py
+-rw-r--r--   0        0        0     1804 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo7k.py
+-rw-r--r--   0        0        0     1108 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo7kc.py
+-rw-r--r--   0        0        0     1798 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dsa70k.py
+-rw-r--r--   0        0        0     1117 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dsa70kc.py
+-rw-r--r--   0        0        0     1117 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dsa70kd.py
+-rw-r--r--   0        0        0     1804 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/mso5k.py
+-rw-r--r--   0        0        0     1108 2024-05-06 18:52:31.350466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/mso5kb.py
+-rw-r--r--   0        0        0     1798 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/mso70k.py
+-rw-r--r--   0        0        0     1117 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/mso70kc.py
+-rw-r--r--   0        0        0     1123 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/mso70kdx.py
+-rw-r--r--   0        0        0     3037 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/tekscope_5k_7k_70k.py
+-rw-r--r--   0        0        0      117 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tso/__init__.py
+-rw-r--r--   0        0        0     1766 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tso/tsovu.py
+-rw-r--r--   0        0        0      298 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/__init__.py
+-rw-r--r--   0        0        0      443 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/afgs/__init__.py
+-rw-r--r--   0        0        0     6878 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/afgs/afg.py
+-rw-r--r--   0        0        0     2043 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/afgs/afg31k.py
+-rw-r--r--   0        0        0     1283 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/afgs/afg3k.py
+-rw-r--r--   0        0        0     1327 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/afgs/afg3kb.py
+-rw-r--r--   0        0        0     1330 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/afgs/afg3kc.py
+-rw-r--r--   0        0        0      859 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/awgs/__init__.py
+-rw-r--r--   0        0        0     5783 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/awgs/awg.py
+-rw-r--r--   0        0        0     1517 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/awgs/awg5200.py
+-rw-r--r--   0        0        0     1505 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/awgs/awg5k.py
+-rw-r--r--   0        0        0     1091 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/awgs/awg5kb.py
+-rw-r--r--   0        0        0     1106 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/awgs/awg5kc.py
+-rw-r--r--   0        0        0     1519 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/awgs/awg70ka.py
+-rw-r--r--   0        0        0     1115 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/awgs/awg70kb.py
+-rw-r--r--   0        0        0     1505 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/awgs/awg7k.py
+-rw-r--r--   0        0        0     1091 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/awgs/awg7kb.py
+-rw-r--r--   0        0        0     1329 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/awgs/awg7kc.py
+-rw-r--r--   0        0        0     5211 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/signal_source.py
+-rw-r--r--   0        0        0      633 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/__init__.py
+-rw-r--r--   0        0        0      963 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2400/__init__.py
+-rw-r--r--   0        0        0     1141 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2400.py
+-rw-r--r--   0        0        0     3358 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2400_interactive.py
+-rw-r--r--   0        0        0     5707 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2400_standard.py
+-rw-r--r--   0        0        0     1141 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2401.py
+-rw-r--r--   0        0        0     1141 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2410.py
+-rw-r--r--   0        0        0     1173 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2450.py
+-rw-r--r--   0        0        0     1173 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2460.py
+-rw-r--r--   0        0        0     1173 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2461.py
+-rw-r--r--   0        0        0     1173 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2470.py
+-rw-r--r--   0        0        0     2487 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/__init__.py
+-rw-r--r--   0        0        0     3814 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2600.py
+-rw-r--r--   0        0        0      216 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2600a.py
+-rw-r--r--   0        0        0     1196 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2600b.py
+-rw-r--r--   0        0        0     1123 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2601a.py
+-rw-r--r--   0        0        0     1139 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2601b.py
+-rw-r--r--   0        0        0     1172 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2601b_pulse.py
+-rw-r--r--   0        0        0     1123 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2602a.py
+-rw-r--r--   0        0        0     1139 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2602b.py
+-rw-r--r--   0        0        0     1123 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2604a.py
+-rw-r--r--   0        0        0     1139 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2604b.py
+-rw-r--r--   0        0        0     1139 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2606b.py
+-rw-r--r--   0        0        0     1123 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2611a.py
+-rw-r--r--   0        0        0     1139 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2611b.py
+-rw-r--r--   0        0        0     1123 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2612a.py
+-rw-r--r--   0        0        0     1139 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2612b.py
+-rw-r--r--   0        0        0     1123 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2614a.py
+-rw-r--r--   0        0        0     1139 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2614b.py
+-rw-r--r--   0        0        0     1123 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2634a.py
+-rw-r--r--   0        0        0     1139 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2634b.py
+-rw-r--r--   0        0        0     1123 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2635a.py
+-rw-r--r--   0        0        0     1139 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2635b.py
+-rw-r--r--   0        0        0     1123 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2636a.py
+-rw-r--r--   0        0        0     1139 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2636b.py
+-rw-r--r--   0        0        0      718 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2650a.py
+-rw-r--r--   0        0        0     1139 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2651a.py
+-rw-r--r--   0        0        0     1139 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2657a.py
+-rw-r--r--   0        0        0      409 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu6000/__init__.py
+-rw-r--r--   0        0        0     5922 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu6000/smu6000.py
+-rw-r--r--   0        0        0     1109 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu6000/smu6430.py
+-rw-r--r--   0        0        0     1109 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu6000/smu6514.py
+-rw-r--r--   0        0        0     1113 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu6000/smu6517b.py
+-rw-r--r--   0        0        0      587 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/source_measure_unit.py
+-rw-r--r--   0        0        0      241 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/systems_switches/__init__.py
+-rw-r--r--   0        0        0     3584 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/systems_switches/ss3706a.py
+-rw-r--r--   0        0        0      527 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/systems_switches/systems_switch.py
+-rw-r--r--   0        0        0    10612 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/drivers/pi/tsp_device.py
+-rw-r--r--   0        0        0     2235 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/helpers/__init__.py
+-rw-r--r--   0        0        0     3788 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/helpers/alias_dict.py
+-rw-r--r--   0        0        0    29480 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/helpers/constants_and_dataclasses.py
+-rw-r--r--   0        0        0     2733 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/helpers/dataclass_mixins.py
+-rw-r--r--   0        0        0     6836 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/helpers/enums.py
+-rw-r--r--   0        0        0    27496 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/helpers/functions.py
+-rw-r--r--   0        0        0     3603 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/helpers/read_only_cached_property.py
+-rw-r--r--   0        0        0     1149 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/helpers/singleton_metaclass.py
+-rw-r--r--   0        0        0     1408 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/helpers/standalone_functions.py
+-rw-r--r--   0        0        0     3914 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/helpers/stubgen.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:52:31.354466 tm_devices-1.4.1/src/tm_devices/py.typed
+-rw-r--r--   0        0        0    20954 1970-01-01 00:00:00.000000 tm_devices-1.4.1/PKG-INFO
```

### Comparing `tm_devices-1.4.0/LICENSE.md` & `tm_devices-1.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/README.md` & `tm_devices-1.4.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     scope = device_manager.add_scope("192.168.0.100")
     scope.query("*IDN?")
     print(scope)
 ```
 
 ### Supported Devices & Software Solutions
 
-> \[!TIP\]
+> [!TIP]
 > Visit the [Glossary](https://tinyurl.com/tek-tm-devices/docs/glossary.md) to see definitions for all symbols and abbreviations.
 
 <div markdown="1" class="custom-table-center-cells device-support-table">
 
 <div markdown="1" class="custom-table-title">
 
 _Device Support Levels_
```

### Comparing `tm_devices-1.4.0/pyproject.toml` & `tm_devices-1.4.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 maintainers = [
   "Tektronix <opensource@tektronix.com>",
   "Nicholas Felt <nicholas.felt@tektronix.com>"
 ]
 name = "tm_devices"
 readme = "README.md"
 repository = "https://github.com/tektronix/tm_devices"
-version = "1.4.0"
+version = "1.4.1"
 
 [tool.poetry.dependencies]
 gpib-ctypes = "^0.3.0"
 libusb-package = "^1.0.26.0,!=1.0.26.2"  # 1.0.26.2 doesn't work with Python 3.12
 packaging = "^24.0"
 psutil = "^5.9.0"
 pyserial = "^3.5"
@@ -88,15 +88,15 @@
 tomli-w = "^1.0.0"
 traceback-with-variables = "^2.0.4"
 typing-extensions = "^4.10.0"
 urllib3 = "^2.0"
 zeroconf = "^0.132.2"
 
 [tool.poetry.group.dev.dependencies]
-docformatter = {extras = ["tomli"], version = "1.7.5"}  # Update this by running scripts/update_development_dependencies.py
+docformatter = {extras = ["tomli"], version = "1.7.5"}
 docutils = "^0.20"
 docutils-stubs = "^0.0.22"
 matplotlib = [
   {python = ">=3.9", version = "^3.8"},
   {python = "3.8", version = "^3.7"}
 ]
 memory-profiler = "^0.61.0"
@@ -107,19 +107,19 @@
 poetry-pre-commit-plugin = "^0.1.2"
 pre-commit = [
   {python = ">=3.9", version = "^3.7"},
   {python = "3.8", version = "^3.5"}
 ]
 pre-commit-update = "^0.3.0"
 pyclean = "^3.0.0"
-pylint = "3.1.0"  # Update this by running scripts/update_development_dependencies.py
-pyright = "1.1.361"  # Update this by running scripts/update_development_dependencies.py
+pylint = "3.1.0"
+pyright = "1.1.361"
 pyroma = "^4.2"
 python-semantic-release = "^9.6.0"
-ruff = "0.4.2"  # Update this by running scripts/update_development_dependencies.py
+ruff = "0.4.3"
 safety = "^3.2.0"
 toml-sort = "^0.23.0"
 tox = "^4.0"
 tox-gh-actions = "^3.1.0"
 twine = "^5.0.0"
 types-python-dateutil = "^2.9"
 types-pyyaml = "^6.0"
@@ -134,16 +134,15 @@
 mkdocs-ezglossary-plugin = "^1.6.8"
 mkdocs-gen-files = "^0.5.0"
 mkdocs-include-markdown-plugin = "^6.0.5"
 mkdocs-literate-nav = "^0.6.1"
 mkdocs-macros-plugin = "^1.0.5"
 mkdocs-mermaid2-plugin = "^1.1.1"
 mkdocs-section-index = "^0.3.9"
-# mkdocs-spellcheck = "^1.0.4"  # TODO: switch to this once the official package is updated
-mkdocs-spellcheck = {git = "https://github.com/nfelt14/mkdocs-spellcheck.git", rev = "main"}
+mkdocs-spellcheck = "^1.1.0"
 mkdocstrings = "^0.25.0"
 mkdocstrings-python = "^1.10.0"
 pygments = "^2.17.2"
 pymdown-extensions = "^10.8.1"
 symspellpy = "^6.7.7"
 tomli = "^2.0.1"
 
@@ -156,15 +155,15 @@
 pytest = "^8.2.0"
 pytest-cov = "^5.0.0"
 pytest-depends = "^1.0.1"
 pytest-env = "^1.1.3"
 pytest-github-report = "^0.0.1"
 pytest-html = "^4.1.1"
 pytest-order = "^1.2.1"
-ruff = "0.4.2"  # Update this by running scripts/update_development_dependencies.py
+ruff = "0.4.3"
 tomli = "^2.0.1"
 
 [tool.poetry.scripts]
 list-visa-resources = "tm_devices:print_available_visa_devices"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/tektronix/tm_devices/issues"
```

### Comparing `tm_devices-1.4.0/src/tm_devices/__init__.py` & `tm_devices-1.4.1/src/tm_devices/__init__.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/__init__.py` & `tm_devices-1.4.1/src/tm_devices/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/afg3k_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/afg3k_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/afg3kb_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/afg3kb_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/afg3kc_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/afg3kc_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/awg5200_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/awg5200_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/awg5k_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/awg5k_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/awg5kc_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/awg5kc_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/awg70ka_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/awg70ka_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/awg70kb_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/awg70kb_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/awg7k_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/awg7k_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/awg7kc_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/awg7kc_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/daq6510_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/daq6510_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/dmm6500_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/dmm6500_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/dmm7510_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/dmm7510_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/dpo2k_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/dpo2k_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/dpo2kb_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/dpo2kb_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/dpo4k_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/dpo4k_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/dpo4kb_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/dpo4kb_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/dpo5k_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/dpo5k_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/dpo5kb_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/dpo5kb_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/dpo70kc_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/dpo70kc_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/dpo70kd_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/dpo70kd_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/dpo70kdx_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/dpo70kdx_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/dpo70ksx_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/dpo70ksx_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/dpo7k_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/dpo7k_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/dpo7kc_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/dpo7kc_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/dsa70kc_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/dsa70kc_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/dsa70kd_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/dsa70kd_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_163n04_mdo/search.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_163n04_mdo/search.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_16x4xq_mdo/search.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_16x4xq_mdo/search.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1jzp7o_mdodpo/trigger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1jzp7o_mdodpo/trigger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1kdqwg_mdo/search.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1kdqwg_mdo/search.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1kdqwg_mdo/trigger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1kdqwg_mdo/trigger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1kjd62_mdo/rf.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1kjd62_mdo/rf.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1kozfv_dpo/search.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1kozfv_dpo/search.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1l4fot_mdomso/cursor.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1l4fot_mdomso/cursor.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1la1ym_msomdodpo/trigger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1la1ym_msomdodpo/trigger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1lcv3a_msodpomdo/message.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1lcv3a_msodpomdo/message.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1lcv3a_msodpomdo/setup_1.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1lcv3a_msodpomdo/setup_1.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1lh2st_msodpo/search.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1lh2st_msodpo/search.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/actonevent.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/actonevent.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/afg.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/afg.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/alias.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/alias.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/application.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/application.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/autoset.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/autoset.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/auxin.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/auxin.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/auxout.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/auxout.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/bus.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/bus.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/calibrate.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/calibrate.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/ch.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/ch.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/d.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/d.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/data.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/data.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/diag.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/diag.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/dvm.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/dvm.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/email.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/email.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/ethernet.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/ethernet.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/filesystem.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/filesystem.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/fpanel.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/fpanel.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/gpibusb.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/gpibusb.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/hardcopy.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/hardcopy.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/histogram.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/histogram.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/horizontal.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/horizontal.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/mark.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/mark.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/marker.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/marker.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/math1.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/math1.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/pictbridge.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/pictbridge.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/power.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/power.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/reboot.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/reboot.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/ref.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/ref.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/save.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/save.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/socketserver.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/socketserver.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/time.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/time.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/vidpic.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/vidpic.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/wfminpre.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/wfminpre.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/wfmoutpre.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/wfmoutpre.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/zoom.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1ltpwt_mdomsodpo/zoom.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1lwj1r_msomdodpo/rosc.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1lwj1r_msomdodpo/rosc.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1lxxm9_msomdodpo/cursor.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1lxxm9_msomdodpo/cursor.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/acquire.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/acquire.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/configuration.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/configuration.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/deskew.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/deskew.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/display.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/display.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/mask.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/mask.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/measurement.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/measurement.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/recall.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/recall.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/select.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1mlt9u_mdomsodpo/select.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1mq0z9_msodpo/rf.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1mq0z9_msodpo/rf.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1nmc1o_msodpomdo/clearmenu.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1nmc1o_msodpomdo/clearmenu.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1nmc1o_msodpomdo/errlog.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1nmc1o_msodpomdo/errlog.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1nmc1o_msodpomdo/header.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1nmc1o_msodpomdo/header.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1nmc1o_msodpomdo/language.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1nmc1o_msodpomdo/language.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1nmc1o_msodpomdo/status_and_error.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1nmc1o_msodpomdo/status_and_error.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1nmc1o_msodpomdo/usbdevice.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1nmc1o_msodpomdo/usbdevice.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1nmc1o_msodpomdo/usbtmc.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1nmc1o_msodpomdo/usbtmc.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1nmc1o_msodpomdo/verbose.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1nmc1o_msodpomdo/verbose.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/acquire.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/acquire.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/actonevent.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/actonevent.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/auxout.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/auxout.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/battery.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/battery.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/bus.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/bus.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/callouts.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/callouts.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/ch.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/ch.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/data.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/data.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/dch.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/dch.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/diag.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/diag.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/display.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/display.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/fpanel.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/fpanel.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/horizontal.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/horizontal.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/lic.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/lic.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/license.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/license.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/mask.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/mask.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/math.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/math.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/measurement.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/measurement.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/pg.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/pg.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/plot.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/plot.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/power.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/power.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/ref.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/ref.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/save.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/save.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/saveon.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/saveon.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/saveonevent.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/saveonevent.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/search.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/search.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/select.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/select.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/touchscreen.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/touchscreen.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_1zn03_mso/trigger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_1zn03_mso/trigger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/afgcontrol.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/afgcontrol.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/data.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/data.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/diagnostic.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/diagnostic.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/display.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/display.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/hcopy.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/hcopy.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/memory.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/memory.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/mmemory.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/mmemory.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/output.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/output.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/output1.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/output1.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/output2.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/output2.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/source.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/source.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/source1.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/source1.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/source2.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/source2.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/source3.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/source3.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/source4.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/source4.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/status.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/status.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/system.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/system.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_22daqs_afg/trigger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_22daqs_afg/trigger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/abort.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/abort.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/auxoutput.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/auxoutput.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/awgcontrol.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/awgcontrol.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/bwaveform.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/bwaveform.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/clock.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/clock.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/cplayback.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/cplayback.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/fgen.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/fgen.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/instrument.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/instrument.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/mmemory.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/mmemory.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/output.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/output.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/source.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/source.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/synchronize.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/synchronize.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/system.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/system.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/trigger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/trigger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_2i1z2s_awg/wlist.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_2i1z2s_awg/wlist.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/awgcontrol.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/awgcontrol.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/diagnostic.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/diagnostic.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/display.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/display.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/event.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/event.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/instrument.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/instrument.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/mmemory.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/mmemory.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/output.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/output.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/sequence.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/sequence.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/slist.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/slist.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/source.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/source.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/status.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/status.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/system.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/system.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/trigger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/trigger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_32dszm_awg/wlist.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_32dszm_awg/wlist.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_33ijgq_afgawg/abort.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_33ijgq_afgawg/abort.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_33ijgq_afgawg/calibration.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_33ijgq_afgawg/calibration.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_3n9auv_awg/active.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_3n9auv_awg/active.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_3n9auv_awg/calibration.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_3n9auv_awg/calibration.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_3n9auv_awg/diagnostic.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_3n9auv_awg/diagnostic.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_3n9auv_awg/display.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_3n9auv_awg/display.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_3n9auv_awg/output.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_3n9auv_awg/output.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_3n9auv_awg/slist.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_3n9auv_awg/slist.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_3n9auv_awg/status.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_3n9auv_awg/status.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_3n9auv_awg/wplugin.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_3n9auv_awg/wplugin.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/auxoutput.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/auxoutput.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/awgcontrol.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/awgcontrol.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/bwaveform.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/bwaveform.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/clock.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/clock.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/cplayback.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/cplayback.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/fgen.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/fgen.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/instrument.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/instrument.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/mmemory.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/mmemory.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/output.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/output.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/source.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/source.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/synchronize.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/synchronize.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/system.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/system.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/trigger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/trigger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_3rs8qy_awg/wlist.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_3rs8qy_awg/wlist.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_3skc3w_dpo/trigger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_3skc3w_dpo/trigger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_3tjgb2_dpo/trigger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_3tjgb2_dpo/trigger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_4jiykk_dpo/channelmapping.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_4jiykk_dpo/channelmapping.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_4jiykk_dpo/counter.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_4jiykk_dpo/counter.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_4jiykk_dpo/errordetector.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_4jiykk_dpo/errordetector.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_4jiykk_dpo/idnmultiscope.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_4jiykk_dpo/idnmultiscope.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_4jiykk_dpo/linktraining.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_4jiykk_dpo/linktraining.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_4jiykk_dpo/rosc.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_4jiykk_dpo/rosc.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_4jiykk_dpo/trigger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_4jiykk_dpo/trigger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_53md2e_dpomso/fpanel.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_53md2e_dpomso/fpanel.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_561g9r_mso/trigger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_561g9r_mso/trigger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_5ri0nj_dpomso/bus.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_5ri0nj_dpomso/bus.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_5vmwut_dpodsamso/trigger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_5vmwut_dpodsamso/trigger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_5xwdsk_dpodsamso/errordetector.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_5xwdsk_dpodsamso/errordetector.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_5y90wx_dpodsamso/dpojet.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_5y90wx_dpodsamso/dpojet.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_5yyb4r_mso/trigger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_5yyb4r_mso/trigger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_60xy3r_smu/buffer.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_60xy3r_smu/buffer.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_60xy3r_smu/script.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_60xy3r_smu/script.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_60xy3r_smu/smu.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_60xy3r_smu/smu.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_60xy3r_smu/upgrade.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_60xy3r_smu/upgrade.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_6ocqvh_smu/buffer.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_6ocqvh_smu/buffer.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_6srh1x_smu/smu.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_6srh1x_smu/smu.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_6srh1x_smu/upgrade.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_6srh1x_smu/upgrade.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_6vynmi_smu/acal.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_6vynmi_smu/acal.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_6vynmi_smu/smu.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_6vynmi_smu/smu.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_6vynmi_smu/trigger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_6vynmi_smu/trigger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_6vynmi_smu/upgrade.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_6vynmi_smu/upgrade.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_6w7311_smu/trigger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_6w7311_smu/trigger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_6xiuc2_smu/buffer.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_6xiuc2_smu/buffer.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_6xiuc2_smu/smu.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_6xiuc2_smu/smu.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_6xiuc2_smu/upgrade.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_6xiuc2_smu/upgrade.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_7kqm9p_smu/buffervar.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_7kqm9p_smu/buffervar.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_7kqm9p_smu/display.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_7kqm9p_smu/display.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_7kqm9p_smu/tsplink.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_7kqm9p_smu/tsplink.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_7kqm9p_smu/tspnet.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_7kqm9p_smu/tspnet.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_7ryhce_smu/status.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_7ryhce_smu/status.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/beeper.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/beeper.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/buffervar.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/buffervar.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/dataqueue.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/dataqueue.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/digio.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/digio.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/display.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/display.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/errorqueue.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/errorqueue.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/eventlog.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/eventlog.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/format.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/format.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/lan.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/lan.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/localnode.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/localnode.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/serial.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/serial.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/smux.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/smux.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/status.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/status.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/trigger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/trigger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/tsplink.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/tsplink.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_7s2p1p_smu/tspnet.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_7s2p1p_smu/tspnet.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_7s43m8_smu/status.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_7s43m8_smu/status.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_7s6wr5_smu/status.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_7s6wr5_smu/status.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_8ojdkz_smu/display.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_8ojdkz_smu/display.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_8ojdkz_smu/node.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_8ojdkz_smu/node.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_8ojdkz_smu/smux.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_8ojdkz_smu/smux.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_8ojdkz_smu/status.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_8ojdkz_smu/status.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_8wm55i_smu/smux.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_8wm55i_smu/smux.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_9kezla_smu/smux.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_9kezla_smu/smux.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_9mzp2j_smu/digio.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_9mzp2j_smu/digio.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_9mzp2j_smu/display.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_9mzp2j_smu/display.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_9mzp2j_smu/tsplink.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_9mzp2j_smu/tsplink.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_9ncc6e_smu/display.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_9ncc6e_smu/display.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_9nnkq7_smu/status.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_9nnkq7_smu/status.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_9slyux_smu/status.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_9slyux_smu/status.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ahkybr_smu/beeper.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ahkybr_smu/beeper.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ahkybr_smu/buffervar.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ahkybr_smu/buffervar.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ahkybr_smu/eventlog.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ahkybr_smu/eventlog.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ahkybr_smu/lan.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ahkybr_smu/lan.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ahkybr_smu/os.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ahkybr_smu/os.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ahkybr_smu/script.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ahkybr_smu/script.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ahkybr_smu/scriptvar.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ahkybr_smu/scriptvar.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ahkybr_smu/setup_1.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ahkybr_smu/setup_1.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ahkybr_smu/tspnet.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ahkybr_smu/tspnet.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_aih9e2_smu/trigger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_aih9e2_smu/trigger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ak4990_smu/smux.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ak4990_smu/smux.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_am6pcr_smu/smux.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_am6pcr_smu/smux.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_am6pcr_smu/status.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_am6pcr_smu/status.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_amm5lc_smu/digio.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_amm5lc_smu/digio.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_amm5lc_smu/tsplink.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_amm5lc_smu/tsplink.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_aostep_smu/serial.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_aostep_smu/serial.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_aqr1t1_smu/localnode.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_aqr1t1_smu/localnode.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_as1ejq_smu/localnode.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_as1ejq_smu/localnode.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_as1ejq_smu/smux.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_as1ejq_smu/smux.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_as1ejq_smu/status.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_as1ejq_smu/status.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_at7jl1_smu/display.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_at7jl1_smu/display.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_au597k_smu/digio.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_au597k_smu/digio.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_au597k_smu/format.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_au597k_smu/format.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_au597k_smu/tsplink.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_au597k_smu/tsplink.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_auyr50_smu/format.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_auyr50_smu/format.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_auyr50_smu/localnode.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_auyr50_smu/localnode.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_auyr50_smu/node.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_auyr50_smu/node.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_avh0iw_smu/display.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_avh0iw_smu/display.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_avh0iw_smu/trigger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_avh0iw_smu/trigger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_awhjao_smu/status.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_awhjao_smu/status.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_by991s_smudaq/digio.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_by991s_smudaq/digio.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_by991s_smudaq/status.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_by991s_smudaq/status.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_canxny_daq/buffer.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_canxny_daq/buffer.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_canxny_daq/buffervar.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_canxny_daq/buffervar.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_canxny_daq/channel.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_canxny_daq/channel.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_canxny_daq/display.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_canxny_daq/display.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_canxny_daq/dmm.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_canxny_daq/dmm.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_canxny_daq/scan.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_canxny_daq/scan.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_canxny_daq/slot.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_canxny_daq/slot.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_canxny_daq/trigger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_canxny_daq/trigger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_canxny_daq/tsplink.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_canxny_daq/tsplink.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_canxny_daq/upgrade.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_canxny_daq/upgrade.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_d6b496_dmm/acal.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_d6b496_dmm/acal.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_d6b496_dmm/buffer.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_d6b496_dmm/buffer.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_d6b496_dmm/buffervar.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_d6b496_dmm/buffervar.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_d6b496_dmm/display.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_d6b496_dmm/display.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_d6b496_dmm/dmm.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_d6b496_dmm/dmm.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_d6b496_dmm/fan.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_d6b496_dmm/fan.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_d6b496_dmm/localnode.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_d6b496_dmm/localnode.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_d6b496_dmm/trigger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_d6b496_dmm/trigger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_d83qe0_dmm/buffer.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_d83qe0_dmm/buffer.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_d83qe0_dmm/buffervar.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_d83qe0_dmm/buffervar.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_d83qe0_dmm/channel.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_d83qe0_dmm/channel.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_d83qe0_dmm/display.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_d83qe0_dmm/display.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_d83qe0_dmm/dmm.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_d83qe0_dmm/dmm.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_d83qe0_dmm/scan.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_d83qe0_dmm/scan.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_d83qe0_dmm/slot.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_d83qe0_dmm/slot.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_d83qe0_dmm/trigger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_d83qe0_dmm/trigger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_dawv9y_smudaqdmm/localnode.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_dawv9y_smudaqdmm/localnode.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/beeper.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/beeper.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/eventlog.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/eventlog.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/file.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/file.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/format.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/format.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/lan.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/lan.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/scriptvar.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/scriptvar.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/timer.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_dbdq3i_smudaqdmm/timer.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_dbqd7k_dmm/digio.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_dbqd7k_dmm/digio.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_dbqd7k_dmm/node.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_dbqd7k_dmm/node.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_dbqd7k_dmm/status.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_dbqd7k_dmm/status.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_dbqd7k_dmm/tsplink.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_dbqd7k_dmm/tsplink.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_dbqd7k_dmm/tspnet.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_dbqd7k_dmm/tspnet.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_dbqd7k_dmm/upgrade.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_dbqd7k_dmm/upgrade.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_dcpheg_daqdmm/smu.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_dcpheg_daqdmm/smu.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_dd4xnb_smudaqdmm/script.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_dd4xnb_smudaqdmm/script.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/acquire.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/acquire.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/actonevent.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/actonevent.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/application.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/application.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/auxout.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/auxout.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/bus.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/bus.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/callouts.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/callouts.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/ch.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/ch.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/data.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/data.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/diag.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/diag.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/diggrp.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/diggrp.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/display.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/display.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/dvm.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/dvm.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/eyemask.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/eyemask.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/fpanel.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/fpanel.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/histogram.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/histogram.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/horizontal.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/horizontal.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/license.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/license.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/mask.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/mask.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/math.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/math.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/matharbflt.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/matharbflt.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/measurement.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/measurement.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/peakstable.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/peakstable.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/pilogger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/pilogger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/plot.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/plot.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/power.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/power.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/ref.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/ref.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/rosc.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/rosc.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/save.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/save.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/saveon.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/saveon.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/saveonevent.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/saveonevent.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/search.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/search.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/searchtable.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/searchtable.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/select.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/select.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/sv.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/sv.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/touchscreen.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/touchscreen.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/trigger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/trigger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/tstamptable.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/tstamptable.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3e9uu_lpdmso/visual.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3e9uu_lpdmso/visual.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/afg.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/afg.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/autosavepitimeout.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/autosavepitimeout.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/autosaveuitimeout.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/autosaveuitimeout.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/autoset.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/autoset.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/bustable.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/bustable.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/calibrate.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/calibrate.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/configuration.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/configuration.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/connected.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/connected.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/curve.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/curve.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/curvestream.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/curvestream.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/customtable.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/customtable.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/date.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/date.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/ethernet.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/ethernet.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/filesystem.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/filesystem.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/mainwindow.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/mainwindow.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/meastable.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/meastable.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/recall.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/recall.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/socketserver.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/socketserver.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/time.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/time.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/undo.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/undo.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/usbdevice.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/usbdevice.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/vertical.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/vertical.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3h2zs_lpdmso/wfmoutpre.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3h2zs_lpdmso/wfmoutpre.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/beeper.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/beeper.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/buffervar.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/buffervar.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/channel.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/channel.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/comm.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/comm.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/digio.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/digio.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/display.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/display.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/dmm.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/dmm.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/eventlog.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/eventlog.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/format.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/format.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/lan.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/lan.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/localnode.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/localnode.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/memory.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/memory.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/os.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/os.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/ptp.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/ptp.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/scan.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/scan.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/schedule.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/schedule.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/script.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/script.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/scriptvar.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/scriptvar.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/setup_1.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/setup_1.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/slot.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/slot.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/status.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/status.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/trigger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/trigger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/tsplink.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/tsplink.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e3pief_ss/upgrade.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e3pief_ss/upgrade.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e4de2d_lpdmsomdo/clear.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e4de2d_lpdmsomdo/clear.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e6606z_lpdmsomdodpo/pause.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e6606z_lpdmsomdodpo/pause.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e6lgg1_lpdmsodpomdo/totaluptime.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e6lgg1_lpdmsodpomdo/totaluptime.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_e7aqno_smudaqss/node.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_e7aqno_smudaqss/node.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_eat5s3_smudaqdmmss/dataqueue.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_eat5s3_smudaqdmmss/dataqueue.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_eat5s3_smudaqdmmss/fs.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_eat5s3_smudaqdmmss/fs.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_eat5s3_smudaqdmmss/userstring.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_eat5s3_smudaqdmmss/userstring.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ed9nkc_daqss/tspnet.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ed9nkc_daqss/tspnet.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_efap3f_smuss/bit.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_efap3f_smuss/bit.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_efap3f_smuss/errorqueue.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_efap3f_smuss/errorqueue.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_efap3f_smuss/io.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_efap3f_smuss/io.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_efap3f_smuss/timer.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_efap3f_smuss/timer.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_eg5ll2_smudaqdmmss/gpib.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_eg5ll2_smudaqdmmss/gpib.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ffz2xs_dpodsamso/bus.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ffz2xs_dpodsamso/bus.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fhrp27_msodpomdodsa/curve.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fhrp27_msodpomdodsa/curve.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fhrp27_msodpomdodsa/date.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fhrp27_msodpomdodsa/date.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fhrp27_msodpomdodsa/mathvar.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fhrp27_msodpomdodsa/mathvar.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fhrp27_msodpomdodsa/save_and_recall.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fhrp27_msodpomdodsa/save_and_recall.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/acquire.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/acquire.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/allocate.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/allocate.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/application.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/application.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/autoset.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/autoset.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/auxin.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/auxin.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/auxout.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/auxout.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/bell.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/bell.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/calibrate.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/calibrate.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/ch.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/ch.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/clear.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/clear.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/cmdbatch.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/cmdbatch.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/cq.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/cq.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/cursor.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/cursor.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/curvenext.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/curvenext.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/curvestream.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/curvestream.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/custom.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/custom.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/d.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/d.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/data.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/data.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/delete.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/delete.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/diag.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/diag.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/display.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/display.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/email.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/email.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/export.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/export.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/fastacq.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/fastacq.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/filesystem.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/filesystem.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/gpibusb.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/gpibusb.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/hardcopy.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/hardcopy.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/hdr.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/hdr.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/histogram.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/histogram.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/horizontal.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/horizontal.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/limit.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/limit.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/mark.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/mark.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/mask.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/mask.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/math.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/math.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/matharbflt.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/matharbflt.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/mch.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/mch.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/measurement.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/measurement.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/multiscope.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/multiscope.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/opcextended.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/opcextended.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/pcenable.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/pcenable.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/recall.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/recall.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/ref.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/ref.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/save.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/save.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/save_and_recall.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/save_and_recall.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/saveon.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/saveon.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/search.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/search.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/select.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/select.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/setup_1.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/setup_1.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/system.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/system.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/teklink.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/teklink.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/test.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/test.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/trig.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/trig.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/usbtmc.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/usbtmc.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/visual.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/visual.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/wavfrmstream.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/wavfrmstream.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/wfminpre.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/wfminpre.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/wfmoutpre.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/wfmoutpre.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/wfmpre.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/wfmpre.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fk3z56_dpodsamso/zoom.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fk3z56_dpodsamso/zoom.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fkjfe8_msodpodsa/time.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fkjfe8_msodpodsa/time.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fn2qbf_msodpo/errordetector.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fn2qbf_msodpo/errordetector.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fn2qbf_msodpo/trigger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fn2qbf_msodpo/trigger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fpx9s1_dpodsamso/counter.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fpx9s1_dpodsamso/counter.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fpx9s1_dpodsamso/linktraining.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fpx9s1_dpodsamso/linktraining.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fpx9s1_dpodsamso/rosc.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fpx9s1_dpodsamso/rosc.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ft5uww_lpdmsodpomdoafgawgdsa/calibration.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ft5uww_lpdmsodpomdoafgawgdsa/calibration.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ft5uww_lpdmsodpomdoafgawgdsa/miscellaneous.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ft5uww_lpdmsodpomdoafgawgdsa/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ft5uww_lpdmsodpomdoafgawgdsa/status_and_error.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ft5uww_lpdmsodpomdoafgawgdsa/status_and_error.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fteabn_lpdmsomdodpoafgawgdsa/status_and_error.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fteabn_lpdmsomdodpoafgawgdsa/status_and_error.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fug7nl_lpdmsodpomdoawgdsa/status_and_error.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fug7nl_lpdmsodpomdoawgdsa/status_and_error.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fuzvln_lpdmsodpodsa/alias.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fuzvln_lpdmsodpodsa/alias.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fuzvln_lpdmsodpodsa/header.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fuzvln_lpdmsodpodsa/header.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fuzvln_lpdmsodpodsa/status_and_error.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fuzvln_lpdmsodpodsa/status_and_error.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fuzvln_lpdmsodpodsa/verbose.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fuzvln_lpdmsodpodsa/verbose.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/allev.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/allev.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/busy.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/busy.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/dese.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/dese.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/event.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/event.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/evmsg.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/evmsg.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/evqty.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/evqty.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/factory.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/factory.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/id.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/id.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/miscellaneous.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/newpass.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/newpass.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/password.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/password.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/rem.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/rem.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/set.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/set.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/status_and_error.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/status_and_error.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/teksecure.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/teksecure.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/wavfrm.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fx54ua_lpdmsodpomdodsa/wavfrm.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fzn174_lpdmsodpomdodsa/lock.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fzn174_lpdmsodpomdodsa/lock.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_fzn174_lpdmsodpomdodsa/unlock.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_fzn174_lpdmsodpomdodsa/unlock.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/acquire.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/acquire.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/alias.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/alias.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/autoset.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/autoset.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/auxin.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/auxin.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/bus.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/bus.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/calibrate.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/calibrate.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/ch.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/ch.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/cursor.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/cursor.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/d.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/d.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/data.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/data.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/diag.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/diag.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/display.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/display.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/ethernet.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/ethernet.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/filesystem.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/filesystem.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/filtervu.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/filtervu.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/fpanel.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/fpanel.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/gpibusb.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/gpibusb.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/hardcopy.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/hardcopy.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/horizontal.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/horizontal.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/mark.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/mark.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/math1.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/math1.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/measurement.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/measurement.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/pictbridge.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/pictbridge.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/recall.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/recall.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/ref.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/ref.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/save.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/save.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/search.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/search.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/select.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/select.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/trigger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/trigger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/wfminpre.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/wfminpre.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/wfmoutpre.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/wfmoutpre.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_u301s_msodpo/zoom.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_u301s_msodpo/zoom.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/acquire.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/acquire.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/configuration.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/configuration.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/cursor.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/cursor.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/deskew.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/deskew.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/display.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/display.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/lock.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/lock.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/mask.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/mask.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/measurement.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/measurement.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/message.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/message.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/recall.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/recall.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/rf.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/rf.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/rrb.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/rrb.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/search.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/search.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/select.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/select.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/setup1.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/setup1.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_ujuvb_mdo/trigger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_ujuvb_mdo/trigger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_usaa3_mdo/rf.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_usaa3_mdo/rf.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_usaa3_mdo/search.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_usaa3_mdo/search.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/gen_usaa3_mdo/trigger.py` & `tm_devices-1.4.1/src/tm_devices/commands/gen_usaa3_mdo/trigger.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/helpers/__init__.py` & `tm_devices-1.4.1/src/tm_devices/commands/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/helpers/generic_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/helpers/generic_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/helpers/scpi_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/helpers/scpi_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/helpers/tsp_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/helpers/tsp_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/lpd6_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/lpd6_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/mdo3_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/mdo3_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/mdo3k_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/mdo3k_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/mdo4k_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/mdo4k_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/mdo4kb_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/mdo4kb_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/mdo4kc_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/mdo4kc_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/mso2_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/mso2_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/mso2k_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/mso2k_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/mso2kb_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/mso2kb_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/mso4_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/mso4_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/mso4b_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/mso4b_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/mso4k_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/mso4k_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/mso4kb_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/mso4kb_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/mso5_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/mso5_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/mso5b_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/mso5b_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/mso5k_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/mso5k_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/mso5kb_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/mso5kb_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/mso5lp_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/mso5lp_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/mso6_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/mso6_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/mso6b_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/mso6b_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/mso70kc_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/mso70kc_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/mso70kdx_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/mso70kdx_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/smu2450_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/smu2450_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/smu2460_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/smu2460_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/smu2461_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/smu2461_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/smu2470_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/smu2470_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/smu2601b_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/smu2601b_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/smu2601b_pulse_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/smu2601b_pulse_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/smu2602b_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/smu2602b_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/smu2604b_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/smu2604b_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/smu2606b_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/smu2606b_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/smu2611b_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/smu2611b_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/smu2612b_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/smu2612b_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/smu2614b_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/smu2614b_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/smu2634b_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/smu2634b_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/smu2635b_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/smu2635b_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/smu2636b_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/smu2636b_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/smu2651a_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/smu2651a_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/smu2657a_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/smu2657a_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/commands/ss3706a_commands.py` & `tm_devices-1.4.1/src/tm_devices/commands/ss3706a_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/components/dm_config_parser.py` & `tm_devices-1.4.1/src/tm_devices/components/dm_config_parser.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/device_manager.py` & `tm_devices-1.4.1/src/tm_devices/device_manager.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/driver_mixins/analysis_object_mixins.py` & `tm_devices-1.4.1/src/tm_devices/driver_mixins/analysis_object_mixins.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/driver_mixins/class_extension_mixin.py` & `tm_devices-1.4.1/src/tm_devices/driver_mixins/class_extension_mixin.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/driver_mixins/licensed_mixin.py` & `tm_devices-1.4.1/src/tm_devices/driver_mixins/licensed_mixin.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/driver_mixins/signal_generator_mixin.py` & `tm_devices-1.4.1/src/tm_devices/driver_mixins/signal_generator_mixin.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/driver_mixins/usb_drives_mixin.py` & `tm_devices-1.4.1/src/tm_devices/driver_mixins/usb_drives_mixin.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/__init__.py` & `tm_devices-1.4.1/src/tm_devices/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/api/rest_api/margin_testers/margin_tester.py` & `tm_devices-1.4.1/src/tm_devices/drivers/api/rest_api/margin_testers/margin_tester.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/api/rest_api/margin_testers/tmt4.py` & `tm_devices-1.4.1/src/tm_devices/drivers/api/rest_api/margin_testers/tmt4.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/api/rest_api/rest_api_device.py` & `tm_devices-1.4.1/src/tm_devices/drivers/api/rest_api/rest_api_device.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/device.py` & `tm_devices-1.4.1/src/tm_devices/drivers/device.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/device_driver_mapping.py` & `tm_devices-1.4.1/src/tm_devices/drivers/device_driver_mapping.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/device_type_classes.py` & `tm_devices-1.4.1/src/tm_devices/drivers/device_type_classes.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/data_acquisition_systems/daq6510.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/data_acquisition_systems/daq6510.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/data_acquisition_systems/data_acquisition_system.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/data_acquisition_systems/data_acquisition_system.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/digital_multimeters/digital_multimeter.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/digital_multimeters/digital_multimeter.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/digital_multimeters/dmm6500/dmm6500.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/digital_multimeters/dmm6500/dmm6500.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/digital_multimeters/dmm7500/dmm7500.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/digital_multimeters/dmm7500/dmm7500.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/digital_multimeters/dmm7500/dmm7510.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/digital_multimeters/dmm7500/dmm7510.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/digital_multimeters/dmm7500/dmm7512.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/digital_multimeters/dmm7500/dmm7512.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/ieee488_2_commands.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/ieee488_2_commands.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/pi_device.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/pi_device.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/power_supplies/power_supply.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/power_supplies/power_supply.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/power_supplies/psu2200/__init__.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/power_supplies/psu2200/__init__.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/power_supplies/psu2200/psu2200.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/power_supplies/psu2200/psu2200.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/power_supplies/psu2200/psu2220.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/power_supplies/psu2200/psu2220.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/power_supplies/psu2200/psu2230.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/power_supplies/psu2200/psu2230.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/power_supplies/psu2200/psu2231.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/power_supplies/psu2200/psu2231.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/power_supplies/psu2200/psu2231a.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/power_supplies/psu2200/psu2231a.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/power_supplies/psu2200/psu2280.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/power_supplies/psu2200/psu2280.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/power_supplies/psu2200/psu2281.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/power_supplies/psu2200/psu2281.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/__init__.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/__init__.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/scope.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/scope.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope/__init__.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope/__init__.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope/lpd6.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope/lpd6.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope/mso2.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope/mso2.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope/mso4.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope/mso4.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope/mso4b.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope/mso4b.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope/mso5.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope/mso5.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope/mso5b.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope/mso5b.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope/mso5lp.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope/mso5lp.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope/mso6.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope/mso6.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope/mso6b.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope/mso6b.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope/tekscope.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope/tekscope.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope/tekscopesw.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope/tekscopesw.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_2k/dpo2k.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_2k/dpo2k.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_2k/dpo2kb.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_2k/dpo2kb.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_2k/mso2k.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_2k/mso2k.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_2k/mso2kb.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_2k/mso2kb.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_2k/tekscope_2k.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_2k/tekscope_2k.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/__init__.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/__init__.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/dpo4k.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/dpo4k.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/dpo4kb.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/dpo4kb.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/mdo3.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/mdo3.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/mdo3k.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/mdo3k.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/mdo4k.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/mdo4k.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/mdo4kb.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/mdo4kb.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/mdo4kc.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/mdo4kc.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/mso4k.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/mso4k.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/mso4kb.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/mso4kb.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/tekscope_3k_4k.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_3k_4k/tekscope_3k_4k.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/__init__.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/__init__.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo5k.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo5k.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo5kb.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo5kb.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo70k.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo70k.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo70kc.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo70kc.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo70kd.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo70kd.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo70kdx.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo70kdx.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo70ksx.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo70ksx.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo7k.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo7k.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo7kc.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dpo7kc.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dsa70k.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dsa70k.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dsa70kc.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dsa70kc.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dsa70kd.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/dsa70kd.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/mso5k.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/mso5k.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/mso5kb.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/mso5kb.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/mso70k.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/mso70k.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/mso70kc.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/mso70kc.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/mso70kdx.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/mso70kdx.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/tekscope_5k_7k_70k.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tekscope_5k_7k_70k/tekscope_5k_7k_70k.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/scopes/tso/tsovu.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/scopes/tso/tsovu.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/afgs/afg.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/afgs/afg.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/afgs/afg31k.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/afgs/afg31k.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/afgs/afg3k.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/afgs/afg3k.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/afgs/afg3kb.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/afgs/afg3kb.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/afgs/afg3kc.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/afgs/afg3kc.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/awgs/__init__.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/awgs/__init__.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/awgs/awg.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/awgs/awg.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/awgs/awg5200.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/awgs/awg5200.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/awgs/awg5k.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/awgs/awg5k.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/awgs/awg5kb.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/awgs/awg5kb.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/awgs/awg5kc.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/awgs/awg5kc.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/awgs/awg70ka.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/awgs/awg70ka.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/awgs/awg70kb.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/awgs/awg70kb.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/awgs/awg7k.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/awgs/awg7k.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/awgs/awg7kb.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/awgs/awg7kb.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/awgs/awg7kc.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/awgs/awg7kc.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/signal_sources/signal_source.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/signal_sources/signal_source.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/__init__.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/__init__.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2400/__init__.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2400/__init__.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2400.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2400.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2400_interactive.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2400_interactive.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2400_standard.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2400_standard.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2401.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2401.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2410.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2410.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2450.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2450.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2460.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2460.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2461.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2461.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2470.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2400/smu2470.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/__init__.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/__init__.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2600.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2600.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2600b.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2600b.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2601a.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2601a.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2601b.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2601b.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2601b_pulse.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2601b_pulse.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2602a.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2602a.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2602b.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2602b.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2604a.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2604a.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2604b.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2604b.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2606b.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2606b.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2611a.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2611a.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2611b.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2611b.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2612a.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2612a.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2612b.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2612b.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2614a.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2614a.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2614b.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2614b.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2634a.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2634a.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2634b.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2634b.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2635a.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2635a.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2635b.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2635b.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2636a.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2636a.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2636b.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2636b.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2650a.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2650a.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2651a.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2651a.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2657a.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu2600/smu2657a.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu6000/smu6000.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu6000/smu6000.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu6000/smu6430.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu6000/smu6430.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu6000/smu6514.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu6000/smu6514.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/smu6000/smu6517b.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/smu6000/smu6517b.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/source_measure_units/source_measure_unit.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/source_measure_units/source_measure_unit.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/systems_switches/ss3706a.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/systems_switches/ss3706a.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/systems_switches/systems_switch.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/systems_switches/systems_switch.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/drivers/pi/tsp_device.py` & `tm_devices-1.4.1/src/tm_devices/drivers/pi/tsp_device.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/helpers/__init__.py` & `tm_devices-1.4.1/src/tm_devices/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/helpers/alias_dict.py` & `tm_devices-1.4.1/src/tm_devices/helpers/alias_dict.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/helpers/constants_and_dataclasses.py` & `tm_devices-1.4.1/src/tm_devices/helpers/constants_and_dataclasses.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/helpers/dataclass_mixins.py` & `tm_devices-1.4.1/src/tm_devices/helpers/dataclass_mixins.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/helpers/enums.py` & `tm_devices-1.4.1/src/tm_devices/helpers/enums.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/helpers/functions.py` & `tm_devices-1.4.1/src/tm_devices/helpers/functions.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/helpers/read_only_cached_property.py` & `tm_devices-1.4.1/src/tm_devices/helpers/read_only_cached_property.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/helpers/singleton_metaclass.py` & `tm_devices-1.4.1/src/tm_devices/helpers/singleton_metaclass.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/helpers/standalone_functions.py` & `tm_devices-1.4.1/src/tm_devices/helpers/standalone_functions.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/src/tm_devices/helpers/stubgen.py` & `tm_devices-1.4.1/src/tm_devices/helpers/stubgen.py`

 * *Files identical despite different names*

### Comparing `tm_devices-1.4.0/PKG-INFO` & `tm_devices-1.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tm_devices
-Version: 1.4.0
+Version: 1.4.1
 Summary: Manage connections and interactions with Test & Measurement devices.
 Home-page: https://pypi.org/project/tm_devices/
 License: Apache-2.0
 Keywords: REST API,SCPI,TSP,Tektronix,Test & Measurement,VISA
 Author: Tektronix
 Author-email: opensource@tektronix.com
 Maintainer: Tektronix
@@ -115,15 +115,15 @@
     scope = device_manager.add_scope("192.168.0.100")
     scope.query("*IDN?")
     print(scope)
 ```
 
 ### Supported Devices & Software Solutions
 
-> \[!TIP\]
+> [!TIP]
 > Visit the [Glossary](https://tinyurl.com/tek-tm-devices/docs/glossary.md) to see definitions for all symbols and abbreviations.
 
 <div markdown="1" class="custom-table-center-cells device-support-table">
 
 <div markdown="1" class="custom-table-title">
 
 _Device Support Levels_
```

