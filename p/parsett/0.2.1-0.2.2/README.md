# Comparing `tmp/parsett-0.2.1.tar.gz` & `tmp/parsett-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parsett-0.2.1.tar", max compression
+gzip compressed data, was "parsett-0.2.2.tar", max compression
```

## Comparing `parsett-0.2.1.tar` & `parsett-0.2.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1084 2024-04-05 03:14:24.724214 parsett-0.2.1/LICENSE
--rw-r--r--   0        0        0       57 2024-04-28 22:36:49.894118 parsett-0.2.1/PTT/__init__.py
--rw-r--r--   0        0        0    44677 2024-04-28 09:11:48.041816 parsett-0.2.1/PTT/handlers.py
--rw-r--r--   0        0        0     9785 2024-04-28 22:43:06.993134 parsett-0.2.1/PTT/parse.py
--rw-r--r--   0        0        0     3522 2024-04-28 09:11:48.042818 parsett-0.2.1/PTT/transformers.py
--rw-r--r--   0        0        0     2605 2024-04-28 23:26:25.218964 parsett-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      449 1970-01-01 00:00:00.000000 parsett-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-06 19:33:45.939820 parsett-0.2.2/LICENSE
+-rw-r--r--   0        0        0      108 2024-05-06 19:33:45.948819 parsett-0.2.2/PTT/__init__.py
+-rw-r--r--   0        0        0    44237 2024-05-06 19:33:48.912965 parsett-0.2.2/PTT/handlers.py
+-rw-r--r--   0        0        0     8689 2024-05-06 19:33:48.917963 parsett-0.2.2/PTT/parse.py
+-rw-r--r--   0        0        0     3880 2024-05-06 19:33:48.926971 parsett-0.2.2/PTT/transformers.py
+-rw-r--r--   0        0        0     2499 2024-05-06 19:38:32.994091 parsett-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      449 1970-01-01 00:00:00.000000 parsett-0.2.2/PKG-INFO
```

### Comparing `parsett-0.2.1/LICENSE` & `parsett-0.2.2/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2024 Spoked
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2024 Spoked
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `parsett-0.2.1/PTT/handlers.py` & `parsett-0.2.2/PTT/handlers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,411 +1,407 @@
-import regex
-
-from PTT.parse import Parser
-from PTT.transformers import (
-    none, value, integer, boolean, lowercase, uppercase, date,
-    range_func, year_range, array, uniq_concat
-)
-
-
-def add_defaults(parser: Parser):
-    # Episode code
-    parser.add_handler("episode_code", regex.compile(r"[[(]([a-zA-Z0-9]{8})[\])](?=\.[a-zA-Z0-9]{1,5}$|$)"), uppercase, {"remove": True})
-    parser.add_handler("episode_code", regex.compile(r"\[([A-Z0-9]{8})]"), uppercase, {"remove": True})
-
-    # Resolution
-    parser.add_handler("resolution", regex.compile(r"\b(?:\[?\]?4k[\])?]?)\b", regex.IGNORECASE), value("4k"), {"remove": True})
-    parser.add_handler("resolution", regex.compile(r"21600?[pi]", regex.IGNORECASE), value("4k"), {"skipIfAlreadyFound": False, "remove": True})
-    parser.add_handler("resolution", regex.compile(r"\[?\]?3840x\d{4}[\])?]?", regex.IGNORECASE), value("4k"), {"remove": True})
-    parser.add_handler("resolution", regex.compile(r"\[?\]?1920x\d{3,4}[\])?]?", regex.IGNORECASE), value("1080p"), {"remove": True})
-    parser.add_handler("resolution", regex.compile(r"\[?\]?1280x\d{3}[\])?]?", regex.IGNORECASE), value("720p"), {"remove": True})
-    parser.add_handler("resolution", regex.compile(r"\[?\]?(\d{3,4}x\d{3,4})[\])?]?", regex.IGNORECASE), value("$1p"), {"remove": True})
-    parser.add_handler("resolution", regex.compile(r"(480|720|1080)0[pi]", regex.IGNORECASE), value("$1p"), {"remove": True})
-    parser.add_handler("resolution", regex.compile(r"(?:BD|HD|M)(720|1080|2160)"), value("$1p"), {"remove": True})
-    parser.add_handler("resolution", regex.compile(r"(480|576|720|1080|2160)[pi]", regex.IGNORECASE), value("$1p"), {"remove": True})
-    parser.add_handler("resolution", regex.compile(r"(?:^|\D)(\d{3,4})[pi]", regex.IGNORECASE), value("$1p"), {"remove": True})
-
-    # Date
-    parser.add_handler("date", regex.compile(r"(?:\W|^)([[(]?(?:19[6-9]|20[012])[0-9]([. \-/\\])(?:0[1-9]|1[012])\2(?:0[1-9]|[12][0-9]|3[01])[])]?)(?:\W|$)"), date("YYYY MM DD"), {"remove": True})
-    parser.add_handler("date", regex.compile(r"(?:\W|^)(\[?\]?(?:0[1-9]|[12][0-9]|3[01])([. \-/\\])(?:0[1-9]|1[012])\2(?:19[6-9]|20[01])[0-9][\])]?)(?:\W|$)"), date("DD MM YYYY"), {"remove": True})
-    parser.add_handler("date", regex.compile(r"(?:\W)(\[?\]?(?:0[1-9]|1[012])([. \-/\\])(?:0[1-9]|[12][0-9]|3[01])\2(?:[0][1-9]|[0126789][0-9])[\])]?)(?:\W|$)"), date("MM DD YY"), {"remove": True})
-    parser.add_handler("date", regex.compile(r"(?:\W)(\[?\]?(?:0[1-9]|[12][0-9]|3[01])([. \-/\\])(?:0[1-9]|1[012])\2(?:[0][1-9]|[0126789][0-9])[\])]?)(?:\W|$)"), date("DD MM YY"), {"remove": True})
-    parser.add_handler("date", regex.compile(r"(?:\W|^)(\[?\]?(?:0?[1-9]|[12][0-9]|3[01])[. ]?(?:st|nd|rd|th)?([. \-\/\\])(?:feb(?:ruary)?|jan(?:uary)?|mar(?:ch)?|apr(?:il)?|may|june?|july?|aug(?:ust)?|sept?(?:ember)?|oct(?:ober)?|nov(?:ember)?|dec(?:ember)?)\2(?:19[7-9]|20[012])[0-9][\])]?)(?:\W|$)", regex.IGNORECASE), date(["DD MMM YYYY", "Do MMM YYYY", "Do MMMM YYYY"]), {"remove": True})
-    parser.add_handler("date", regex.compile(r"(?:\W|^)(\[?\]?(?:0?[1-9]|[12][0-9]|3[01])[. ]?(?:st|nd|rd|th)?([. \-\/\\])(?:feb(?:ruary)?|jan(?:uary)?|mar(?:ch)?|apr(?:il)?|may|june?|july?|aug(?:ust)?|sept?(?:ember)?|oct(?:ober)?|nov(?:ember)?|dec(?:ember)?)\2(?:0[1-9]|[0126789][0-9])[\])]?)(?:\W|$)", regex.IGNORECASE), date("DD MMM YY"), {"remove": True})
-    parser.add_handler("date", regex.compile(r"(?:\W|^)(\[?\]?20[012][0-9](?:0[1-9]|1[012])(?:0[1-9]|[12][0-9]|3[01])[\])]?)(?:\W|$)"), date("YYYYMMDD"), {"remove": True})
-
-    # Year
-    parser.add_handler("year", regex.compile(r"[([]?[ .]?((?:19\d|20[012])\d[ .]?-[ .]?(?:19\d|20[012])\d)[ .]?[)\]]?"), year_range, { "remove": True })
-    parser.add_handler("year", regex.compile(r"[([][ .]?((?:19\d|20[012])\d[ .]?-[ .]?\d{2})[ .]?[)\]]"), year_range, { "remove": True })
-    parser.add_handler("year", regex.compile(r"[([]?(?!^)(?<!\d|Cap[. ]?)((?:19\d|20[012])\d)(?!\d|kbps)[)\]]?", regex.IGNORECASE), integer, { "remove": True })
-    parser.add_handler("year", regex.compile(r"^[([]?((?:19\d|20[012])\d)(?!\d|kbps)[)\]]?", regex.IGNORECASE), integer, { "remove": True })
-
-    # Extended
-    parser.add_handler("extended", regex.compile(r"EXTENDED"), boolean)
-
-    # Convert
-    parser.add_handler("convert", regex.compile(r"CONVERT"), boolean)
-
-    # Hardcoded
-    parser.add_handler("hardcoded", regex.compile(r"HC|HARDCODED"), boolean)
-
-    # Proper
-    parser.add_handler("proper", regex.compile(r"(?:REAL.)?PROPER"), boolean)
-
-    # Repack
-    parser.add_handler("repack", regex.compile(r"REPACK|RERIP"), boolean)
-
-    # Retail
-    parser.add_handler("retail", regex.compile(r"\bRetail\b", regex.IGNORECASE), boolean)
-
-    # Remastered
-    parser.add_handler("remastered", regex.compile(r"\bRemaster(?:ed)?\b", regex.IGNORECASE), boolean)
-
-    # Unrated
-    parser.add_handler("unrated", regex.compile(r"\bunrated|uncensored\b", regex.IGNORECASE), boolean)
-
-    # Region
-    parser.add_handler("region", regex.compile(r"R\d\b"), none, { "skipIfFirst": True })
-
-    # Source
-    parser.add_handler("source", regex.compile(r"\b(?:H[DQ][ .-]*)?CAM(?:H[DQ])?(?:[ .-]*Rip)?\b", regex.IGNORECASE), value("CAM"), {"remove": True})
-    parser.add_handler("source", regex.compile(r"\b(?:H[DQ][ .-]*)?S[ .-]*print", regex.IGNORECASE), value("CAM"), {"remove": True})
-    parser.add_handler("source", regex.compile(r"\b(?:HD[ .-]*)?T(?:ELE)?S(?:YNC)?(?:Rip)?\b", regex.IGNORECASE), value("TeleSync"), {"remove": True})
-    parser.add_handler("source", regex.compile(r"\b(?:HD[ .-]*)?T(?:ELE)?C(?:INE)?(?:Rip)?\b"), value("TeleCine"), {"remove": True})
-    parser.add_handler("source", regex.compile(r"\bBlu[ .-]*Ray\b(?=.*remux)", regex.IGNORECASE), value("BluRay REMUX"), {"remove": True})
-    parser.add_handler("source", regex.compile(r"(?:BD|BR|UHD)[- ]?remux", regex.IGNORECASE), value("BluRay REMUX"), {"remove": True})
-    parser.add_handler("source", regex.compile(r"(?<=remux.*)\bBlu[ .-]*Ray\b", regex.IGNORECASE), value("BluRay REMUX"), {"remove": True})
-    parser.add_handler("source", regex.compile(r"\bBlu[ .-]*Ray\b(?![ .-]*Rip)", regex.IGNORECASE), value("BluRay"), {"remove": True})
-    parser.add_handler("source", regex.compile(r"\bUHD[ .-]*Rip\b", regex.IGNORECASE), value("UHDRip"), {"remove": True})
-    parser.add_handler("source", regex.compile(r"\bHD[ .-]*Rip\b", regex.IGNORECASE), value("HDRip"), {"remove": True})
-    parser.add_handler("source", regex.compile(r"\bMicro[ .-]*HD\b", regex.IGNORECASE), value("HDRip"), {"remove": True})
-    parser.add_handler("source", regex.compile(r"\b(?:BR|Blu[ .-]*Ray)[ .-]*Rip\b", regex.IGNORECASE), value("BRRip"), {"remove": True})
-    parser.add_handler("source", regex.compile(r"\bBD[ .-]*Rip\b|\bBDR\b|\bBD-RM\b|[[(]BD[\]) .,-]", regex.IGNORECASE), value("BDRip"), {"remove": True})
-    parser.add_handler("source", regex.compile(r"\b(?:HD[ .-]*)?DVD[ .-]*Rip\b", regex.IGNORECASE), value("DVDRip"), {"remove": True})
-    parser.add_handler("source", regex.compile(r"\bVHS[ .-]*Rip\b", regex.IGNORECASE), value("DVDRip"), {"remove": True})
-    parser.add_handler("source", regex.compile(r"\b(?:DVD?|BD|BR)?[ .-]*Scr(?:eener)?\b", regex.IGNORECASE), value("SCR"), {"remove": True})
-    parser.add_handler("source", regex.compile(r"\bP(?:re)?DVD(?:Rip)?\b", regex.IGNORECASE), value("SCR"), {"remove": True})
-    parser.add_handler("source", regex.compile(r"\bDVD(?:R\d?)?\b", regex.IGNORECASE), value("DVD"), {"remove": True})
-    parser.add_handler("source", regex.compile(r"\bVHS\b", regex.IGNORECASE), value("DVD"), {"remove": True})
-    parser.add_handler("source", regex.compile(r"\bPPVRip\b", regex.IGNORECASE), value("PPVRip"), {"remove": True})
-    parser.add_handler("source", regex.compile(r"\bHD[ .-]*TV(?:Rip)?\b", regex.IGNORECASE), value("HDTV"), {"remove": True})
-    parser.add_handler("source", regex.compile(r"\bDVB[ .-]*(?:Rip)?\b", regex.IGNORECASE), value("HDTV"), {"remove": True})
-    parser.add_handler("source", regex.compile(r"\bSAT[ .-]*Rips?\b", regex.IGNORECASE), value("SATRip"), {"remove": True})
-    parser.add_handler("source", regex.compile(r"\bTVRips?\b", regex.IGNORECASE), value("TVRip"), {"remove": True})
-    parser.add_handler("source", regex.compile(r"\bR5\b", regex.IGNORECASE), value("R5"), {"remove": True})
-    parser.add_handler("source", regex.compile(r"\bWEB[ .-]*DL(?:Rip)?\b", regex.IGNORECASE), value("WEB-DL"), {"remove": True})
-    parser.add_handler("source", regex.compile(r"\bWEB[ .-]*Rip\b", regex.IGNORECASE), value("WEBRip"), {"remove": True})
-    parser.add_handler("source", regex.compile(r"\b(?:DL|WEB|BD|BR)MUX\b", regex.IGNORECASE), none, {"remove": True})
-    parser.add_handler("source", regex.compile(r"\b(DivX|XviD)\b"), none, {"remove": True})
-
-    # Video depth
-    parser.add_handler("bit_depth", regex.compile(r"\bhevc\s?10\b", regex.IGNORECASE), value("10bit"))
-    parser.add_handler("bit_depth", regex.compile(r"(?:8|10|12)[- ]?bit", regex.IGNORECASE), lowercase, {"remove": True})
-    parser.add_handler("bit_depth", regex.compile(r"\bhdr10\b", regex.IGNORECASE), value("10bit"))
-    parser.add_handler("bit_depth", regex.compile(r"\bhi10\b", regex.IGNORECASE), value("10bit"))
-    def handle_bit_depth(context):
-        result = context['result']
-        if 'bitDepth' in result:
-            # Replace hyphens and spaces with nothing (effectively removing them)
-            result['bit_depth'] = result['bit_depth'].replace(" ", "").replace("-", "")
-    parser.add_handler("bit_depth", handle_bit_depth)
-
-    # HDR
-    parser.add_handler("hdr", regex.compile(r"\bDV\b|dolby.?vision|\bDoVi\b", regex.IGNORECASE), uniq_concat(value("DV")), {"remove": True, "skipIfAlreadyFound": False})
-    parser.add_handler("hdr", regex.compile(r"HDR10(?:\+|plus)", regex.IGNORECASE), uniq_concat(value("HDR10+")), {"remove": True, "skipIfAlreadyFound": False})
-    parser.add_handler("hdr", regex.compile(r"\bHDR(?:10)?\b", regex.IGNORECASE), uniq_concat(value("HDR")), {"remove": True, "skipIfAlreadyFound": False})
-
-    # Codec
-    parser.add_handler("codec", regex.compile(r"\b[xh][-. ]?26[45]", regex.IGNORECASE), lowercase, {"remove": True})
-    parser.add_handler("codec", regex.compile(r"\bhevc(?:\s?10)?\b", regex.IGNORECASE), value("hevc"), {"remove": True, "skipIfAlreadyFound": False})
-    parser.add_handler("codec", regex.compile(r"\b(?:dvix|mpeg2|divx|xvid|avc)\b", regex.IGNORECASE), lowercase, {"remove": True, "skipIfAlreadyFound": False})
-
-    # Audio
-    parser.add_handler("audio", regex.compile(r"7\.1[. ]?Atmos\b", regex.IGNORECASE), value("7.1 Atmos"), {"remove": True})
-    parser.add_handler("audio", regex.compile(r"\b(?:mp3|Atmos|DTS(?:-HD)?|TrueHD)\b", regex.IGNORECASE), lowercase)
-    parser.add_handler("audio", regex.compile(r"\bFLAC(?:\+?2\.0)?(?:x[2-4])?\b", regex.IGNORECASE), value("flac"), {"remove": True})
-    parser.add_handler("audio", regex.compile(r"\bEAC-?3(?:[. -]?[256]\.[01])?", regex.IGNORECASE), value("eac3"), {"remove": True, "skipIfAlreadyFound": False})
-    parser.add_handler("audio", regex.compile(r"\bAC-?3(?:[.-]5\.1|x2\.?0?)?\b", regex.IGNORECASE), value("ac3"), {"remove": True, "skipIfAlreadyFound": False})
-    parser.add_handler("audio", regex.compile(r"\b5\.1(?:x[2-4]+)?\+2\.0(?:x[2-4])?\b", regex.IGNORECASE), value("2.0"), {"remove": True, "skipIfAlreadyFound": False})
-    parser.add_handler("audio", regex.compile(r"\b2\.0(?:x[2-4]|\+5\.1(?:x[2-4])?)\b", regex.IGNORECASE), value("2.0"), {"remove": True, "skipIfAlreadyFound": False})
-    parser.add_handler("audio", regex.compile(r"\b5\.1ch\b", regex.IGNORECASE), value("ac3"), {"remove": True, "skipIfAlreadyFound": False})
-    parser.add_handler("audio", regex.compile(r"\bDD5[. ]?1\b", regex.IGNORECASE), value("dd5.1"), {"remove": True})
-    parser.add_handler("audio", regex.compile(r"\bQ?AAC(?:[. ]?2[. ]0|x2)?\b", regex.IGNORECASE), value("aac"), {"remove": True})
-
-    # Group
-    parser.add_handler("group", regex.compile(r"- ?(?!\d+$|S\d+|\d+x|ep?\d+|[^[]+]$)([^\-. []+[^\-. [)\]\d][^\-. [)\]]*)(?:\[[\w.-]+])?(?=\.\w{2,4}$|$)", regex.IGNORECASE), none, {"remove": True})
-
-    # Container
-    parser.add_handler("container", regex.compile(r"\.?[\[(]?\b(MKV|AVI|MP4|WMV|MPG|MPEG)\b[\])]?", regex.IGNORECASE), lowercase)
-
-    # Volume
-    parser.add_handler("volumes", regex.compile(r"\bvol(?:s|umes?)?[. -]*(?:\d{1,2}[., +/\\&-]+)+\d{1,2}\b", regex.IGNORECASE), range_func, {"remove": True})
-    # parser.add_handler("volumes", regex.compile(r"\bvol(?:s|umes?)?[. -]*(\d{1,2})\b", regex.IGNORECASE), integer, {"remove": True})
-    def handle_volumes(context):
-        title = context['title']
-        result = context['result']
-        matched = context['matched']
-
-        # Determine the start index based on whether the year is matched
-        start_index = matched.get('year', {}).get('match_index', 0)
-
-        # Regular expression to find volume numbers
-        match = regex.search(r'\bvol(?:ume)?[. -]*(\d{1,2})', title[start_index:], regex.IGNORECASE)
-
-        if match:
-            # Update the matched information for volumes
-            matched['volumes'] = {'match': match.group(0), 'match_index': match.start()}
-
-            # Convert the captured group to an integer and store it in the result
-            result['volumes'] = [int(match.group(1))]
-
-            # Return a dictionary with details of the raw match and its index
-            return {
-                'raw_match': match.group(0),
-                'match_index': match.start() + start_index,
-                'remove': True
-            }
-        return None
-    parser.add_handler("volumes", handle_volumes)
-
-    # Seasons
-    parser.add_handler("seasons", regex.compile(r"(?:complete\W|seasons?\W|\W|^)((?:s\d{1,2}[., +/\\&-]+)+s\d{1,2}\b)", regex.IGNORECASE), range_func, { "remove": True })
-    parser.add_handler("seasons", regex.compile(r"(?:complete\W|seasons?\W|\W|^)[([]?(s\d{2,}-\d{2,}\b)[)\]]?", regex.IGNORECASE), range_func, { "remove": True })
-    parser.add_handler("seasons", regex.compile(r"(?:complete\W|seasons?\W|\W|^)[([]?(s[1-9]-[2-9]\b)[)\]]?", regex.IGNORECASE), range_func, { "remove": True })
-    parser.add_handler("seasons", regex.compile(r"(?:(?:\bthe\W)?\bcomplete\W)?(?:seasons?|[Сс]езони?|temporadas?)[. ]?[-:]?[. ]?[([]?((?:\d{1,2}[., /\\&]+)+\d{1,2}\b)[)\]]?", regex.IGNORECASE), range_func, { "remove": True })
-    parser.add_handler("seasons", regex.compile(r"(?:(?:\bthe\W)?\bcomplete\W)?(?:seasons|[Сс]езони?|temporadas?)[. ]?[-:]?[. ]?[([]?((?:\d{1,2}[. -]+)+[1-9]\d?\b)[)\]]?", regex.IGNORECASE), range_func, { "remove": True })
-    parser.add_handler("seasons", regex.compile(r"(?:(?:\bthe\W)?\bcomplete\W)?season[. ]?[([]?((?:\d{1,2}[. -]+)+[1-9]\d?\b)[)\]]?(?!.*\.\w{2,4}$)", regex.IGNORECASE), range_func, { "remove": True })
-    parser.add_handler("seasons", regex.compile(r"(?:(?:\bthe\W)?\bcomplete\W)?\bseasons?\b[. -]?(\d{1,2}[. -]?(?:to|thru|and|\+|:)[. -]?\d{1,2})\b", regex.IGNORECASE), range_func, { "remove": True })
-    parser.add_handler("seasons", regex.compile(r"(?:(?:\bthe\W)?\bcomplete\W)?(?:saison|seizoen|season|series|temp(?:orada)?):?[. ]?(\d{1,2})", regex.IGNORECASE), array(integer))
-    parser.add_handler("seasons", regex.compile(r"(\d{1,2})(?:-?й)?[. _]?(?:[Сс]езон|sez(?:on)?)(?:\W?\D|$)", regex.IGNORECASE), array(integer))
-    parser.add_handler("seasons", regex.compile(r"[Сс]езон:?[. _]?№?(\d{1,2})(?!\d)", regex.IGNORECASE), array(integer))
-    parser.add_handler("seasons", regex.compile(r"(?:\D|^)(\d{1,2})Â?[°ºªa]?[. ]*temporada", regex.IGNORECASE), array(integer), { "remove": True })
-    parser.add_handler("seasons", regex.compile(r"t(\d{1,3})(?:[ex]+|$)", regex.IGNORECASE), array(integer), { "remove": True })
-    parser.add_handler("seasons", regex.compile(r"(?:(?:\bthe\W)?\bcomplete)?(?:\W|^)s(\d{1,3})(?:[\Wex]|\d{2}\b|$)", regex.IGNORECASE), array(integer), { "skipIfAlreadyFound": False })
-    parser.add_handler("seasons", regex.compile(r"(?:(?:\bthe\W)?\bcomplete\W)?(?:\W|^)(\d{1,2})[. ]?(?:st|nd|rd|th)[. ]*season", regex.IGNORECASE), array(integer))
-    parser.add_handler("seasons", regex.compile(r"(?:\D|^)(\d{1,2})[xх]\d{1,3}(?:\D|$)"), array(integer))
-    parser.add_handler("seasons", regex.compile(r"\bSn([1-9])(?:\D|$)"), array(integer))
-    parser.add_handler("seasons", regex.compile(r"[[(](\d{1,2})\.\d{1,3}[)\]]"), array(integer))
-    parser.add_handler("seasons", regex.compile(r"-\s?(\d{1,2})\.\d{2,3}\s?-"), array(integer))
-    parser.add_handler("seasons", regex.compile(r"(?:^|\/)(\d{1,2})-\d{2}\b(?!-\d)"), array(integer))
-    parser.add_handler("seasons", regex.compile(r"[^\w-](\d{1,2})-\d{2}(?=\.\w{2,4}$)"), array(integer))
-    parser.add_handler("seasons", regex.compile(r"(?<!\bEp?(?:isode)? ?\d+\b.*)\b(\d{2})[ ._]\d{2}(?:.F)?\.\w{2,4}$"), array(integer))
-    parser.add_handler("seasons", regex.compile(r"\bEp(?:isode)?\W+(\d{1,2})\.\d{1,3}\b", regex.IGNORECASE), array(integer))
-
-    # Episodes
-    parser.add_handler("episodes", regex.compile(r"(?:[\W\d]|^)e[ .]?[([]?(\d{1,3}(?:[ .-]*(?:[&+]|e){1,2}[ .]?\d{1,3})+)(?:\W|$)", regex.IGNORECASE), range_func)
-    parser.add_handler("episodes", regex.compile(r"(?:[\W\d]|^)ep[ .]?[([]?(\d{1,3}(?:[ .-]*(?:[&+]|ep){1,2}[ .]?\d{1,3})+)(?:\W|$)", regex.IGNORECASE), range_func)
-    parser.add_handler("episodes", regex.compile(r"(?:[\W\d]|^)\d+[xх][ .]?[([]?(\d{1,3}(?:[ .]?[xх][ .]?\d{1,3})+)(?:\W|$)", regex.IGNORECASE), range_func)
-    parser.add_handler("episodes", regex.compile(r"(?:[\W\d]|^)(?:episodes?|[Сс]ерии:?)[ .]?[([]?(\d{1,3}(?:[ .+]*[&+][ .]?\d{1,3})+)(?:\W|$)", regex.IGNORECASE), range_func)
-    parser.add_handler("episodes", regex.compile(r"[([]?(?:\D|^)(\d{1,3}[ .]?ao[ .]?\d{1,3})[)\]]?(?:\W|$)", regex.IGNORECASE), range_func)
-    parser.add_handler("episodes", regex.compile(r"(?:[\W\d]|^)(?:e|eps?|episodes?|[Сс]ерии:?|\d+[xх])[ .]*[([]?(\d{1,3}(?:-\d{1,3})+)(?:\W|$)", regex.IGNORECASE), range_func)
-    parser.add_handler("episodes", regex.compile(r"(?:\W|^)[st]\d{1,2}[. ]?[xх-]?[. ]?(?:e|x|х|ep|-|\.)[. ]?(\d{1,3})(?:[abc]|v0?[1-4]|\D|$)", regex.IGNORECASE), array(integer))
-    parser.add_handler("episodes", regex.compile(r"\b[st]\d{2}(\d{2})\b", regex.IGNORECASE), array(integer))
-    parser.add_handler("episodes", regex.compile(r"(?:\W|^)(\d{1,3}(?:[ .]*~[ .]*\d{1,3})+)(?:\W|$)", regex.IGNORECASE), range_func)
-    parser.add_handler("episodes", regex.compile(r"-\s(\d{1,3}[ .]*-[ .]*\d{1,3})(?!-\d)(?:\W|$)", regex.IGNORECASE), range_func)
-    parser.add_handler("episodes", regex.compile(r"s\d{1,2}\s?\((\d{1,3}[ .]*-[ .]*\d{1,3})\)", regex.IGNORECASE), range_func)
-    parser.add_handler("episodes", regex.compile(r"(?:^|\/)\d{1,2}-(\d{2})\b(?!-\d)"), array(integer))
-    parser.add_handler("episodes", regex.compile(r"(?<!\d-)\b\d{1,2}-(\d{2})(?=\.\w{2,4}$)"), array(integer))
-    parser.add_handler("episodes", regex.compile(r"(?<!(?:seasons?|[Сс]езони?)\W*)(?:[ .([-]|^)(\d{1,3}(?:[ .]?[,&+~][ .]?\d{1,3})+)(?:[ .)\]-]|$)", regex.IGNORECASE), range_func)
-    parser.add_handler("episodes", regex.compile(r"(?<!(?:seasons?|[Сс]езони?)\W*)(?:[ .([-]|^)(\d{1,3}(?:-\d{1,3})+)(?:[ .)(\]]|-\D|$)", regex.IGNORECASE), range_func)
-    parser.add_handler("episodes", regex.compile(r"\bEp(?:isode)?\W+\d{1,2}\.(\d{1,3})\b", regex.IGNORECASE), array(integer))
-    parser.add_handler("episodes", regex.compile(r"(?:\b[ée]p?(?:isode)?|[Ээ]пизод|[Сс]ер(?:ии|ия|\.)?|cap(?:itulo)?|epis[oó]dio)[. ]?[-:#№]?[. ]?(\d{1,4})(?:[abc]|v0?[1-4]|\W|$)", regex.IGNORECASE), array(integer))
-    parser.add_handler("episodes", regex.compile(r"\b(\d{1,3})(?:-?я)?[ ._-]*(?:ser(?:i?[iyj]a|\b)|[Сс]ер(?:ии|ия|\.)?)", regex.IGNORECASE), array(integer))
-    parser.add_handler("episodes", regex.compile(r"(?:\D|^)\d{1,2}[. ]?[xх][. ]?(\d{1,3})(?:[abc]|v0?[1-4]|\D|$)"), array(integer)) # Fixed: Was catching `1.x265` as episode.
-    parser.add_handler("episodes", regex.compile(r"[[(]\d{1,2}\.(\d{1,3})[)\]]"), array(integer))
-    parser.add_handler("episodes", regex.compile(r"\b[Ss]\d{1,2}[ .](\d{1,2})\b"), array(integer))
-    parser.add_handler("episodes", regex.compile(r"-\s?\d{1,2}\.(\d{2,3})\s?-"), array(integer))
-    parser.add_handler("episodes", regex.compile(r"(?<=\D|^)(\d{1,3})[. ]?(?:of|из|iz)[. ]?\d{1,3}(?=\D|$)", regex.IGNORECASE), array(integer))
-    parser.add_handler("episodes", regex.compile(r"\b\d{2}[ ._-](\d{2})(?:.F)?\.\w{2,4}$"), array(integer))
-    parser.add_handler("episodes", regex.compile(r"(?<!^)\[(\d{2,3})](?!(?:\.\w{2,4})?$)"), array(integer))
-    def handle_episodes(context):
-        title = context['title']
-        result = context.get('result', {})
-        matched = context.get('matched', {})
-
-        if 'episodes' not in result:
-            # Gather start indexes from relevant matched fields
-            start_indexes = [comp.get('match_index') for comp in [matched.get('year'), matched.get('seasons')] if comp and comp.get('match_index', None)]
-            end_indexes = [comp['match_index'] for comp in
-                           [matched.get('resolution'), matched.get('source'), matched.get('codec'),
-                            matched.get('audio')] if comp and comp.get('match_index', None)]
-
-            # Define the range of the title to search based on detected components
-            start_index = min(start_indexes) if start_indexes else 0
-            end_index = min(end_indexes + [len(title)])
-
-            # Extract relevant parts of the title for detailed scanning
-            beginning_title = title[:end_index]
-            middle_title = title[start_index:end_index]
-
-            # Regex patterns to capture episode information, avoiding common prefixes like "movie" or "film"
-            regex_patterns = [
-                r'(?<!movie\W*|film\W*|^)(?:[ .]+-[ .]+|[([][ .]*)(\d{1,4})(?:a|b|v\d)?(?:\W|$)(?!movie|film)',
-                r'^(?:[([-][ .]?)?(\d{1,4})(?:a|b|v\d)?(?:\W|$)(?!movie|film)'
-            ]
-
-            # Attempt to match episodes within the defined sections of the title
-            for pattern in regex_patterns:
-                matches = regex.search(pattern, beginning_title, regex.IGNORECASE) or regex.search(pattern, middle_title,
-                                                                                          regex.IGNORECASE)
-                if matches:
-                    # Extract episode numbers, remove non-digits and convert to integers
-                    episode_numbers = [int(num) for num in regex.findall(r'\d+', matches.group(1))]
-                    result['episodes'] = episode_numbers
-                    return {'match_index': title.index(matches.group(0))}
-
-        return None
-    parser.add_handler("episodes", handle_episodes)
-
-    # Complete
-    parser.add_handler("complete", regex.compile(r"(?:\bthe\W)?(?:\bcomplete|collection|dvd)?\b[ .]?\bbox[ .-]?set\b", regex.IGNORECASE), boolean)
-    parser.add_handler("complete", regex.compile(r"(?:\bthe\W)?(?:\bcomplete|collection|dvd)?\b[ .]?\bmini[ .-]?series\b", regex.IGNORECASE), boolean)
-    parser.add_handler("complete", regex.compile(r"(?:\bthe\W)?(?:\bcomplete|full|all)\b.*\b(?:series|seasons|collection|episodes|set|pack|movies)\b", regex.IGNORECASE), boolean)
-    parser.add_handler("complete", regex.compile(r"\b(?:series|seasons|movies?)\b.*\b(?:complete|collection)\b", regex.IGNORECASE), boolean)
-    parser.add_handler("complete", regex.compile(r"(?:\bthe\W)?\bultimate\b[ .]\bcollection\b", regex.IGNORECASE), boolean, { "skipIfAlreadyFound": False })
-    parser.add_handler("complete", regex.compile(r"\bcollection\b.*\b(?:set|pack|movies)\b", regex.IGNORECASE), boolean)
-    parser.add_handler("complete", regex.compile(r"\bcollection\b", regex.IGNORECASE), boolean, { "skipFromTitle": True })
-    parser.add_handler("complete", regex.compile(r"duology|trilogy|quadr[oi]logy|tetralogy|pentalogy|hexalogy|heptalogy|anthology|saga", regex.IGNORECASE), boolean, { "skipIfAlreadyFound": False })
-
-    # Languages
-    parser.add_handler("languages", regex.compile(r"\bmulti(?:ple)?[ .-]*(?:su?$|sub\w*|dub\w*)\b|msub", regex.IGNORECASE), uniq_concat(value("multi subs")), {"skipIfAlreadyFound": False, "remove": True})
-    parser.add_handler("languages", regex.compile(r"\bmulti(?:ple)?[ .-]*(?:lang(?:uages?)?|audio|VF2)?\b", regex.IGNORECASE), uniq_concat(value("multi audio")), {"skipIfAlreadyFound": False})
-    parser.add_handler("languages", regex.compile(r"\btri(?:ple)?[ .-]*(?:audio|dub\w*)\b", regex.IGNORECASE), uniq_concat(value("multi audio")), {"skipIfAlreadyFound": False})
-    parser.add_handler("languages", regex.compile(r"\bdual[ .-]*(?:au?$|[aá]udio|line)\b", regex.IGNORECASE), uniq_concat(value("dual audio")), {"skipIfAlreadyFound": False})
-    parser.add_handler("languages", regex.compile(r"\bdual\b(?![ .-]*sub)", regex.IGNORECASE), uniq_concat(value("dual audio")), {"skipIfAlreadyFound": False})
-    parser.add_handler("languages", regex.compile(r"\bengl?(?:sub[A-Z]*)?\b", regex.IGNORECASE), uniq_concat(value("english")), {"skipIfAlreadyFound": False})
-    parser.add_handler("languages", regex.compile(r"\beng?sub[A-Z]*\b", regex.IGNORECASE), uniq_concat(value("english")), {"skipIfAlreadyFound": False})
-    parser.add_handler("languages", regex.compile(r"\bing(?:l[eéê]s)?\b", regex.IGNORECASE), uniq_concat(value("english")), {"skipIfAlreadyFound": False})
-    parser.add_handler("languages", regex.compile(r"\benglish\W+(?:subs?|sdh|hi)\b", regex.IGNORECASE), uniq_concat(value("english")), {"skipIfAlreadyFound": False})
-    parser.add_handler("languages", regex.compile(r"\bEN\b", regex.IGNORECASE), uniq_concat(value("english")), {"skipFromTitle": True, "skipIfAlreadyFound": False})
-    parser.add_handler("languages", regex.compile(r"\benglish?\b", regex.IGNORECASE), uniq_concat(value("english")), {"skipIfFirst": True, "skipIfAlreadyFound": False})
-    parser.add_handler("languages", regex.compile(r"\b(?:JP|JAP|JPN)\b", regex.IGNORECASE), uniq_concat(value("japanese")), {"skipIfAlreadyFound": False})
-    parser.add_handler("languages", regex.compile(r"\b(japanese|japon[eê]s)\b", regex.IGNORECASE), uniq_concat(value("japanese")), {"skipIfFirst": True, "skipIfAlreadyFound": False})
-    parser.add_handler("languages", regex.compile(r"\b(?:KOR|kor[ .-]?sub)\b", regex.IGNORECASE), uniq_concat(value("korean")), {"skipIfAlreadyFound": False})
-    parser.add_handler("languages", regex.compile(r"\b(korean|coreano)\b", regex.IGNORECASE), uniq_concat(value("korean")), {"skipIfFirst": True, "skipIfAlreadyFound": False})
-    parser.add_handler("languages", regex.compile(r"\b(?:traditional\W*chinese|chinese\W*traditional)(?:\Wchi)?\b", regex.IGNORECASE), uniq_concat(value("taiwanese")), {"skipIfAlreadyFound": False, "remove": True})
-    parser.add_handler("languages", regex.compile(r"\bzh-hant\b", regex.IGNORECASE), uniq_concat(value("taiwanese")), {"skipIfAlreadyFound": False})
-    parser.add_handler("languages", regex.compile(r"\b(?:mand[ae]rin|ch[sn])\b", regex.IGNORECASE), uniq_concat(value("chinese")), {"skipIfAlreadyFound": False})
-    parser.add_handler("languages", regex.compile(r"\bCH[IT]\b", regex.IGNORECASE), uniq_concat(value("chinese")), {"skipFromTitle": True, "skipIfAlreadyFound": False})
-    parser.add_handler("languages", regex.compile(r"\b(chinese|chin[eê]s|chi)\b", regex.IGNORECASE), uniq_concat(value("chinese")), {"skipIfFirst": True, "skipIfAlreadyFound": False})
-    parser.add_handler("languages", regex.compile(r"\bzh-hans\b", regex.IGNORECASE), uniq_concat(value("chinese")), {"skipIfAlreadyFound": False})
-    parser.add_handler("languages", regex.compile(r"\bFR(?:ench|a|e|anc[eê]s)?\b", regex.IGNORECASE), uniq_concat(value("french")), {"skipIfAlreadyFound": False})
-    parser.add_handler("languages", regex.compile(r"\b(Truefrench|VF[FI])\b", regex.IGNORECASE), uniq_concat(value("french")), {"skipIfAlreadyFound": False})
-    parser.add_handler("languages", regex.compile(r"\b(VOST(?:FR?|A)?|SUBFRENCH)\b", regex.IGNORECASE), uniq_concat(value("french")), {"skipIfAlreadyFound": False})
-    parser.add_handler("languages", regex.compile(r"\bspanish\W?latin|american\W*(?:spa|esp?)", regex.IGNORECASE), uniq_concat(value("latino")), { "skipFromTitle": True, "skipIfAlreadyFound": False, "remove": True })
-    parser.add_handler("languages", regex.compile(r"\b(?:audio.)?lat(?:i|ino)?\b", regex.IGNORECASE), uniq_concat(value("latino")), { "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(?:audio.)?(?:ESP|spa|(en[ .]+)?espa[nñ]ola?|castellano)\b", regex.IGNORECASE), uniq_concat(value("spanish")), { "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bes(?=[ .,/-]+(?:[A-Z]{2}[ .,/-]+){2,})\b", regex.IGNORECASE), uniq_concat(value("spanish")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(?<=[ .,/-]+(?:[A-Z]{2}[ .,/-]+){2,})es\b", regex.IGNORECASE), uniq_concat(value("spanish")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(?<=[ .,/-]+[A-Z]{2}[ .,/-]+)es(?=[ .,/-]+[A-Z]{2}[ .,/-]+)\b", regex.IGNORECASE), uniq_concat(value("spanish")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bes(?=\.(?:ass|ssa|srt|sub|idx)$)", regex.IGNORECASE), uniq_concat(value("spanish")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bspanish\W+subs?\b", regex.IGNORECASE), uniq_concat(value("spanish")), { "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(spanish|espanhol)\b", regex.IGNORECASE), uniq_concat(value("spanish")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(?:p[rt]|en|port)[. (\\/-]*BR\b", regex.IGNORECASE), uniq_concat(value("portuguese")), { "skipIfAlreadyFound": False, "remove": True })
-    parser.add_handler("languages", regex.compile(r"\bbr(?:a|azil|azilian)\W+(?:pt|por)\b", regex.IGNORECASE), uniq_concat(value("portuguese")), { "skipIfAlreadyFound": False, "remove": True })
-    parser.add_handler("languages", regex.compile(r"\b(?:leg(?:endado|endas?)?|dub(?:lado)?|portugu[eèê]se?)[. -]*BR\b", regex.IGNORECASE), uniq_concat(value("portuguese")), { "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bleg(?:endado|endas?)\b", regex.IGNORECASE), uniq_concat(value("portuguese")), { "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bportugu[eèê]s[ea]?\b", regex.IGNORECASE), uniq_concat(value("portuguese")), { "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bPT[. -]*(?:PT|ENG?|sub(?:s|titles?))\b", regex.IGNORECASE), uniq_concat(value("portuguese")), { "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bpt(?=\.(?:ass|ssa|srt|sub|idx)$)", regex.IGNORECASE), uniq_concat(value("portuguese")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bpor\b", regex.IGNORECASE), uniq_concat(value("portuguese")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bITA\b", regex.IGNORECASE), uniq_concat(value("italian")), { "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(?<!w{3}\.\w+\.)IT(?=[ .,/-]+(?:[a-zA-Z]{2}[ .,/-]+){2,})\b"), uniq_concat(value("italian")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bit(?=\.(?:ass|ssa|srt|sub|idx)$)", regex.IGNORECASE), uniq_concat(value("italian")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bitaliano?\b", regex.IGNORECASE), uniq_concat(value("italian")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bgreek[ .-]*(?:audio|lang(?:uage)?|subs?(?:titles?)?)?\b", regex.IGNORECASE), uniq_concat(value("greek")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(?:GER|DEU)\b", regex.IGNORECASE), uniq_concat(value("german")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bde(?=[ .,/-]+(?:[A-Z]{2}[ .,/-]+){2,})\b", regex.IGNORECASE), uniq_concat(value("german")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(?<=[ .,/-]+(?:[A-Z]{2}[ .,/-]+){2,})de\b", regex.IGNORECASE), uniq_concat(value("german")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(?<=[ .,/-]+[A-Z]{2}[ .,/-]+)de(?=[ .,/-]+[A-Z]{2}[ .,/-]+)\b", regex.IGNORECASE), uniq_concat(value("german")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bde(?=\.(?:ass|ssa|srt|sub|idx)$)", regex.IGNORECASE), uniq_concat(value("german")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(german|alem[aã]o)\b", regex.IGNORECASE), uniq_concat(value("german")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bRUS?\b", regex.IGNORECASE), uniq_concat(value("russian")), { "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(russian|russo)\b", regex.IGNORECASE), uniq_concat(value("russian")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bUKR\b", regex.IGNORECASE), uniq_concat(value("ukrainian")), { "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bukrainian\b", regex.IGNORECASE), uniq_concat(value("ukrainian")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bhin(?:di)?\b", regex.IGNORECASE), uniq_concat(value("hindi")), { "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(?:(?<!w{3}\.\w+\.)tel(?!\W*aviv)|telugu)\b", regex.IGNORECASE), uniq_concat(value("telugu")), { "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bt[aâ]m(?:il)?\b", regex.IGNORECASE), uniq_concat(value("tamil")), { "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(?<!YTS\.)LT\b"), uniq_concat(value("lithuanian")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\blithuanian\b", regex.IGNORECASE), uniq_concat(value("lithuanian")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\blatvian\b", regex.IGNORECASE), uniq_concat(value("latvian")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bestonian\b", regex.IGNORECASE), uniq_concat(value("estonian")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(?:(?<!w{3}\.\w+\.)PL|pol)\b", regex.IGNORECASE), uniq_concat(value("polish")), { "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(polish|polon[eê]s|polaco)\b", regex.IGNORECASE), uniq_concat(value("polish")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bCZ[EH]?\b", regex.IGNORECASE), uniq_concat(value("czech")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bczech\b", regex.IGNORECASE), uniq_concat(value("czech")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bslo(?:vak|vakian|subs|[\]_)]?\.\w{2,4}$)\b", regex.IGNORECASE), uniq_concat(value("slovakian")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bHU\b"), uniq_concat(value("hungarian")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bHUN(?:garian)?\b", regex.IGNORECASE), uniq_concat(value("hungarian")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bROM(?:anian)?\b", regex.IGNORECASE), uniq_concat(value("romanian")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bRO(?=[ .,/-]*(?:[A-Z]{2}[ .,/-]+)*sub)", regex.IGNORECASE), uniq_concat(value("romanian")), { "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bbul(?:garian)?\b", regex.IGNORECASE), uniq_concat(value("bulgarian")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(?:srp|serbian)\b", regex.IGNORECASE), uniq_concat(value("serbian")), { "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(?:HRV|croatian)\b", regex.IGNORECASE), uniq_concat(value("croatian")), { "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bHR(?=[ .,/-]*(?:[A-Z]{2}[ .,/-]+)*sub)\b", regex.IGNORECASE), uniq_concat(value("croatian")), { "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bslovenian\b", regex.IGNORECASE), uniq_concat(value("slovenian")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(?:(?<!w{3}\.\w+\.)NL|dut|holand[eê]s)\b", regex.IGNORECASE), uniq_concat(value("dutch")), { "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bdutch\b", regex.IGNORECASE), uniq_concat(value("dutch")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bflemish\b", regex.IGNORECASE), uniq_concat(value("dutch")), { "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(?:DK|danska|dansub|nordic)\b", regex.IGNORECASE), uniq_concat(value("danish")), { "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(danish|dinamarqu[eê]s)\b", regex.IGNORECASE), uniq_concat(value("danish")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bdan\b(?=.*\.(?:srt|vtt|ssa|ass|sub|idx)$)", regex.IGNORECASE), uniq_concat(value("danish")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(?:(?<!w{3}\.\w+\.)FI|finsk|finsub|nordic)\b", regex.IGNORECASE), uniq_concat(value("finnish")), { "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bfinnish\b", regex.IGNORECASE), uniq_concat(value("finnish")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(?:(?<!w{3}\.\w+\.)SE|swe|swesubs?|sv(?:ensk)?|nordic)\b", regex.IGNORECASE), uniq_concat(value("swedish")), { "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(swedish|sueco)\b", regex.IGNORECASE), uniq_concat(value("swedish")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(?:NOR|norsk|norsub|nordic)\b", regex.IGNORECASE), uniq_concat(value("norwegian")), { "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(norwegian|noruegu[eê]s|bokm[aå]l|nob|nor(?=[\]_)]?\.\w{2,4}$))\b", regex.IGNORECASE), uniq_concat(value("norwegian")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(?:arabic|[aá]rabe|ara)\b", regex.IGNORECASE), uniq_concat(value("arabic")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\barab.*(?:audio|lang(?:uage)?|sub(?:s|titles?)?)\b", regex.IGNORECASE), uniq_concat(value("arabic")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bar(?=\.(?:ass|ssa|srt|sub|idx)$)", regex.IGNORECASE), uniq_concat(value("arabic")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(?:turkish|tur(?:co)?)\b", regex.IGNORECASE), uniq_concat(value("turkish")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bvietnamese\b|\bvie(?=[\]_)]?\.\w{2,4}$)", regex.IGNORECASE), uniq_concat(value("vietnamese")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bind(?:onesian)?\b", regex.IGNORECASE), uniq_concat(value("indonesian")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(thai|tailand[eê]s)\b", regex.IGNORECASE), uniq_concat(value("thai")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(THA|tha)\b"), uniq_concat(value("thai")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(?:malay|may(?=[\]_)]?\.\w{2,4}$)|(?<=subs?\([a-z,]+)may)\b", regex.IGNORECASE), uniq_concat(value("malay")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\bheb(?:rew|raico)?\b", regex.IGNORECASE), uniq_concat(value("hebrew")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    parser.add_handler("languages", regex.compile(r"\b(persian|persa)\b", regex.IGNORECASE), uniq_concat(value("persian")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
-    def infer_language_based_on_naming(context):
-        title = context['title']
-        result = context['result']
-        matched = context['matched']
-        if 'languages' not in result or not any(lang in result['languages'] for lang in ['portuguese', 'spanish']):
-            # Checking if episode naming convention suggests Portuguese language
-            if (matched.get('episodes') and regex.search(r'capitulo|ao', matched['episodes'].get('raw_match', ''),
-                                                         regex.IGNORECASE)) or \
-                    regex.search(r'dublado', title, regex.IGNORECASE):
-                result['languages'] = result.get('languages', []) + ['portuguese']
-
-        return {'match_index': 0}
-    parser.add_handler("languages", infer_language_based_on_naming)
-
-    # Dubbed
-    parser.add_handler("dubbed", regex.compile(r"\b(?:DUBBED|dublado|dubbing|DUBS?)\b", regex.IGNORECASE), boolean)
-    def handle_dubbed(context):
-        result = context['result']
-        if 'languages' in result and any(lang in ['multi audio', 'dual audio'] for lang in result['languages']):
-            result['dubbed'] = True
-        return {'match_index': 0}
-    parser.add_handler("dubbed", handle_dubbed)
-
-    # Group
-    parser.add_handler("group", regex.compile(r"^\[([^[\]]+)]"))
-    parser.add_handler("group", regex.compile(r"\(([\w-]+)\)(?:$|\.\w{2,4}$)"))
-    def handle_group(context):
-        result = context['result']
-        matched = context['matched']
-        if 'group' in matched and matched['group'].get('raw_match', '').startswith('[') and matched['group']['raw_match'].endswith(']'):
-            end_index = matched['group']['match_index'] + len(matched['group']['raw_match']) if 'group' in matched else 0
-
-            # Check if there's any overlap with other matched elements
-            if any(key != 'group' and matched[key]['match_index'] < end_index for key in matched if
-                   'match_index' in matched[key]):
-                if 'group' in result:
-                    del result['group']
-        return {'match_index': 0}
-    parser.add_handler("group", handle_group)
-
-    # Extension
-    parser.add_handler("extension", regex.compile(r"\.(3g2|3gp|avi|flv|mkv|mk3d|mov|mp2|mp4|m4v|mpe|mpeg|mpg|mpv|webm|wmv|ogm|divx|ts|m2ts|iso|vob|sub|idx|ttxt|txt|smi|srt|ssa|ass|vtt|nfo|html)$", regex.IGNORECASE), lowercase)
+import regex
+
+from PTT.parse import Parser
+from PTT.transformers import (
+    none, value, integer, boolean, lowercase, uppercase, date,
+    range_func, year_range, array, uniq_concat
+)
+
+
+def add_defaults(parser: Parser):
+    # Episode code
+    parser.add_handler("episode_code", regex.compile(r"[[(]([a-zA-Z0-9]{8})[\])](?=\.[a-zA-Z0-9]{1,5}$|$)"), uppercase, {"remove": True})
+    parser.add_handler("episode_code", regex.compile(r"\[([A-Z0-9]{8})]"), uppercase, {"remove": True})
+
+    # Resolution
+    parser.add_handler("resolution", regex.compile(r"\b(?:\[?\]?4k[\])?]?)\b", regex.IGNORECASE), value("4k"), {"remove": True})
+    parser.add_handler("resolution", regex.compile(r"21600?[pi]", regex.IGNORECASE), value("4k"), {"skipIfAlreadyFound": False, "remove": True})
+    parser.add_handler("resolution", regex.compile(r"\[?\]?3840x\d{4}[\])?]?", regex.IGNORECASE), value("4k"), {"remove": True})
+    parser.add_handler("resolution", regex.compile(r"\[?\]?1920x\d{3,4}[\])?]?", regex.IGNORECASE), value("1080p"), {"remove": True})
+    parser.add_handler("resolution", regex.compile(r"\[?\]?1280x\d{3}[\])?]?", regex.IGNORECASE), value("720p"), {"remove": True})
+    parser.add_handler("resolution", regex.compile(r"\[?\]?(\d{3,4}x\d{3,4})[\])?]?", regex.IGNORECASE), value("$1p"), {"remove": True})
+    parser.add_handler("resolution", regex.compile(r"(480|720|1080)0[pi]", regex.IGNORECASE), value("$1p"), {"remove": True})
+    parser.add_handler("resolution", regex.compile(r"(?:BD|HD|M)(720|1080|2160)"), value("$1p"), {"remove": True})
+    parser.add_handler("resolution", regex.compile(r"(480|576|720|1080|2160)[pi]", regex.IGNORECASE), value("$1p"), {"remove": True})
+    parser.add_handler("resolution", regex.compile(r"(?:^|\D)(\d{3,4})[pi]", regex.IGNORECASE), value("$1p"), {"remove": True})
+
+    # Date
+    parser.add_handler("date", regex.compile(r"(?:\W|^)([[(]?(?:19[6-9]|20[012])[0-9]([. \-/\\])(?:0[1-9]|1[012])\2(?:0[1-9]|[12][0-9]|3[01])[])]?)(?:\W|$)"), date("YYYY MM DD"), {"remove": True})
+    parser.add_handler("date", regex.compile(r"(?:\W|^)(\[?\]?(?:0[1-9]|[12][0-9]|3[01])([. \-/\\])(?:0[1-9]|1[012])\2(?:19[6-9]|20[01])[0-9][\])]?)(?:\W|$)"), date("DD MM YYYY"), {"remove": True})
+    parser.add_handler("date", regex.compile(r"(?:\W)(\[?\]?(?:0[1-9]|1[012])([. \-/\\])(?:0[1-9]|[12][0-9]|3[01])\2(?:[0][1-9]|[0126789][0-9])[\])]?)(?:\W|$)"), date("MM DD YY"), {"remove": True})
+    parser.add_handler("date", regex.compile(r"(?:\W)(\[?\]?(?:0[1-9]|[12][0-9]|3[01])([. \-/\\])(?:0[1-9]|1[012])\2(?:[0][1-9]|[0126789][0-9])[\])]?)(?:\W|$)"), date("DD MM YY"), {"remove": True})
+    parser.add_handler("date", regex.compile(r"(?:\W|^)([([]?(?:0?[1-9]|[12][0-9]|3[01])[. ]?(?:st|nd|rd|th)?([. \-/\\])(?:feb(?:ruary)?|jan(?:uary)?|mar(?:ch)?|apr(?:il)?|may|june?|july?|aug(?:ust)?|sept?(?:ember)?|oct(?:ober)?|nov(?:ember)?|dec(?:ember)?)\2(?:19[7-9]|20[012])[0-9][)\]]?)(?=\W|$)", regex.IGNORECASE), date(["DD MMM YYYY", "Do MMM YYYY", "Do MMMM YYYY"]), {"remove": True})
+    parser.add_handler("date", regex.compile(r"(?:\W|^)(\[?\]?(?:0?[1-9]|[12][0-9]|3[01])[. ]?(?:st|nd|rd|th)?([. \-\/\\])(?:feb(?:ruary)?|jan(?:uary)?|mar(?:ch)?|apr(?:il)?|may|june?|july?|aug(?:ust)?|sept?(?:ember)?|oct(?:ober)?|nov(?:ember)?|dec(?:ember)?)\2(?:0[1-9]|[0126789][0-9])[\])]?)(?:\W|$)", regex.IGNORECASE), date("DD MMM YY"), {"remove": True})
+    parser.add_handler("date", regex.compile(r"(?:\W|^)(\[?\]?20[012][0-9](?:0[1-9]|1[012])(?:0[1-9]|[12][0-9]|3[01])[\])]?)(?:\W|$)"), date("YYYYMMDD"), {"remove": True})
+
+    # Year
+    parser.add_handler("year", regex.compile(r"[([]?[ .]?((?:19\d|20[012])\d[ .]?-[ .]?(?:19\d|20[012])\d)[ .]?[)\]]?"), year_range, { "remove": True })
+    parser.add_handler("year", regex.compile(r"[([][ .]?((?:19\d|20[012])\d[ .]?-[ .]?\d{2})[ .]?[)\]]"), year_range, { "remove": True })
+    parser.add_handler("year", regex.compile(r"[([]?(?!^)(?<!\d|Cap[. ]?)((?:19\d|20[012])\d)(?!\d|kbps)[)\]]?", regex.IGNORECASE), integer, { "remove": True })
+    parser.add_handler("year", regex.compile(r"^[([]?((?:19\d|20[012])\d)(?!\d|kbps)[)\]]?", regex.IGNORECASE), integer, { "remove": True })
+
+    # Extended
+    parser.add_handler("extended", regex.compile(r"EXTENDED"), boolean)
+
+    # Convert
+    parser.add_handler("convert", regex.compile(r"CONVERT"), boolean)
+
+    # Hardcoded
+    parser.add_handler("hardcoded", regex.compile(r"HC|HARDCODED"), boolean)
+
+    # Proper
+    parser.add_handler("proper", regex.compile(r"(?:REAL.)?PROPER"), boolean)
+
+    # Repack
+    parser.add_handler("repack", regex.compile(r"REPACK|RERIP"), boolean)
+
+    # Retail
+    parser.add_handler("retail", regex.compile(r"\bRetail\b", regex.IGNORECASE), boolean)
+
+    # Remastered
+    parser.add_handler("remastered", regex.compile(r"\bRemaster(?:ed)?\b", regex.IGNORECASE), boolean)
+
+    # Unrated
+    parser.add_handler("unrated", regex.compile(r"\bunrated|uncensored\b", regex.IGNORECASE), boolean)
+
+    # Region
+    parser.add_handler("region", regex.compile(r"R\d\b"), none, { "skipIfFirst": True })
+
+    # Source
+    parser.add_handler("source", regex.compile(r"\b(?:H[DQ][ .-]*)?CAM(?:H[DQ])?(?:[ .-]*Rip)?\b", regex.IGNORECASE), value("CAM"), {"remove": True})
+    parser.add_handler("source", regex.compile(r"\b(?:H[DQ][ .-]*)?S[ .-]*print", regex.IGNORECASE), value("CAM"), {"remove": True})
+    parser.add_handler("source", regex.compile(r"\b(?:HD[ .-]*)?T(?:ELE)?S(?:YNC)?(?:Rip)?\b", regex.IGNORECASE), value("TeleSync"), {"remove": True})
+    parser.add_handler("source", regex.compile(r"\b(?:HD[ .-]*)?T(?:ELE)?C(?:INE)?(?:Rip)?\b"), value("TeleCine"), {"remove": True})
+    parser.add_handler("source", regex.compile(r"\bBlu[ .-]*Ray\b(?=.*remux)", regex.IGNORECASE), value("BluRay REMUX"), {"remove": True})
+    parser.add_handler("source", regex.compile(r"(?:BD|BR|UHD)[- ]?remux", regex.IGNORECASE), value("BluRay REMUX"), {"remove": True})
+    parser.add_handler("source", regex.compile(r"(?<=remux.*)\bBlu[ .-]*Ray\b", regex.IGNORECASE), value("BluRay REMUX"), {"remove": True})
+    parser.add_handler("source", regex.compile(r"\bBlu[ .-]*Ray\b(?![ .-]*Rip)", regex.IGNORECASE), value("BluRay"), {"remove": True})
+    parser.add_handler("source", regex.compile(r"\bUHD[ .-]*Rip\b", regex.IGNORECASE), value("UHDRip"), {"remove": True})
+    parser.add_handler("source", regex.compile(r"\bHD[ .-]*Rip\b", regex.IGNORECASE), value("HDRip"), {"remove": True})
+    parser.add_handler("source", regex.compile(r"\bMicro[ .-]*HD\b", regex.IGNORECASE), value("HDRip"), {"remove": True})
+    parser.add_handler("source", regex.compile(r"\b(?:BR|Blu[ .-]*Ray)[ .-]*Rip\b", regex.IGNORECASE), value("BRRip"), {"remove": True})
+    parser.add_handler("source", regex.compile(r"\bBD[ .-]*Rip\b|\bBDR\b|\bBD-RM\b|[[(]BD[\]) .,-]", regex.IGNORECASE), value("BDRip"), {"remove": True})
+    parser.add_handler("source", regex.compile(r"\b(?:HD[ .-]*)?DVD[ .-]*Rip\b", regex.IGNORECASE), value("DVDRip"), {"remove": True})
+    parser.add_handler("source", regex.compile(r"\bVHS[ .-]*Rip\b", regex.IGNORECASE), value("DVDRip"), {"remove": True})
+    parser.add_handler("source", regex.compile(r"\b(?:DVD?|BD|BR)?[ .-]*Scr(?:eener)?\b", regex.IGNORECASE), value("SCR"), {"remove": True})
+    parser.add_handler("source", regex.compile(r"\bP(?:re)?DVD(?:Rip)?\b", regex.IGNORECASE), value("SCR"), {"remove": True})
+    parser.add_handler("source", regex.compile(r"\bDVD(?:R\d?)?\b", regex.IGNORECASE), value("DVD"), {"remove": True})
+    parser.add_handler("source", regex.compile(r"\bVHS\b", regex.IGNORECASE), value("DVD"), {"remove": True})
+    parser.add_handler("source", regex.compile(r"\bPPVRip\b", regex.IGNORECASE), value("PPVRip"), {"remove": True})
+    parser.add_handler("source", regex.compile(r"\bHD[ .-]*TV(?:Rip)?\b", regex.IGNORECASE), value("HDTV"), {"remove": True})
+    parser.add_handler("source", regex.compile(r"\bDVB[ .-]*(?:Rip)?\b", regex.IGNORECASE), value("HDTV"), {"remove": True})
+    parser.add_handler("source", regex.compile(r"\bSAT[ .-]*Rips?\b", regex.IGNORECASE), value("SATRip"), {"remove": True})
+    parser.add_handler("source", regex.compile(r"\bTVRips?\b", regex.IGNORECASE), value("TVRip"), {"remove": True})
+    parser.add_handler("source", regex.compile(r"\bR5\b", regex.IGNORECASE), value("R5"), {"remove": True})
+    parser.add_handler("source", regex.compile(r"\bWEB[ .-]*DL(?:Rip)?\b", regex.IGNORECASE), value("WEB-DL"), {"remove": True})
+    parser.add_handler("source", regex.compile(r"\bWEB[ .-]*Rip\b", regex.IGNORECASE), value("WEBRip"), {"remove": True})
+    parser.add_handler("source", regex.compile(r"\b(?:DL|WEB|BD|BR)MUX\b", regex.IGNORECASE), none, {"remove": True})
+    parser.add_handler("source", regex.compile(r"\b(DivX|XviD)\b"), none, {"remove": False}) # TODO: In the js implementation it's true. But then a test case fails in our implementation and i'm not sure why
+
+    # Video depth
+    parser.add_handler("bit_depth", regex.compile(r"\bhevc\s?10\b", regex.IGNORECASE), value("10bit"))
+    parser.add_handler("bit_depth", regex.compile(r"(?:8|10|12)[- ]?bit", regex.IGNORECASE), lowercase, {"remove": True})
+    parser.add_handler("bit_depth", regex.compile(r"\bhdr10\b", regex.IGNORECASE), value("10bit"))
+    parser.add_handler("bit_depth", regex.compile(r"\bhi10\b", regex.IGNORECASE), value("10bit"))
+    def handle_bit_depth(context):
+        result = context['result']
+        if 'bitDepth' in result:
+            # Replace hyphens and spaces with nothing (effectively removing them)
+            result['bit_depth'] = result['bit_depth'].replace(" ", "").replace("-", "")
+    parser.add_handler("bit_depth", handle_bit_depth)
+
+    # HDR
+    parser.add_handler("hdr", regex.compile(r"\bDV\b|dolby.?vision|\bDoVi\b", regex.IGNORECASE), uniq_concat(value("DV")), {"remove": True, "skipIfAlreadyFound": False})
+    parser.add_handler("hdr", regex.compile(r"HDR10(?:\+|plus)", regex.IGNORECASE), uniq_concat(value("HDR10+")), {"remove": True, "skipIfAlreadyFound": False})
+    parser.add_handler("hdr", regex.compile(r"\bHDR(?:10)?\b", regex.IGNORECASE), uniq_concat(value("HDR")), {"remove": True, "skipIfAlreadyFound": False})
+
+    # Codec
+    parser.add_handler("codec", regex.compile(r"\b[xh][-. ]?26[45]", regex.IGNORECASE), lowercase, {"remove": True})
+    parser.add_handler("codec", regex.compile(r"\bhevc(?:\s?10)?\b", regex.IGNORECASE), value("hevc"), {"remove": True, "skipIfAlreadyFound": False})
+    parser.add_handler("codec", regex.compile(r"\b(?:dvix|mpeg2|divx|xvid|avc)\b", regex.IGNORECASE), lowercase, {"remove": True, "skipIfAlreadyFound": False})
+    def handle_space_in_codec(context):
+        if context["result"].get("codec"):
+            context["result"]["codec"] = regex.sub("[ .-]", "", context["result"]["codec"])
+    parser.add_handler("codec", handle_space_in_codec)
+
+    # Audio
+    parser.add_handler("audio", regex.compile(r"7\.1[. ]?Atmos\b", regex.IGNORECASE), value("7.1 Atmos"), {"remove": True})
+    parser.add_handler("audio", regex.compile(r"\b(?:mp3|Atmos|DTS(?:-HD)?|TrueHD)\b", regex.IGNORECASE), lowercase)
+    parser.add_handler("audio", regex.compile(r"\bFLAC(?:\+?2\.0)?(?:x[2-4])?\b", regex.IGNORECASE), value("flac"), {"remove": True})
+    parser.add_handler("audio", regex.compile(r"\bEAC-?3(?:[. -]?[256]\.[01])?", regex.IGNORECASE), value("eac3"), {"remove": True, "skipIfAlreadyFound": False})
+    parser.add_handler("audio", regex.compile(r"\bAC-?3(?:[.-]5\.1|x2\.?0?)?\b", regex.IGNORECASE), value("ac3"), {"remove": True, "skipIfAlreadyFound": False})
+    parser.add_handler("audio", regex.compile(r"\b5\.1(?:x[2-4]+)?\+2\.0(?:x[2-4])?\b", regex.IGNORECASE), value("2.0"), {"remove": True, "skipIfAlreadyFound": False})
+    parser.add_handler("audio", regex.compile(r"\b2\.0(?:x[2-4]|\+5\.1(?:x[2-4])?)\b", regex.IGNORECASE), value("2.0"), {"remove": True, "skipIfAlreadyFound": False})
+    parser.add_handler("audio", regex.compile(r"\b5\.1ch\b", regex.IGNORECASE), value("ac3"), {"remove": True, "skipIfAlreadyFound": False})
+    parser.add_handler("audio", regex.compile(r"\bDD5[. ]?1\b", regex.IGNORECASE), value("dd5.1"), {"remove": True})
+    parser.add_handler("audio", regex.compile(r"\bQ?AAC(?:[. ]?2[. ]0|x2)?\b", regex.IGNORECASE), value("aac"), {"remove": True})
+
+    # Group
+    parser.add_handler("group", regex.compile(r"- ?(?!\d+$|S\d+|\d+x|ep?\d+|[^[]+]$)([^\-. []+[^\-. [)\]\d][^\-. [)\]]*)(?:\[[\w.-]+])?(?=\.\w{2,4}$|$)", regex.IGNORECASE), none, {"remove": False}) # TODO: I js implementation, it's True, but doesn't get removed?!....
+
+    # Container
+    parser.add_handler("container", regex.compile(r"\.?[\[(]?\b(MKV|AVI|MP4|WMV|MPG|MPEG)\b[\])]?", regex.IGNORECASE), lowercase)
+
+    # Volume
+    parser.add_handler("volumes", regex.compile(r"\bvol(?:s|umes?)?[. -]*(?:\d{1,2}[., +/\\&-]+)+\d{1,2}\b", regex.IGNORECASE), range_func, {"remove": True})
+    # parser.add_handler("volumes", regex.compile(r"\bvol(?:s|umes?)?[. -]*(\d{1,2})\b", regex.IGNORECASE), integer, {"remove": True})
+    def handle_volumes(context):
+        title = context['title']
+        result = context['result']
+        matched = context['matched']
+
+        # Determine the start index based on whether the year is matched
+        start_index = matched.get('year', {}).get('match_index', 0)
+
+        # Regular expression to find volume numbers
+        match = regex.search(r'\bvol(?:ume)?[. -]*(\d{1,2})', title[start_index:], regex.IGNORECASE)
+
+        if match:
+            # Update the matched information for volumes
+            matched['volumes'] = {'match': match.group(0), 'match_index': match.start()}
+
+            # Convert the captured group to an integer and store it in the result
+            result['volumes'] = [int(match.group(1))]
+
+            # Return a dictionary with details of the raw match and its index
+            return {
+                'raw_match': match.group(0),
+                'match_index': match.start() + start_index,
+                'remove': True
+            }
+        return None
+    parser.add_handler("volumes", handle_volumes)
+
+    # Seasons
+    parser.add_handler("seasons", regex.compile(r"(?:complete\W|seasons?\W|\W|^)((?:s\d{1,2}[., +/\\&-]+)+s\d{1,2}\b)", regex.IGNORECASE), range_func, { "remove": True })
+    parser.add_handler("seasons", regex.compile(r"(?:complete\W|seasons?\W|\W|^)[([]?(s\d{2,}-\d{2,}\b)[)\]]?", regex.IGNORECASE), range_func, { "remove": True })
+    parser.add_handler("seasons", regex.compile(r"(?:complete\W|seasons?\W|\W|^)[([]?(s[1-9]-[2-9])[)\]]?", regex.IGNORECASE), range_func, { "remove": True })
+    parser.add_handler("seasons", regex.compile(r"(?:(?:\bthe\W)?\bcomplete\W)?(?:seasons?|[Сс]езони?|temporadas?)[. ]?[-:]?[. ]?[([]?((?:\d{1,2}[., /\\&]+)+\d{1,2}\b)[)\]]?", regex.IGNORECASE), range_func, { "remove": True })
+    parser.add_handler("seasons", regex.compile(r"(?:(?:\bthe\W)?\bcomplete\W)?(?:seasons?|[Сс]езони?|temporadas?)[. ]?[-:]?[. ]?[([]?((?:\d{1,2}[.-]+)+[1-9]\d?\b)[)\]]?", regex.IGNORECASE), range_func, { "remove": True })
+    parser.add_handler("seasons", regex.compile(r"(?:(?:\bthe\W)?\bcomplete\W)?season[. ]?[([]?((?:\d{1,2}[. -]+)+[1-9]\d?\b)[)\]]?(?!.*\.\w{2,4}$)", regex.IGNORECASE), range_func, { "remove": True })
+    parser.add_handler("seasons", regex.compile(r"(?:(?:\bthe\W)?\bcomplete\W)?\bseasons?\b[. -]?(\d{1,2}[. -]?(?:to|thru|and|\+|:)[. -]?\d{1,2})\b", regex.IGNORECASE), range_func, { "remove": True })
+    parser.add_handler("seasons", regex.compile(r"(?:(?:\bthe\W)?\bcomplete\W)?(?:saison|seizoen|season|series|temp(?:orada)?):?[. ]?(\d{1,2})", regex.IGNORECASE), array(integer))
+    parser.add_handler("seasons", regex.compile(r"(\d{1,2})(?:-?й)?[. _]?(?:[Сс]езон|sez(?:on)?)(?:\W?\D|$)", regex.IGNORECASE), array(integer))
+    parser.add_handler("seasons", regex.compile(r"[Сс]езон:?[. _]?№?(\d{1,2})(?!\d)", regex.IGNORECASE), array(integer))
+    parser.add_handler("seasons", regex.compile(r"(?:\D|^)(\d{1,2})Â?[°ºªa]?[. ]*temporada", regex.IGNORECASE), array(integer), { "remove": True })
+    parser.add_handler("seasons", regex.compile(r"t(\d{1,3})(?:[ex]+|$)", regex.IGNORECASE), array(integer), { "remove": True })
+    parser.add_handler("seasons", regex.compile(r"(?:(?:\bthe\W)?\bcomplete)?(?:\W|^)s(\d{1,3})(?:[\Wex]|\d{2}\b|$)", regex.IGNORECASE), array(integer), { "skipIfAlreadyFound": False })
+    parser.add_handler("seasons", regex.compile(r"(?:(?:\bthe\W)?\bcomplete\W)?(?:\W|^)(\d{1,2})[. ]?(?:st|nd|rd|th)[. ]*season", regex.IGNORECASE), array(integer))
+    parser.add_handler("seasons", regex.compile(r"(?:\D|^)(\d{1,2})[xх]\d{1,3}(?:\D|$)"), array(integer))
+    parser.add_handler("seasons", regex.compile(r"\bSn([1-9])(?:\D|$)"), array(integer))
+    parser.add_handler("seasons", regex.compile(r"[[(](\d{1,2})\.\d{1,3}[)\]]"), array(integer))
+    parser.add_handler("seasons", regex.compile(r"-\s?(\d{1,2})\.\d{2,3}\s?-"), array(integer))
+    parser.add_handler("seasons", regex.compile(r"(?:^|\/)(\d{1,2})-\d{2}\b(?!-\d)"), array(integer))
+    parser.add_handler("seasons", regex.compile(r"[^\w-](\d{1,2})-\d{2}(?=\.\w{2,4}$)"), array(integer))
+    parser.add_handler("seasons", regex.compile(r"(?<!\bEp?(?:isode)? ?\d+\b.*)\b(\d{2})[ ._]\d{2}(?:.F)?\.\w{2,4}$"), array(integer))
+    parser.add_handler("seasons", regex.compile(r"\bEp(?:isode)?\W+(\d{1,2})\.\d{1,3}\b", regex.IGNORECASE), array(integer))
+
+    # Episodes
+    parser.add_handler("episodes", regex.compile(r"(?:[\W\d]|^)e[ .]?[([]?(\d{1,3}(?:[ .-]*(?:[&+]|e){1,2}[ .]?\d{1,3})+)(?:\W|$)", regex.IGNORECASE), range_func)
+    parser.add_handler("episodes", regex.compile(r"(?:[\W\d]|^)ep[ .]?[([]?(\d{1,3}(?:[ .-]*(?:[&+]|ep){1,2}[ .]?\d{1,3})+)(?:\W|$)", regex.IGNORECASE), range_func)
+    parser.add_handler("episodes", regex.compile(r"(?:[\W\d]|^)\d+[xх][ .]?[([]?(\d{1,3}(?:[ .]?[xх][ .]?\d{1,3})+)(?:\W|$)", regex.IGNORECASE), range_func)
+    parser.add_handler("episodes", regex.compile(r"(?:[\W\d]|^)(?:episodes?|[Сс]ерии:?)[ .]?[([]?(\d{1,3}(?:[ .+]*[&+][ .]?\d{1,3})+)(?:\W|$)", regex.IGNORECASE), range_func)
+    parser.add_handler("episodes", regex.compile(r"[([]?(?:\D|^)(\d{1,3}[ .]?ao[ .]?\d{1,3})[)\]]?(?:\W|$)", regex.IGNORECASE), range_func)
+    parser.add_handler("episodes", regex.compile(r"(?:[\W\d]|^)(?:e|eps?|episodes?|[Сс]ерии:?|\d+[xх])[ .]*[([]?(\d{1,3}(?:-\d{1,3})+)(?:\W|$)", regex.IGNORECASE), range_func)
+    parser.add_handler("episodes", regex.compile(r"(?:\W|^)[st]\d{1,2}[. ]?[xх-]?[. ]?(?:e|x|х|ep|-|\.)[. ]?(\d{1,3})(?:[abc]|v0?[1-4]|\D|$)", regex.IGNORECASE), array(integer))
+    parser.add_handler("episodes", regex.compile(r"\b[st]\d{2}(\d{2})\b", regex.IGNORECASE), array(integer))
+    parser.add_handler("episodes", regex.compile(r"(?:\W|^)(\d{1,3}(?:[ .]*~[ .]*\d{1,3})+)(?:\W|$)", regex.IGNORECASE), range_func)
+    parser.add_handler("episodes", regex.compile(r"-\s(\d{1,3}[ .]*-[ .]*\d{1,3})(?!-\d)(?:\W|$)", regex.IGNORECASE), range_func)
+    parser.add_handler("episodes", regex.compile(r"s\d{1,2}\s?\((\d{1,3}[ .]*-[ .]*\d{1,3})\)", regex.IGNORECASE), range_func)
+    parser.add_handler("episodes", regex.compile(r"(?:^|\/)\d{1,2}-(\d{2})\b(?!-\d)"), array(integer))
+    parser.add_handler("episodes", regex.compile(r"(?<!\d-)\b\d{1,2}-(\d{2})(?=\.\w{2,4}$)"), array(integer))
+    parser.add_handler("episodes", regex.compile(r"(?<!(?:seasons?|[Сс]езони?)\W*)(?:[ .([-]|^)(\d{1,3}(?:[ .]?[,&+~][ .]?\d{1,3})+)(?:[ .)\]-]|$)", regex.IGNORECASE), range_func)
+    parser.add_handler("episodes", regex.compile(r"(?<!(?:seasons?|[Сс]езони?)\W*)(?:[ .([-]|^)(\d{1,3}(?:-\d{1,3})+)(?:[ .)(\]]|-\D|$)", regex.IGNORECASE), range_func)
+    parser.add_handler("episodes", regex.compile(r"\bEp(?:isode)?\W+\d{1,2}\.(\d{1,3})\b", regex.IGNORECASE), array(integer))
+    parser.add_handler("episodes", regex.compile(r"(?:\b[ée]p?(?:isode)?|[Ээ]пизод|[Сс]ер(?:ии|ия|\.)?|cap(?:itulo)?|epis[oó]dio)[. ]?[-:#№]?[. ]?(\d{1,4})(?:[abc]|v0?[1-4]|\W|$)", regex.IGNORECASE), array(integer))
+    parser.add_handler("episodes", regex.compile(r"\b(\d{1,3})(?:-?я)?[ ._-]*(?:ser(?:i?[iyj]a|\b)|[Сс]ер(?:ии|ия|\.)?)", regex.IGNORECASE), array(integer))
+    parser.add_handler("episodes", regex.compile(r"(?:\D|^)\d{1,2}[. ]?[xх][. ]?(\d{1,3})(?:[abc]|v0?[1-4]|\D|$)"), array(integer)) # Fixed: Was catching `1.x265` as episode.
+    parser.add_handler("episodes", regex.compile(r"[[(]\d{1,2}\.(\d{1,3})[)\]]"), array(integer))
+    parser.add_handler("episodes", regex.compile(r"\b[Ss]\d{1,2}[ .](\d{1,2})\b"), array(integer))
+    parser.add_handler("episodes", regex.compile(r"-\s?\d{1,2}\.(\d{2,3})\s?-"), array(integer))
+    parser.add_handler("episodes", regex.compile(r"(?<=\D|^)(\d{1,3})[. ]?(?:of|из|iz)[. ]?\d{1,3}(?=\D|$)", regex.IGNORECASE), array(integer))
+    parser.add_handler("episodes", regex.compile(r"\b\d{2}[ ._-](\d{2})(?:.F)?\.\w{2,4}$"), array(integer))
+    parser.add_handler("episodes", regex.compile(r"(?<!^)\[(\d{2,3})](?!(?:\.\w{2,4})?$)"), array(integer))
+    def handle_episodes(context):
+        title = context['title']
+        result = context.get('result', {})
+        matched = context.get('matched', {})
+
+        if 'episodes' not in result:
+            # Gather start indexes from relevant matched fields
+            start_indexes = [comp.get('match_index') for comp in [matched.get('year'), matched.get('seasons')] if comp and comp.get('match_index', None)]
+            end_indexes = [comp['match_index'] for comp in
+                           [matched.get('resolution'), matched.get('source'), matched.get('codec'),
+                            matched.get('audio')] if comp and comp.get('match_index', None)]
+
+            # Define the range of the title to search based on detected components
+            start_index = min(start_indexes) if start_indexes else 0
+            end_index = min(end_indexes + [len(title)])
+
+            # Extract relevant parts of the title for detailed scanning
+            beginning_title = title[:end_index]
+            middle_title = title[start_index:end_index]
+
+            matches = regex.search(r'(?<!movie\W*|film\W*|^)(?:[ .]+-[ .]+|[([][ .]*)(\d{1,4})(?:a|b|v\d)?(?:\W|$)(?!movie|film)', beginning_title, regex.IGNORECASE) or regex.search(r'^(?:[([-][ .]?)?(\d{1,4})(?:a|b|v\d)?(?:\W|$)(?!movie|film)', middle_title, regex.IGNORECASE)
+
+            if matches:
+                # Extract episode numbers, remove non-digits and convert to integers
+                episode_numbers = [int(num) for num in regex.findall(r'\d+', matches.group(1))]
+                result['episodes'] = episode_numbers
+                return {'match_index': title.index(matches.group(0))}
+
+        return None
+    parser.add_handler("episodes", handle_episodes)
+
+    # Complete
+    parser.add_handler("complete", regex.compile(r"(?:\bthe\W)?(?:\bcomplete|collection|dvd)?\b[ .]?\bbox[ .-]?set\b", regex.IGNORECASE), boolean)
+    parser.add_handler("complete", regex.compile(r"(?:\bthe\W)?(?:\bcomplete|collection|dvd)?\b[ .]?\bmini[ .-]?series\b", regex.IGNORECASE), boolean)
+    parser.add_handler("complete", regex.compile(r"(?:\bthe\W)?(?:\bcomplete|full|all)\b.*\b(?:series|seasons|collection|episodes|set|pack|movies)\b", regex.IGNORECASE), boolean)
+    parser.add_handler("complete", regex.compile(r"\b(?:series|seasons|movies?)\b.*\b(?:complete|collection)\b", regex.IGNORECASE), boolean)
+    parser.add_handler("complete", regex.compile(r"(?:\bthe\W)?\bultimate\b[ .]\bcollection\b", regex.IGNORECASE), boolean, { "skipIfAlreadyFound": False })
+    parser.add_handler("complete", regex.compile(r"\bcollection\b.*\b(?:set|pack|movies)\b", regex.IGNORECASE), boolean)
+    parser.add_handler("complete", regex.compile(r"\bcollection\b", regex.IGNORECASE), boolean, { "skipFromTitle": True })
+    parser.add_handler("complete", regex.compile(r"duology|trilogy|quadr[oi]logy|tetralogy|pentalogy|hexalogy|heptalogy|anthology|saga", regex.IGNORECASE), boolean, { "skipIfAlreadyFound": False })
+
+    # Languages
+    parser.add_handler("languages", regex.compile(r"\bmulti(?:ple)?[ .-]*(?:su?$|sub\w*|dub\w*)\b|msub", regex.IGNORECASE), uniq_concat(value("multi subs")), {"skipIfAlreadyFound": False, "remove": True})
+    parser.add_handler("languages", regex.compile(r"\bmulti(?:ple)?[ .-]*(?:lang(?:uages?)?|audio|VF2)?\b", regex.IGNORECASE), uniq_concat(value("multi audio")), {"skipIfAlreadyFound": False})
+    parser.add_handler("languages", regex.compile(r"\btri(?:ple)?[ .-]*(?:audio|dub\w*)\b", regex.IGNORECASE), uniq_concat(value("multi audio")), {"skipIfAlreadyFound": False})
+    parser.add_handler("languages", regex.compile(r"\bdual[ .-]*(?:au?$|[aá]udio|line)\b", regex.IGNORECASE), uniq_concat(value("dual audio")), {"skipIfAlreadyFound": False})
+    parser.add_handler("languages", regex.compile(r"\bdual\b(?![ .-]*sub)", regex.IGNORECASE), uniq_concat(value("dual audio")), {"skipIfAlreadyFound": False})
+    parser.add_handler("languages", regex.compile(r"\bengl?(?:sub[A-Z]*)?\b", regex.IGNORECASE), uniq_concat(value("english")), {"skipIfAlreadyFound": False})
+    parser.add_handler("languages", regex.compile(r"\beng?sub[A-Z]*\b", regex.IGNORECASE), uniq_concat(value("english")), {"skipIfAlreadyFound": False})
+    parser.add_handler("languages", regex.compile(r"\bing(?:l[eéê]s)?\b", regex.IGNORECASE), uniq_concat(value("english")), {"skipIfAlreadyFound": False})
+    parser.add_handler("languages", regex.compile(r"\benglish\W+(?:subs?|sdh|hi)\b", regex.IGNORECASE), uniq_concat(value("english")), {"skipIfAlreadyFound": False})
+    parser.add_handler("languages", regex.compile(r"\bEN\b", regex.IGNORECASE), uniq_concat(value("english")), {"skipFromTitle": True, "skipIfAlreadyFound": False})
+    parser.add_handler("languages", regex.compile(r"\benglish?\b", regex.IGNORECASE), uniq_concat(value("english")), {"skipIfFirst": True, "skipIfAlreadyFound": False})
+    parser.add_handler("languages", regex.compile(r"\b(?:JP|JAP|JPN)\b", regex.IGNORECASE), uniq_concat(value("japanese")), {"skipIfAlreadyFound": False})
+    parser.add_handler("languages", regex.compile(r"\b(japanese|japon[eê]s)\b", regex.IGNORECASE), uniq_concat(value("japanese")), {"skipIfFirst": True, "skipIfAlreadyFound": False})
+    parser.add_handler("languages", regex.compile(r"\b(?:KOR|kor[ .-]?sub)\b", regex.IGNORECASE), uniq_concat(value("korean")), {"skipIfAlreadyFound": False})
+    parser.add_handler("languages", regex.compile(r"\b(korean|coreano)\b", regex.IGNORECASE), uniq_concat(value("korean")), {"skipIfFirst": True, "skipIfAlreadyFound": False})
+    parser.add_handler("languages", regex.compile(r"\b(?:traditional\W*chinese|chinese\W*traditional)(?:\Wchi)?\b", regex.IGNORECASE), uniq_concat(value("taiwanese")), {"skipIfAlreadyFound": False, "remove": True})
+    parser.add_handler("languages", regex.compile(r"\bzh-hant\b", regex.IGNORECASE), uniq_concat(value("taiwanese")), {"skipIfAlreadyFound": False})
+    parser.add_handler("languages", regex.compile(r"\b(?:mand[ae]rin|ch[sn])\b", regex.IGNORECASE), uniq_concat(value("chinese")), {"skipIfAlreadyFound": False})
+    parser.add_handler("languages", regex.compile(r"\bCH[IT]\b", regex.IGNORECASE), uniq_concat(value("chinese")), {"skipFromTitle": True, "skipIfAlreadyFound": False})
+    parser.add_handler("languages", regex.compile(r"\b(chinese|chin[eê]s|chi)\b", regex.IGNORECASE), uniq_concat(value("chinese")), {"skipIfFirst": True, "skipIfAlreadyFound": False})
+    parser.add_handler("languages", regex.compile(r"\bzh-hans\b", regex.IGNORECASE), uniq_concat(value("chinese")), {"skipIfAlreadyFound": False})
+    parser.add_handler("languages", regex.compile(r"\bFR(?:ench|a|e|anc[eê]s)?\b", regex.IGNORECASE), uniq_concat(value("french")), {"skipIfAlreadyFound": False})
+    parser.add_handler("languages", regex.compile(r"\b(Truefrench|VF[FI])\b", regex.IGNORECASE), uniq_concat(value("french")), {"skipIfAlreadyFound": False})
+    parser.add_handler("languages", regex.compile(r"\b(VOST(?:FR?|A)?|SUBFRENCH)\b", regex.IGNORECASE), uniq_concat(value("french")), {"skipIfAlreadyFound": False})
+    parser.add_handler("languages", regex.compile(r"\bspanish\W?latin|american\W*(?:spa|esp?)", regex.IGNORECASE), uniq_concat(value("latino")), { "skipFromTitle": True, "skipIfAlreadyFound": False, "remove": True })
+    parser.add_handler("languages", regex.compile(r"\b(?:audio.)?lat(?:i|ino)?\b", regex.IGNORECASE), uniq_concat(value("latino")), { "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(?:audio.)?(?:ESP|spa|(en[ .]+)?espa[nñ]ola?|castellano)\b", regex.IGNORECASE), uniq_concat(value("spanish")), { "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bes(?=[ .,/-]+(?:[A-Z]{2}[ .,/-]+){2,})\b", regex.IGNORECASE), uniq_concat(value("spanish")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(?<=[ .,/-]+(?:[A-Z]{2}[ .,/-]+){2,})es\b", regex.IGNORECASE), uniq_concat(value("spanish")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(?<=[ .,/-]+[A-Z]{2}[ .,/-]+)es(?=[ .,/-]+[A-Z]{2}[ .,/-]+)\b", regex.IGNORECASE), uniq_concat(value("spanish")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bes(?=\.(?:ass|ssa|srt|sub|idx)$)", regex.IGNORECASE), uniq_concat(value("spanish")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bspanish\W+subs?\b", regex.IGNORECASE), uniq_concat(value("spanish")), { "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(spanish|espanhol)\b", regex.IGNORECASE), uniq_concat(value("spanish")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(?:p[rt]|en|port)[. (\\/-]*BR\b", regex.IGNORECASE), uniq_concat(value("portuguese")), { "skipIfAlreadyFound": False, "remove": True })
+    parser.add_handler("languages", regex.compile(r"\bbr(?:a|azil|azilian)\W+(?:pt|por)\b", regex.IGNORECASE), uniq_concat(value("portuguese")), { "skipIfAlreadyFound": False, "remove": True })
+    parser.add_handler("languages", regex.compile(r"\b(?:leg(?:endado|endas?)?|dub(?:lado)?|portugu[eèê]se?)[. -]*BR\b", regex.IGNORECASE), uniq_concat(value("portuguese")), { "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bleg(?:endado|endas?)\b", regex.IGNORECASE), uniq_concat(value("portuguese")), { "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bportugu[eèê]s[ea]?\b", regex.IGNORECASE), uniq_concat(value("portuguese")), { "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bPT[. -]*(?:PT|ENG?|sub(?:s|titles?))\b", regex.IGNORECASE), uniq_concat(value("portuguese")), { "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bpt(?=\.(?:ass|ssa|srt|sub|idx)$)", regex.IGNORECASE), uniq_concat(value("portuguese")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bpor\b", regex.IGNORECASE), uniq_concat(value("portuguese")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bITA\b", regex.IGNORECASE), uniq_concat(value("italian")), { "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(?<!w{3}\.\w+\.)IT(?=[ .,/-]+(?:[a-zA-Z]{2}[ .,/-]+){2,})\b"), uniq_concat(value("italian")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bit(?=\.(?:ass|ssa|srt|sub|idx)$)", regex.IGNORECASE), uniq_concat(value("italian")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bitaliano?\b", regex.IGNORECASE), uniq_concat(value("italian")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bgreek[ .-]*(?:audio|lang(?:uage)?|subs?(?:titles?)?)?\b", regex.IGNORECASE), uniq_concat(value("greek")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(?:GER|DEU)\b", regex.IGNORECASE), uniq_concat(value("german")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bde(?=[ .,/-]+(?:[A-Z]{2}[ .,/-]+){2,})\b", regex.IGNORECASE), uniq_concat(value("german")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(?<=[ .,/-]+(?:[A-Z]{2}[ .,/-]+){2,})de\b", regex.IGNORECASE), uniq_concat(value("german")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(?<=[ .,/-]+[A-Z]{2}[ .,/-]+)de(?=[ .,/-]+[A-Z]{2}[ .,/-]+)\b", regex.IGNORECASE), uniq_concat(value("german")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bde(?=\.(?:ass|ssa|srt|sub|idx)$)", regex.IGNORECASE), uniq_concat(value("german")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(german|alem[aã]o)\b", regex.IGNORECASE), uniq_concat(value("german")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bRUS?\b", regex.IGNORECASE), uniq_concat(value("russian")), { "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(russian|russo)\b", regex.IGNORECASE), uniq_concat(value("russian")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bUKR\b", regex.IGNORECASE), uniq_concat(value("ukrainian")), { "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bukrainian\b", regex.IGNORECASE), uniq_concat(value("ukrainian")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bhin(?:di)?\b", regex.IGNORECASE), uniq_concat(value("hindi")), { "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(?:(?<!w{3}\.\w+\.)tel(?!\W*aviv)|telugu)\b", regex.IGNORECASE), uniq_concat(value("telugu")), { "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bt[aâ]m(?:il)?\b", regex.IGNORECASE), uniq_concat(value("tamil")), { "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(?<!YTS\.)LT\b"), uniq_concat(value("lithuanian")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\blithuanian\b", regex.IGNORECASE), uniq_concat(value("lithuanian")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\blatvian\b", regex.IGNORECASE), uniq_concat(value("latvian")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bestonian\b", regex.IGNORECASE), uniq_concat(value("estonian")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(?:(?<!w{3}\.\w+\.)PL|pol)\b", regex.IGNORECASE), uniq_concat(value("polish")), { "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(polish|polon[eê]s|polaco)\b", regex.IGNORECASE), uniq_concat(value("polish")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bCZ[EH]?\b", regex.IGNORECASE), uniq_concat(value("czech")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bczech\b", regex.IGNORECASE), uniq_concat(value("czech")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bslo(?:vak|vakian|subs|[\]_)]?\.\w{2,4}$)\b", regex.IGNORECASE), uniq_concat(value("slovakian")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bHU\b"), uniq_concat(value("hungarian")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bHUN(?:garian)?\b", regex.IGNORECASE), uniq_concat(value("hungarian")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bROM(?:anian)?\b", regex.IGNORECASE), uniq_concat(value("romanian")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bRO(?=[ .,/-]*(?:[A-Z]{2}[ .,/-]+)*sub)", regex.IGNORECASE), uniq_concat(value("romanian")), { "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bbul(?:garian)?\b", regex.IGNORECASE), uniq_concat(value("bulgarian")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(?:srp|serbian)\b", regex.IGNORECASE), uniq_concat(value("serbian")), { "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(?:HRV|croatian)\b", regex.IGNORECASE), uniq_concat(value("croatian")), { "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bHR(?=[ .,/-]*(?:[A-Z]{2}[ .,/-]+)*sub)\b", regex.IGNORECASE), uniq_concat(value("croatian")), { "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bslovenian\b", regex.IGNORECASE), uniq_concat(value("slovenian")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(?:(?<!w{3}\.\w+\.)NL|dut|holand[eê]s)\b", regex.IGNORECASE), uniq_concat(value("dutch")), { "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bdutch\b", regex.IGNORECASE), uniq_concat(value("dutch")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bflemish\b", regex.IGNORECASE), uniq_concat(value("dutch")), { "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(?:DK|danska|dansub|nordic)\b", regex.IGNORECASE), uniq_concat(value("danish")), { "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(danish|dinamarqu[eê]s)\b", regex.IGNORECASE), uniq_concat(value("danish")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bdan\b(?=.*\.(?:srt|vtt|ssa|ass|sub|idx)$)", regex.IGNORECASE), uniq_concat(value("danish")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(?:(?<!w{3}\.\w+\.)FI|finsk|finsub|nordic)\b", regex.IGNORECASE), uniq_concat(value("finnish")), { "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bfinnish\b", regex.IGNORECASE), uniq_concat(value("finnish")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(?:(?<!w{3}\.\w+\.)SE|swe|swesubs?|sv(?:ensk)?|nordic)\b", regex.IGNORECASE), uniq_concat(value("swedish")), { "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(swedish|sueco)\b", regex.IGNORECASE), uniq_concat(value("swedish")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(?:NOR|norsk|norsub|nordic)\b", regex.IGNORECASE), uniq_concat(value("norwegian")), { "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(norwegian|noruegu[eê]s|bokm[aå]l|nob|nor(?=[\]_)]?\.\w{2,4}$))\b", regex.IGNORECASE), uniq_concat(value("norwegian")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(?:arabic|[aá]rabe|ara)\b", regex.IGNORECASE), uniq_concat(value("arabic")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\barab.*(?:audio|lang(?:uage)?|sub(?:s|titles?)?)\b", regex.IGNORECASE), uniq_concat(value("arabic")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bar(?=\.(?:ass|ssa|srt|sub|idx)$)", regex.IGNORECASE), uniq_concat(value("arabic")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(?:turkish|tur(?:co)?)\b", regex.IGNORECASE), uniq_concat(value("turkish")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bvietnamese\b|\bvie(?=[\]_)]?\.\w{2,4}$)", regex.IGNORECASE), uniq_concat(value("vietnamese")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bind(?:onesian)?\b", regex.IGNORECASE), uniq_concat(value("indonesian")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(thai|tailand[eê]s)\b", regex.IGNORECASE), uniq_concat(value("thai")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(THA|tha)\b"), uniq_concat(value("thai")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(?:malay|may(?=[\]_)]?\.\w{2,4}$)|(?<=subs?\([a-z,]+)may)\b", regex.IGNORECASE), uniq_concat(value("malay")), { "skipIfFirst": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\bheb(?:rew|raico)?\b", regex.IGNORECASE), uniq_concat(value("hebrew")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    parser.add_handler("languages", regex.compile(r"\b(persian|persa)\b", regex.IGNORECASE), uniq_concat(value("persian")), { "skipFromTitle": True, "skipIfAlreadyFound": False })
+    def infer_language_based_on_naming(context):
+        title = context['title']
+        result = context['result']
+        matched = context['matched']
+        if 'languages' not in result or not any(lang in result['languages'] for lang in ['portuguese', 'spanish']):
+            # Checking if episode naming convention suggests Portuguese language
+            if (matched.get('episodes') and regex.search(r'capitulo|ao', matched['episodes'].get('raw_match', ''),
+                                                         regex.IGNORECASE)) or \
+                    regex.search(r'dublado', title, regex.IGNORECASE):
+                result['languages'] = result.get('languages', []) + ['portuguese']
+
+        return {'match_index': 0}
+    parser.add_handler("languages", infer_language_based_on_naming)
+
+    # Dubbed
+    parser.add_handler("dubbed", regex.compile(r"\b(?:DUBBED|dublado|dubbing|DUBS?)\b", regex.IGNORECASE), boolean)
+    def handle_dubbed(context):
+        result = context['result']
+        if 'languages' in result and any(lang in ['multi audio', 'dual audio'] for lang in result['languages']):
+            result['dubbed'] = True
+        return {'match_index': 0}
+    parser.add_handler("dubbed", handle_dubbed)
+
+    # Group
+    parser.add_handler("group", regex.compile(r"^\[([^[\]]+)]"))
+    parser.add_handler("group", regex.compile(r"\(([\w-]+)\)(?:$|\.\w{2,4}$)"))
+    def handle_group(context):
+        result = context['result']
+        matched = context['matched']
+        if 'group' in matched and matched['group'].get('raw_match', '').startswith('[') and matched['group']['raw_match'].endswith(']'):
+            end_index = matched['group']['match_index'] + len(matched['group']['raw_match']) if 'group' in matched else 0
+
+            # Check if there's any overlap with other matched elements
+            if any(key != 'group' and matched[key]['match_index'] < end_index for key in matched if
+                   'match_index' in matched[key]):
+                if 'group' in result:
+                    del result['group']
+        return {'match_index': 0}
+    parser.add_handler("group", handle_group)
+
+    # Extension
+    parser.add_handler("extension", regex.compile(r"\.(3g2|3gp|avi|flv|mkv|mk3d|mov|mp2|mp4|m4v|mpe|mpeg|mpg|mpv|webm|wmv|ogm|divx|ts|m2ts|iso|vob|sub|idx|ttxt|txt|smi|srt|ssa|ass|vtt|nfo|html)$", regex.IGNORECASE), lowercase)
```

