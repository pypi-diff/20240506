# Comparing `tmp/eflips_ingest-1.2.0.tar.gz` & `tmp/eflips_ingest-1.2.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eflips_ingest-1.2.0.tar", max compression
+gzip compressed data, was "eflips_ingest-1.2.0a0.tar", max compression
```

## Comparing `eflips_ingest-1.2.0.tar` & `eflips_ingest-1.2.0a0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    34143 2024-05-06 16:17:04.686006 eflips_ingest-1.2.0/LICENSE.md
--rw-r--r--   0        0        0     7014 2024-05-06 16:17:04.686006 eflips_ingest-1.2.0/README.md
--rw-r--r--   0        0        0      207 2024-05-06 16:17:04.690006 eflips_ingest-1.2.0/eflips/ingest/__init__.py
--rw-r--r--   0        0        0     5978 2024-05-06 16:17:04.690006 eflips_ingest-1.2.0/eflips/ingest/base.py
--rw-r--r--   0        0        0    16293 2024-05-06 16:17:04.690006 eflips_ingest-1.2.0/eflips/ingest/dummy.py
--rw-r--r--   0        0        0        0 2024-05-06 16:17:04.690006 eflips_ingest-1.2.0/eflips/ingest/legacy/__init__.py
--rw-r--r--   0        0        0    63454 2024-05-06 16:17:04.690006 eflips_ingest-1.2.0/eflips/ingest/legacy/bvgxml.py
--rw-r--r--   0        0        0      549 2024-05-06 16:17:04.690006 eflips_ingest-1.2.0/eflips/ingest/legacy/vdv452/vdv2.py
--rw-r--r--   0        0        0      383 2024-05-06 16:17:04.690006 eflips_ingest-1.2.0/eflips/ingest/legacy/xmldata/README.md
--rw-r--r--   0        0        0     1065 2024-05-06 16:17:04.690006 eflips_ingest-1.2.0/eflips/ingest/legacy/xmldata/__init__.py
--rw-r--r--   0        0        0    47033 2024-05-06 16:17:04.690006 eflips_ingest-1.2.0/eflips/ingest/legacy/xmldata/bvg_xml.py
--rw-r--r--   0        0        0     4027 2024-05-06 16:17:04.690006 eflips_ingest-1.2.0/eflips/ingest/util.py
--rw-r--r--   0        0        0    54731 2024-05-06 16:17:04.690006 eflips_ingest-1.2.0/eflips/ingest/vdv.py
--rw-r--r--   0        0        0      618 2024-05-06 16:17:04.690006 eflips_ingest-1.2.0/eflips/ingest/vdv452data/__init__.py
--rw-r--r--   0        0        0    54461 2024-05-06 16:17:04.690006 eflips_ingest-1.2.0/eflips/ingest/vdv452data/vdv452_v1_5.py
--rw-r--r--   0        0        0     1120 2024-05-06 16:17:04.690006 eflips_ingest-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     8056 1970-01-01 00:00:00.000000 eflips_ingest-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    34143 2024-02-13 18:24:50.048548 eflips_ingest-1.2.0a0/LICENSE.md
+-rw-r--r--   0        0        0     7014 2024-04-01 14:04:27.651157 eflips_ingest-1.2.0a0/README.md
+-rw-r--r--   0        0        0      207 2024-04-01 14:04:27.651494 eflips_ingest-1.2.0a0/eflips/ingest/__init__.py
+-rw-r--r--   0        0        0     5978 2024-04-19 12:42:52.197526 eflips_ingest-1.2.0a0/eflips/ingest/base.py
+-rw-r--r--   0        0        0    16283 2024-04-19 12:42:52.197795 eflips_ingest-1.2.0a0/eflips/ingest/dummy.py
+-rw-r--r--   0        0        0        0 2024-04-01 14:16:33.464380 eflips_ingest-1.2.0a0/eflips/ingest/legacy/__init__.py
+-rw-r--r--   0        0        0    63454 2024-04-01 14:16:33.465214 eflips_ingest-1.2.0a0/eflips/ingest/legacy/bvgxml.py
+-rw-r--r--   0        0        0      549 2024-04-29 11:48:41.323942 eflips_ingest-1.2.0a0/eflips/ingest/legacy/vdv452/vdv2.py
+-rw-r--r--   0        0        0      383 2024-04-01 14:16:33.465541 eflips_ingest-1.2.0a0/eflips/ingest/legacy/xmldata/README.md
+-rw-r--r--   0        0        0     1065 2024-04-01 14:16:33.465853 eflips_ingest-1.2.0a0/eflips/ingest/legacy/xmldata/__init__.py
+-rw-r--r--   0        0        0    47033 2024-04-01 14:16:33.466102 eflips_ingest-1.2.0a0/eflips/ingest/legacy/xmldata/bvg_xml.py
+-rw-r--r--   0        0        0     3049 2024-04-01 14:16:33.466569 eflips_ingest-1.2.0a0/eflips/ingest/util.py
+-rw-r--r--   0        0        0    46557 2024-04-30 19:00:38.473490 eflips_ingest-1.2.0a0/eflips/ingest/vdv.py
+-rw-r--r--   0        0        0      618 2024-04-29 12:47:00.182773 eflips_ingest-1.2.0a0/eflips/ingest/vdv452data/__init__.py
+-rw-r--r--   0        0        0    45974 2024-04-30 19:00:38.477621 eflips_ingest-1.2.0a0/eflips/ingest/vdv452data/vdv452_v1_5.py
+-rw-r--r--   0        0        0     1126 2024-04-30 19:00:47.173640 eflips_ingest-1.2.0a0/pyproject.toml
+-rw-r--r--   0        0        0     8058 1970-01-01 00:00:00.000000 eflips_ingest-1.2.0a0/PKG-INFO
```

### Comparing `eflips_ingest-1.2.0/LICENSE.md` & `eflips_ingest-1.2.0a0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.2.0/README.md` & `eflips_ingest-1.2.0a0/README.md`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.2.0/eflips/ingest/base.py` & `eflips_ingest-1.2.0a0/eflips/ingest/base.py`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.2.0/eflips/ingest/dummy.py` & `eflips_ingest-1.2.0a0/eflips/ingest/dummy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import os
 import pickle
-import shutil
 from dataclasses import dataclass
 from datetime import timedelta, datetime
 from enum import Enum
 from pathlib import Path
 from typing import Dict, Tuple, Callable
 from uuid import UUID, uuid4
 
+import shutil
 import sqlalchemy
 from eflips.model.depot import Depot, AssocPlanProcess, Process, Area, Plan, AreaType
 from eflips.model.general import Scenario, VehicleType
 from eflips.model.network import Station, Line, Route, VoltageLevel, ChargeType
 from eflips.model.schedule import Trip, Rotation, TripType
 from sqlalchemy import create_engine
 from sqlalchemy.orm import Session
@@ -90,15 +90,15 @@
                     opportunity_charging_capable=True,
                     consumption=1,
                 )
                 session.add(vehicle_type_3)
             case _:
                 raise ValueError("Invalid bus type")
 
