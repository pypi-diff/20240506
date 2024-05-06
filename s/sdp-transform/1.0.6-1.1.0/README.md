# Comparing `tmp/sdp_transform-1.0.6.tar.gz` & `tmp/sdp_transform-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdp_transform-1.0.6.tar", max compression
+gzip compressed data, was "sdp_transform-1.1.0.tar", max compression
```

## Comparing `sdp_transform-1.0.6.tar` & `sdp_transform-1.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-06-24 11:30:55.940385 sdp_transform-1.0.6/LICENSE
--rw-r--r--   0        0        0      345 2023-06-24 11:31:18.163274 sdp_transform-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      113 2023-06-24 11:30:55.940674 sdp_transform-1.0.6/sdp_transform/__init__.py
--rw-r--r--   0        0        0       66 2023-06-24 11:31:50.012658 sdp_transform-1.0.6/sdp_transform/__version__.py
--rw-r--r--   0        0        0    18198 2023-06-24 11:30:55.940914 sdp_transform-1.0.6/sdp_transform/grammar.py
--rw-r--r--   0        0        0     3275 2023-06-24 11:30:55.941035 sdp_transform-1.0.6/sdp_transform/parser.py
--rw-r--r--   0        0        0     2796 2023-06-24 11:30:55.941111 sdp_transform-1.0.6/sdp_transform/writer.py
--rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 sdp_transform-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-06 02:57:30.581056 sdp_transform-1.1.0/LICENSE
+-rw-r--r--   0        0        0      345 2024-05-06 03:51:57.966775 sdp_transform-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      234 2024-05-06 03:23:38.450076 sdp_transform-1.1.0/sdp_transform/__init__.py
+-rw-r--r--   0        0        0       66 2024-05-06 03:25:51.038055 sdp_transform-1.1.0/sdp_transform/__version__.py
+-rw-r--r--   0        0        0    18550 2024-05-06 03:23:38.539643 sdp_transform-1.1.0/sdp_transform/grammar.py
+-rw-r--r--   0        0        0     3299 2024-05-06 03:14:41.183615 sdp_transform-1.1.0/sdp_transform/parser.py
+-rw-r--r--   0        0        0     2820 2024-05-06 03:07:43.183061 sdp_transform-1.1.0/sdp_transform/writer.py
+-rw-r--r--   0        0        0      649 1970-01-01 00:00:00.000000 sdp_transform-1.1.0/PKG-INFO
```

### Comparing `sdp_transform-1.0.6/LICENSE` & `sdp_transform-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sdp_transform-1.0.6/sdp_transform/grammar.py` & `sdp_transform-1.1.0/sdp_transform/grammar.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import re
 
 
 grammar = {
-    "v": [{"name": "version", "reg": "^(\d*)$"}],
+    "v": [{"name": "version", "reg": r"^(\d*)$"}],
     "o": [
         {
             # o=- 20518 0 IN IP4 203.0.113.1
             # NB: sessionId will be a String in most cases because it is huge
             "name": "origin",
-            "reg": "^(\S*) (\d*) (\d*) (\S*) IP(\d) (\S*)",
+            "reg": r"^(\S*) (\d*) (\d*) (\S*) IP(\d) (\S*)",
             "names": [
                 "username",
                 "sessionId",
                 "sessionVersion",
                 "netType",
                 "ipVer",
                 "address",
@@ -30,190 +30,196 @@
     "z": [{"name": "timezones"}],
     "r": [{"name": "repeats"}],  # TODO: this one can also be parsed properly
     # k: [{}], # outdated thing ignored
     "t": [
         {
             # t=0 0
             "name": "timing",
-            "reg": "^(\d*) (\d*)",
+            "reg": r"^(\d*) (\d*)",
             "names": ["start", "stop"],
             "format": "%d %d",
         }
     ],
     "c": [
         {
             # c=IN IP4 10.47.197.26
             "name": "connection",
-            "reg": "^IN IP(\d) (\S*)",
+            "reg": r"^IN IP(\d) (\S*)",
             "names": ["version", "ip"],
             "format": "IN IP%d %s",
         }
     ],
     "b": [
         {
             # b=AS:4000
             "push": "bandwidth",
-            "reg": "^(TIAS|AS|CT|RR|RS):(\d*)",
+            "reg": r"^(TIAS|AS|CT|RR|RS):(\d*)",
             "names": ["type", "limit"],
             "format": "%s:%s",
         }
     ],
     "m": [
         {
             # m=video 51744 RTP/AVP 126 97 98 34 31
             # NB: special - pushes to session
             # TODO: rtp/fmtp should be filtered by the payloads found here?
-            "reg": "^(\w*) (\d*) ([\w/]*)(?: (.*))?",
+            "reg": r"^(\w*) (\d*) ([\w/]*)(?: (.*))?",
             "names": ["type", "port", "protocol", "payloads"],
             "format": "%s %d %s %s",
         }
     ],
     "a": [
         {
             # a=rtpmap:110 opus/48000/2
             "push": "rtp",
-            "reg": "^rtpmap:(\d*) ([\w\-.]*)(?:\s*\/(\d*)(?:\s*\/(\S*))?)?",
+            "reg": r"^rtpmap:(\d*) ([\w\-.]*)(?:\s*\/(\d*)(?:\s*\/(\S*))?)?",
             "names": ["payload", "codec", "rate", "encoding"],
-            "format": lambda o: "rtpmap:%d %s/%s/%s"
-            if o.get("encoding") != None
-            else ("rtpmap:%d %s/%s" if o.get("rate") != None else "rtpmap:%d %s"),
+            "format": lambda o: (
+                "rtpmap:%d %s/%s/%s"
+                if o.get("encoding") is not None
+                else (
+                    "rtpmap:%d %s/%s" if o.get("rate") is not None else "rtpmap:%d %s"
+                )
+            ),
         },
         {
             # a=fmtp:108 profile-level-id=24;object=23;bitrate=64000
             # a=fmtp:111 minptime=10; useinbandfec=1
             "push": "fmtp",
-            "reg": "^fmtp:(\d*) ([\S| ]*)",
+            "reg": r"^fmtp:(\d*) ([\S| ]*)",
             "names": ["payload", "config"],
             "format": "fmtp:%d %s",
         },
         {
             # a=control:streamid=0
             "name": "control",
-            "reg": "^control:(.*)",
+            "reg": r"^control:(.*)",
             "format": "control:%s",
         },
         {
             # a=rtcp:65179 IN IP4 193.84.77.194
             "name": "rtcp",
-            "reg": "^rtcp:(\d*)(?: (\S*) IP(\d) (\S*))?",
+            "reg": r"^rtcp:(\d*)(?: (\S*) IP(\d) (\S*))?",
             "names": ["port", "netType", "ipVer", "address"],
-            "format": lambda o: "rtcp:%d %s IP%d %s"
-            if o.get("address") != None
-            else "rtcp:%d",
+            "format": lambda o: (
+                "rtcp:%d %s IP%d %s" if o.get("address") is not None else "rtcp:%d"
+            ),
         },
         {
             # a=rtcp-fb:98 trr-int 100
             "push": "rtcpFbTrrInt",
-            "reg": "^rtcp-fb:(\*|\d*) trr-int (\d*)",
+            "reg": r"^rtcp-fb:(\*|\d*) trr-int (\d*)",
             "names": ["payload", "value"],
             "format": "rtcp-fb:%s trr-int %d",
         },
         {
             # a=rtcp-fb:98 nack rpsi
             "push": "rtcpFb",
-            "reg": "^rtcp-fb:(\*|\d*) ([\w\-_]*)(?: ([\w\-_]*))?",
+            "reg": r"^rtcp-fb:(\*|\d*) ([\w\-_]*)(?: ([\w\-_]*))?",
             "names": ["payload", "type", "subtype"],
-            "format": lambda o: "rtcp-fb:%s %s %s"
-            if o.get("subtype") != None
-            else "rtcp-fb:%s %s",
+            "format": lambda o: (
+                "rtcp-fb:%s %s %s" if o.get("subtype") is not None else "rtcp-fb:%s %s"
+            ),
         },
         {
             # a=extmap:2 urn:ietf:params:rtp-hdrext:toffset
             # a=extmap:1/recvonly URI-gps-string
             # a=extmap:3 urn:ietf:params:rtp-hdrext:encrypt urn:ietf:params:rtp-hdrext:smpte-tc 25@600/24
             "push": "ext",
-            "reg": "^extmap:(\d+)(?:\/(\w+))?(?: (urn:ietf:params:rtp-hdrext:encrypt))? (\S*)(?: (\S*))?",
+            "reg": r"^extmap:(\d+)(?:\/(\w+))?(?: (urn:ietf:params:rtp-hdrext:encrypt))? (\S*)(?: (\S*))?",
             "names": ["value", "direction", "encrypt-uri", "uri", "config"],
             "format": lambda o: "extmap:%d"
-            + ("/%s" if o.get("direction") != None else "")
-            + (" %s" if o.get("encrypt-uri") != None else "")
+            + ("/%s" if o.get("direction") is not None else "")
+            + (" %s" if o.get("encrypt-uri") is not None else "")
             + " %s"
-            + (" %s" if o.get("config") != None else ""),
+            + (" %s" if o.get("config") is not None else ""),
         },
         {
             # a=extmap-allow-mixed
             "name": "extmapAllowMixed",
-            "reg": "^(extmap-allow-mixed)",
+            "reg": r"^(extmap-allow-mixed)",
         },
         {
             # a=crypto:1 AES_CM_128_HMAC_SHA1_80 inline:PS1uQCVeeCFCanVmcjkpPywjNWhcYD0mXXtxaVBR|2^20|1:32
             "push": "crypto",
-            "reg": "^crypto:(\d*) ([\w_]*) (\S*)(?: (\S*))?",
+            "reg": r"^crypto:(\d*) ([\w_]*) (\S*)(?: (\S*))?",
             "names": ["id", "suite", "config", "sessionConfig"],
-            "format": lambda o: "crypto:%d %s %s %s"
-            if o.get("sessionConfig") != None
-            else "crypto:%d %s %s",
+            "format": lambda o: (
+                "crypto:%d %s %s %s"
+                if o.get("sessionConfig") is not None
+                else "crypto:%d %s %s"
+            ),
         },
         {
             # a=setup:actpass
             "name": "setup",
-            "reg": "^setup:(\w*)",
+            "reg": r"^setup:(\w*)",
             "format": "setup:%s",
         },
         {
             # a=connection:new
             "name": "connectionType",
-            "reg": "^connection:(new|existing)",
+            "reg": r"^connection:(new|existing)",
             "format": "connection:%s",
         },
         {
             # a=msid:0c8b064d-d807-43b4-b434-f92a889d8587 98178685-d409-46e0-8e16-7ef0db0db64a
             "name": "msid",
-            "reg": "^msid:(.*)",
+            "reg": r"^msid:(.*)",
             "format": "msid:%s",
         },
         {
             # a=ptime:20
             "name": "ptime",
-            "reg": "^ptime:(\d*(?:\.\d*)*)",
+            "reg": r"^ptime:(\d*(?:\.\d*)*)",
             "format": lambda o: "ptime:%d" if isinstance(o, int) else "ptime:%g",
         },
         {
             # a=maxptime:60
             "name": "maxptime",
-            "reg": "^maxptime:(\d*(?:\.\d*)*)",
+            "reg": r"^maxptime:(\d*(?:\.\d*)*)",
             "format": "maxptime:%d",
         },
         {
             # a=sendrecv
             "name": "direction",
-            "reg": "^(sendrecv|recvonly|sendonly|inactive)",
+            "reg": r"^(sendrecv|recvonly|sendonly|inactive)",
         },
         {
             # a=ice-lite
             "name": "icelite",
-            "reg": "^(ice-lite)",
+            "reg": r"^(ice-lite)",
         },
         {
             # a=ice-ufrag:F7gI
             "name": "iceUfrag",
-            "reg": "^ice-ufrag:(\S*)",
+            "reg": r"^ice-ufrag:(\S*)",
             "format": "ice-ufrag:%s",
         },
         {
             # a=ice-pwd:x9cml/YzichV2+XlhiMu8g
             "name": "icePwd",
-            "reg": "^ice-pwd:(\S*)",
+            "reg": r"^ice-pwd:(\S*)",
             "format": "ice-pwd:%s",
         },
         {
             # a=fingerprint:SHA-1 00:11:22:33:44:55:66:77:88:99:AA:BB:CC:DD:EE:FF:00:11:22:33
             "name": "fingerprint",
-            "reg": "^fingerprint:(\S*) (\S*)",
+            "reg": r"^fingerprint:(\S*) (\S*)",
             "names": ["type", "hash"],
             "format": "fingerprint:%s %s",
         },
         {
             # a=candidate:0 1 UDP 2113667327 203.0.113.1 54400 typ host
-            # a=candidate:1162875081 1 udp 2113937151 192.168.34.75 60017 typ host generation 0 network-id 3 network-cost 10
-            # a=candidate:3289912957 2 udp 1845501695 193.84.77.194 60017 typ srflx raddr 192.168.34.75 rport 60017 generation 0 network-id 3 network-cost 10
-            # a=candidate:229815620 1 tcp 1518280447 192.168.150.19 60017 typ host tcpfield active generation 0 network-id 3 network-cost 10
-            # a=candidate:3289912957 2 tcp 1845501695 193.84.77.194 60017 typ srflx raddr 192.168.34.75 rport 60017 tcpfield passive generation 0 network-id 3 network-cost 10
+            # a=candidate:1162875081 1 udp 2113937151 192.168.34.75 60017 typ host generation 0 network-id 3 network-cost 10 # noqa
+            # a=candidate:3289912957 2 udp 1845501695 193.84.77.194 60017 typ srflx raddr 192.168.34.75 rport 60017 generation 0 network-id 3 network-cost 10 # noqa
+            # a=candidate:229815620 1 tcp 1518280447 192.168.150.19 60017 typ host tcpfield active generation 0 network-id 3 network-cost 10 # noqa
+            # a=candidate:3289912957 2 tcp 1845501695 193.84.77.194 60017 typ srflx raddr 192.168.34.75 rport 60017 tcpfield passive generation 0 network-id 3 network-cost 10 # noqa
             "push": "candidates",
-            "reg": "^candidate:(\S*) (\d*) (\S*) (\d*) (\S*) (\d*) typ (\S*)(?: raddr (\S*) rport (\d*))?(?: tcpfield (\S*))?(?: generation (\d*))?(?: network-id (\d*))?(?: network-cost (\d*))?",
+            "reg": r"^candidate:(\S*) (\d*) (\S*) (\d*) (\S*) (\d*) typ (\S*)(?: raddr (\S*) rport (\d*))?(?: tcpfield (\S*))?(?: generation (\d*))?(?: network-id (\d*))?(?: network-cost (\d*))?",  # noqa
             "names": [
                 "foundation",
                 "component",
                 "protocol",
                 "priority",
                 "ip",
                 "port",
@@ -222,268 +228,270 @@
                 "rport",
                 "tcptype",
                 "generation",
                 "network-id",
                 "network-cost",
             ],
             "format": lambda o: "candidate:%s %d %s %d %s %d typ %s"
-            + (" raddr %s rport %d" if o.get("raddr") != None else "")
-            + (" tcpfield %s" if o.get("tcptype") != None else "")
-            + (" generation %d" if o.get("generation") != None else "")
-            + (" network-id %d" if o.get("network-id") != None else "")
-            + (" network-cost %d" if o.get("network-cost") != None else ""),
+            + (" raddr %s rport %d" if o.get("raddr") is not None else "")
+            + (" tcpfield %s" if o.get("tcptype") is not None else "")
+            + (" generation %d" if o.get("generation") is not None else "")
+            + (" network-id %d" if o.get("network-id") is not None else "")
+            + (" network-cost %d" if o.get("network-cost") is not None else ""),
         },
         {
             # a=end-of-candidates (keep after the candidates line for readability)
             "name": "endOfCandidates",
-            "reg": "^(end-of-candidates)",
+            "reg": r"^(end-of-candidates)",
         },
         {
             # a=remote-candidates:1 203.0.113.1 54400 2 203.0.113.1 54401 ...
             "name": "remoteCandidates",
-            "reg": "^remote-candidates:(.*)",
+            "reg": r"^remote-candidates:(.*)",
             "format": "remote-candidates:%s",
         },
         {
             # a=ice-options:google-ice
             "name": "iceOptions",
-            "reg": "^ice-options:(\S*)",
+            "reg": r"^ice-options:(\S*)",
             "format": "ice-options:%s",
         },
         {
             # a=ssrc:2566107569 c'name':t9YU8M1UxTF8Y1A1
             "push": "ssrcs",
-            "reg": "^ssrc:(\d*) ([\w_-]*)(?::(.*))?",
+            "reg": r"^ssrc:(\d*) ([\w_-]*)(?::(.*))?",
             "names": ["id", "attribute", "value"],
             "format": lambda o: "ssrc:%d"
-            + (" %s" if o.get("attribute") != None else "")
-            + (":%s" if o.get("value") != None else ""),
+            + (" %s" if o.get("attribute") is not None else "")
+            + (":%s" if o.get("value") is not None else ""),
         },
         {
             # a=ssrc-group:FEC 1 2
             # a=ssrc-group:FEC-FR 3004364195 1080772241
             "push": "ssrcGroups",
             # token-char = %x21 / %x23-27 / %x2A-2B / %x2D-2E / %x30-39 / %x41-5A / %x5E-7E
-            "reg": "^ssrc-group:([\x21\x23\x24\x25\x26\x27\x2A\x2B\x2D\x2E\w]*) (.*)",
+            "reg": r"^ssrc-group:([\x21\x23\x24\x25\x26\x27\x2A\x2B\x2D\x2E\w]*) (.*)",
             "names": ["semantics", "ssrcs"],
             "format": "ssrc-group:%s %s",
         },
         {
             # a=msid-semantic: WMS Jvlam5X3SX1OP6pn20zWogvaKJz5Hjf9OnlV
             "name": "msidSemantic",
-            "reg": "^msid-semantic:\s?(\w*) (\S*)",
+            "reg": r"^msid-semantic:\s?(\w*) (\S*)",
             "names": ["semantic", "token"],
             "format": "msid-semantic: %s %s",  # space after ':' is not accidental
         },
         {
             # a=group:BUNDLE audio video
             "push": "groups",
-            "reg": "^group:(\w*) (.*)",
+            "reg": r"^group:(\w*) (.*)",
             "names": ["type", "mids"],
             "format": "group:%s %s",
         },
         {
             # a=rtcp-mux
             "name": "rtcpMux",
-            "reg": "^(rtcp-mux)",
+            "reg": r"^(rtcp-mux)",
         },
         {
             # a=rtcp-rsize
             "name": "rtcpRsize",
-            "reg": "^(rtcp-rsize)",
+            "reg": r"^(rtcp-rsize)",
         },
         {
             # a=sctpmap:5000 webrtc-datachannel 1024
             "name": "sctpmap",
-            "reg": "^sctpmap:([\w_/]*) (\S*)(?: (\S*))?",
+            "reg": r"^sctpmap:([\w_/]*) (\S*)(?: (\S*))?",
             "names": ["sctpmapNumber", "app", "maxMessageSize"],
-            "format": lambda o: "sctpmap:%s %s %s"
-            if o.get("maxMessageSize") != None
-            else "sctpmap:%s %s",
+            "format": lambda o: (
+                "sctpmap:%s %s %s"
+                if o.get("maxMessageSize") is not None
+                else "sctpmap:%s %s"
+            ),
         },
         {
             # a=x-google-flag:conference
             "name": "xGoogleFlag",
-            "reg": "^x-google-flag:([^\s]*)",
+            "reg": r"^x-google-flag:([^\s]*)",
             "format": "x-google-flag:%s",
         },
         {
             # a=rid:1 send max-width=1280;max-height=720;max-fps=30;depend=0
             "push": "rids",
-            "reg": "^rid:([\d\w]+) (\w+)(?: ([\S| ]*))?",
+            "reg": r"^rid:([\d\w]+) (\w+)(?: ([\S| ]*))?",
             "names": ["id", "direction", "params"],
-            "format": lambda o: "rid:%s %s %s"
-            if o.get("params") != None
-            else "rid:%s %s",
+            "format": lambda o: (
+                "rid:%s %s %s" if o.get("params") is not None else "rid:%s %s"
+            ),
         },
         {
             # a=imageattr:97 send [x=800,y=640,sar=1.1,q=0.6] [x=480,y=320] recv [x=330,y=250]
             # a=imageattr:* send [x=800,y=640] recv *
             # a=imageattr:100 recv [x=320,y=240]
             "push": "imageattrs",
             "reg": re.compile(
                 # a=imageattr:97
-                "^imageattr:(\\d+|\\*)"
+                r"^imageattr:(\d+|\*)"
                 +
                 # send [x=800,y=640,sar=1.1,q=0.6] [x=480,y=320]
-                "[\\s\\t]+(send|recv)[\\s\\t]+(\\*|\\[\\S+\\](?:[\\s\\t]+\\[\\S+\\])*)"
+                r"[\s\t]+(send|recv)[\s\t]+(\*|\[\S+\](?:[\s\t]+\[\S+\])*)"
                 +
                 # recv [x=330,y=250]
-                "(?:[\\s\\t]+(recv|send)[\\s\\t]+(\\*|\\[\\S+\\](?:[\\s\\t]+\\[\\S+\\])*))?"
+                r"(?:[\s\t]+(recv|send)[\s\t]+(\*|\[\S+\](?:[\s\t]+\[\S+\])*))?"
             ),
             "names": ["pt", "dir1", "attrs1", "dir2", "attrs2"],
             "format": lambda o: "imageattr:%s %s %s"
-            + (" %s %s" if o.get("dir2") != None else ""),
+            + (" %s %s" if o.get("dir2") is not None else ""),
         },
         {
             # a=simulcast:send 1,2,3;~4,~5 recv 6;~7,~8
             # a=simulcast:recv 1;4,5 send 6;7
             "name": "simulcast",
             "reg": re.compile(
                 # a=simulcast:
-                "^simulcast:"
+                r"^simulcast:"
                 +
                 # send 1,2,3;~4,~5
-                "(send|recv) ([a-zA-Z0-9\\-_~;,]+)"
+                r"(send|recv) ([a-zA-Z0-9\-_~;,]+)"
                 +
                 # space + recv 6;~7,~8
-                "(?:\\s?(send|recv) ([a-zA-Z0-9\\-_~;,]+))?"
+                r"(?:\s?(send|recv) ([a-zA-Z0-9\-_~;,]+))?"
                 +
                 # end
-                "$"
+                r"$"
             ),
             "names": ["dir1", "list1", "dir2", "list2"],
             "format": lambda o: "simulcast:%s %s"
-            + (" %s %s" if o.get("dir2") != None else ""),
+            + (" %s %s" if o.get("dir2") is not None else ""),
         },
         {
             # old simulcast draft 03 (implemented by Firefox)
             #   https://tools.ietf.org/html/draft-ietf-mmusic-sdp-simulcast-03
             # a=simulcast: recv pt=97;98 send pt=97
             # a=simulcast: send rid=5;6;7 paused=6,7
             "name": "simulcast_03",
-            "reg": "^simulcast:[\s\t]+([\S+\s\t]+)$",
+            "reg": r"^simulcast:[\s\t]+([\S+\s\t]+)$",
             "names": ["value"],
             "format": "simulcast: %s",
         },
         {
             # a=framerate:25
             # a=framerate:29.97
             "name": "framerate",
-            "reg": "^framerate:(\d+(?:$|\.\d+))",
+            "reg": r"^framerate:(\d+(?:$|\.\d+))",
             "format": "framerate:%s",
         },
         {
             # RFC4570
             # a=source-filter: incl IN IP4 239.5.2.31 10.1.15.5
             "name": "sourceFilter",
-            "reg": "^source-filter: *(excl|incl) (\S*) (IP4|IP6|\*) (\S*) (.*)",
+            "reg": r"^source-filter: *(excl|incl) (\S*) (IP4|IP6|\*) (\S*) (.*)",
             "names": [
                 "filterMode",
                 "netType",
                 "addressTypes",
                 "destAddress",
                 "srcList",
             ],
             "format": "source-filter: %s %s %s %s %s",
         },
         {
             # a=bundle-only
             "name": "bundleOnly",
-            "reg": "^(bundle-only)",
+            "reg": r"^(bundle-only)",
         },
         {
             # a=label:1
             "name": "label",
-            "reg": "^label:(.+)",
+            "reg": r"^label:(.+)",
             "format": "label:%s",
         },
         {
             # RFC version 26 for SCTP over DTLS
             # https://tools.ietf.org/html/draft-ietf-mmusic-sctp-sdp-26#section-5
             "name": "sctpPort",
-            "reg": "^sctp-port:(\d+)$",
+            "reg": r"^sctp-port:(\d+)$",
             "format": "sctp-port:%s",
         },
         {
             # RFC version 26 for SCTP over DTLS
             # https://tools.ietf.org/html/draft-ietf-mmusic-sctp-sdp-26#section-6
             "name": "maxMessageSize",
-            "reg": "^max-message-size:(\d+)$",
+            "reg": r"^max-message-size:(\d+)$",
             "format": "max-message-size:%s",
         },
         {
             # RFC7273
             # a=ts-refclk:ptp=IEEE1588-2008:39-A7-94-FF-FE-07-CB-D0:37
             "push": "tsRefClocks",
-            "reg": "^ts-refclk:([^\s=]*)(?:=(\S*))?",
+            "reg": r"^ts-refclk:([^\s=]*)(?:=(\S*))?",
             "names": ["clksrc", "clksrcExt"],
             "format": lambda o: "ts-refclk:%s"
-            + ("=%s" if o.get("clksrcExt") != None else ""),
+            + ("=%s" if o.get("clksrcExt") is not None else ""),
         },
         {
             # RFC7273
             # a=mediaclk:direct=963214424
             "name": "mediaClk",
-            "reg": "^mediaclk:(?:id=(\S*))? *([^\s=]*)(?:=(\S*))?(?: *rate=(\d+)\/(\d+))?",
+            "reg": r"^mediaclk:(?:id=(\S*))? *([^\s=]*)(?:=(\S*))?(?: *rate=(\d+)\/(\d+))?",
             "names": [
                 "id",
                 "mediaClockName",
                 "mediaClockValue",
                 "rateNumerator",
                 "rateDenominator",
             ],
             "format": lambda o: "mediaclk:"
-            + ("id=%s %s" if o.get("id") != None else "%s")
-            + ("=%s" if o.get("mediaClockValue") != None else "")
-            + (" rate=%s" if o.get("rateNumerator") != None else "")
-            + ("/%s" if o.get("rateDenominator") != None else ""),
+            + ("id=%s %s" if o.get("id") is not None else "%s")
+            + ("=%s" if o.get("mediaClockValue") is not None else "")
+            + (" rate=%s" if o.get("rateNumerator") is not None else "")
+            + ("/%s" if o.get("rateDenominator") is not None else ""),
         },
         {
             # a=keywds:keywords
             "name": "keywords",
-            "reg": "^keywds:(.+)$",
+            "reg": r"^keywds:(.+)$",
             "format": "keywds:%s",
         },
         {
             # a=content:main
             "name": "content",
-            "reg": "^content:(.+)",
+            "reg": r"^content:(.+)",
             "format": "content:%s",
         },
         # BFCP https://tools.ietf.org/html/rfc4583
         {
             # a=floorctrl:c-s
             "name": "bfcpFloorCtrl",
-            "reg": "^floorctrl:(c-only|s-only|c-s)",
+            "reg": r"^floorctrl:(c-only|s-only|c-s)",
             "format": "floorctrl:%s",
         },
         {
             # a=confid:1
             "name": "bfcpConfId",
-            "reg": "^confid:(\d+)",
+            "reg": r"^confid:(\d+)",
             "format": "confid:%s",
         },
         {
             # a=userid:1
             "name": "bfcpUserId",
-            "reg": "^userid:(\d+)",
+            "reg": r"^userid:(\d+)",
             "format": "userid:%s",
         },
         {
             # a=floorid:1
             "name": "bfcpFloorId",
-            "reg": "^floorid:(.+) (?:m-stream|mstrm):(.+)",
+            "reg": r"^floorid:(.+) (?:m-stream|mstrm):(.+)",
             "names": ["id", "mStream"],
             "format": "floorid:%s mstrm:%s",
         },
         {
             # a=mid:1
             "name": "mid",
-            "reg": "^mid:([^\s]*)",
+            "reg": r"^mid:([^\s]*)",
             "format": "mid:%s",
         },
         {
             # any a= that we don't understand is kept verbatim on media.invalid
             "push": "invalid",
             "names": ["value"],
         },
```

### Comparing `sdp_transform-1.0.6/sdp_transform/parser.py` & `sdp_transform-1.1.0/sdp_transform/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 
 def toIntIfInt(v):
     try:
         return int(v)
     except ValueError:
         try:
             return float(v)
-        except:
+        except ValueError:
             return v
 
 
 def attachProperties(match, location, names=None, rawName=None):
     if rawName and not names:
         location[rawName] = toIntIfInt(match[1])
     else:
         i = 0
         while i < len(names):
-            if match[i + 1] != None:
+            if match[i + 1] is not None:
                 location[names[i]] = toIntIfInt(match[i + 1])
             i += 1
     return
 
 
 def parseReg(obj, location, content):
     needsBlank = obj.get("name") and obj.get("names")
@@ -50,17 +50,17 @@
 
 
 def parse(sdp: str) -> dict:
     session = {}
     media = []
     location = session
     lines = [line for line in sdp.splitlines() if re.match(r"^([a-z])=(.*)", line)]
-    for l in lines:
-        field = l[0]
-        content = l[2:]
+    for line in lines:
+        field = line[0]
+        content = line[2:]
 
         if field == "m":
             media.append({"rtp": [], "fmtp": []})
             location = media[-1]
 
         for obj in grammar.get(field, []):
             if re.match(obj["reg"], content):
```

### Comparing `sdp_transform-1.0.6/sdp_transform/writer.py` & `sdp_transform-1.1.0/sdp_transform/writer.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,18 +11,18 @@
             else obj["format"]
         )
     )
     args = []
     if obj.get("names"):
         for name in obj.get("names"):
             if obj.get("name"):
-                if location[obj.get("name")].get(name) != None:
+                if location[obj.get("name")].get(name) is not None:
                     args.append(location[obj.get("name")][name])
             else:
-                if location.get(name) != None:
+                if location.get(name) is not None:
                     args.append(location[name])
     else:
         args.append(location[obj.get("name")])
 
     return string % tuple(args)
 
 
@@ -32,48 +32,48 @@
 
 
 def write(
     session: dict,
     outerOrder: list = defaultOuterOrder,
     innerOrder: list = defaultInnerOrder,
 ):
-    if session.get("version") == None:
+    if session.get("version") is None:
         session["version"] = 0  # 'v=0' must be there (only defined version atm)
-    if session.get("name") == None:
+    if session.get("name") is None:
         session["name"] = " "  # 's= ' must be there if no meaningful name set
 
     for media in session.get("media", []):
-        if media.get("payloads") == None:
+        if media.get("payloads") is None:
             media["payloads"] = ""
 
     sdp = []
 
     # loop through outerOrder for matching properties on session
     for field in outerOrder:
         for obj in grammar[field]:
             if obj.get("name"):
                 if obj["name"] in session.keys():
-                    if session.get(obj["name"]) != None:
+                    if session.get(obj["name"]) is not None:
                         sdp.append(makeLine(field, obj, session))
             elif obj.get("push"):
                 if obj["push"] in session.keys():
-                    if session.get(obj["push"]) != None:
+                    if session.get(obj["push"]) is not None:
                         for el in session.get(obj["push"]):
                             sdp.append(makeLine(field, obj, el))
 
     # then for each media line, follow the innerOrder
     for mLine in session.get("media", []):
         sdp.append(makeLine("m", grammar["m"][0], mLine))
 
         for field in innerOrder:
             for obj in grammar[field]:
                 if obj.get("name"):
                     if obj["name"] in mLine.keys():
-                        if mLine.get(obj["name"]) != None:
+                        if mLine.get(obj["name"]) is not None:
                             sdp.append(makeLine(field, obj, mLine))
                 elif obj.get("push"):
                     if obj["push"] in mLine.keys():
-                        if mLine.get(obj["push"]) != None:
+                        if mLine.get(obj["push"]) is not None:
                             for el in mLine.get(obj["push"]):
                                 sdp.append(makeLine(field, obj, el))
 
     return "\r\n".join([*sdp, ""])
```

### Comparing `sdp_transform-1.0.6/PKG-INFO` & `sdp_transform-1.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: sdp-transform
-Version: 1.0.6
+Version: 1.1.0
 Summary: A simple Python parser and writer of SDP.
 License: MIT
 Author: Jiang Yue
 Author-email: maze1024@gmail.com
 Requires-Python: >=3.6.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
```