### Comparing `parsett-0.2.1/PTT/parse.py` & `parsett-0.2.2/PTT/parse.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,212 +1,201 @@
-import inspect
-from typing import Any
-import regex
-
-from .transformers import none
-
-NON_ENGLISH_CHARS = "\u3040-\u30ff\u3400-\u4dbf\u4e00-\u9fff\uf900-\ufaff\uff66-\uff9f\u0400-\u04ff"
-RUSSIAN_CAST_REGEX = regex.compile(r"\([^)]*[\u0400-\u04ff][^)]*\)$|(?<=\/.*)\(.*\)$")
-ALT_TITLES_REGEX = regex.compile(rf"[^/|(]*[{NON_ENGLISH_CHARS}][^/|]*[/|]|[/|][^/|(]*[{NON_ENGLISH_CHARS}][^/|]*")
-NOT_ONLY_NON_ENGLISH_REGEX = regex.compile(
-    rf"(?<=[a-zA-Z][^{NON_ENGLISH_CHARS}]+)[{NON_ENGLISH_CHARS}].*[{NON_ENGLISH_CHARS}]|[{NON_ENGLISH_CHARS}].*[{NON_ENGLISH_CHARS}](?=[^{NON_ENGLISH_CHARS}]+[a-zA-Z])")
-NOT_ALLOWED_SYMBOLS_AT_START_AND_END = regex.compile(rf"^[^\w{NON_ENGLISH_CHARS}#[【★]+|[ \-:/\\[|{{(#$&^]+$")
-REMAINING_NOT_ALLOWED_SYMBOLS_AT_START_AND_END = regex.compile(rf"^[^\w{NON_ENGLISH_CHARS}#]+|]$")
-
-DEBUG_HANDLER = None
-
-
-def extend_options(options=None):
-    """Extend the options dictionary with default values."""
-    default_options = {
-        "skipIfAlreadyFound": True,
-        "skipFromTitle": False,
-        "skipIfFirst": False,
-        "remove": False,
-    }
-    if options is None:
-        options = {}
-    for key, value in default_options.items():
-        options.setdefault(key, value)
-    return options
-
-
-def create_handler_from_regexp(name, reg_exp, transformer, options):
-    """Create a handler function from a regular expression pattern."""
-    def handler(context):
-        title = context['title']
-        result = context['result']
-        matched = context['matched']
-
-        if name in result and options.get('skipIfAlreadyFound', False):
-            return None
-
-        if name == DEBUG_HANDLER:
-            print(f"Regexp Pattern: {reg_exp.pattern}")
-            print(f"Title: {title}")
-
-        match = reg_exp.search(title)
-        if name == DEBUG_HANDLER:
-            print(f"Match: {match}")
-        if match:
-            raw_match = match.group(0)
-            clean_match = match.group(1) if len(match.groups()) >= 1 else raw_match
-            sig = inspect.signature(transformer)
-            param_count = len(sig.parameters)
-            transformed = transformer(clean_match or raw_match, *([result.get(name)] if param_count > 1 else []))
-
-            before_title_match = regex.match(r'^\[([^\[\]]+)]', title)
-            is_before_title = before_title_match is not None and raw_match in before_title_match.group(1)
-
-            other_matches = {k: v for k, v in matched.items() if k != name}
-            if name == DEBUG_HANDLER:
-                print(f"Other Matches: {other_matches}")
-            is_skip_if_first = options.get('skipIfFirst', False) and other_matches and all(
-                match.start() < other_matches[k]['match_index'] for k in other_matches
-            )
-            # is_skip_if_first = False
-
-            if transformed is not None and not is_skip_if_first:
-                matched[name] = matched.get(name, {'raw_match': raw_match, 'match_index': match.start()})
-                result[name] = options.get('value', transformed)
-                return {
-                    'raw_match': raw_match,
-                    'match_index': match.start(),
-                    'remove': options.get('remove', False),
-                    'skip_from_title': is_before_title or options.get('skipFromTitle', False)
-                }
-        return None
-
-    handler.__name__ = name
-    handler.handler_name = name
-    return handler
-
-
-def clean_title(raw_title):
-    """Clean up a title string by removing unwanted characters and patterns."""
-    cleaned_title = raw_title
-
-    if " " not in cleaned_title and "." in cleaned_title:
-        cleaned_title = regex.sub(r"\.", " ", cleaned_title)
-
-    cleaned_title = regex.sub(r"_", " ", cleaned_title)
-    cleaned_title = regex.sub(r"[[(]movie[)\]]", "", cleaned_title, flags=regex.IGNORECASE)
-    cleaned_title = NOT_ALLOWED_SYMBOLS_AT_START_AND_END.sub("", cleaned_title)
-    cleaned_title = RUSSIAN_CAST_REGEX.sub("", cleaned_title)
-    cleaned_title = regex.sub(r"^[[【★].*[\]】★][ .]?(.+)", r"\1", cleaned_title)
-    cleaned_title = regex.sub(r"(.+)[ .]?[[【★].*[\]】★]$", r"\1", cleaned_title)
-    cleaned_title = ALT_TITLES_REGEX.sub("", cleaned_title)
-    cleaned_title = NOT_ONLY_NON_ENGLISH_REGEX.sub("", cleaned_title)
-    cleaned_title = REMAINING_NOT_ALLOWED_SYMBOLS_AT_START_AND_END.sub("", cleaned_title)
-
-    # Trim the resulting title
-    cleaned_title = cleaned_title.strip()
-    return cleaned_title
-
-
-class Parser:
-    """
-    A parser that can parse release titles using a set of handlers.
-
-    The parser can be used to parse release titles using a set of handlers. Each handler is a function that takes a
-    title and returns a dictionary with the parsed data. The parser will iterate over all handlers and return the first
-    non-None result.
-
-    The parser can be extended with new handlers using the add_handler method. The handler can be a function or a
-    regular expression pattern. If a regular expression pattern is used, the parser will use the first group as the
-    match to be transformed by the transformer function.
-    
-    Example:
-        >>> parser = Parser()
-        >>> parser.add_handler("seasons", r"Season (\\d+)", int)
-        >>> parser.add_handler("episodes", r"Episode (\\d+)", int)
-        >>> parser.add_handler("languages", r"(English|Spanish|French)", str)
-        >>> result = parser.parse("The Simpsons Season 1 Episode 1 English")
-        >>> print(result)
-    """
-    def __init__(self):
-        self.handlers = []
-
-    def add_handler(self, handler_name, handler, transformer=None, options=None):
-
-        if not handler and callable(handler_name):
-            handler = handler_name
-            handler.handler_name = "unknown"
-        elif type(handler_name) == str and type(handler) == regex.Pattern:
-            transformer = transformer if callable(transformer) else none
-            options = extend_options(transformer if type(transformer) == dict else options)
-            handler = create_handler_from_regexp(handler_name, handler, transformer, options)
-        elif type(handler_name) == str and callable(handler):
-            handler.handler_name = handler_name
-        else:
-            raise ValueError(
-                f"Handler for {handler_name} should be either a regex pattern or a function. Got {type(handler)}")
-
-        self.handlers.append(handler)
-
-    def parse(self, title: str) -> dict: # type: ignore
-        """Parse a release title and return the parsed data as a dictionary."""
-        title: str = regex.sub(r"_+", " ", title)
-        result: dict[str, Any] = {}
-        matched: dict[str, Any] = {}
-        end_of_title: int = len(title)
-
-        for handler in self.handlers:
-            match_result = handler(
-                {
-                    "title": title,
-                    "result": result,
-                    "matched": matched
-                }
-            )
-
-            if handler.handler_name == DEBUG_HANDLER:
-                print(f"Result: {match_result}")
-
-            if match_result is None:
-                continue
-
-            if match_result.get('remove', False):
-                title = title[:match_result['match_index']] + title[match_result['match_index'] + len(
-                    match_result['raw_match']):]
-            if match_result.get('skip_from_title') and match_result.get('match_index') and match_result[
-                'match_index'] < end_of_title:
-                end_of_title = match_result['match_index']
-            if match_result.get('remove') and match_result.get('skip_from_title') and match_result[
-                'match_index'] < end_of_title:
-                # adjust title index in case part of it should be removed and skipped
-                end_of_title -= match_result.raw_match.length
-
-            # if match_result:
-            #     raw_match = match_result.group(0)
-            #     clean_match = match_result.group(1) if len(match_result.groups()) >= 1 else None
-            #     transformed_match = raw_match if clean_match is None else clean_match
-            #     if handler["transformer"]:
-            #         transformed = handler["transformer"](transformed_match)
-            #     else:
-            #         transformed = transformed_match
-            #
-            #     # If the handler demands removal, adjust the title and end_of_title accordingly.
-            #     if options.get("remove", False) and match_result.start() < end_of_title:
-            #         title = title[:match_result.start()] + title[match_result.end():]
-            #         end_of_title -= len(raw_match)
-            #
-            #     # Save matched data and result.
-            #     matched[handler["name"]] = {"raw_match": raw_match, "match_index": match_result.start()}
-            #     result[handler["name"]] = transformed
-            #
-            #     # If skipping from title, adjust the title and potentially end_of_title.
-            #     if options.get("skipFromTitle", False) and match_result.start() < end_of_title:
-            #         title = title.replace(raw_match, "", 1)
-            #         end_of_title = min(end_of_title, match_result.start())
-
-        if not result.get("episodes"):
-            result["episodes"] = []
-        if not result.get("seasons"):
-            result["seasons"] = []
-        if not result.get("languages"):
-            result["languages"] = []
-
-        # Clean the title up to end_of_title before further processing.
-        title: str = title[:end_of_title]
-        result["title"] = clean_title(title)
-        return result
+import inspect
+from typing import Any
+import regex
+
+from .transformers import none
+
+NON_ENGLISH_CHARS = "\u3040-\u30ff\u3400-\u4dbf\u4e00-\u9fff\uf900-\ufaff\uff66-\uff9f\u0400-\u04ff"
+RUSSIAN_CAST_REGEX = regex.compile(r"\([^)]*[\u0400-\u04ff][^)]*\)$|(?<=\/.*)\(.*\)$")
+ALT_TITLES_REGEX = regex.compile(rf"[^/|(]*[{NON_ENGLISH_CHARS}][^/|]*[/|]|[/|][^/|(]*[{NON_ENGLISH_CHARS}][^/|]*")
+NOT_ONLY_NON_ENGLISH_REGEX = regex.compile(
+    rf"(?<=[a-zA-Z][^{NON_ENGLISH_CHARS}]+)[{NON_ENGLISH_CHARS}].*[{NON_ENGLISH_CHARS}]|[{NON_ENGLISH_CHARS}].*[{NON_ENGLISH_CHARS}](?=[^{NON_ENGLISH_CHARS}]+[a-zA-Z])")
+NOT_ALLOWED_SYMBOLS_AT_START_AND_END = regex.compile(rf"^[^\w{NON_ENGLISH_CHARS}#[【★]+|[ \-:/\\[|{{(#$&^]+$")
+REMAINING_NOT_ALLOWED_SYMBOLS_AT_START_AND_END = regex.compile(rf"^[^\w{NON_ENGLISH_CHARS}#]+|]$")
+
+DEBUG_HANDLER = "seasons"
+
+
+def extend_options(options=None):
+    """Extend the options dictionary with default values."""
+    default_options = {
+        "skipIfAlreadyFound": True,
+        "skipFromTitle": False,
+        "skipIfFirst": False,
+        "remove": False,
+    }
+    if options is None:
+        options = {}
+    for key, value in default_options.items():
+        options.setdefault(key, value)
+    return options
+
+
+def create_handler_from_regexp(name, reg_exp, transformer, options):
+    """Create a handler function from a regular expression pattern."""
+    def handler(context):
+        title = context['title']
+        result = context['result']
+        matched = context['matched']
+
+        if name in result and options.get('skipIfAlreadyFound', False):
+            return None
+
+        # if name == DEBUG_HANDLER:
+        #     print(f"Regexp Pattern: {reg_exp.pattern}")
+        #     print(f"Title: {title}")
+
+        match = reg_exp.search(title)
+        # if name == DEBUG_HANDLER:
+        #     print(f"Match: {match}")
+        if match:
+            raw_match = match.group(0)
+            clean_match = match.group(1) if len(match.groups()) >= 1 else raw_match
+            sig = inspect.signature(transformer)
+            param_count = len(sig.parameters)
+            transformed = transformer(clean_match or raw_match, *([result.get(name)] if param_count > 1 else []))
+
+            before_title_match = regex.match(r'^\[([^[\]]+)]', title) # or '^\[([^\[\]]+)]'
+            is_before_title = before_title_match is not None and raw_match in before_title_match.group(1)
+
+            other_matches = {k: v for k, v in matched.items() if k != name}
+            # if name == DEBUG_HANDLER:
+            #     print(f"Other Matches: {other_matches}")
+            is_skip_if_first = options.get('skipIfFirst', False) and other_matches and all(
+                match.start() < other_matches[k]['match_index'] for k in other_matches
+            )
+            # is_skip_if_first = False
+
+            if transformed is not None and not is_skip_if_first:
+                matched[name] = matched.get(name, {'raw_match': raw_match, 'match_index': match.start()})
+                result[name] = options.get('value', transformed)
+                return {
+                    'raw_match': raw_match,
+                    'match_index': match.start(),
+                    'remove': options.get('remove', False),
+                    'skip_from_title': is_before_title or options.get('skipFromTitle', False)
+                }
+        return None
+
+    handler.__name__ = name
+    handler.handler_name = name
+    return handler
+
+
+def clean_title(raw_title):
+    """Clean up a title string by removing unwanted characters and patterns."""
+    cleaned_title = raw_title
+
+    if " " not in cleaned_title and "." in cleaned_title:
+        cleaned_title = regex.sub(r"\.", " ", cleaned_title)
+
+    cleaned_title = regex.sub(r"_", " ", cleaned_title)
+    cleaned_title = regex.sub(r"[[(]movie[)\]]", "", cleaned_title, flags=regex.IGNORECASE)
+    cleaned_title = NOT_ALLOWED_SYMBOLS_AT_START_AND_END.sub("", cleaned_title)
+    cleaned_title = RUSSIAN_CAST_REGEX.sub("", cleaned_title)
+    # maybe [\[\[【★].*[\]】★][ .]?(.+)
+    cleaned_title = regex.sub(r"^[[【★].*[\]】★][ .]?(.+)", r"\1", cleaned_title)
+    cleaned_title = regex.sub(r"(.+)[ .]?[[【★].*[\]】★]$", r"\1", cleaned_title)
+    cleaned_title = ALT_TITLES_REGEX.sub("", cleaned_title)
+    cleaned_title = NOT_ONLY_NON_ENGLISH_REGEX.sub("", cleaned_title)
+    cleaned_title = REMAINING_NOT_ALLOWED_SYMBOLS_AT_START_AND_END.sub("", cleaned_title)
+
+    # Trim the resulting title
+    cleaned_title = cleaned_title.strip()
+    return cleaned_title
+
+
+class Parser:
+    """
+    A parser that can parse release titles using a set of handlers.
+
+    The parser can be used to parse release titles using a set of handlers. Each handler is a function that takes a
+    title and returns a dictionary with the parsed data. The parser will iterate over all handlers and return the first
+    non-None result.
+
+    The parser can be extended with new handlers using the add_handler method. The handler can be a function or a
+    regular expression pattern. If a regular expression pattern is used, the parser will use the first group as the
+    match to be transformed by the transformer function.
+    
+    Example:
+        >>> parser = Parser()
+        >>> parser.add_handler("seasons", r"Season (\\d+)", int)
+        >>> parser.add_handler("episodes", r"Episode (\\d+)", int)
+        >>> parser.add_handler("languages", r"(English|Spanish|French)", str)
+        >>> result = parser.parse("The Simpsons Season 1 Episode 1 English")
+        >>> print(result)
+    """
+    def __init__(self):
+        self.handlers: list = []
+
+    def add_handler(self, handler_name, handler, transformer=None, options=None):
+
+        if not handler and callable(handler_name):
+            handler = handler_name
+            handler.handler_name = "unknown"
+        elif type(handler_name) == str and type(handler) == regex.Pattern:
+            transformer = transformer if callable(transformer) else none
+            options = extend_options(transformer if type(transformer) == dict else options)
+            handler = create_handler_from_regexp(handler_name, handler, transformer, options)
+        elif type(handler_name) == str and callable(handler):
+            handler.handler_name = handler_name
+        else:
+            raise ValueError(
+                f"Handler for {handler_name} should be either a regex pattern or a function. Got {type(handler)}")
+
+        self.handlers.append(handler)
+
+    def parse(self, title: str) -> dict: # type: ignore
+        """Parse a release title and return the parsed data as a dictionary."""
+        title: str = regex.sub(r"_+", " ", title)
+        result: dict[str, Any] = {}
+        matched: dict[str, Any] = {}
+        end_of_title: int = len(title)
+
+        for handler in self.handlers:
+            match_result = handler(
+                {
+                    "title": title,
+                    "result": result,
+                    "matched": matched
+                }
+            )
+
+            # if handler.handler_name == DEBUG_HANDLER:
+            #     print(f"Result: {match_result}")
+            #
+            # if DEBUG_HANDLER:
+            #     print(handler.handler_name)
+            #     print("Title before: " + title)
+
+            if match_result is None:
+                # if DEBUG_HANDLER:
+                #     print("Title after: " + title)
+                #     print(end_of_title)
+                continue
+
+            if match_result.get('remove', False):
+                title = title[:match_result['match_index']] + title[match_result['match_index'] + len(
+                    match_result['raw_match']):]
+            if not match_result.get('skip_from_title') and match_result.get('match_index') and match_result[
+                'match_index'] < end_of_title:
+                end_of_title = match_result['match_index']
+            if match_result.get('remove') and match_result.get('skip_from_title') and match_result[
+                'match_index'] < end_of_title:
+                # adjust title index in case part of it should be removed and skipped
+                end_of_title -= len(match_result.get("raw_match", ""))
+
+            # if DEBUG_HANDLER:
+            #     print("Title after: " + title)
+            #     print(end_of_title)
+
+        if not result.get("episodes"):
+            result["episodes"] = []
+        if not result.get("seasons"):
+            result["seasons"] = []
+        if not result.get("languages"):
+            result["languages"] = []
+
+        # Clean the title up to end_of_title before further processing.
+        title: str = title[:end_of_title]
+        result["title"] = clean_title(title)
+        return result
```

### Comparing `parsett-0.2.1/PTT/transformers.py` & `parsett-0.2.2/PTT/transformers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,122 +1,141 @@
-
-import arrow
-import regex
-
-
-def none(input_value: str) -> str:
-    return input_value
-
-
-def value(val):
-    def inner(input_value, existing_value=None):
-        if isinstance(val, str) and isinstance(input_value, str):
-            return val.replace("$1", input_value)
-        return val
-
-    return inner
-
-
-def integer(input_value):
-    try:
-        return int(input_value)
-    except ValueError:
-        return None
-
-
-def boolean(*args, **kwargs):
-    return True
-
-
-def lowercase(input_value):
-    return input_value.lower()
-
-
-def uppercase(input_value):
-    return input_value.upper()
-
-
-def date(date_format):
-    def inner(input_value):
-        sanitized = regex.sub(r"\W+", " ", input_value).strip()
-        print(f"Attempting to parse date: {sanitized}")
-        formats = [date_format] if not isinstance(date_format, list) else date_format
-        for fmt in formats:
-            try:
-                return arrow.get(sanitized, fmt).format("YYYY-MM-DD")
-            except ValueError as e:
-                print(f"Failed to parse date: {input_value} with format: {fmt}")
-                print(e)
-        return None
-
-    return inner
-
-
-# def range_func(input):
-#     array = [int(x) for x in regex.sub(r"\D+", " ", input).strip().split() if x.isdigit()]
-#     if len(array) == 2 and array[0] < array[1]:
-#         return list(range(array[0], array[1] + 1))
-#     if all(array[i] + 1 == array[i + 1] for i in range(len(array) - 1)):
-#         return array
-#     return None
-
-def range_func(input_str):
-    # Extract numbers from the input string and convert them to integers
-    numbers = [int(x) for x in regex.findall(r'\d+', input_str)]
-
-    # Check if the extracted list of numbers forms a continuous, ascending sequence
-    if len(numbers) == 2:
-        # If exactly two numbers, generate a range if they form a valid range
-        if numbers[0] < numbers[1]:
-            return list(range(numbers[0], numbers[1] + 1))
-    elif len(numbers) > 2:
-        # If more than two numbers, check if they form a continuous, ascending sequence
-        if all(numbers[i] + 1 == numbers[i + 1] for i in range(len(numbers) - 1)):
-            return numbers
-    else:
-        # Return the list as-is if it's a single number or empty
-        return numbers
-
-    # Return None if the sequence is not continuous or not just a single number
-    return None
-
-
-def year_range(input_value):
-    parts = regex.findall(r"\d+", input_value)
-    if not parts:
-        return None  # Return None if no numeric parts are found
-
-    try:
-        start = int(parts[0])
-        end = int(parts[1]) if len(parts) > 1 else None
-    except ValueError:
-        return None  # Return None if conversion to integer fails
-
-    if not end:
-        return str(start)  # If there's no end part, return the start as string
-
-    if end < 100:
-        end += start - start % 100  # Adjust for two-digit years
-
-    if end <= start:
-        return None  # If the end year is not after the start year, it's not a valid range
-
-    return f"{start}-{end}"
-
-
-def array(chain=None):
-    def inner(input_value):
-        return [chain(input_value) if chain else input_value]
-
-    return inner
-
-
-def uniq_concat(chain):
-    def inner(input, result=None):
-        if result is None:
-            result = []
-        value = chain(input)
-        if value not in result:
-            result.append(value)
-        return result
-
-    return inner
+import arrow
+import regex
+
+
+def none(input_value: str) -> str:
+    return input_value
+
+
+def value(val):
+    def inner(input_value, existing_value=None):
+        if isinstance(val, str) and isinstance(input_value, str):
+            return val.replace("$1", input_value)
+        return val
+
+    return inner
+
+
+def integer(input_value):
+    try:
+        return int(input_value)
+    except ValueError:
+        return None
+
+
+def boolean(*args, **kwargs):
+    return True
+
+
+def lowercase(input_value):
+    return input_value.lower()
+
+
+def uppercase(input_value):
+    return input_value.upper()
+
+month_mapping = {
+    r"\bJanu\b": "Jan",
+    r"\bFebr\b": "Feb",
+    r"\bMarc\b": "Mar",
+    r"\bApri\b": "Apr",
+    r"\bMay\b": "May",
+    r"\bJune\b": "Jun",
+    r"\bJuly\b": "Jul",
+    r"\bAugu\b": "Aug",
+    r"\bSept\b": "Sep",
+    r"\bOcto\b": "Oct",
+    r"\bNove\b": "Nov",
+    r"\bDece\b": "Dec",
+}
+
+
+def convert_months(date_str):
+    for month, shortened in month_mapping.items():
+        date_str = regex.sub(month, shortened, date_str, flags=regex.IGNORECASE)
+    return date_str
+
+def date(date_format):
+    def inner(input_value):
+        sanitized = regex.sub(r"\W+", " ", input_value).strip()
+        sanitized = convert_months(sanitized)
+        formats = [date_format] if not isinstance(date_format, list) else date_format
+        for fmt in formats:
+            try:
+                return arrow.get(sanitized, fmt).format("YYYY-MM-DD")
+            except ValueError as e:
+                print(f"Failed to parse date: {input_value} with format: {fmt}")
+                print(e)
+        return None
+
+    return inner
+
+
+# def range_func(input):
+#     array = [int(x) for x in regex.sub(r"\D+", " ", input).strip().split() if x.isdigit()]
+#     if len(array) == 2 and array[0] < array[1]:
+#         return list(range(array[0], array[1] + 1))
+#     if all(array[i] + 1 == array[i + 1] for i in range(len(array) - 1)):
+#         return array
+#     return None
+
+def range_func(input_str):
+    # Extract numbers from the input string and convert them to integers
+    numbers = [int(x) for x in regex.findall(r'\d+', input_str)]
+
+    # Check if the extracted list of numbers forms a continuous, ascending sequence
+    if len(numbers) == 2:
+        # If exactly two numbers, generate a range if they form a valid range
+        if numbers[0] < numbers[1]:
+            return list(range(numbers[0], numbers[1] + 1))
+    elif len(numbers) > 2:
+        # If more than two numbers, check if they form a continuous, ascending sequence
+        if all(numbers[i] + 1 == numbers[i + 1] for i in range(len(numbers) - 1)):
+            return numbers
+    else:
+        # Return the list as-is if it's a single number or empty
+        return numbers
+
+    # Return None if the sequence is not continuous or not just a single number
+    return None
+
+
+def year_range(input_value):
+    parts = regex.findall(r"\d+", input_value)
+    if not parts:
+        return None  # Return None if no numeric parts are found
+
+    try:
+        start = int(parts[0])
+        end = int(parts[1]) if len(parts) > 1 else None
+    except ValueError:
+        return None  # Return None if conversion to integer fails
+
+    if not end:
+        return str(start)  # If there's no end part, return the start as string
+
+    if end < 100:
+        end += start - start % 100  # Adjust for two-digit years
+
+    if end <= start:
+        return None  # If the end year is not after the start year, it's not a valid range
+
+    return f"{start}-{end}"
+
+
+def array(chain=None):
+    def inner(input_value):
+        return [chain(input_value) if chain else input_value]
+
+    return inner
+
+
+def uniq_concat(chain):
+    def inner(input, result=None):
+        if result is None:
+            result = []
+        value = chain(input)
+        if value not in result:
+            result.append(value)
+        return result
+
+    return inner
```