-    def prepare(  # type: ignore[override]
+    def prepare(  # type: ignore
         self,
         name: str,
         depot_count: int,
         line_count: int,
         rotation_per_line: int,
         opportunity_charging: bool,
         bus_type: BusType,
```

### Comparing `eflips_ingest-1.2.0/eflips/ingest/legacy/bvgxml.py` & `eflips_ingest-1.2.0a0/eflips/ingest/legacy/bvgxml.py`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.2.0/eflips/ingest/legacy/vdv452/vdv2.py` & `eflips_ingest-1.2.0a0/eflips/ingest/legacy/vdv452/vdv2.py`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.2.0/eflips/ingest/legacy/xmldata/__init__.py` & `eflips_ingest-1.2.0a0/eflips/ingest/legacy/xmldata/__init__.py`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.2.0/eflips/ingest/legacy/xmldata/bvg_xml.py` & `eflips_ingest-1.2.0a0/eflips/ingest/legacy/xmldata/bvg_xml.py`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.2.0/eflips/ingest/vdv.py` & `eflips_ingest-1.2.0a0/eflips/ingest/vdv.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import csv
 import enum
 import glob
 import logging
 import os
 import pickle
 import re
+import warnings
 from dataclasses import dataclass
 from datetime import date, timedelta, datetime, time
 from enum import Enum
 from pathlib import Path
 from typing import Dict, Callable, Tuple, Optional, List
 from uuid import UUID, uuid4
 from zipfile import ZipFile
 from zoneinfo import ZoneInfo
 
 from eflips.model import VehicleType, Scenario, Rotation, Station, Line, Route, Trip, TripType, StopTime
 from sqlalchemy import create_engine
 from sqlalchemy.orm import Session
 from tqdm.auto import tqdm
 
-from eflips.ingest.base import AbstractIngester
+from eflips.ingest import AbstractIngester
 from eflips.ingest.vdv452data import (
     VdvBaseObject,
     BasisVerGueltigkeit,
     Firmenkalender,
     RecOrt,
     MengeFzgTyp,
     RecSel,
@@ -41,16 +42,15 @@
     """
     An enum for the data types as specified in VDV 451/452. We map the different data types to two main types:
     - CHAR: Character data
     - NUM: Numeric data
     """
 
     CHAR = "char"
-    INT = "num"
-    FLOAT = enum.auto
+    NUM = "num"
 
 
 class VDV_Table_Name(enum.Enum):
     """
     An enum for the table names as Specified in VDV 451/452. Only the strings are used here as the numbers
     have never been encountered in practice.
     """
@@ -161,66 +161,16 @@
     character_set: str
     table_name: VDV_Table_Name
     column_names_and_data_types: list[
         Tuple[str, Optional[VDV_Data_Type]]
     ]  # None (optional) in the VDV_Data_Type represents "other / invalid data type" here
 
 
-def fix_identical_stop_times(stop_times: List[StopTime]) -> None:
-    """
-    This function goes through a list of stop times and changes the arrival time of a stop time to be the same as the
-
-    :param stop_times: A list of stop times. The list is assumed to be sorted by arrival time.
-    :return: Nothing. The list is modified in place.
-    """
-    # First, identify the indizes of the stop times that have the same arrival time
-    indizes_of_identical_arrival_times: Dict[datetime, List[int]] = {}
-    for i, stop_time in enumerate(stop_times):
-        if stop_time.arrival_time not in indizes_of_identical_arrival_times:
-            indizes_of_identical_arrival_times[stop_time.arrival_time] = []
-        indizes_of_identical_arrival_times[stop_time.arrival_time].append(i)
-    indizes_of_identical_arrival_times = {k: v for k, v in indizes_of_identical_arrival_times.items() if len(v) > 1}
-
-    # Now depending on the length of the list, we have to adjust the arrival times, so they are evenly spaced
-    # throughout a minute (e.g. with 2 stops, the first one arrives at 12:00:00 and the second one at 12:00:30)
-    # We do this by adding a timedelta to the arrival time of the stop time.
-    # However, if the stop time is the last one in the list, we then need to *subtract* the offest, so the last
-    # time stays the same
-
-    for identical_arrival_times in indizes_of_identical_arrival_times.values():
-        assert len(identical_arrival_times) > 1
-        # We cannot assume the minimum resolution is one minute. So we need to check the minimum difference
-        # Before and after
-        if identical_arrival_times[0] != 0:
-            diff_before = (
-                stop_times[identical_arrival_times[0]].arrival_time
-                - stop_times[identical_arrival_times[0] - 1].arrival_time
-            )
-        else:
-            diff_before = timedelta(seconds=60)
-        if identical_arrival_times[-1] != len(stop_times) - 1:
-            diff_after = (
-                stop_times[identical_arrival_times[-1] + 1].arrival_time
-                - stop_times[identical_arrival_times[-1]].arrival_time
-            )
-        else:
-            diff_after = timedelta(seconds=60)
-        # We take the minimum of the two
-        offset = min(diff_before, diff_after) / len(identical_arrival_times)
-        for i, idx in enumerate(identical_arrival_times):
-            stop_times[idx].arrival_time += i * offset
-        if idx == len(stop_times) - 1:
-            # This is how much we shifted the last stop time, so we need to subtract it again
-            max_offset = (len(identical_arrival_times) - 1) * offset
-            for idx in identical_arrival_times:
-                stop_times[idx].arrival_time -= max_offset
-
-
 class VdvIngester(AbstractIngester):
-    def prepare(  # type: ignore[override]
+    def prepare(
         self,
         x10_zip_file: Path,
         progress_callback: None | Callable[[float], None] = None,
     ) -> Tuple[bool, UUID | Dict[str, str]]:
         """
         Prepare and validate the input data for ingestion.
 
@@ -253,16 +203,14 @@
         with open(dir / "all_tables.pkl", "wb") as fp:
             pickle.dump(all_tables, fp)
 
         # If all tables are present, return the UUID
         return True, uuid
 
     def ingest(self, uuid: UUID, progress_callback: None | Callable[[float], None] = None) -> None:
-        logger = logging.getLogger(__name__)
-
         # Load the paths to the tables
         temp_dir = self.path_for_uuid(uuid)
         all_tables_file = Path(temp_dir) / "all_tables.pkl"
         with open(all_tables_file, "rb") as fp:
             all_tables = pickle.load(fp)
 
         # For each table, turn it into a list of VDV base objects
@@ -278,33 +226,39 @@
         engine = create_engine(self.database_url)
         with Session(engine) as session:
             try:
                 scenario = Scenario(name=f"Created from VDV data with UUID {uuid}")
                 session.add(scenario)
 
                 # Vehicle Types
-                vehicle_types_by_vdv_pk: Dict[Tuple[int | date | str, ...], VehicleType] = {}
+                vehicle_types_by_vdv_pk: Dict[Tuple[int, int], VehicleType] = {}
                 for vdv_vehicle_type in all_data[VDV_Table_Name.MENGE_FZG_TYP]:
                     assert isinstance(vdv_vehicle_type, MengeFzgTyp)
                     db_vehicle_type = vdv_vehicle_type.to_vehicle_type(scenario)
                     session.add(db_vehicle_type)
                     vehicle_types_by_vdv_pk[vdv_vehicle_type.primary_key] = db_vehicle_type
 
                 # Rotations
-                rotations_by_vdv_pk: Dict[Tuple[int | str | date, ...], Rotation] = {}
+                rotations_by_vdv_pk: Dict[Tuple[int, str, date, ...], Rotation] = {}
 
                 # We may need a dummy vehicle type for rotations that do not have a vehicle type associated with them
                 dummy_vehicle_type: VehicleType | None = None
 
                 for vdv_rotation in all_data[VDV_Table_Name.REC_UMLAUF]:
                     assert isinstance(vdv_rotation, RecUmlauf)
 
                     if vdv_rotation.fzg_typ_nr is None and dummy_vehicle_type is None:
                         # We need to add a dummy vehicle type for the first time, create it
-                        dummy_vehicle_type = self.create_dummy_vehicle_type(scenario)
+                        dummy_vehicle_type = VehicleType(
+                            scenario=scenario,
+                            name="Dummy Vehicle Type",
+                            opportunity_charging_capable=False,
+                            battery_capacity=10000,
+                            charging_curve=[[0, 1], [1000, 1000]],
+                        )
                         session.add(dummy_vehicle_type)
 
                     db_rotation = vdv_rotation.to_rotation(
                         scenario, vehicle_types_by_vdv_pk, dummy_vehicle_type=dummy_vehicle_type
                     )
                     session.add(db_rotation)
                     rotations_by_vdv_pk[vdv_rotation.primary_key] = db_rotation
@@ -322,15 +276,15 @@
                 # The values of this dict are not unique, so we only add the unique ones to the database
                 for station in set(stations_by_vdv_pk.values()):
                     session.add(station)
 
                 # Lines
                 # The same Line might be shared by multiple RecLid objects, but is unique by li_kuerzel
                 lines_by_li_kuerzel: Dict[str, Line] = {}
-                lines_by_vdv_pk: Dict[Tuple[int | date | str, ...], Line] = {}
+                lines_by_vdv_pk: Dict[Tuple[int, ...], Line] = {}
 
                 assert all(isinstance(x, RecLid) for x in all_data[VDV_Table_Name.REC_LID])
                 rec_lids = [x for x in all_data[VDV_Table_Name.REC_LID] if isinstance(x, RecLid)]
 
                 for rec_lid in rec_lids:
                     line_name = rec_lid.li_kuerzel
                     if line_name not in lines_by_li_kuerzel:
@@ -340,18 +294,18 @@
                     else:
                         line = lines_by_li_kuerzel[line_name]
                     lines_by_vdv_pk[rec_lid.primary_key] = line
 
                 # Routes
                 # Those are more intricate, as we will have to compose them from the RecLid and RecSel and ??? tables
                 # We need to construct quite a few helper dictionaries for this
-                lines_by_basis_version_and_li_nr: Dict[Tuple[int | date | str, ...], Line] = {
-                    (k[0], k[1]): v for k, v in lines_by_vdv_pk.items()
-                }
+                lines_by_basis_version_and_li_nr = {(k[0], k[1]): v for k, v in lines_by_vdv_pk.items()}
 
+                assert all(isinstance(x, RecSel) for x in all_data[VDV_Table_Name.REC_SEL])
+                rec_orts: List[RecOrt] = [x for x in all_data[VDV_Table_Name.REC_ORT] if isinstance(x, RecOrt)]
                 rec_orts_by_basis_version_and_onr_typ_nr_and_ort_nr = {
                     (r.basis_version, r.onr_typ_nr, r.ort_nr): r for r in rec_orts
                 }
 
                 assert all(isinstance(x, RecSel) for x in all_data[VDV_Table_Name.REC_SEL])
                 rec_sels: List[RecSel] = [x for x in all_data[VDV_Table_Name.REC_SEL] if isinstance(x, RecSel)]
                 rec_sel_by_basis_version_and_start_type_and_start_nr_and_end_type_and_end_nr = {
@@ -371,24 +325,21 @@
                         lid_verlaufs_by_basis_version_and_li_nr_and_str_li_var[key] = []
                     # Insert it in the correct order, by the lid_verlauf.li_lfd_nr
                     # Runtime expensive, but works
                     lid_verlaufs_by_basis_version_and_li_nr_and_str_li_var[key].append(lid_verlauf)
                     lid_verlaufs_by_basis_version_and_li_nr_and_str_li_var[key].sort(key=lambda x: x.li_lfd_nr)
 
                 # Now we can construct the routes
-                routes_by_vdv_pk: Dict[Tuple[int | date | str, ...], Route] = {}
+                routes_by_vdv_pk: Dict[Tuple[int, ...], Route] = {}
                 assert all(isinstance(x, RecLid) for x in all_data[VDV_Table_Name.REC_LID])
                 rec_lids = [x for x in all_data[VDV_Table_Name.REC_LID] if isinstance(x, RecLid)]
 
-                rec_selss: Dict[
-                    Tuple[int | date | str, ...], List[RecSel]
-                ] = {}  # Later we will use this to construct the trips
+                rec_selss: Dict[Tuple[int, int, str], Route] = {}  # Later we will use this to construct the trips
 
                 for rec_lid in rec_lids:
-                    route: Route
                     route, rec_selss[(rec_lid.basis_version, rec_lid.li_nr, rec_lid.str_li_var)] = rec_lid.to_route(
                         scenario=scenario,
                         lines_by_basis_version_andli_nr=lines_by_basis_version_and_li_nr,
                         rec_orts_by_basis_version_and_onr_typ_nr_and_ort_nr=rec_orts_by_basis_version_and_onr_typ_nr_and_ort_nr,
                         lid_verlaufs_by_basis_version_and_li_nr_and_str_li_var=lid_verlaufs_by_basis_version_and_li_nr_and_str_li_var,
                         stations_by_basis_version_and_onr_typ_nr_and_ort_nr=stations_by_vdv_pk,
                         rec_sel_by_basis_version_and_start_type_and_start_nr_and_end_type_and_end_nr=rec_sel_by_basis_version_and_start_type_and_start_nr_and_end_type_and_end_nr,
@@ -396,20 +347,14 @@
                     session.add(route)
                     routes_by_vdv_pk[rec_lid.primary_key] = route
 
                 # Now we can construct the trips
 
                 assert all(isinstance(x, SelFztFeld) for x in all_data[VDV_Table_Name.SEL_FZT_FELD])
                 sel_fzt_felds = [x for x in all_data[VDV_Table_Name.SEL_FZT_FELD] if isinstance(x, SelFztFeld)]
-                sel_fzt_felds_by_pk: Dict[Tuple[int | date | str, ...], List[SelFztFeld]] = {}
-                for this_sel_fzt_feld in sel_fzt_felds:
-                    pk = this_sel_fzt_feld.primary_key
-                    if pk not in sel_fzt_felds_by_pk:
-                        sel_fzt_felds_by_pk[pk] = []
-                    sel_fzt_felds_by_pk[pk].append(this_sel_fzt_feld)
 
                 assert all(isinstance(x, RecFrt) for x in all_data[VDV_Table_Name.REC_FRT])
                 rec_frts = [x for x in all_data[VDV_Table_Name.REC_FRT] if isinstance(x, RecFrt)]
 
                 if VDV_Table_Name.ORT_HZTF in all_data.keys():
                     assert all(isinstance(x, OrtHztf) for x in all_data[VDV_Table_Name.ORT_HZTF])
                     ort_hztfs = [x for x in all_data[VDV_Table_Name.ORT_HZTF] if isinstance(x, OrtHztf)]
@@ -448,63 +393,28 @@
                             rec_sel.bereich_nr,
                             rec_frt.fgr_nr,
                             rec_sel.onr_typ_nr,
                             rec_sel.ort_nr,
                             rec_sel.sel_ziel_typ,
                             rec_sel.sel_ziel,
                         )
-
-                        if sel_fzt_feld_pk in sel_fzt_felds_by_pk.keys():
-                            sel_fzt_feld = sel_fzt_felds_by_pk[sel_fzt_feld_pk]
-                        else:
-                            logger.debug(f"Could not find SelFztFeld for {sel_fzt_feld_pk}")
-                            # Find one by relaxing the constraints
-                            sel_fzt_feld = [
-                                x
-                                for x in sel_fzt_felds
-                                if (x.basis_version, x.bereich_nr, x.onr_typ_nr, x.ort_nr, x.sel_ziel_typ, x.sel_ziel)
-                                == (
-                                    rec_sel.basis_version,
-                                    rec_sel.bereich_nr,
-                                    rec_sel.onr_typ_nr,
-                                    rec_sel.ort_nr,
-                                    rec_sel.sel_ziel_typ,
-                                    rec_sel.sel_ziel,
-                                )
-                            ]
-                            sel_fzt_feld = [sel_fzt_feld[0]]
-
+                        sel_fzt_feld = [x for x in sel_fzt_felds if x.primary_key == sel_fzt_feld_pk]
                         if len(sel_fzt_feld) != 1:
-                            logger.info(f"Could not find exactly one SelFztFeld for {sel_fzt_feld_pk}")
-                            # If there are more than one, make sure the durations are the same
-                            if len(sel_fzt_feld) > 1:
-                                durations = [x.sel_fzt for x in sel_fzt_feld]
-                                if len(set(durations)) != 1:
-                                    logger.warning(
-                                        f"Multiple SelFztFelds for {sel_fzt_feld_pk} have different durations: {durations}"
-                                    )
-                                    raise ValueError(
-                                        f"Multiple SelFztFelds for {sel_fzt_feld_pk} have different durations: {durations}"
-                                    )
-                                else:
-                                    duration = durations[0]
-                            else:
-                                # Length is 0 -- create a zero duration
-                                duration = timedelta(minutes=0)
+                            warnings.warn(f"Could not find exactly one SelFztFeld for {sel_fzt_feld_pk}")
                             # For now, create a dummy one
                             sel_fzt_feld = [
                                 SelFztFeld(
                                     basis_version=rec_sel.basis_version,
                                     bereich_nr=rec_sel.bereich_nr,
                                     fgr_nr=rec_frt.fgr_nr,
                                     onr_typ_nr=rec_sel.onr_typ_nr,
                                     ort_nr=rec_sel.ort_nr,
                                     sel_ziel_typ=rec_sel.sel_ziel_typ,
                                     sel_ziel=rec_sel.sel_ziel,
-                                    sel_fzt=duration,
+                                    sel_fzt=timedelta(minutes=1),
                                 )
                             ]
                         this_route_sel_fzt_felds.append(sel_fzt_feld[0])
 
                     # Calculate the dwell durations and driving durations for each station
                     elapsed_duration = rec_frt.frt_start
                     arrival_time_from_start: List[timedelta] = []
@@ -523,19 +433,19 @@
                             first_station_ort_hztfs = [x for x in ort_hztfs if x.position_key == first_station_pk]
 
                             if len(first_station_rec_frt_hzts) == 1:
                                 dwell_duration = first_station_rec_frt_hzts[0].frt_hzt_zeit
                             elif len(first_station_ort_hztfs) == 1:
                                 dwell_duration = first_station_ort_hztfs[0].hp_hzt
                             else:
-                                logger.debug(
-                                    f"Could not find any dwell duration for the station {first_station_pk}. Adding 0s."
+                                warnings.warn(
+                                    f"Could not find any dwell duration for the first station {first_station_pk}"
                                 )
                                 # For now, create a dummy one
-                                dwell_duration = timedelta(seconds=0)
+                                dwell_duration = timedelta(seconds=1)
 
                             arrival_time_from_start.append(
                                 elapsed_duration
                             )  # For the first station, the arrival time is the start of the trip
                             dwell_durations.append(dwell_duration)  # dwell duration for the first station
                             elapsed_duration += dwell_duration
 
@@ -555,26 +465,25 @@
                         next_station_ort_hztfs = [x for x in ort_hztfs if x.position_key == next_station_pk]
 
                         if len(next_station_rec_frt_hzts) == 1:
                             dwell_duration = next_station_rec_frt_hzts[0].frt_hzt_zeit
                         elif len(next_station_ort_hztfs) == 1:
                             dwell_duration = next_station_ort_hztfs[0].hp_hzt
                         else:
-                            logger.debug(
-                                f"Could not find any dwell duration for the station {next_station_pk}. Adding 0s."
-                            )
+                            warnings.warn(f"Could not find any dwell duration for the first station {first_station_pk}")
                             # For now, create a dummy one
-                            dwell_duration = timedelta(seconds=0)
+                            dwell_duration = timedelta(seconds=1)
 
                         dwell_durations.append(dwell_duration)
                         elapsed_duration += dwell_duration
 
                     ### CREATE THE TRIP
                     # We need to do this on all days that have the same tagesart as the rec_frt
                     # We need to find the tagesart of the rec_frt
+                    session.flush()  # TODO: REMOVE THIS FLUSH
                     for firmenkalender in firmenkalenders:
                         if firmenkalender.tagesart_nr == rec_frt.tagesart_nr:
                             the_date = firmenkalender.betriebstag
 
                             # Check if a specific rotation for this day exists
                             vdv_pk_and_date = (rec_frt.basis_version, rec_frt.tagesart_nr, rec_frt.um_uid, the_date)
                             if vdv_pk_and_date in rotations_by_vdv_pk_and_date:
@@ -615,78 +524,32 @@
                                     trip=trip,
                                     station=station,
                                     arrival_time=arrival_time,
                                     dwell_duration=dwell_duration,
                                 )
                                 stop_times.append(stop_time)
 
-                            # Fix identical stop times
-                            fix_identical_stop_times(stop_times)
-
                             # Look up the rotation using the basis_version and um_uid
                             trip.rotation = rotation
                             session.add(trip)
-
-                # Delete all rotations in this scenario with no trips
-                session.flush()
-                for rotation in scenario.rotations:
-                    if len(rotation.trips) == 0:
-                        session.delete(rotation)
+                            session.commit()  # TODO: Remove this flush
 
             except Exception as e:
                 session.rollback()
                 raise e
             finally:
                 session.commit()
 
     @classmethod
-    def create_dummy_vehicle_type(cls, scenario: Scenario) -> VehicleType:
-        dummy_vehicle_type = VehicleType(
-            scenario=scenario,
-            name="Dummy Vehicle Type",
-            opportunity_charging_capable=False,
-            battery_capacity=10000,
-            charging_curve=[[0, 1], [1000, 1000]],
-        )
-        return dummy_vehicle_type
-
-    @classmethod
     def prepare_param_names(cls) -> Dict[str, str | Dict[Enum, str]]:
-        """
-        A dictionary containing the parameter names for :meth:`prepare`.
-
-        These should be short, descriptive names for the parameters of the :meth:`prepare` method. The keys must be the
-        names of the parameters, and the values should be strings describing the parameter. If the keyword argument is
-        an enumerated type, the value should be a dictionary with the keys being the members.
-
-        This method can then be used to generate a help text for the user.
-
-        :return: A dictionary containing the parameter hints for the prepare method.
-        """
-        return {
-            "x10_zip_file": "VDV data archive",
-        }
+        pass
 
     @classmethod
     def prepare_param_description(cls) -> Dict[str, str | Dict[Enum, str]]:
-        """
-        A dictionary containing the parameter descriptions for :meth:`prepare`.
-
-        These should be longer, more detailed descriptions of the parameters of the :meth:`prepare`
-        method. The keys must be the names of the parameters, and the values should be strings describing the parameter.
-
-        This method can then be used to generate a help text for the user.
-
-        :return: A dictionary containing the parameter hints for the prepare method.
-        """
-        return {
-            "x10_zip_file": "A zip file containing the VDV data. The zip file must contain all necessary tables for the"
-            " VDV 451/452 format. These should be in the form of .x10 files in the top level of the zip"
-            " file.",
-        }
+        pass
 
 
 def validate_zip_file(zipfile: Path) -> bool | Dict[str, str]:
     """
     Validate the zip file.
 
     :param zipfile: A pathlib.Path object representing the path to the zip file.
@@ -756,15 +619,15 @@
                 )
 
             else:
                 all_tables[eingangsdatentable.table_name] = eingangsdatentable
 
         except (ValueError, UnicodeDecodeError) as e:
             msg = "While processing " + abs_file_path + " the following exception occurred: "
-            logger.debug(msg, exc_info=e)
+            logger.warning(msg, exc_info=e)
             continue
 
     # Required Tables:
     # siehe ganz oben in der File fuer explanation
 
     if not set(VdvRequiredTables.required_tables.keys()) <= set(all_tables.keys()):
         # Compute all tables that are required but not in the tables in the files, to display them to the user
@@ -950,35 +813,30 @@
     dtypes: list[Optional[VDV_Data_Type]] = []
     for part in datatype_str:
         part = part.lstrip()  # remove leading spaces
 
         # check if the datatype is valid (e.g. 'num[9.0]' or 'char[40]' etc.)
         # according to the VDV 451 specification, only 'char[n]' and 'num[n.0]' are allowed
 
-        regex = r"(char\[[0-9]+\]|num\[[0-9]+.[0-9]+\])+"
+        regex = r"(char\[[0-9]+\]|num\[[0-9]+.0\])+"
 
         if not re.match(regex, part):
             # Avoid the program to crash if the datatype is invalid, but still log a warning
             # Sometimes, there are floats used for additional columns (columns not formally included the VDV 452 specification)
             dtypes.append(None)
             # todo genauere angabe, in welcher Datei / Spalte es auftrat?
-            msg = f"Invalid datatype formatting in VDV 451 file: {part} does not match 'char[n]' or 'num[n.n]'. Column will not be imported."
+            msg = f"Invalid datatype formatting in VDV 451 file: {part} does not match 'char[n]' or 'num[n.0]'. Column will not be imported."
             logger.warning(msg)
             continue
 
-        regex_for_char = r"char\[[0-9]+\]"
-        regex_for_int = r"num\[[0-9]+.0\]"
-        regex_for_float = r"num\[[0-9]+.[0-9]+\]"
-
-        if re.match(regex_for_char, part):
+        type_info, size_info = part.split("[")
+        if type_info == "num":
+            dtypes.append(VDV_Data_Type.NUM)
+        else:
             dtypes.append(VDV_Data_Type.CHAR)
-        elif re.match(regex_for_int, part):
-            dtypes.append(VDV_Data_Type.INT)
-        elif re.match(regex_for_float, part):
-            dtypes.append(VDV_Data_Type.FLOAT)
 
     return dtypes
 
 
 def import_vdv452_table_records(EingangsdatenTabelle: VDVTable) -> list[VdvBaseObject]:
     """
     Imports the records of a VDV 451 table into the database.
@@ -996,15 +854,15 @@
                 logger.debug("Skipping line: " + str(row))
                 continue
 
             # Remove the 'rec' from the row
             row_data = row[1:]
 
             # create the json obj and give every column value the correct datatype
-            e_data: Dict[str, str | int | float | None] = {}
+            e_data: Dict[str, str | int | None] = {}
 
             if len(row_data) != len(EingangsdatenTabelle.column_names_and_data_types):
                 raise ValueError(
                     "The file"
                     + str(EingangsdatenTabelle.abs_file_path)
                     + " contains an record that has more or less columns than the header specifies. "
                     + "The record contains "
@@ -1021,63 +879,44 @@
                     # NULL Entry (Also possible for numbers - thats why it is done BEFORE the Int conversion!)
                     e_data[column_name] = None
 
                 elif column_data_type is None:
                     # Skip the column as it has an invalid data type.
                     continue
 
-                elif column_data_type == VDV_Data_Type.INT:
+                elif column_data_type == VDV_Data_Type.NUM:
                     try:
                         e_data[column_name] = int(row_data[i_col])
                     except ValueError as e:
                         e.add_note(
                             "The file"
                             + str(EingangsdatenTabelle.abs_file_path)
                             + " contains a non-numeric value in a column that is specified as numeric. Aborting."
                         )
                         raise e
-                elif column_data_type == VDV_Data_Type.FLOAT:
-                    try:
-                        e_data[column_name] = float(row_data[i_col])
-                    except ValueError as e:
-                        e.add_note(
-                            "The file"
-                            + str(EingangsdatenTabelle.abs_file_path)
-                            + " contains a non-numeric value in a column that is specified as numeric. Aborting."
-                        )
-                        raise e
-                elif column_data_type == VDV_Data_Type.CHAR:
+                else:  # CHAR
                     e_data[column_name] = row_data[i_col]
-                else:
-                    raise ValueError(
-                        "The file"
-                        + str(EingangsdatenTabelle.abs_file_path)
-                        + " contains a column with an invalid data type: "
-                        + str(column_data_type)
-                        + ". Aborting."
-                    )
             dict_list.append(e_data)
 
         # Now that we have created a nice dictionary, turn it into an object of the corresponding dataclass
         match EingangsdatenTabelle.table_name:
             case VDV_Table_Name.BASIS_VER_GUELTIGKEIT:
                 # At the current time, we only support one distinct entry for this table.
                 # If there are multiple. raise an error.
                 # However, if the same entry is present multiple times, we do not raise an error.
                 # So we need to turn the list of dictionaries inso a set of objects and check if the length is 1.
-                objects: List[VdvBaseObject] = []
+                objects = []
                 for d in dict_list:
                     objects.append(BasisVerGueltigkeit.from_dict(d))
                 if len(set(objects)) != 1:
                     raise ValueError(
                         "The table"
                         + str(EingangsdatenTabelle.table_name)
                         + " contains multiple distinct entries. Only one entry is allowed. Aborting."
                     )
-                return objects
 
             case VDV_Table_Name.FIRMENKALENDER:
                 return [Firmenkalender.from_dict(d) for d in dict_list]
             case VDV_Table_Name.REC_ORT:
                 return [RecOrt.from_dict(d) for d in dict_list]
             case VDV_Table_Name.MENGE_FZG_TYP:
                 return [MengeFzgTyp.from_dict(d) for d in dict_list]
```

### Comparing `eflips_ingest-1.2.0/eflips/ingest/vdv452data/__init__.py` & `eflips_ingest-1.2.0a0/eflips/ingest/vdv452data/__init__.py`

 * *Files identical despite different names*

### Comparing `eflips_ingest-1.2.0/eflips/ingest/vdv452data/vdv452_v1_5.py` & `eflips_ingest-1.2.0a0/eflips/ingest/vdv452data/vdv452_v1_5.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 """This file was originally generated by xsdata, v24.1, on 2024-01-29 15:42:25
 + modified
 
 Generator: DataclassGenerator
 See: https://xsdata.readthedocs.io/
 """
-import logging
 import warnings
 from abc import ABC, abstractmethod
 from collections import Counter
 from dataclasses import dataclass
 from datetime import date, timedelta
 from enum import Enum
 from typing import Optional, Dict, Tuple, List
 
-from eflips.model import VehicleType, Scenario, Rotation, Line, Route, AssocRouteStation, Station
-
-from eflips.ingest.util import get_altitude
+from eflips.model import VehicleType, Scenario, Rotation, TripType, Line, Route, AssocRouteStation, Station
 
 
 class OnrTyp(Enum):
     """
     The type of point in the schedule.
     """
 
@@ -35,14 +32,20 @@
 
 class RoutenArt(Enum):
     NORMAL = 1
     TO_DEPOT = 2
     FROM_DEPOT = 3
     ZUFAHRT = 4
 
+    def to_trip_type(self) -> TripType:
+        if self.type == RoutenArt.NORMAL:
+            return TripType.PASSENGER
+        else:
+            return TripType.EMPTY
+
 
 @dataclass
 class VdvBaseObject(ABC):
     basis_version: int
     """
     The `BasisVerGueltigkeit.basis_version` this object belongs to. Currently not used. 
 
@@ -57,15 +60,15 @@
         """
         The primary key of the object.
         """
         pass
 
     @classmethod
     @abstractmethod
-    def from_dict(cls, data: Dict[str, int | str | float | None]) -> "VdvBaseObject":
+    def from_dict(cls, data: Dict[str, int | str | None]) -> "VdvBaseObject":
         """
         Load the data from a dictionary.
         """
         pass
 
 
 @dataclass
@@ -101,15 +104,15 @@
     """
     This seems to be a dupllicate of `onr_typ_nr`. We do store it, but we do not use it.
 
     Restriction: Should be a positive integer.
     """
 
 
-@dataclass
+@dataclass()
 class BasisVerGueltigkeit(VdvBaseObject):
     """
     The dataclass corresponding to BASIS_VER_GUELTIGKEIT (993) in the VDV-452 specification.
 
     It allows different versions of the schedule to be stored in the same database. It is *not implemented* in the curent
     importer, we only allow there to be a single version of the schedule in the database.
 
@@ -119,47 +122,46 @@
     """
 
     ver_gueltigkeit: date
     """
     The date after which the schedule is valid.
     """
 
+    basis_version: str
+    """
+    A nine-digit numeric string that identifies the version of the schedule.
+    """
+
     @classmethod
-    def from_dict(cls, data: Dict[str, str | int | float | None]) -> "BasisVerGueltigkeit":
+    def from_dict(cls, data: Dict[str, int]) -> "BasisVerGueltigkeit":
         """
         Load the data from a dictionary.
         :param data: A dictionary with the data. It should contain:
             - "ver_gueltigkeit": The date after which the schedule is valid. in the format "YYYYMMDD".
             - "basis_version": A nine-digit numeric string that identifies the version of the schedule.
         :return: The object itself.
 
         """
-        assert isinstance(data["VER_GUELTIGKEIT"], int), "The `ver_gueltigkeit` should be an integer."
         year = data["VER_GUELTIGKEIT"] // 10000
         month = (data["VER_GUELTIGKEIT"] % 10000) // 100
         day = data["VER_GUELTIGKEIT"] % 100
 
-        assert isinstance(data["BASIS_VERSION"], int), "The `basis_version` should be an integer."
-
-        return BasisVerGueltigkeit(ver_gueltigkeit=date(year, month, day), basis_version=data["BASIS_VERSION"])
+        return BasisVerGueltigkeit(ver_gueltigkeit=date(year, month, day), basis_version=str(data["BASIS_VERSION"]))
 
-    @property
     def primary_key(self) -> Tuple[int | date | str, ...]:
         """
         The primary key of the object. Used e.g. to store it in a dictionary.
         :return:
         """
         return (self.ver_gueltigkeit,)
 
-    def __eq__(self: "BasisVerGueltigkeit", other: object) -> bool:
-        if not isinstance(other, BasisVerGueltigkeit):
-            return False
+    def __eq__(self, other):
         return self.ver_gueltigkeit == other.ver_gueltigkeit and self.basis_version == other.basis_version
 
-    def __hash__(self: "BasisVerGueltigkeit") -> int:
+    def __hash__(self):
         return hash((self.ver_gueltigkeit, self.basis_version))
 
 
 @dataclass(kw_only=True)
 class Firmenkalender(VdvBaseObject):
     """
     This class corresponds to the FIRMENKALENDER (384) in the VDV-452 specification.
@@ -175,38 +177,34 @@
 
     tagesart_nr: int
     """
     The type of day this is.
     """
 
     @classmethod
-    def from_dict(cls, data: Dict[str, str | int | float | None]) -> "Firmenkalender":
+    def from_dict(cls, data: Dict[str, int | str | None]) -> "Firmenkalender":
         """
         Load the data from a dictionary.
         :param data: A dictionary with the data. It should contain:
             - "BASIS_VERSION": The `BasisVerGueltigkeit.basis_version` this object belongs to. Currently not used.
             - "BETRIEBSTAG": The actual date of the day in the format "YYYYMMDD".
             - "TAGESART_NR": The type of day this is.
         :return: The object itself.
         """
-        assert isinstance(data["BETRIEBSTAG"], int), "The `betriebstag` should be an integer."
+
         year = data["BETRIEBSTAG"] // 10000
         month = (data["BETRIEBSTAG"] % 10000) // 100
         day = data["BETRIEBSTAG"] % 100
 
-        assert isinstance(data["BASIS_VERSION"], int), "The `basis_version` should be an integer."
-        assert isinstance(data["TAGESART_NR"], int), "The `tagesart_nr` should be an integer."
-
         return Firmenkalender(
             basis_version=data["BASIS_VERSION"],
             betriebstag=date(year, month, day),
             tagesart_nr=data["TAGESART_NR"],
         )
 
-    @property
     def primary_key(self) -> Tuple[int | date | str, ...]:
         """
         The primary key of the object. Used e.g. to store it in a dictionary.
         :return:
         """
         return self.basis_version, self.betriebstag
 
@@ -244,24 +242,53 @@
     str_li_var: str
     """
     An identifier for the line variant. TODO: Unclear at this point whether this is a route name?
     
     Restriction: Should be a six-character string.
     """
 
-    @property
+    produktiv: Optional[bool]
+    """
+    This is a flag that indicates whether the trip is a productive trip -> TripType.PASSENGER in eflips-model world or 
+    a non-productive trip -> TripType.EMPTY in eflips-model world.
+    """
+
     def primary_key(self) -> Tuple[int | date | str, ...]:
         """
         The primary key of the object. Used e.g. to store it in a dictionary.
         :return:
         """
         return self.basis_version, self.li_nr, self.str_li_var, self.li_lfd_nr
 
     @classmethod
-    def from_dict(cls, data: Dict[str, str | int | float | None]) -> "LidVerlauf":
+    def dict_by_first_three_pk(
+        cls, all_lid_verlaufs: List["LidVerlauf"]
+    ) -> Dict[Tuple[int, int, int], List["LidVerlauf"]]:
+        """
+        Create a dict of lists of the LiadVeralaufs for each route.
+        :param all_lid_verlaufs: A list of LidVerlauf objects.
+        :return: A Dict that maps the first three primary key elements to a list of LidVerlauf objects.
+        """
+        result = {}
+        for lid_verlauf in all_lid_verlaufs:
+            key = lid_verlauf.primary_key()[:3]
+            if key not in result:
+                result[key] = []
+            # Insert the LidVerlauf into the list, at a place so that the list will be sorted by li_lfd_nr
+            for i, other_lid_verlauf in enumerate(result[key]):
+                if lid_verlauf.li_lfd_nr < other_lid_verlauf.li_lfd_nr:
+                    result[key].insert(i, lid_verlauf)
+                    break
+            else:
+                result[key].append(lid_verlauf)
+
+        return result
+
+    @classmethod
+    def from_dict(cls, data: Dict[str, str | int | None]) -> "LidVerlauf":
         """
         Load the data from a dictionary.
         :param data: A dictionary with the data. It should contain:
             - "basis_version": The `BasisVerGueltigkeit.basis_version` this object belongs to. Currently not used.
             - "li_lfd_nr": The ordinal number of the line this object belongs to.
             - "li_nr": The "line number", which most closely corresponds to the `Line.name` in the eflips-model world.
             - "str_li_var": An identifier for the line variant. TODO: Unclear at this point whether this is a route name?
@@ -269,64 +296,59 @@
                 of point we are dealing with.
             - "ort_nr": This seems to be a dupllicate of `onr_typ_nr`. We do store it, but we do not use it.
             - "produktiv": This is a flag that indicates whether the trip is a productive trip -> TripType.PASSENGER in eflips-model world or
                 a non-productive trip -> TripType.EMPTY in eflips-model world.
         :return: The object itself.
         """
 
-        assert isinstance(data["LI_LFD_NR"], int), "The `li_lfd_nr` should be an integer."
         assert data["LI_LFD_NR"] > 0, "The `li_lfd_nr` should be a positive integer."
         assert isinstance(data["LI_NR"], int), "The `li_nr` should be an integer."
         assert isinstance(data["STR_LI_VAR"], str), "The `str_li_var` should be a string."
 
-        assert isinstance(data["ONR_TYP_NR"], int), "The `onr_typ_nr` should be an integer."
         assert data["ONR_TYP_NR"] > 0, "The `onr_typ_nr` should be a positive integer."
-        assert isinstance(data["ORT_NR"], int), "The `ort_nr` should be an integer."
         assert data["ORT_NR"] > 0, "The `ort_nr` should be a positive integer."
 
-        assert isinstance(data["BASIS_VERSION"], int), "The `basis_version` should be an integer."
+        if "PRODUKTIV" in data:
+            assert isinstance(data["PRODUKTIV"], bool), "The `produktiv` should be a boolean."
+        else:
+            data["PRODUKTIV"] = None
 
         return LidVerlauf(
             basis_version=data["BASIS_VERSION"],
             li_lfd_nr=data["LI_LFD_NR"],
             li_nr=data["LI_NR"],
             str_li_var=data["STR_LI_VAR"],
             onr_typ_nr=data["ONR_TYP_NR"],
             ort_nr=data["ORT_NR"],
+            produktiv=data["PRODUKTIV"],
         )
 
 
 @dataclass
 class OrtHztf(VdvBaseObjectWithONR):
     """
     ORT_HZTF (999) Stores the dwell duration at a stop for a trip. It is most equivalent to the `StopTime.dwell_duration`
     """
 
     fgr_nr: int
     """The number of the timing group. Part of primary key."""
 
     @property
-    def position_key(self) -> Tuple[int, int, int]:
+    def position_key(self):
         return self.basis_version, self.onr_typ_nr, self.ort_nr
 
     hp_hzt: timedelta
     """The time the trip waits at the stop in seconds."""
 
     @property
     def primary_key(self) -> Tuple[int | date | str, ...]:
         return self.basis_version, self.fgr_nr, self.onr_typ_nr, self.ort_nr
 
     @classmethod
-    def from_dict(cls, data: Dict[str, str | int | float | None]) -> "OrtHztf":
-        assert isinstance(data["BASIS_VERSION"], int), "The `basis_version` should be an integer."
-        assert isinstance(data["ONR_TYP_NR"], int), "The `onr_typ_nr` should be an integer."
-        assert isinstance(data["ORT_NR"], int), "The `ort_nr` should be an integer."
-        assert isinstance(data["FGR_NR"], int), "The `fgr_nr` should be an integer."
-        assert isinstance(data["HP_HZT"], int), "The `hp_hzt` should be an integer."
-
+    def from_dict(cls, data: Dict[str, int | str | None]) -> "OrtHztf":
         return OrtHztf(
             basis_version=data["BASIS_VERSION"],
             onr_typ_nr=data["ONR_TYP_NR"],
             ort_nr=data["ORT_NR"],
             fgr_nr=data["FGR_NR"],
             hp_hzt=timedelta(seconds=data["HP_HZT"]),
         )
@@ -341,32 +363,26 @@
 
     """
 
     frt_fid: int
     """The Identifier of the trip. Part of primary key."""
 
     @property
-    def position_key(self) -> Tuple[int, int, int]:
+    def position_key(self):
         return self.basis_version, self.onr_typ_nr, self.ort_nr
 
     @property
     def primary_key(self) -> Tuple[int | date | str, ...]:
         return self.basis_version, self.frt_fid, self.onr_typ_nr, self.ort_nr
 
     frt_hzt_zeit: timedelta
     """The time the trip waits at the stop in seconds."""
 
     @classmethod
-    def from_dict(cls, data: Dict[str, str | int | float | None]) -> "RecFrtHzt":
-        assert isinstance(data["BASIS_VERSION"], int), "The `basis_version` should be an integer."
-        assert isinstance(data["ONR_TYP_NR"], int), "The `onr_typ_nr` should be an integer."
-        assert isinstance(data["ORT_NR"], int), "The `ort_nr` should be an integer."
-        assert isinstance(data["FRT_FID"], int), "The `frt_fid` should be an integer."
-        assert isinstance(data["FRT_HZT_ZEIT"], int), "The `frt_hzt_zeit` should be an integer."
-
+    def from_dict(cls, data: Dict[str, int | str | None]) -> "RecFrtHzt":
         return RecFrtHzt(
             basis_version=data["BASIS_VERSION"],
             onr_typ_nr=data["ONR_TYP_NR"],
             ort_nr=data["ORT_NR"],
             frt_fid=data["FRT_FID"],
             frt_hzt_zeit=timedelta(seconds=data["FRT_HZT_ZEIT"]),
         )
@@ -428,24 +444,15 @@
             self.onr_typ_nr,
             self.ort_nr,
             self.sel_ziel_typ,
             self.sel_ziel,
         )
 
     @classmethod
-    def from_dict(cls, data: Dict[str, str | int | float | None]) -> "SelFztFeld":
-        assert isinstance(data["BASIS_VERSION"], int), "The `basis_version` should be an integer."
-        assert isinstance(data["BEREICH_NR"], int), "The `bereich_nr` should be an integer."
-        assert isinstance(data["FGR_NR"], int), "The `fgr_nr` should be an integer."
-        assert isinstance(data["ONR_TYP_NR"], int), "The `onr_typ_nr` should be an integer."
-        assert isinstance(data["ORT_NR"], int), "The `ort_nr` should be an integer."
-        assert isinstance(data["SEL_ZIEL_TYP"], int), "The `sel_ziel_typ` should be an integer."
-        assert isinstance(data["SEL_ZIEL"], int), "The `sel_ziel` should be an integer."
-        assert isinstance(data["SEL_FZT"], int), "The `sel_fzt` should be an integer."
-
+    def from_dict(cls, data: Dict[str, int | str | None]) -> "SelFztFeld":
         return SelFztFeld(
             basis_version=data["BASIS_VERSION"],
             bereich_nr=data["BEREICH_NR"],
             fgr_nr=data["FGR_NR"],
             onr_typ_nr=data["ONR_TYP_NR"],
             ort_nr=data["ORT_NR"],
             sel_ziel_typ=data["SEL_ZIEL_TYP"],
@@ -503,24 +510,15 @@
             self.onr_typ_nr,
             self.ort_nr,
             self.ueb_ziel_typ,
             self.ueb_ziel,
         )
 
     @classmethod
-    def from_dict(cls, data: Dict[str, str | int | float | None]) -> "UebFzt":
-        assert isinstance(data["BASIS_VERSION"], int), "The `basis_version` should be an integer."
-        assert isinstance(data["BEREICH_NR"], int), "The `bereich_nr` should be an integer."
-        assert isinstance(data["FGR_NR"], int), "The `fgr_nr` should be an integer."
-        assert isinstance(data["ONR_TYP_NR"], int), "The `onr_typ_nr` should be an integer."
-        assert isinstance(data["ORT_NR"], int), "The `ort_nr` should be an integer."
-        assert isinstance(data["UEB_ZIEL_TYP"], int), "The `ueb_ziel_typ` should be an integer."
-        assert isinstance(data["UEB_ZIEL"], int), "The `ueb_ziel` should be an integer."
-        assert isinstance(data["UEB_FAHRZEIT"], int), "The `ueb_fahrzeit` should be an integer."
-
+    def from_dict(cls, data: Dict[str, int | str | None]) -> "UebFzt":
         return UebFzt(
             basis_version=data["BASIS_VERSION"],
             bereich_nr=data["BEREICH_NR"],
             fgr_nr=data["FGR_NR"],
             onr_typ_nr=data["ONR_TYP_NR"],
             ort_nr=data["ORT_NR"],
             ueb_ziel_typ=data["UEB_ZIEL_TYP"],
@@ -531,14 +529,23 @@
 
 @dataclass()
 class RecFrt(VdvBaseObject):
     """
     This seems to be the equivalent of a trip in the eflips-model world. It is a trip that is part of a line.
     """
 
+    basis_version: str
+    """
+    The `BasisVerGueltigkeit.basis_version` this object belongs to. Currently not used. 
+
+    Later, it may be a good idea to allow the user to select a version of the schedule to import.
+
+    Restriction: Should be a nine-digit numeric string.
+    """
+
     frt_fid: int
     """
     The unique identifier of the trip. This is the primary key of the table.
     """
 
     frt_start: timedelta
     """
@@ -576,15 +583,15 @@
     """
 
     @property
     def primary_key(self) -> Tuple[int | date | str, ...]:
         return self.basis_version, self.frt_fid
 
     @classmethod
-    def from_dict(cls, data: Dict[str, str | int | float | None]) -> "RecFrt":
+    def from_dict(cls, data: Dict[str, str | int | None]) -> "RecFrt":
         """
         Load the data from a dictionary.
 
         :param data: A dictionary with the following keys:
             - "BASE_VERSION": The `BasisVerGueltigkeit.basis_version` this object belongs to. Currently not used.
             - "FRT_FID": The unique identifier of the trip. This is the primary key of the table.
             - "FRT_START": The start time of the trip. Expressed as an offset from midnight in the "Europe/Berlin" timezone.
@@ -593,32 +600,23 @@
             - "FAHRTART_NR": The type of trip this is. We simpilfy to a boolean in the eflips-model world.
             - "FGR_NR": The name of the timing group number this trip belongs to. Used to look up the timing group.
             - "STR_LI_VAR": An identifier for the line variant. TODO: Unclear at this point whether this is a route name?
             - "UM_UID": A unique identifier of the rotation this trip belongs to.
         :return: The object itself.
         """
 
-        assert isinstance(data["FRT_FID"], int), "The `frt_fid` should be an integer."
         assert data["FRT_FID"] > 0, "The `frt_fid` should be a positive integer."
-        assert isinstance(data["FRT_START"], int), "The `frt_start` should be an integer."
         assert data["FRT_START"] >= 0, "The `frt_start` should be a positive integer."
-        assert isinstance(data["LI_NR"], int), "The `li_nr` should be an integer."
         assert data["LI_NR"] > 0, "The `li_nr` should be a positive integer."
-        assert isinstance(data["TAGESART_NR"], int), "The `tagesart_nr` should be an integer."
         assert data["TAGESART_NR"] > 0, "The `tagesart_nr` should be a positive integer."
-        assert isinstance(data["FAHRTART_NR"], int), "The `fahrtart_nr` should be an integer."
         assert data["FAHRTART_NR"] > 0, "The `fahrtart_nr` should be a positive integer."
-        assert isinstance(data["FGR_NR"], int), "The `fgr_nr` should be an integer."
         assert data["FGR_NR"] > 0, "The `fgr_nr` should be a positive integer."
         assert isinstance(data["STR_LI_VAR"], str), "The `str_li_var` should be a six-character string."
-        assert isinstance(data["UM_UID"], int), "The `um_uid` should be an integer."
         assert data["UM_UID"] > 0, "The `um_uid` should be a positive integer."
 
-        assert isinstance(data["BASIS_VERSION"], int), "The `basis_version` should be an integer."
-
         return RecFrt(
             basis_version=data["BASIS_VERSION"],
             frt_fid=data["FRT_FID"],
             frt_start=timedelta(seconds=data["FRT_START"]),
             li_nr=data["LI_NR"],
             tagesart_nr=data["TAGESART_NR"],
             fahrtart_nr=data["FAHRTART_NR"],
@@ -672,111 +670,90 @@
 
     altitude: Optional[float]
     """
     The altitude of the point.
     """
 
     @property
-    def parent_station_primary_key(self) -> Tuple[int, int, int]:
-        assert self.ort_ref_ort is not None, "The `ort_ref_ort` cannot be none for this property."
-        assert self.ort_ref_ort_typ is not None, "The `ort_ref_ort_typ` cannot be none for this property."
+    def parent_station_primary_key(self):
         return self.basis_version, self.ort_ref_ort, self.ort_ref_ort_typ
 
     @property
     def primary_key(self) -> Tuple[int | date | str, ...]:
         return self.basis_version, self.onr_typ_nr, self.ort_nr
 
     @classmethod
-    def from_dict(cls, data: Dict[str, str | int | float | None]) -> "RecOrt":
+    def from_dict(cls, data: Dict[str, int | str | None]) -> "RecOrt":
         """
         Load the data from a dictionary.
         """
 
         if "WGS_XKOOR" in data:
-            assert isinstance(data["WGS_XKOOR"], float), "The `WGS_XKOOR` should be a float."
+            assert data["WGS_XKOOR"] is not None, "The `WGS_XKOOR` should not be None."
             assert data["WGS_XKOOR"] != 0, "The `WGS_XKOOR` should not be 0."
-            longitude: Optional[float] = data["WGS_XKOOR"]
+            longitude = data["WGS_XKOOR"]
         elif "ORT_POS_LAENGE" in data:
             # According to spec: Latitude in WGS 84 Format:
             # gggmmssnnn (Gradzahl, Minuten,
             # Sekunden mit 3
             # Nachkommastellen, Kein
             # Vorzeichen (+) heißt n.B. (nördliche
             # Breite)
             # Ein Minuszeichen (-) heißt s.B.
             # (südliche Breite))
 
             warnings.warn("Untested code.")
 
-            assert isinstance(data["ORT_POS_LAENGE"], int), "The `ORT_POS_LAENGE` should be an integer."
             assert data["ORT_POS_LAENGE"] is not None, "The `ORT_POS_LAENGE` should not be None."
             assert data["ORT_POS_LAENGE"] != 0, "The `ORT_POS_LAENGE` should not be 0."
             longitude_seconds = data["ORT_POS_LAENGE"] % 100000 / 1000
             longitude_minutes = (data["ORT_POS_LAENGE"] % 10000000) // 100000
             longitude_degrees = data["ORT_POS_LAENGE"] // 10000000
             longitude = longitude_degrees + longitude_minutes / 60 + longitude_seconds / 3600
         elif "ORT_POS_X" in data:
             # This seems to be longitude * 1e6
-            assert isinstance(data["ORT_POS_X"], int), "The `ORT_POS_X` should be an integer."
             longitude = data["ORT_POS_X"] / 1e6
         else:
             longitude = None
 
         if "WGS_YKOOR" in data:
-            assert isinstance(data["WGS_YKOOR"], float), "The `WGS_YKOOR` should be a float."
+            assert data["WGS_YKOOR"] is not None, "The `WGS_YKOOR` should not be None."
             assert data["WGS_YKOOR"] != 0, "The `WGS_YKOOR` should not be 0."
-            latitude: Optional[float] = data["WGS_YKOOR"]
+            latitude = data["WGS_YKOOR"]
         elif "ORT_POS_BREITE" in data:
             # According to Spec:
             # Longitude in WGS 84 Format:
             # gggmmssnnn (Gradzahl, Minuten,
             # Sekunden mit 3
             # Nachkommastellen, Kein
             # Vorzeichen (+) heißt ö.L. (östliche
             # Länge)
             # Ein Minuszeichen (-) heißt w.L.
             # (westliche Länge))
 
             warnings.warn("Untested code.")
 
-            assert isinstance(data["ORT_POS_BREITE"], int), "The `ORT_POS_BREITE` should be an integer."
             assert data["ORT_POS_BREITE"] is not None, "The `ORT_POS_BREITE` should not be None."
             assert data["ORT_POS_BREITE"] != 0, "The `ORT_POS_BREITE` should not be 0."
             latitude_seconds = data["ORT_POS_BREITE"] % 100000 / 1000
             latitude_minutes = (data["ORT_POS_BREITE"] % 10000000) // 100000
             latitude_degrees = data["ORT_POS_BREITE"] // 10000000
             latitude = latitude_degrees + latitude_minutes / 60 + latitude_seconds / 3600
         elif "ORT_POS_Y" in data:
             # This seems to be latitude * 1e6
-            assert isinstance(data["ORT_POS_Y"], int), "The `ORT_POS_Y` should be an integer."
             latitude = data["ORT_POS_Y"] / 1e6
         else:
             latitude = None
 
         if "ORT_POS_HOEHE" in data:
-            assert isinstance(data["ORT_POS_HOEHE"], int), "The `ORT_POS_HOEHE` should be an integer."
-            altitude: int | None = data["ORT_POS_HOEHE"]
+            altitude = data["ORT_POS_HOEHE"]
         else:
-            if latitude is not None and longitude is not None:
-                altitude = int(round(get_altitude((latitude, longitude))))
-            else:
-                altitude = None
-
-        assert isinstance(data["BASIS_VERSION"], int), "The `basis_version` should be an integer."
-        assert isinstance(data["ONR_TYP_NR"], int), "The `onr_typ_nr` should be an integer."
-        assert isinstance(data["ORT_NR"], int), "The `ort_nr` should be an integer."
-        assert isinstance(data["ORT_NAME"], str), "The `ort_name` should be a string."
-        assert isinstance(data["ORT_REF_ORT"], int), "The `ort_ref_ort` should be an integer."
-        assert isinstance(data["ORT_REF_ORT_TYP"], int), "The `ort_ref_ort_typ` should be an integer."
-        if data["ORT_REF_ORT_KUERZEL"] is not None:
-            assert isinstance(data["ORT_REF_ORT_KUERZEL"], str), "The `ort_ref_ort_kuerzel` should be a string."
-            ort_ref_ort_kuerzel = data["ORT_REF_ORT_KUERZEL"]
-        else:
-            ort_ref_ort_kuerzel = None
-        assert isinstance(data["ORT_REF_ORT_NAME"], str), "The `ort_ref_ort_name` should be a string."
+            # TODO: Enable
+            # altitude = get_altitude(latitude, longitude)
+            altitude = 9999
 
         return RecOrt(
             basis_version=data["BASIS_VERSION"],
             onr_typ_nr=data["ONR_TYP_NR"],
             ort_nr=data["ORT_NR"],
             ort_name=data["ORT_NAME"],
             ort_ref_ort=data["ORT_REF_ORT"],
@@ -811,32 +788,26 @@
         for rec_ort_ref_ort, rec_orts in rec_orts_by_ref_ort.items():
             if rec_orts[0].ort_ref_ort_name is not None:
                 name = rec_orts[0].ort_ref_ort_name
             else:
                 # The name is the most used one of the ort_name fields
                 # Count how many times each name appears
                 name_counts = Counter([rec_ort.ort_name for rec_ort in rec_orts])
-                name = name_counts.most_common(1)[0][0]
+                name = max(name_counts, key=name_counts.get)
 
             if (
                 all([rec_ort.latitude is not None for rec_ort in rec_orts])
                 and all([rec_ort.longitude is not None for rec_ort in rec_orts])
                 and all([rec_ort.altitude is not None for rec_ort in rec_orts])
             ):
                 # The latitude and longitude are the average of the coordinates
-                latitude = sum([rec_ort.latitude for rec_ort in rec_orts if rec_ort.latitude is not None]) / len(
-                    rec_orts
-                )
-                longitude = sum([rec_ort.longitude for rec_ort in rec_orts if rec_ort.longitude is not None]) / len(
-                    rec_orts
-                )
+                latitude = sum([rec_ort.latitude for rec_ort in rec_orts]) / len(rec_orts)
+                longitude = sum([rec_ort.longitude for rec_ort in rec_orts]) / len(rec_orts)
                 # The altitude is the average of the altitudes
-                altitude = sum([rec_ort.altitude for rec_ort in rec_orts if rec_ort.altitude is not None]) / len(
-                    rec_orts
-                )
+                altitude = sum([rec_ort.altitude for rec_ort in rec_orts]) / len(rec_orts)
 
                 geom = f"POINT({longitude} {latitude} {altitude})"
             else:
                 geom = None
 
             # The short name is the kuezel field, if it exists
             if rec_orts[0].ort_ref_ort_kuerzel is not None:
@@ -903,15 +874,15 @@
             self.onr_typ_nr,
             self.ort_nr,
             self.sel_ziel,
             self.sel_ziel_typ,
         )
 
     @classmethod
-    def from_dict(cls, data: Dict[str, str | int | float | None]) -> "RecSel":
+    def from_dict(cls, data: Dict[str, int | str | None]) -> "RecSel":
         """
         Load the data from a dictionary.
 
         :param data: A dictionary with the following keys:
         - "BASIS_VERSION": The `BasisVerGueltigkeit.basis_version` this object belongs to. Currently not used.
         - "BEREICH_NR": An identifier of the area. Unclear what this is used for.
         - "ONR_TYP_NR": This is a freign key to the `ONR_TYP_NR` in the MENGE_ONR_TYP table. The `STR_ONR_TYP` in this table is the type
@@ -920,22 +891,14 @@
         - "SEL_ZIEL": The identifier of the target point.
         - "SEL_ZIEL_TYP": The type of the target point.
         - "SEL_LAENGE": The length of the element in meters.
 
         :return: The object itself.
         """
 
-        assert isinstance(data["BASIS_VERSION"], int), "The `basis_version` should be an integer."
-        assert isinstance(data["BEREICH_NR"], int), "The `bereich_nr` should be an integer."
-        assert isinstance(data["ONR_TYP_NR"], int), "The `onr_typ_nr` should be an integer."
-        assert isinstance(data["ORT_NR"], int), "The `ort_nr` should be an integer."
-        assert isinstance(data["SEL_ZIEL_TYP"], int), "The `sel_ziel_typ` should be an integer."
-        assert isinstance(data["SEL_ZIEL"], int), "The `sel_ziel` should be an integer."
-        assert isinstance(data["SEL_LAENGE"], int), "The `sel_laenge` should be an integer."
-
         return RecSel(
             basis_version=data["BASIS_VERSION"],
             bereich_nr=data["BEREICH_NR"],
             onr_typ_nr=data["ONR_TYP_NR"],
             ort_nr=data["ORT_NR"],
             sel_ziel=data["SEL_ZIEL"],
             sel_ziel_typ=data["SEL_ZIEL_TYP"],
@@ -1015,27 +978,18 @@
             arrival_station=stations_by_basis_version_and_onr_typ_nr_and_ort_nr[self.end_station_primary_key],
             distance=self.ueb_laenge,
         )
 
         return route
 
     @classmethod
-    def from_dict(cls, data: Dict[str, str | int | float | None]) -> "RecUeb":
+    def from_dict(cls, data: Dict[str, int | str | None]) -> "RecUeb":
         """
         Load the data from a dictionary.
         """
-
-        assert isinstance(data["BASIS_VERSION"], int), "The `basis_version` should be an integer."
-        assert isinstance(data["BEREICH_NR"], int), "The `bereich_nr` should be an integer."
-        assert isinstance(data["ONR_TYP_NR"], int), "The `onr_typ_nr` should be an integer."
-        assert isinstance(data["ORT_NR"], int), "The `ort_nr` should be an integer."
-        assert isinstance(data["UEB_ZIEL_TYP"], int), "The `ueb_ziel_typ` should be an integer."
-        assert isinstance(data["UEB_ZIEL"], int), "The `ueb_ziel` should be an integer."
-        assert isinstance(data["UEB_LAENGE"], int), "The `ueb_laenge` should be an integer."
-
         return RecUeb(
             basis_version=data["BASIS_VERSION"],
             bereich_nr=data["BEREICH_NR"],
             onr_typ_nr=data["ONR_TYP_NR"],
             ort_nr=data["ORT_NR"],
             ueb_ziel_typ=data["UEB_ZIEL_TYP"],
             ueb_ziel=data["UEB_ZIEL"],
@@ -1080,27 +1034,18 @@
     """
 
     @property
     def primary_key(self) -> Tuple[int | date | str, ...]:
         return self.basis_version, self.li_nr, self.str_li_var
 
     @classmethod
-    def from_dict(cls, data: Dict[str, str | int | float | None]) -> "RecLid":
+    def from_dict(cls, data: Dict[str, int | str | None]) -> "RecLid":
         """
         Load the data from a dictionary.
         """
-
-        assert isinstance(data["BASIS_VERSION"], int), "The `basis_version` should be an integer."
-        assert isinstance(data["LI_NR"], int), "The `li_nr` should be an integer."
-        assert isinstance(data["STR_LI_VAR"], str), "The `str_li_var` should be a string."
-        assert isinstance(data["BEREICH_NR"], int), "The `bereich_nr` should be an integer."
-        assert isinstance(data["LI_KUERZEL"], str), "The `li_kuerzel` should be a string."
-        assert isinstance(data["LIDNAME"], str), "The `lidname` should be a string."
-        assert isinstance(data["ROUTEN_ART"], int), "The `routen_art` should be an integer."
-
         return RecLid(
             basis_version=data["BASIS_VERSION"],
             li_nr=data["LI_NR"],
             str_li_var=data["STR_LI_VAR"],
             bereich_nr=data["BEREICH_NR"],
             li_kuerzel=data["LI_KUERZEL"],
             lidname=data["LIDNAME"],
@@ -1119,30 +1064,28 @@
             scenario=scenario,
             name=self.li_kuerzel,
         )
 
     def to_route(
         self,
         scenario: Scenario,
-        lines_by_basis_version_andli_nr: Dict[Tuple[int | date | str, ...], Line],
+        lines_by_basis_version_andli_nr: Dict[Tuple[int, int], Line],
         rec_orts_by_basis_version_and_onr_typ_nr_and_ort_nr: Dict[Tuple[int, int, int], RecOrt],
         lid_verlaufs_by_basis_version_and_li_nr_and_str_li_var: Dict[Tuple[int, int, str], List[LidVerlauf]],
-        stations_by_basis_version_and_onr_typ_nr_and_ort_nr: Dict[Tuple[int | date | str, ...], Station],
+        stations_by_basis_version_and_onr_typ_nr_and_ort_nr: Dict[Tuple[int, int, int], Station],
         rec_sel_by_basis_version_and_start_type_and_start_nr_and_end_type_and_end_nr: Dict[
             Tuple[int, int, int, int, int], RecSel
         ],
     ) -> Tuple[Route, List[RecSel]]:
         """
         Convert to a route.
 
         :param scenario: The scenario to associate the route with
         :return: An instance of the Route class
         """
-        logger = logging.getLogger(__name__)
-
         route = Route(
             scenario=scenario,
             line=lines_by_basis_version_andli_nr[(self.basis_version, self.li_nr)],
             name=self.lidname,
         )
 
         assoc_route_stations: List[AssocRouteStation] = []
@@ -1153,15 +1096,15 @@
         elapsed_distance = 0
         rec_sels = []
         for i in range(len(this_routes_lid_verlaufs)):
             this_lid_verlauf = this_routes_lid_verlaufs[i]
 
             this_rec_ort = rec_orts_by_basis_version_and_onr_typ_nr_and_ort_nr[this_lid_verlauf.position_key]
             if this_rec_ort.latitude is None or this_rec_ort.longitude is None:
-                logger.debug(f"Encountered a station without coordinates: {this_rec_ort}")
+                warnings.warn("The latitude and longitude should not be None.")
                 location = None
             else:
                 location = f"POINT({this_rec_ort.longitude} {this_rec_ort.latitude} {this_rec_ort.altitude})"
 
             this_station = stations_by_basis_version_and_onr_typ_nr_and_ort_nr[this_lid_verlauf.position_key]
 
             assoc = AssocRouteStation(
@@ -1184,15 +1127,15 @@
                         this_lid_verlauf.ort_nr,
                         this_routes_lid_verlaufs[i + 1].onr_typ_nr,
                         this_routes_lid_verlaufs[i + 1].ort_nr,
                     )
                 ]
                 rec_sels.append(this_rec_sel)
                 if this_rec_sel.sel_laenge is None or this_rec_sel.sel_laenge == 0:
-                    logger.debug(f"Encountered a segment without length: {this_rec_sel.primary_key}")
+                    warnings.warn("The `sel_laenge` should not be None or 0.")
                     # put a default value
                     elapsed_distance += 1
                 else:
                     elapsed_distance += this_rec_sel.sel_laenge
         route.arrival_station = this_station
         route.distance = elapsed_distance
         route.assoc_route_stations = assoc_route_stations
@@ -1259,44 +1202,34 @@
     """
 
     @property
     def primary_key(self) -> Tuple[int | date | str, ...]:
         return self.basis_version, self.tagesart_nr, self.um_uid
 
     @classmethod
-    def from_dict(cls, data: Dict[str, str | int | float | None]) -> "RecUmlauf":
+    def from_dict(cls, data: Dict[str, int | str | None]) -> "RecUmlauf":
         """
         Load the data from a dictionary.
         """
 
-        assert isinstance(data["BASIS_VERSION"], int), "The `basis_version` should be an integer."
-        assert isinstance(data["TAGESART_NR"], int), "The `tagesart_nr` should be an integer."
-        assert isinstance(data["UM_UID"], int), "The `um_uid` should be an integer."
-        assert isinstance(data["ANF_ORT"], int), "The `anf_ort` should be an integer."
-        assert isinstance(data["ANF_ONR_TYP"], int), "The `anf_onr_typ` should be an integer."
-        assert isinstance(data["END_ORT"], int), "The `end_ort` should be an integer."
-        assert isinstance(data["END_ONR_TYP"], int), "The `end_onr_typ` should be an integer."
-
         return RecUmlauf(
             basis_version=data["BASIS_VERSION"],
             tagesart_nr=data["TAGESART_NR"],
             um_uid=data["UM_UID"],
-            anf_ort=data["ANF_ORT"],
-            anf_onr_typ=data["ANF_ONR_TYP"],
-            end_ort=data["END_ORT"],
-            end_onr_typ=data["END_ONR_TYP"],
-            fzg_typ_nr=data["FZG_TYP_NR"]
-            if "FZG_TYP_NR" in data.keys() and isinstance(data["FZG_TYP_NR"], int) and data["FZG_TYP_NR"] != 0
-            else None,
+            anf_ort=data["ANF_ORT"] if "ANF_ORT" in data.keys() and data["ANF_ORT"] != 0 else None,
+            anf_onr_typ=data["ANF_ONR_TYP"] if "ANF_ONR_TYP" in data.keys() and data["ANF_ONR_TYP"] != 0 else None,
+            end_ort=data["END_ORT"] if "END_ORT" in data.keys() and data["END_ORT"] != 0 else None,
+            end_onr_typ=data["END_ONR_TYP"] if "END_ONR_TYP" in data.keys() and data["END_ONR_TYP"] != 0 else None,
+            fzg_typ_nr=data["FZG_TYP_NR"] if "FZG_TYP_NR" in data.keys() and data["FZG_TYP_NR"] != 0 else None,
         )
 
     def to_rotation(
         self,
         scenario: Scenario,
-        db_vehicle_types_by_vdv_pk: Dict[Tuple[int | date | str, ...], VehicleType],
+        db_vehicle_types_by_vdv_pk: Dict[Tuple[int, int], VehicleType],
         allow_opportunity_charging: bool = False,
         dummy_vehicle_type: Optional[VehicleType] = None,
     ) -> Rotation:
         """
         Converts to a database rotation object.
         :param db_vehicle_types_by_vdv_pk: A dictionary of already-imported vehicle type objects by their VDV-style
         primary key, which is defined as BASIS_VERSION + FZG_TYPE_NR
@@ -1367,51 +1300,24 @@
     """
 
     @property
     def primary_key(self) -> Tuple[int | date | str, ...]:
         return self.basis_version, self.fzg_typ_nr
 
     @classmethod
-    def from_dict(cls, data: Dict[str, str | int | float | None]) -> "MengeFzgTyp":
+    def from_dict(cls, data: Dict[str, int | str | None]) -> "MengeFzgTyp":
         """
         Load the data from a dictionary.
         """
-
-        if "FZG_TYP_TEXT" in data:
-            assert isinstance(data["FZG_TYP_TEXT"], str), "The `FZG_TYP_TEXT` should be a string."
-            fzg_typ_text = data["FZG_TYP_TEXT"]
-        else:
-            fzg_typ_text = None
-
-        if "STR_FZG_TYP" in data:
-            assert isinstance(data["STR_FZG_TYP"], str), "The `STR_FZG_TYP` should be a string."
-            str_fzg_typ = data["STR_FZG_TYP"]
-        else:
-            str_fzg_typ = None
-
-        if "FZG_LAENGE" in data:
-            assert isinstance(data["FZG_LAENGE"], int), "The `FZG_LAENGE` should be an integer."
-            fzg_laenge = data["FZG_LAENGE"]
-        else:
-            fzg_laenge = None
-        if "FZG_TYP_HOEHE" in data:
-            assert isinstance(data["FZG_TYP_HOEHE"], int), "The `FZG_TYP_HOEHE` should be an integer."
-            fzg_hoehe = data["FZG_TYP_HOEHE"] / 100
-        else:
-            fzg_hoehe = None
-        if "FZG_TYP_BREITE" in data:
-            assert isinstance(data["FZG_TYP_BREITE"], int), "The `FZG_TYP_BREITE` should be an integer."
-            fzg_breite = data["FZG_TYP_BREITE"] / 100
-        else:
-            fzg_breite = None
-        if "FZG_TYP_GEWICHT" in data:
-            assert isinstance(data["FZG_TYP_GEWICHT"], int), "The `FZG_TYP_GEWICHT` should be an integer."
-            fzg_gewicht = data["FZG_TYP_GEWICHT"]
-        else:
-            fzg_gewicht = None
+        fzg_typ_text = data["FZG_TYP_TEXT"] if "FZG_TYP_TEXT" in data else None
+        str_fzg_typ = data["STR_FZG_TYP"] if "STR_FZG_TYP" in data else None
+        fzg_laenge = data["FZG_LAENGE"] if "FZG_LAENGE" in data else None
+        fzg_hoehe = data["FZG_TYP_HOEHE"] / 100 if "FZG_TYP_HOEHE" in data else None
+        fzg_breite = data["FZG_TYP_BREITE"] / 100 if "FZG_TYP_BREITE" in data else None
+        fzg_gewicht = data["FZG_TYP_GEWICHT"] if "FZG_TYP_GEWICHT" in data else None
 
         # zero values are also invalid here
         if (
             fzg_laenge == 0
             or fzg_breite == 0
             or fzg_hoehe == 0
             or fzg_laenge is None
@@ -1421,39 +1327,25 @@
             # In our code, they either all need to be set or none of them.
             fzg_laenge = None
             fzg_breite = None
             fzg_hoehe = None
         if fzg_gewicht == 0:
             fzg_gewicht = None
 
-        if "VERBRAUCH_DISTANZ" in data:
-            assert isinstance(data["VERBRAUCH_DISTANZ"], int), "The `VERBRAUCH_DISTANZ` should be an integer."
-            verbrauch_distanz = data["VERBRAUCH_DISTANZ"] / 1000  # Wh per km to kWh per km
-        else:
-            verbrauch_distanz = None
-
-        if "VERBRAUCH_ZEIT" in data:
-            assert isinstance(data["VERBRAUCH_ZEIT"], int), "The `VERBRAUCH_ZEIT` should be an integer."
-            verbrauch_zeit = data["VERBRAUCH_ZEIT"] / 1000  # W to kW
-        else:
-            verbrauch_zeit = None
+        verbrauch_distanz = data["VERBRAUCH_DISTANZ"] / 1000 if "VERBRAUCH_DISTANZ" in data else None
+        verbrauch_zeit = data["VERBRAUCH_ZEIT"] / 1000 if "VERBRAUCH_ZEIT" in data else None
 
         if verbrauch_distanz is not None and verbrauch_zeit is not None:
             # We cannot do a distance and time consumption at the same time. For now, assume an average speed of 20 km_h
             AVERAGE_SPEED = 20
             time_per_kilometer = 1 / AVERAGE_SPEED  # hours
             verbrauch = verbrauch_distanz + verbrauch_zeit * time_per_kilometer
         else:
             verbrauch = None
 
-        assert isinstance(data["BASIS_VERSION"], int), "The `basis_version` should be an integer."
-        assert isinstance(data["FZG_TYP_NR"], int), "The `fzg_typ_nr` should be an integer."
-        assert isinstance(data["FZG_TYP_TEXT"], str), "The `fzg_typ_text` should be a string."
-        assert isinstance(data["STR_FZG_TYP"], str), "The `str_fzg_typ` should be a string."
-
         return MengeFzgTyp(
             basis_version=data["BASIS_VERSION"],
             fzg_typ_nr=data["FZG_TYP_NR"],
             fzg_typ_text=fzg_typ_text,
             str_fzg_typ=str_fzg_typ,
             fzg_laenge=fzg_laenge,
             fzg_hoehe=fzg_hoehe,
```

### Comparing `eflips_ingest-1.2.0/pyproject.toml` & `eflips_ingest-1.2.0a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eflips-ingest"
-version = "1.2.0"
+version = "1.2.0-alpha"
 description = "A collection of import scripts for converting bus schedule data into the [eflips-model](https://github.com/mpm-tu-berlin/eflips-model) data format."
 authors = [
     "Ludger Heide <ludger.heide@lhtechnologies.de>"
 ]
 readme = "README.md"
 license = "AGPL-3.0-or-later"
 homepage = "https://github.com/mpm-tu-berlin/eflips-import"
```

### Comparing `eflips_ingest-1.2.0/PKG-INFO` & `eflips_ingest-1.2.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eflips-ingest
-Version: 1.2.0
+Version: 1.2.0a0
 Summary: A collection of import scripts for converting bus schedule data into the [eflips-model](https://github.com/mpm-tu-berlin/eflips-model) data format.
 Home-page: https://github.com/mpm-tu-berlin/eflips-import
 License: AGPL-3.0-or-later
 Author: Ludger Heide
 Author-email: ludger.heide@lhtechnologies.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

