# Comparing `tmp/monobit-0.43.0.tar.gz` & `tmp/monobit-0.43.1.tar.gz`

## Comparing `monobit-0.43.0.tar` & `monobit-0.43.1.tar`

### file list

```diff
@@ -1,543 +1,544 @@
--rw-r--r--   0        0        0    27256 2020-02-02 00:00:00.000000 monobit-0.43.0/YAFF.md
--rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 monobit-0.43.0/banner.py
--rwxr-xr-x   0        0        0       71 2020-02-02 00:00:00.000000 monobit-0.43.0/convert.py
--rwxr-xr-x   0        0        0     7145 2020-02-02 00:00:00.000000 monobit-0.43.0/explore.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/__init__.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/constants.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/base/__init__.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/base/basetypes.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/base/binary.py
--rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/base/blocks.py
--rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/base/cachedprops.py
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/base/properties.py
--rw-r--r--   0        0        0     9488 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/base/struct.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/core/__init__.py
--rw-r--r--   0        0        0    51020 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/core/font.py
--rw-r--r--   0        0        0    33937 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/core/glyph.py
--rw-r--r--   0        0        0     9420 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/core/labels.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/core/pack.py
--rw-r--r--   0        0        0    22882 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/core/raster.py
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/core/vector.py
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/__init__.py
--rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/base.py
--rw-r--r--   0        0        0    18338 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/charmaps.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/definitions.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/indexers.py
--rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/registry.py
--rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/taggers.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/unicode.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/__init__.py
--rw-r--r--   0        0        0    51488 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/charmaps.json
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/adobe/README.md
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/adobe/ReadMe.txt
--rw-r--r--   0        0        0     8143 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/adobe/stdenc.txt
--rw-r--r--   0        0        0    10489 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/adobe/symbol.txt
--rw-r--r--   0        0        0    12033 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/adobe/zdingbat.txt
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/agl/LICENSE.md
--rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/agl/README.md
--rw-r--r--   0        0        0    27655 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/agl/aglfn.txt
--rw-r--r--   0        0        0    78060 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/agl/glyphlist.txt
--rw-r--r--   0        0        0    24830 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/ARABIC.TXT
--rw-r--r--   0        0        0    13008 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/CELTIC.TXT
--rw-r--r--   0        0        0    13065 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/CENTEURO.TXT
--rw-r--r--   0        0        0   197055 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/CHINSIMP.TXT
--rw-r--r--   0        0        0   323716 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/CHINTRAD.TXT
--rw-r--r--   0        0        0    26610 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/CORPCHAR.TXT
--rw-r--r--   0        0        0    13388 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/CROATIAN.TXT
--rw-r--r--   0        0        0    13497 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/CYRILLIC.TXT
--rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/DEVANAGA.TXT
--rw-r--r--   0        0        0    14320 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/DINGBATS.TXT
--rw-r--r--   0        0        0    23987 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/FARSI.TXT
--rw-r--r--   0        0        0    14055 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/GAELIC.TXT
--rw-r--r--   0        0        0    14042 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/GREEK.TXT
--rw-r--r--   0        0        0    13940 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/GUJARATI.TXT
--rw-r--r--   0        0        0    16096 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/GURMUKHI.TXT
--rw-r--r--   0        0        0    27034 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/HEBREW.TXT
--rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/ICELAND.TXT
--rw-r--r--   0        0        0    11800 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/INUIT.TXT
--rw-r--r--   0        0        0   198175 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/JAPANESE.TXT
--rw-r--r--   0        0        0    10252 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/KEYBOARD.TXT
--rw-r--r--   0        0        0   369061 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/KOREAN.TXT
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/README.md
--rw-r--r--   0        0        0    14385 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/ROMAN.TXT
--rw-r--r--   0        0        0    14153 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/ROMANIAN.TXT
--rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/ReadMe.txt
--rw-r--r--   0        0        0    16882 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/SYMBOL.TXT
--rw-r--r--   0        0        0    15564 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/THAI.TXT
--rw-r--r--   0        0        0    12808 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/TURKISH.TXT
--rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/apple/UKRAINE.TXT
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/czyborra/README.md
--rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/czyborra/bulgarian-mik.txt
--rw-r--r--   0        0        0     7866 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/czyborra/cp866.txt
--rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/czyborra/gost19768-87.txt
--rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/czyborra/hp-roman8.txt
--rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/czyborra/koi-0.txt
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/czyborra/koi-7.txt
--rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/czyborra/koi8-a.txt
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/czyborra/koi8-b.txt
--rw-r--r--   0        0        0     6374 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/czyborra/koi8-e.txt
--rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/czyborra/koi8-f.txt
--rw-r--r--   0        0        0     7801 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/czyborra/koi8-r.txt
--rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/czyborra/koi8-u.txt
--rw-r--r--   0        0        0    12047 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-ca
--rw-r--r--   0        0        0    12034 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-ca2
--rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-cn
--rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-cu
--rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-de
--rw-r--r--   0        0        0    11938 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-dk
--rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-es
--rw-r--r--   0        0        0    11888 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-es2
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-fr
--rw-r--r--   0        0        0    11847 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-gb
--rw-r--r--   0        0        0    11997 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-hu
--rw-r--r--   0        0        0    11926 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-it
--rw-r--r--   0        0        0    11841 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-jp
--rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-jp-ocr-b
--rw-r--r--   0        0        0    11773 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-kr
--rw-r--r--   0        0        0    11949 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-us
--rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-yu
--rw-r--r--   0        0        0    17534 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/jis_x0201
--rw-r--r--   0        0        0    10319 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/dkuug/x0201-7
--rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/emacs/MULE-ethiopic.map
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/emacs/MULE-ipa.map
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/emacs/MULE-is13194.map
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/emacs/MULE-lviscii.map
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/emacs/MULE-sisheng.map
--rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/emacs/MULE-tibetan.map
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/emacs/MULE-uviscii.map
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/emacs/README.md
--rw-r--r--   0        0        0    10137 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/evertype/ARMENIAN.TXT
--rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/evertype/GEORGIAN.TXT
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/evertype/README.md
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/1116.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/1117.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/1118.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/1119.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/1125.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/113.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/1131.ucp
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30000.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30001.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30002.ucp
--rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30003.ucp
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30004.ucp
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30005.ucp
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30006.ucp
--rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30007.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30008.ucp
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30009.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30010.ucp
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30011.ucp
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30012.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30013.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30014.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30015.ucp
--rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30016.ucp
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30017.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30018.ucp
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30019.ucp
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30020.ucp
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30021.ucp
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30022.ucp
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30023.ucp
--rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30024.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30025.ucp
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30026.ucp
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30027.ucp
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30028.ucp
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30029.ucp
--rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30030.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30031.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30032.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30033.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30034.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30039.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/30040.ucp
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/3012.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/3021.ucp
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/3845.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/3846.ucp
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/3848.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/437.ucp
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/57781.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/58152.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/58210.ucp
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/58335.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/59234.ucp
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/59829.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/60258.ucp
--rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/60853.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/61282.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/62306.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/667.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/668.ucp
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/737.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/770.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/771.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/772.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/773.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/774.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/775.ucp
--rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/777.ucp
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/778.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/790.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/808.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/848.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/849.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/850.ucp
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/851.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/852.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/853.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/855.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/856.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/857.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/858.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/859.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/860.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/861.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/862.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/863.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/864.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/865.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/866.ucp
--rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/867.ucp
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/869.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/872.ucp
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/895.ucp
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/899.ucp
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/991.ucp
--rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/freedos/README.md
--rw-r--r--   0        0        0     9255 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iana/Amiga-1251
--rw-r--r--   0        0        0    13371 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iana/PTCP154
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iana/README.md
--rw-r--r--   0        0        0    14491 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/ibm-cdra/037B34B0.UPMAP100
--rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/ibm-cdra/038834B0.UPMAP100
--rw-r--r--   0        0        0   323573 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/ibm-cdra/039E44B0.UPMAP101
--rw-r--r--   0        0        0   973501 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/ibm-cdra/039F34B0.UPMAP100
--rw-r--r--   0        0        0    17655 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/ibm-cdra/readme.txt
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/ibm-cdra/url
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/icu/README.md
--rw-r--r--   0        0        0   177606 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/icu/aix-KSC5601.1987_0-4.3.6.ucm
--rw-r--r--   0        0        0  1348868 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/icu/cns-11643-1992.ucm
--rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/icu/ibm-1125_P100-1997.ucm
--rw-r--r--   0        0        0   433127 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/icu/ibm-1375_P100-2008.ucm
--rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/icu/ibm-720_P100-1997.ucm
--rw-r--r--   0        0        0     5972 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/icu/ibm-806_P100-1998.ucm
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/icu/ibm-851_P100-1995.ucm
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/icu/ibm-858_P100-1997.ucm
--rw-r--r--   0        0        0     8451 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/icu/ibm-868_P100-1995.ucm
--rw-r--r--   0        0        0   199596 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/icu/ibm-932_P120-1999.ucm
--rw-r--r--   0        0        0   351895 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/icu/windows-1361-2000.ucm
--rw-r--r--   0        0        0   490901 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/icu/windows-936-2000.ucm
--rw-r--r--   0        0        0     9995 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-1.TXT
--rw-r--r--   0        0        0    10385 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-10.TXT
--rw-r--r--   0        0        0     9192 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-11.TXT
--rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-13.TXT
--rw-r--r--   0        0        0    10459 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-14.TXT
--rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-15.TXT
--rw-r--r--   0        0        0    10390 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-16.TXT
--rw-r--r--   0        0        0    10219 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-2.TXT
--rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-3.TXT
--rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-4.TXT
--rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-5.TXT
--rw-r--r--   0        0        0     7723 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-6.TXT
--rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-7.TXT
--rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-8.TXT
--rw-r--r--   0        0        0    10030 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-9.TXT
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/README.md
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/iso-8859/ReadMe.txt
--rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ADAMOS7.TXT
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ADAMSWTR.TXT
--rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/AMSCPC.TXT
--rw-r--r--   0        0        0    10266 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/AMSCPM.TXT
--rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/APL2ALT1.TXT
--rw-r--r--   0        0        0    10929 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/APL2ALT2.TXT
--rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/APL2ICHG.TXT
--rw-r--r--   0        0        0    11100 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/APL2PRIM.TXT
--rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ATARI8IG.TXT
--rw-r--r--   0        0        0    11148 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ATARI8II.TXT
--rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ATARI8VG.TXT
--rw-r--r--   0        0        0    12144 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ATARI8VI.TXT
--rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ATARISTI.TXT
--rw-r--r--   0        0        0     9561 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ATARISTV.TXT
--rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/C64IALT.TXT
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/C64IPRI.TXT
--rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/C64VALT.TXT
--rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/C64VPRI.TXT
--rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/COCOICHG.TXT
--rw-r--r--   0        0        0    11149 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/COCOSGR4.TXT
--rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/COCOSGR6.TXT
--rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/CPETIALT.TXT
--rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/CPETIPRI.TXT
--rw-r--r--   0        0        0    11521 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/CPETVALT.TXT
--rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/CPETVPRI.TXT
--rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/CVICIALT.TXT
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/CVICIPRI.TXT
--rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/CVICVALT.TXT
--rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/CVICVPRI.TXT
--rw-r--r--   0        0        0     8974 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/IBMPCICH.TXT
--rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/IBMPCVID.TXT
--rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/MINITLG0.TXT
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/MINITLG1.TXT
--rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/MSX.TXT
--rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ORICG0.TXT
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ORICG1.TXT
--rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/RISCEFF.TXT
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/RISCOSB.TXT
--rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/RISCOSI.TXT
--rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/RISCOSV.TXT
--rw-r--r--   0        0        0    14920 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ReadMe.txt
--rw-r--r--   0        0        0     9603 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/SINCLRQL.TXT
--rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TELTXTG0.TXT
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TELTXTG1.TXT
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TELTXTG2.TXT
--rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TELTXTG3.TXT
--rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TI994A.TXT
--rw-r--r--   0        0        0     5639 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM1ICH.TXT
--rw-r--r--   0        0        0     9089 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM1ORG.TXT
--rw-r--r--   0        0        0     9064 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM1REV.TXT
--rw-r--r--   0        0        0     7983 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM3IIN.TXT
--rw-r--r--   0        0        0     8497 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM3IJP.TXT
--rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM3IRV.TXT
--rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM3VIN.TXT
--rw-r--r--   0        0        0     9877 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM3VJP.TXT
--rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM3VRV.TXT
--rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM4AIA.TXT
--rw-r--r--   0        0        0     7974 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM4AIP.TXT
--rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM4AIR.TXT
--rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM4AVA.TXT
--rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM4AVP.TXT
--rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM4AVR.TXT
--rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZX80.TXT
--rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZX81.TXT
--rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZXDESKTP.TXT
--rw-r--r--   0        0        0     6617 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZXFZXKOI.TXT
--rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZXFZXLT1.TXT
--rw-r--r--   0        0        0     7590 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZXFZXLT5.TXT
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZXFZXPUA.TXT
--rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZXFZXSLT.TXT
--rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZXSPCTRM.TXT
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/README.md
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/c0-pictures.txt
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/currency-sign-0x9c.ucp
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/currency-sign-0xdb.ucp
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/dec-vt100.ucp
--rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/hp48.txt
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/ibm897graph.ucp
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/iso2047.txt
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/mac-cyrillic-pre9.0.ucp
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/mac-system.ucp
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/mac-ukrainian-pre9.0.ucp
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/russup3.ucp
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/russup4ac.ucp
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/russup4na.ucp
--rw-r--r--   0        0        0     7901 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/windows-1.0.txt
--rw-r--r--   0        0        0     8028 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/windows-2.0.txt
--rw-r--r--   0        0        0     9006 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/manual/windows-3.1.txt
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/README.md
--rw-r--r--   0        0        0     9000 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/EBCDIC/CP037.TXT
--rw-r--r--   0        0        0     9012 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/EBCDIC/CP1026.TXT
--rw-r--r--   0        0        0     9027 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/EBCDIC/CP500.TXT
--rw-r--r--   0        0        0     8721 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/EBCDIC/CP875.TXT
--rw-r--r--   0        0        0     9177 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/MAC/CYRILLIC.TXT
--rw-r--r--   0        0        0     9413 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/MAC/GREEK.TXT
--rw-r--r--   0        0        0     9253 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/MAC/ICELAND.TXT
--rw-r--r--   0        0        0     9862 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/MAC/LATIN2.TXT
--rw-r--r--   0        0        0     9229 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/MAC/ROMAN.TXT
--rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/MAC/TURKISH.TXT
--rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP437.TXT
--rw-r--r--   0        0        0     9827 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP737.TXT
--rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP775.TXT
--rw-r--r--   0        0        0     9640 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP850.TXT
--rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP852.TXT
--rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP855.TXT
--rw-r--r--   0        0        0     9617 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP857.TXT
--rw-r--r--   0        0        0     9845 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP860.TXT
--rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP861.TXT
--rw-r--r--   0        0        0     9396 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP862.TXT
--rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP863.TXT
--rw-r--r--   0        0        0     9560 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP864.TXT
--rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP865.TXT
--rw-r--r--   0        0        0     9765 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP866.TXT
--rw-r--r--   0        0        0     9318 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP869.TXT
--rw-r--r--   0        0        0     8452 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP874.TXT
--rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1250.TXT
--rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1251.TXT
--rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1252.TXT
--rw-r--r--   0        0        0     8938 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1253.TXT
--rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1254.TXT
--rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1255.TXT
--rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1256.TXT
--rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1257.TXT
--rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1258.TXT
--rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP874.TXT
--rw-r--r--   0        0        0   295324 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP932.TXT
--rw-r--r--   0        0        0   817310 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP936.TXT
--rw-r--r--   0        0        0   790736 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP949.TXT
--rw-r--r--   0        0        0   508978 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP950.TXT
--rw-r--r--   0        0        0    11537 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/APL-ISO-IR-68.TXT
--rw-r--r--   0        0        0    21171 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/ATARIST.TXT
--rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/CP1006.TXT
--rw-r--r--   0        0        0     8978 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/CP424.TXT
--rw-r--r--   0        0        0     9281 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/CP856.TXT
--rw-r--r--   0        0        0     8707 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/GSM0338.TXT
--rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/IBMGRAPH.TXT
--rw-r--r--   0        0        0   210734 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/JIS0208.TXT
--rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/KOI8-R.TXT
--rw-r--r--   0        0        0    11041 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/KOI8-U.TXT
--rw-r--r--   0        0        0   784637 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/KPS9566.TXT
--rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/KZ1048.TXT
--rw-r--r--   0        0        0     7093 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/NEXTSTEP.TXT
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/README.md
--rw-r--r--   0        0        0    49569 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/SGML.TXT
--rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/US-ASCII-QUOTES.TXT
--rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/dashen-map.txt
--rw-r--r--   0        0        0    92930 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/misc/ibm-ugl.txt
--rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/mleisher/ALTVAR.TXT
--rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/mleisher/ARMSCII-7.TXT
--rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/mleisher/ARMSCII-8.TXT
--rw-r--r--   0        0        0     9049 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/mleisher/ARMSCII-8A.TXT
--rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/mleisher/DECMCS.TXT
--rw-r--r--   0        0        0     9870 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/mleisher/GEO-ITA.TXT
--rw-r--r--   0        0        0     9758 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/mleisher/GEO-PS.TXT
--rw-r--r--   0        0        0    13439 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/mleisher/IRANSYSTEM.TXT
--rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/mleisher/KOI8RU.TXT
--rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/mleisher/OSNOVAR.TXT
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/mleisher/README.md
--rw-r--r--   0        0        0     9566 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/mleisher/TIS620.TXT
--rw-r--r--   0        0        0   274176 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/moztw/big5_2003-b2u.txt
--rw-r--r--   0        0        0   340277 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/moztw/eten.txt
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/moztw/url
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/python/README.md
--rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/python/TCVN5712-1.TXT
--rw-r--r--   0        0        0    10621 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/python/TCVN5712-2.TXT
--rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/python/TCVN5712-3.TXT
--rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/vietstd/unicode.html
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/vietstd/url
--rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/vietstd/viscii1.1.txt
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/README.md
--rw-r--r--   0        0        0   156347 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/abicomp.html
--rw-r--r--   0        0        0   180593 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/brascii.html
--rw-r--r--   0        0        0   144572 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/cp853.html
--rw-r--r--   0        0        0   156279 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/cwi2.html
--rw-r--r--   0        0        0   134679 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/dec-special.html
--rw-r--r--   0        0        0   153445 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/dec-technical.html
--rw-r--r--   0        0        0   192405 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/gem.html
--rw-r--r--   0        0        0   172501 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/kamenicky.html
--rw-r--r--   0        0        0   216297 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/lics.html
--rw-r--r--   0        0        0   150793 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/mattel-aquarius.html
--rw-r--r--   0        0        0   159296 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/mazovia.html
--rw-r--r--   0        0        0   167964 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/pascii.html
--rw-r--r--   0        0        0   217224 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/ventura.html
--rw-r--r--   0        0        0   254035 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/windows-1252.html
--rw-r--r--   0        0        0   245126 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/wingdings.html
--rw-r--r--   0        0        0   160779 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/wikipedia/wiscii.html
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/xfonts/README.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/xfonts/mulearabic-0.enc
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/xfonts/mulearabic-1.enc
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/xfonts/mulearabic-2.enc
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/xfonts/mulelao-1.enc
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/encoding/tables/xfonts/suneu-greek.enc
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/plumbing/__init__.py
--rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/plumbing/args.py
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/plumbing/help.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/plumbing/history.py
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/plumbing/scripting.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/render/__init__.py
--rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/render/chart.py
--rw-r--r--   0        0        0     6890 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/render/glyphmap.py
--rw-r--r--   0        0        0    13254 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/render/renderer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/scripts/__init__.py
--rwxr-xr-x   0        0        0     9536 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/scripts/banner.py
--rwxr-xr-x   0        0        0     3293 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/scripts/convert.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/__init__.py
--rw-r--r--   0        0        0    10443 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/converters.py
--rw-r--r--   0        0        0    10137 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/magic.py
--rw-r--r--   0        0        0     7817 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/streams.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/containers/__init__.py
--rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/containers/container.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/containers/directory.py
--rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/containers/tar.py
--rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/containers/zip.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/__init__.py
--rw-r--r--   0        0        0    14372 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/amiga.py
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/bbc.py
--rw-r--r--   0        0        0     9428 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/common.py
--rw-r--r--   0        0        0    22576 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/cpi.py
--rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/daisydot.py
--rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/dashen.py
--rw-r--r--   0        0        0    13377 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/dec.py
--rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/dosstart.py
--rw-r--r--   0        0        0    11173 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/figlet.py
--rw-r--r--   0        0        0     6163 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/fontx.py
--rw-r--r--   0        0        0    11297 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/fzx.py
--rw-r--r--   0        0        0    25615 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/gdos.py
--rw-r--r--   0        0        0    12651 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/geos.py
--rw-r--r--   0        0        0    10476 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/nearlyraw.py
--rw-r--r--   0        0        0    29873 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/pcl.py
--rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/pcpaint.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/pdf.py
--rw-r--r--   0        0        0    12842 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/pkfont.py
--rw-r--r--   0        0        0    10737 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/prebuilt.py
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/printshop.py
--rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/psf.py
--rw-r--r--   0        0        0     8611 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/raw.py
--rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/signum.py
--rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/vfont.py
--rw-r--r--   0        0        0    12487 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/xerox.py
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/apple/__init__.py
--rw-r--r--   0        0        0    21642 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/apple/dfont.py
--rw-r--r--   0        0        0    29326 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/apple/fond.py
--rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/apple/iigs.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/apple/lisa.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/apple/mgtk.py
--rw-r--r--   0        0        0    27670 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/apple/nfnt.py
--rw-r--r--   0        0        0     8335 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/apple/palm.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/fon/__init__.py
--rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/fon/fon.py
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/fon/mz.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/fon/os2/__init__.py
--rw-r--r--   0        0        0    21331 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/fon/os2/gpifont.py
--rw-r--r--   0        0        0    11075 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/fon/os2/lx.py
--rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/fon/os2/ne.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/fon/windows/LICENSE.md
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/fon/windows/__init__.py
--rw-r--r--   0        0        0    25636 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/fon/windows/fnt.py
--rw-r--r--   0        0        0    14238 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/fon/windows/ne.py
--rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/fon/windows/pe.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/image/__init__.py
--rw-r--r--   0        0        0    40795 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/image/bmfont.py
--rw-r--r--   0        0        0    10995 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/image/image.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/sfnt/__init__.py
--rw-r--r--   0        0        0    29213 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/sfnt/sfnt.py
--rw-r--r--   0        0        0    17626 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/sfnt/sfnt_writer.py
--rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/sfnt/fonttools/E_B_S_C_.py
--rw-r--r--   0        0        0     6239 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/sfnt/fonttools/__init__.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/sfnt/fonttools/_b_d_a_t.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/sfnt/fonttools/_b_h_e_d.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/sfnt/fonttools/_b_l_o_c.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/text/__init__.py
--rw-r--r--   0        0        0    17135 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/text/draw.py
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/text/edwin.py
--rw-r--r--   0        0        0     4608 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/text/hex.py
--rw-r--r--   0        0        0    14694 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/text/yaff.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/vector/__init__.py
--rw-r--r--   0        0        0     8053 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/vector/borland.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/vector/hurt.py
--rw-r--r--   0        0        0     8489 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/vector/svg.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/xlfd/__init__.py
--rw-r--r--   0        0        0    18342 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/xlfd/bdf.py
--rw-r--r--   0        0        0    18138 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/xlfd/hbf.py
--rw-r--r--   0        0        0    33850 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/xlfd/pcf.py
--rw-r--r--   0        0        0    25969 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/formats/xlfd/xlfd.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/wrappers/__init__.py
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/wrappers/apple.py
--rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/wrappers/binhex.py
--rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/wrappers/compressors.py
--rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/wrappers/macbinary.py
--rw-r--r--   0        0        0    15800 2020-02-02 00:00:00.000000 monobit-0.43.0/monobit/storage/wrappers/source.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 monobit-0.43.0/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 monobit-0.43.0/LICENSE
--rw-r--r--   0        0        0    18929 2020-02-02 00:00:00.000000 monobit-0.43.0/README.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 monobit-0.43.0/pyproject.toml
--rw-r--r--   0        0        0    20882 2020-02-02 00:00:00.000000 monobit-0.43.0/PKG-INFO
+-rw-r--r--   0        0        0    27256 2020-02-02 00:00:00.000000 monobit-0.43.1/YAFF.md
+-rwxr-xr-x   0        0        0       70 2020-02-02 00:00:00.000000 monobit-0.43.1/banner.py
+-rwxr-xr-x   0        0        0       71 2020-02-02 00:00:00.000000 monobit-0.43.1/convert.py
+-rwxr-xr-x   0        0        0     7145 2020-02-02 00:00:00.000000 monobit-0.43.1/explore.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/__init__.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/constants.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/base/__init__.py
+-rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/base/basetypes.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/base/binary.py
+-rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/base/blocks.py
+-rw-r--r--   0        0        0     3906 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/base/cachedprops.py
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/base/properties.py
+-rw-r--r--   0        0        0     9488 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/base/struct.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/core/__init__.py
+-rw-r--r--   0        0        0    51020 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/core/font.py
+-rw-r--r--   0        0        0    33937 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/core/glyph.py
+-rw-r--r--   0        0        0     9420 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/core/labels.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/core/pack.py
+-rw-r--r--   0        0        0    22882 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/core/raster.py
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/core/vector.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/__init__.py
+-rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/base.py
+-rw-r--r--   0        0        0    18338 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/charmaps.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/definitions.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/indexers.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/registry.py
+-rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/taggers.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/unicode.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/__init__.py
+-rw-r--r--   0        0        0    51488 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/charmaps.json
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/adobe/README.md
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/adobe/ReadMe.txt
+-rw-r--r--   0        0        0     8143 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/adobe/stdenc.txt
+-rw-r--r--   0        0        0    10489 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/adobe/symbol.txt
+-rw-r--r--   0        0        0    12033 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/adobe/zdingbat.txt
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/agl/LICENSE.md
+-rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/agl/README.md
+-rw-r--r--   0        0        0    27655 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/agl/aglfn.txt
+-rw-r--r--   0        0        0    78060 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/agl/glyphlist.txt
+-rw-r--r--   0        0        0    24830 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/ARABIC.TXT
+-rw-r--r--   0        0        0    13008 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/CELTIC.TXT
+-rw-r--r--   0        0        0    13065 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/CENTEURO.TXT
+-rw-r--r--   0        0        0   197055 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/CHINSIMP.TXT
+-rw-r--r--   0        0        0   323716 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/CHINTRAD.TXT
+-rw-r--r--   0        0        0    26610 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/CORPCHAR.TXT
+-rw-r--r--   0        0        0    13388 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/CROATIAN.TXT
+-rw-r--r--   0        0        0    13497 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/CYRILLIC.TXT
+-rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/DEVANAGA.TXT
+-rw-r--r--   0        0        0    14320 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/DINGBATS.TXT
+-rw-r--r--   0        0        0    23987 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/FARSI.TXT
+-rw-r--r--   0        0        0    14055 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/GAELIC.TXT
+-rw-r--r--   0        0        0    14042 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/GREEK.TXT
+-rw-r--r--   0        0        0    13940 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/GUJARATI.TXT
+-rw-r--r--   0        0        0    16096 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/GURMUKHI.TXT
+-rw-r--r--   0        0        0    27034 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/HEBREW.TXT
+-rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/ICELAND.TXT
+-rw-r--r--   0        0        0    11800 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/INUIT.TXT
+-rw-r--r--   0        0        0   198175 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/JAPANESE.TXT
+-rw-r--r--   0        0        0    10252 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/KEYBOARD.TXT
+-rw-r--r--   0        0        0   369061 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/KOREAN.TXT
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/README.md
+-rw-r--r--   0        0        0    14385 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/ROMAN.TXT
+-rw-r--r--   0        0        0    14153 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/ROMANIAN.TXT
+-rw-r--r--   0        0        0    28151 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/ReadMe.txt
+-rw-r--r--   0        0        0    16882 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/SYMBOL.TXT
+-rw-r--r--   0        0        0    15564 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/THAI.TXT
+-rw-r--r--   0        0        0    12808 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/TURKISH.TXT
+-rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/apple/UKRAINE.TXT
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/czyborra/README.md
+-rw-r--r--   0        0        0     7380 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/czyborra/bulgarian-mik.txt
+-rw-r--r--   0        0        0     7866 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/czyborra/cp866.txt
+-rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/czyborra/gost19768-87.txt
+-rw-r--r--   0        0        0     6552 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/czyborra/hp-roman8.txt
+-rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/czyborra/koi-0.txt
+-rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/czyborra/koi-7.txt
+-rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/czyborra/koi8-a.txt
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/czyborra/koi8-b.txt
+-rw-r--r--   0        0        0     6374 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/czyborra/koi8-e.txt
+-rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/czyborra/koi8-f.txt
+-rw-r--r--   0        0        0     7801 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/czyborra/koi8-r.txt
+-rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/czyborra/koi8-u.txt
+-rw-r--r--   0        0        0    12047 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-ca
+-rw-r--r--   0        0        0    12034 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-ca2
+-rw-r--r--   0        0        0    11838 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-cn
+-rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-cu
+-rw-r--r--   0        0        0    11978 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-de
+-rw-r--r--   0        0        0    11938 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-dk
+-rw-r--r--   0        0        0    11868 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-es
+-rw-r--r--   0        0        0    11888 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-es2
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-fr
+-rw-r--r--   0        0        0    11847 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-gb
+-rw-r--r--   0        0        0    11997 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-hu
+-rw-r--r--   0        0        0    11926 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-it
+-rw-r--r--   0        0        0    11841 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-jp
+-rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-jp-ocr-b
+-rw-r--r--   0        0        0    11773 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-kr
+-rw-r--r--   0        0        0    11949 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-us
+-rw-r--r--   0        0        0    12023 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-yu
+-rw-r--r--   0        0        0    17534 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/dkuug/jis_x0201
+-rw-r--r--   0        0        0    10319 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/dkuug/x0201-7
+-rw-r--r--   0        0        0     4900 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/emacs/MULE-ethiopic.map
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/emacs/MULE-ipa.map
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/emacs/MULE-is13194.map
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/emacs/MULE-lviscii.map
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/emacs/MULE-sisheng.map
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/emacs/MULE-tibetan.map
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/emacs/MULE-uviscii.map
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/emacs/README.md
+-rw-r--r--   0        0        0    10137 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/evertype/ARMENIAN.TXT
+-rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/evertype/GEORGIAN.TXT
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/evertype/README.md
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/1116.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/1117.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/1118.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/1119.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/1125.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/113.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/1131.ucp
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30000.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30001.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30002.ucp
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30003.ucp
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30004.ucp
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30005.ucp
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30006.ucp
+-rw-r--r--   0        0        0     2233 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30007.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30008.ucp
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30009.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30010.ucp
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30011.ucp
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30012.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30013.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30014.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30015.ucp
+-rw-r--r--   0        0        0     2794 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30016.ucp
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30017.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30018.ucp
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30019.ucp
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30020.ucp
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30021.ucp
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30022.ucp
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30023.ucp
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30024.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30025.ucp
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30026.ucp
+-rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30027.ucp
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30028.ucp
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30029.ucp
+-rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30030.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30031.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30032.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30033.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30034.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30039.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/30040.ucp
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/3012.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/3021.ucp
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/3845.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/3846.ucp
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/3848.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/437.ucp
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/57781.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/58152.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/58210.ucp
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/58335.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/59234.ucp
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/59829.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/60258.ucp
+-rw-r--r--   0        0        0     2189 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/60853.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/61282.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/62306.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/667.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/668.ucp
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/737.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/770.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/771.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/772.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/773.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/774.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/775.ucp
+-rw-r--r--   0        0        0     3970 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/777.ucp
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/778.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/790.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/808.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/848.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/849.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/850.ucp
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/851.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/852.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/853.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/855.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/856.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/857.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/858.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/859.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/860.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/861.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/862.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/863.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/864.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/865.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/866.ucp
+-rw-r--r--   0        0        0     2066 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/867.ucp
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/869.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/872.ucp
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/895.ucp
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/899.ucp
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/991.ucp
+-rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/freedos/README.md
+-rw-r--r--   0        0        0     9255 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/iana/Amiga-1251
+-rw-r--r--   0        0        0    13371 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/iana/PTCP154
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/iana/README.md
+-rw-r--r--   0        0        0    14491 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/ibm-cdra/037B34B0.UPMAP100
+-rw-r--r--   0        0        0    11755 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/ibm-cdra/038834B0.UPMAP100
+-rw-r--r--   0        0        0   323573 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/ibm-cdra/039E44B0.UPMAP101
+-rw-r--r--   0        0        0   973501 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/ibm-cdra/039F34B0.UPMAP100
+-rw-r--r--   0        0        0    17655 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/ibm-cdra/readme.txt
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/ibm-cdra/url
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/icu/README.md
+-rw-r--r--   0        0        0   177606 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/icu/aix-KSC5601.1987_0-4.3.6.ucm
+-rw-r--r--   0        0        0  1348868 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/icu/cns-11643-1992.ucm
+-rw-r--r--   0        0        0     7072 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/icu/ibm-1125_P100-1997.ucm
+-rw-r--r--   0        0        0   433127 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/icu/ibm-1375_P100-2008.ucm
+-rw-r--r--   0        0        0     6350 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/icu/ibm-720_P100-1997.ucm
+-rw-r--r--   0        0        0     5972 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/icu/ibm-806_P100-1998.ucm
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/icu/ibm-851_P100-1995.ucm
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/icu/ibm-858_P100-1997.ucm
+-rw-r--r--   0        0        0     8451 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/icu/ibm-868_P100-1995.ucm
+-rw-r--r--   0        0        0   199596 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/icu/ibm-932_P120-1999.ucm
+-rw-r--r--   0        0        0   351895 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/icu/windows-1361-2000.ucm
+-rw-r--r--   0        0        0   490901 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/icu/windows-936-2000.ucm
+-rw-r--r--   0        0        0     9995 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-1.TXT
+-rw-r--r--   0        0        0    10385 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-10.TXT
+-rw-r--r--   0        0        0     9192 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-11.TXT
+-rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-13.TXT
+-rw-r--r--   0        0        0    10459 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-14.TXT
+-rw-r--r--   0        0        0    10039 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-15.TXT
+-rw-r--r--   0        0        0    10390 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-16.TXT
+-rw-r--r--   0        0        0    10219 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-2.TXT
+-rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-3.TXT
+-rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-4.TXT
+-rw-r--r--   0        0        0     9830 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-5.TXT
+-rw-r--r--   0        0        0     7723 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-6.TXT
+-rw-r--r--   0        0        0    10053 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-7.TXT
+-rw-r--r--   0        0        0     7943 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-8.TXT
+-rw-r--r--   0        0        0    10030 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-9.TXT
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/iso-8859/README.md
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/iso-8859/ReadMe.txt
+-rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/ADAMOS7.TXT
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/ADAMSWTR.TXT
+-rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/AMSCPC.TXT
+-rw-r--r--   0        0        0    10266 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/AMSCPM.TXT
+-rw-r--r--   0        0        0    10898 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/APL2ALT1.TXT
+-rw-r--r--   0        0        0    10929 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/APL2ALT2.TXT
+-rw-r--r--   0        0        0     6461 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/APL2ICHG.TXT
+-rw-r--r--   0        0        0    11100 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/APL2PRIM.TXT
+-rw-r--r--   0        0        0    10985 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/ATARI8IG.TXT
+-rw-r--r--   0        0        0    11148 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/ATARI8II.TXT
+-rw-r--r--   0        0        0    11734 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/ATARI8VG.TXT
+-rw-r--r--   0        0        0    12144 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/ATARI8VI.TXT
+-rw-r--r--   0        0        0     8280 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/ATARISTI.TXT
+-rw-r--r--   0        0        0     9561 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/ATARISTV.TXT
+-rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/C64IALT.TXT
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/C64IPRI.TXT
+-rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/C64VALT.TXT
+-rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/C64VPRI.TXT
+-rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/COCOICHG.TXT
+-rw-r--r--   0        0        0    11149 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/COCOSGR4.TXT
+-rw-r--r--   0        0        0     4792 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/COCOSGR6.TXT
+-rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/CPETIALT.TXT
+-rw-r--r--   0        0        0     7797 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/CPETIPRI.TXT
+-rw-r--r--   0        0        0    11521 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/CPETVALT.TXT
+-rw-r--r--   0        0        0    12016 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/CPETVPRI.TXT
+-rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/CVICIALT.TXT
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/CVICIPRI.TXT
+-rw-r--r--   0        0        0    11514 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/CVICVALT.TXT
+-rw-r--r--   0        0        0    12009 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/CVICVPRI.TXT
+-rw-r--r--   0        0        0     8974 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/IBMPCICH.TXT
+-rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/IBMPCVID.TXT
+-rw-r--r--   0        0        0     6045 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/MINITLG0.TXT
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/MINITLG1.TXT
+-rw-r--r--   0        0        0     9910 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/MSX.TXT
+-rw-r--r--   0        0        0     3292 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/ORICG0.TXT
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/ORICG1.TXT
+-rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/RISCEFF.TXT
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/RISCOSB.TXT
+-rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/RISCOSI.TXT
+-rw-r--r--   0        0        0    10499 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/RISCOSV.TXT
+-rw-r--r--   0        0        0    14920 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/ReadMe.txt
+-rw-r--r--   0        0        0     9603 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/SINCLRQL.TXT
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/TELTXTG0.TXT
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/TELTXTG1.TXT
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/TELTXTG2.TXT
+-rw-r--r--   0        0        0     6062 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/TELTXTG3.TXT
+-rw-r--r--   0        0        0     3825 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/TI994A.TXT
+-rw-r--r--   0        0        0     5639 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM1ICH.TXT
+-rw-r--r--   0        0        0     9089 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM1ORG.TXT
+-rw-r--r--   0        0        0     9064 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM1REV.TXT
+-rw-r--r--   0        0        0     7983 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM3IIN.TXT
+-rw-r--r--   0        0        0     8497 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM3IJP.TXT
+-rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM3IRV.TXT
+-rw-r--r--   0        0        0     9363 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM3VIN.TXT
+-rw-r--r--   0        0        0     9877 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM3VJP.TXT
+-rw-r--r--   0        0        0    11778 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM3VRV.TXT
+-rw-r--r--   0        0        0     8379 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM4AIA.TXT
+-rw-r--r--   0        0        0     7974 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM4AIP.TXT
+-rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM4AIR.TXT
+-rw-r--r--   0        0        0     9808 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM4AVA.TXT
+-rw-r--r--   0        0        0     9402 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM4AVP.TXT
+-rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM4AVR.TXT
+-rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/ZX80.TXT
+-rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/ZX81.TXT
+-rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/ZXDESKTP.TXT
+-rw-r--r--   0        0        0     6617 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/ZXFZXKOI.TXT
+-rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/ZXFZXLT1.TXT
+-rw-r--r--   0        0        0     7590 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/ZXFZXLT5.TXT
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/ZXFZXPUA.TXT
+-rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/ZXFZXSLT.TXT
+-rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/kreativekorp/ZXSPCTRM.TXT
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/manual/README.md
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/manual/c0-pictures.txt
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/manual/currency-sign-0x9c.ucp
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/manual/currency-sign-0xdb.ucp
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/manual/dec-vt100.ucp
+-rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/manual/hp48.txt
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/manual/ibm897graph.ucp
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/manual/iso2047.txt
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/manual/mac-cyrillic-pre9.0.ucp
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/manual/mac-system.ucp
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/manual/mac-ukrainian-pre9.0.ucp
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/manual/russup3.ucp
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/manual/russup4ac.ucp
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/manual/russup4na.ucp
+-rw-r--r--   0        0        0     7901 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/manual/windows-1.0.txt
+-rw-r--r--   0        0        0     8028 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/manual/windows-2.0.txt
+-rw-r--r--   0        0        0     9006 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/manual/windows-3.1.txt
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/README.md
+-rw-r--r--   0        0        0     9000 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/EBCDIC/CP037.TXT
+-rw-r--r--   0        0        0     9012 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/EBCDIC/CP1026.TXT
+-rw-r--r--   0        0        0     9027 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/EBCDIC/CP500.TXT
+-rw-r--r--   0        0        0     8721 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/EBCDIC/CP875.TXT
+-rw-r--r--   0        0        0     9177 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/MAC/CYRILLIC.TXT
+-rw-r--r--   0        0        0     9413 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/MAC/GREEK.TXT
+-rw-r--r--   0        0        0     9253 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/MAC/ICELAND.TXT
+-rw-r--r--   0        0        0     9862 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/MAC/LATIN2.TXT
+-rw-r--r--   0        0        0     9229 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/MAC/ROMAN.TXT
+-rw-r--r--   0        0        0     9251 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/MAC/TURKISH.TXT
+-rw-r--r--   0        0        0     9794 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP437.TXT
+-rw-r--r--   0        0        0     9827 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP737.TXT
+-rw-r--r--   0        0        0     9766 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP775.TXT
+-rw-r--r--   0        0        0     9640 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP850.TXT
+-rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP852.TXT
+-rw-r--r--   0        0        0     9562 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP855.TXT
+-rw-r--r--   0        0        0     9617 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP857.TXT
+-rw-r--r--   0        0        0     9845 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP860.TXT
+-rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP861.TXT
+-rw-r--r--   0        0        0     9396 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP862.TXT
+-rw-r--r--   0        0        0     9693 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP863.TXT
+-rw-r--r--   0        0        0     9560 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP864.TXT
+-rw-r--r--   0        0        0     9812 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP865.TXT
+-rw-r--r--   0        0        0     9765 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP866.TXT
+-rw-r--r--   0        0        0     9318 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP869.TXT
+-rw-r--r--   0        0        0     8452 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP874.TXT
+-rw-r--r--   0        0        0     9530 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/WINDOWS/CP1250.TXT
+-rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/WINDOWS/CP1251.TXT
+-rw-r--r--   0        0        0     9355 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/WINDOWS/CP1252.TXT
+-rw-r--r--   0        0        0     8938 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/WINDOWS/CP1253.TXT
+-rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/WINDOWS/CP1254.TXT
+-rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/WINDOWS/CP1255.TXT
+-rw-r--r--   0        0        0     8657 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/WINDOWS/CP1256.TXT
+-rw-r--r--   0        0        0     9218 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/WINDOWS/CP1257.TXT
+-rw-r--r--   0        0        0     9208 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/WINDOWS/CP1258.TXT
+-rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/WINDOWS/CP874.TXT
+-rw-r--r--   0        0        0   295324 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/WINDOWS/CP932.TXT
+-rw-r--r--   0        0        0   817310 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/WINDOWS/CP936.TXT
+-rw-r--r--   0        0        0   790736 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/WINDOWS/CP949.TXT
+-rw-r--r--   0        0        0   508978 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/microsoft/WINDOWS/CP950.TXT
+-rw-r--r--   0        0        0    11537 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/misc/APL-ISO-IR-68.TXT
+-rw-r--r--   0        0        0    21171 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/misc/ATARIST.TXT
+-rw-r--r--   0        0        0    10895 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/misc/CP1006.TXT
+-rw-r--r--   0        0        0     8978 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/misc/CP424.TXT
+-rw-r--r--   0        0        0     9281 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/misc/CP856.TXT
+-rw-r--r--   0        0        0     8707 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/misc/GSM0338.TXT
+-rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/misc/IBMGRAPH.TXT
+-rw-r--r--   0        0        0   210734 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/misc/JIS0208.TXT
+-rw-r--r--   0        0        0    10692 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/misc/KOI8-R.TXT
+-rw-r--r--   0        0        0    11041 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/misc/KOI8-U.TXT
+-rw-r--r--   0        0        0   784637 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/misc/KPS9566.TXT
+-rw-r--r--   0        0        0    10532 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/misc/KZ1048.TXT
+-rw-r--r--   0        0        0     7093 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/misc/NEXTSTEP.TXT
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/misc/README.md
+-rw-r--r--   0        0        0    49569 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/misc/SGML.TXT
+-rw-r--r--   0        0        0     7054 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/misc/US-ASCII-QUOTES.TXT
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/misc/dashen-map.txt
+-rw-r--r--   0        0        0    92930 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/misc/ibm-ugl.txt
+-rw-r--r--   0        0        0     9996 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/mleisher/ALTVAR.TXT
+-rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/mleisher/ARMSCII-7.TXT
+-rw-r--r--   0        0        0     8606 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/mleisher/ARMSCII-8.TXT
+-rw-r--r--   0        0        0     9049 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/mleisher/ARMSCII-8A.TXT
+-rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/mleisher/DECMCS.TXT
+-rw-r--r--   0        0        0     9870 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/mleisher/GEO-ITA.TXT
+-rw-r--r--   0        0        0     9758 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/mleisher/GEO-PS.TXT
+-rw-r--r--   0        0        0    13439 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/mleisher/IRANSYSTEM.TXT
+-rw-r--r--   0        0        0    10796 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/mleisher/KOI8RU.TXT
+-rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/mleisher/OSNOVAR.TXT
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/mleisher/README.md
+-rw-r--r--   0        0        0     9566 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/mleisher/TIS620.TXT
+-rw-r--r--   0        0        0   274176 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/moztw/big5_2003-b2u.txt
+-rw-r--r--   0        0        0   340277 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/moztw/eten.txt
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/moztw/url
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/python/README.md
+-rw-r--r--   0        0        0    11789 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/python/TCVN5712-1.TXT
+-rw-r--r--   0        0        0    10621 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/python/TCVN5712-2.TXT
+-rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/python/TCVN5712-3.TXT
+-rw-r--r--   0        0        0    10088 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/vietstd/unicode.html
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/vietstd/url
+-rw-r--r--   0        0        0     7055 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/vietstd/viscii1.1.txt
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/wikipedia/README.md
+-rw-r--r--   0        0        0   156347 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/wikipedia/abicomp.html
+-rw-r--r--   0        0        0   180593 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/wikipedia/brascii.html
+-rw-r--r--   0        0        0   144572 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/wikipedia/cp853.html
+-rw-r--r--   0        0        0   156279 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/wikipedia/cwi2.html
+-rw-r--r--   0        0        0   134679 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/wikipedia/dec-special.html
+-rw-r--r--   0        0        0   153445 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/wikipedia/dec-technical.html
+-rw-r--r--   0        0        0   192405 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/wikipedia/gem.html
+-rw-r--r--   0        0        0   172501 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/wikipedia/kamenicky.html
+-rw-r--r--   0        0        0   216297 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/wikipedia/lics.html
+-rw-r--r--   0        0        0   150793 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/wikipedia/mattel-aquarius.html
+-rw-r--r--   0        0        0   159296 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/wikipedia/mazovia.html
+-rw-r--r--   0        0        0   167964 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/wikipedia/pascii.html
+-rw-r--r--   0        0        0   217224 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/wikipedia/ventura.html
+-rw-r--r--   0        0        0   254035 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/wikipedia/windows-1252.html
+-rw-r--r--   0        0        0   245126 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/wikipedia/wingdings.html
+-rw-r--r--   0        0        0   160779 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/wikipedia/wiscii.html
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/xfonts/README.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/xfonts/mulearabic-0.enc
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/xfonts/mulearabic-1.enc
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/xfonts/mulearabic-2.enc
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/xfonts/mulelao-1.enc
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/encoding/tables/xfonts/suneu-greek.enc
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/plumbing/__init__.py
+-rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/plumbing/args.py
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/plumbing/help.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/plumbing/history.py
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/plumbing/scripting.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/render/__init__.py
+-rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/render/chart.py
+-rw-r--r--   0        0        0     6890 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/render/glyphmap.py
+-rw-r--r--   0        0        0    13254 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/render/renderer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/scripts/__init__.py
+-rwxr-xr-x   0        0        0     9536 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/scripts/banner.py
+-rwxr-xr-x   0        0        0     3293 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/scripts/convert.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/__init__.py
+-rw-r--r--   0        0        0    10443 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/converters.py
+-rw-r--r--   0        0        0    10137 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/magic.py
+-rw-r--r--   0        0        0     7817 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/streams.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/containers/__init__.py
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/containers/container.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/containers/directory.py
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/containers/tar.py
+-rw-r--r--   0        0        0     3780 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/containers/zip.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/__init__.py
+-rw-r--r--   0        0        0    14372 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/amiga.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/bbc.py
+-rw-r--r--   0        0        0     9428 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/common.py
+-rw-r--r--   0        0        0    22576 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/cpi.py
+-rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/daisydot.py
+-rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/dashen.py
+-rw-r--r--   0        0        0    13377 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/dec.py
+-rw-r--r--   0        0        0     3975 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/dosstart.py
+-rw-r--r--   0        0        0    11173 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/figlet.py
+-rw-r--r--   0        0        0     6163 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/fontx.py
+-rw-r--r--   0        0        0    11297 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/fzx.py
+-rw-r--r--   0        0        0    25615 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/gdos.py
+-rw-r--r--   0        0        0    12651 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/geos.py
+-rw-r--r--   0        0        0    10476 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/nearlyraw.py
+-rw-r--r--   0        0        0    29873 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/pcl.py
+-rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/pcpaint.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/pdf.py
+-rw-r--r--   0        0        0    12842 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/pkfont.py
+-rw-r--r--   0        0        0    10737 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/prebuilt.py
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/printshop.py
+-rw-r--r--   0        0        0     5712 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/psf.py
+-rw-r--r--   0        0        0     8611 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/raw.py
+-rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/signum.py
+-rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/vfont.py
+-rw-r--r--   0        0        0    12487 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/xerox.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/apple/__init__.py
+-rw-r--r--   0        0        0    21642 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/apple/dfont.py
+-rw-r--r--   0        0        0    29326 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/apple/fond.py
+-rw-r--r--   0        0        0     5472 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/apple/iigs.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/apple/lisa.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/apple/mgtk.py
+-rw-r--r--   0        0        0    27670 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/apple/nfnt.py
+-rw-r--r--   0        0        0     8335 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/apple/palm.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/fon/__init__.py
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/fon/fon.py
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/fon/mz.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/fon/os2/__init__.py
+-rw-r--r--   0        0        0    21331 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/fon/os2/gpifont.py
+-rw-r--r--   0        0        0    11075 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/fon/os2/lx.py
+-rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/fon/os2/ne.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/fon/windows/LICENSE.md
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/fon/windows/__init__.py
+-rw-r--r--   0        0        0    25636 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/fon/windows/fnt.py
+-rw-r--r--   0        0        0    14238 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/fon/windows/ne.py
+-rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/fon/windows/pe.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/image/__init__.py
+-rw-r--r--   0        0        0    40795 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/image/bmfont.py
+-rw-r--r--   0        0        0    10995 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/image/image.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/sfnt/__init__.py
+-rw-r--r--   0        0        0    29213 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/sfnt/sfnt.py
+-rw-r--r--   0        0        0    17626 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/sfnt/sfnt_writer.py
+-rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/sfnt/fonttools/E_B_S_C_.py
+-rw-r--r--   0        0        0     6239 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/sfnt/fonttools/__init__.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/sfnt/fonttools/_b_d_a_t.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/sfnt/fonttools/_b_h_e_d.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/sfnt/fonttools/_b_l_o_c.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/text/__init__.py
+-rw-r--r--   0        0        0    17135 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/text/draw.py
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/text/edwin.py
+-rw-r--r--   0        0        0     4608 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/text/hex.py
+-rw-r--r--   0        0        0    14694 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/text/yaff.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/vector/__init__.py
+-rw-r--r--   0        0        0     8053 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/vector/borland.py
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/vector/gimms.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/vector/hurt.py
+-rw-r--r--   0        0        0     8489 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/vector/svg.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/xlfd/__init__.py
+-rw-r--r--   0        0        0    18342 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/xlfd/bdf.py
+-rw-r--r--   0        0        0    18138 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/xlfd/hbf.py
+-rw-r--r--   0        0        0    33850 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/xlfd/pcf.py
+-rw-r--r--   0        0        0    25969 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/formats/xlfd/xlfd.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/wrappers/__init__.py
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/wrappers/apple.py
+-rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/wrappers/binhex.py
+-rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/wrappers/compressors.py
+-rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/wrappers/macbinary.py
+-rw-r--r--   0        0        0    15800 2020-02-02 00:00:00.000000 monobit-0.43.1/monobit/storage/wrappers/source.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 monobit-0.43.1/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 monobit-0.43.1/LICENSE
+-rw-r--r--   0        0        0    19009 2020-02-02 00:00:00.000000 monobit-0.43.1/README.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 monobit-0.43.1/pyproject.toml
+-rw-r--r--   0        0        0    20962 2020-02-02 00:00:00.000000 monobit-0.43.1/PKG-INFO
```

### Comparing `monobit-0.43.0/YAFF.md` & `monobit-0.43.1/YAFF.md`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/explore.py` & `monobit-0.43.1/explore.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/__init__.py` & `monobit-0.43.1/monobit/__init__.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/base/__init__.py` & `monobit-0.43.1/monobit/base/__init__.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/base/basetypes.py` & `monobit-0.43.1/monobit/base/basetypes.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/base/binary.py` & `monobit-0.43.1/monobit/base/binary.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/base/blocks.py` & `monobit-0.43.1/monobit/base/blocks.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/base/cachedprops.py` & `monobit-0.43.1/monobit/base/cachedprops.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/base/properties.py` & `monobit-0.43.1/monobit/base/properties.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/base/struct.py` & `monobit-0.43.1/monobit/base/struct.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/core/font.py` & `monobit-0.43.1/monobit/core/font.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/core/glyph.py` & `monobit-0.43.1/monobit/core/glyph.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/core/labels.py` & `monobit-0.43.1/monobit/core/labels.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/core/pack.py` & `monobit-0.43.1/monobit/core/pack.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/core/raster.py` & `monobit-0.43.1/monobit/core/raster.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/core/vector.py` & `monobit-0.43.1/monobit/core/vector.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/__init__.py` & `monobit-0.43.1/monobit/encoding/__init__.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/base.py` & `monobit-0.43.1/monobit/encoding/base.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/charmaps.py` & `monobit-0.43.1/monobit/encoding/charmaps.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/definitions.py` & `monobit-0.43.1/monobit/encoding/definitions.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/indexers.py` & `monobit-0.43.1/monobit/encoding/indexers.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/registry.py` & `monobit-0.43.1/monobit/encoding/registry.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/taggers.py` & `monobit-0.43.1/monobit/encoding/taggers.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/unicode.py` & `monobit-0.43.1/monobit/encoding/unicode.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/charmaps.json` & `monobit-0.43.1/monobit/encoding/tables/charmaps.json`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/adobe/ReadMe.txt` & `monobit-0.43.1/monobit/encoding/tables/adobe/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/adobe/stdenc.txt` & `monobit-0.43.1/monobit/encoding/tables/adobe/stdenc.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/adobe/symbol.txt` & `monobit-0.43.1/monobit/encoding/tables/adobe/symbol.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/adobe/zdingbat.txt` & `monobit-0.43.1/monobit/encoding/tables/adobe/zdingbat.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/agl/LICENSE.md` & `monobit-0.43.1/monobit/encoding/tables/agl/LICENSE.md`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/agl/README.md` & `monobit-0.43.1/monobit/encoding/tables/agl/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/agl/aglfn.txt` & `monobit-0.43.1/monobit/encoding/tables/agl/aglfn.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/agl/glyphlist.txt` & `monobit-0.43.1/monobit/encoding/tables/agl/glyphlist.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/apple/ARABIC.TXT` & `monobit-0.43.1/monobit/encoding/tables/apple/ARABIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/apple/CELTIC.TXT` & `monobit-0.43.1/monobit/encoding/tables/apple/CELTIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/apple/CENTEURO.TXT` & `monobit-0.43.1/monobit/encoding/tables/apple/CENTEURO.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/apple/CHINSIMP.TXT` & `monobit-0.43.1/monobit/encoding/tables/apple/CHINSIMP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/apple/CHINTRAD.TXT` & `monobit-0.43.1/monobit/encoding/tables/apple/CHINTRAD.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/apple/CORPCHAR.TXT` & `monobit-0.43.1/monobit/encoding/tables/apple/CORPCHAR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/apple/CROATIAN.TXT` & `monobit-0.43.1/monobit/encoding/tables/apple/CROATIAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/apple/CYRILLIC.TXT` & `monobit-0.43.1/monobit/encoding/tables/apple/CYRILLIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/apple/DEVANAGA.TXT` & `monobit-0.43.1/monobit/encoding/tables/apple/DEVANAGA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/apple/DINGBATS.TXT` & `monobit-0.43.1/monobit/encoding/tables/apple/DINGBATS.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/apple/FARSI.TXT` & `monobit-0.43.1/monobit/encoding/tables/apple/FARSI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/apple/GAELIC.TXT` & `monobit-0.43.1/monobit/encoding/tables/apple/GAELIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/apple/GREEK.TXT` & `monobit-0.43.1/monobit/encoding/tables/apple/GREEK.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/apple/GUJARATI.TXT` & `monobit-0.43.1/monobit/encoding/tables/apple/GUJARATI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/apple/GURMUKHI.TXT` & `monobit-0.43.1/monobit/encoding/tables/apple/GURMUKHI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/apple/HEBREW.TXT` & `monobit-0.43.1/monobit/encoding/tables/apple/HEBREW.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/apple/ICELAND.TXT` & `monobit-0.43.1/monobit/encoding/tables/apple/ICELAND.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/apple/INUIT.TXT` & `monobit-0.43.1/monobit/encoding/tables/apple/INUIT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/apple/JAPANESE.TXT` & `monobit-0.43.1/monobit/encoding/tables/apple/JAPANESE.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/apple/KEYBOARD.TXT` & `monobit-0.43.1/monobit/encoding/tables/apple/KEYBOARD.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/apple/KOREAN.TXT` & `monobit-0.43.1/monobit/encoding/tables/apple/KOREAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/apple/ROMAN.TXT` & `monobit-0.43.1/monobit/encoding/tables/apple/ROMAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/apple/ROMANIAN.TXT` & `monobit-0.43.1/monobit/encoding/tables/apple/ROMANIAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/apple/ReadMe.txt` & `monobit-0.43.1/monobit/encoding/tables/apple/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/apple/SYMBOL.TXT` & `monobit-0.43.1/monobit/encoding/tables/apple/SYMBOL.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/apple/THAI.TXT` & `monobit-0.43.1/monobit/encoding/tables/apple/THAI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/apple/TURKISH.TXT` & `monobit-0.43.1/monobit/encoding/tables/apple/TURKISH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/apple/UKRAINE.TXT` & `monobit-0.43.1/monobit/encoding/tables/apple/UKRAINE.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/czyborra/README.md` & `monobit-0.43.1/monobit/encoding/tables/czyborra/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/czyborra/bulgarian-mik.txt` & `monobit-0.43.1/monobit/encoding/tables/czyborra/bulgarian-mik.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/czyborra/cp866.txt` & `monobit-0.43.1/monobit/encoding/tables/czyborra/cp866.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/czyborra/gost19768-87.txt` & `monobit-0.43.1/monobit/encoding/tables/czyborra/gost19768-87.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/czyborra/hp-roman8.txt` & `monobit-0.43.1/monobit/encoding/tables/czyborra/hp-roman8.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/czyborra/koi-0.txt` & `monobit-0.43.1/monobit/encoding/tables/czyborra/koi-0.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/czyborra/koi-7.txt` & `monobit-0.43.1/monobit/encoding/tables/czyborra/koi-7.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/czyborra/koi8-a.txt` & `monobit-0.43.1/monobit/encoding/tables/czyborra/koi8-a.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/czyborra/koi8-b.txt` & `monobit-0.43.1/monobit/encoding/tables/czyborra/koi8-b.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/czyborra/koi8-e.txt` & `monobit-0.43.1/monobit/encoding/tables/czyborra/koi8-e.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/czyborra/koi8-f.txt` & `monobit-0.43.1/monobit/encoding/tables/czyborra/koi8-f.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/czyborra/koi8-r.txt` & `monobit-0.43.1/monobit/encoding/tables/czyborra/koi8-r.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/czyborra/koi8-u.txt` & `monobit-0.43.1/monobit/encoding/tables/czyborra/koi8-u.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-ca` & `monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-ca`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-ca2` & `monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-ca2`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-cn` & `monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-cn`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-cu` & `monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-cu`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-de` & `monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-de`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-dk` & `monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-dk`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-es` & `monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-es`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-es2` & `monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-es2`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-fr` & `monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-fr`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-gb` & `monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-gb`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-hu` & `monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-hu`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-it` & `monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-it`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-jp` & `monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-jp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-jp-ocr-b` & `monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-jp-ocr-b`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-kr` & `monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-kr`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-us` & `monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-us`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/dkuug/iso646-yu` & `monobit-0.43.1/monobit/encoding/tables/dkuug/iso646-yu`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/dkuug/jis_x0201` & `monobit-0.43.1/monobit/encoding/tables/dkuug/jis_x0201`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/dkuug/x0201-7` & `monobit-0.43.1/monobit/encoding/tables/dkuug/x0201-7`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/emacs/MULE-ethiopic.map` & `monobit-0.43.1/monobit/encoding/tables/emacs/MULE-ethiopic.map`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/emacs/MULE-ipa.map` & `monobit-0.43.1/monobit/encoding/tables/emacs/MULE-ipa.map`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/emacs/MULE-is13194.map` & `monobit-0.43.1/monobit/encoding/tables/emacs/MULE-is13194.map`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/emacs/MULE-lviscii.map` & `monobit-0.43.1/monobit/encoding/tables/emacs/MULE-lviscii.map`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/emacs/MULE-sisheng.map` & `monobit-0.43.1/monobit/encoding/tables/emacs/MULE-sisheng.map`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/emacs/MULE-tibetan.map` & `monobit-0.43.1/monobit/encoding/tables/emacs/MULE-tibetan.map`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/emacs/MULE-uviscii.map` & `monobit-0.43.1/monobit/encoding/tables/emacs/MULE-uviscii.map`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/emacs/README.md` & `monobit-0.43.1/monobit/encoding/tables/emacs/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/evertype/ARMENIAN.TXT` & `monobit-0.43.1/monobit/encoding/tables/evertype/ARMENIAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/evertype/GEORGIAN.TXT` & `monobit-0.43.1/monobit/encoding/tables/evertype/GEORGIAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/evertype/README.md` & `monobit-0.43.1/monobit/encoding/tables/evertype/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/1116.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/1116.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/1117.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/1117.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/1118.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/1118.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/1119.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/1119.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/1125.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/1125.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/113.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/113.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/1131.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/1131.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30000.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30000.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30001.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30001.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30002.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30002.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30003.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30003.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30004.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30004.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30005.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30005.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30006.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30006.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30007.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30007.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30008.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30008.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30009.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30009.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30010.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30010.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30011.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30011.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30012.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30012.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30013.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30013.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30014.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30014.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30015.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30015.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30016.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30016.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30017.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30017.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30018.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30018.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30019.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30019.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30020.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30020.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30021.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30021.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30022.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30022.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30023.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30023.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30024.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30024.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30025.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30025.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30026.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30026.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30027.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30027.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30028.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30028.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30029.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30029.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30030.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30030.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30031.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30031.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30032.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30032.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30033.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30033.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30034.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30034.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30039.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30039.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/30040.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/30040.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/3012.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/3012.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/3021.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/3021.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/3845.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/3845.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/3846.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/3846.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/3848.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/3848.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/437.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/437.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/57781.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/57781.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/58152.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/58152.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/58210.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/58210.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/58335.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/58335.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/59234.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/59234.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/59829.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/59829.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/60258.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/60258.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/60853.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/60853.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/61282.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/61282.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/62306.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/62306.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/667.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/667.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/668.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/668.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/737.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/737.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/770.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/770.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/771.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/771.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/772.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/772.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/773.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/773.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/774.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/774.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/775.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/775.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/777.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/777.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/778.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/778.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/790.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/790.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/808.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/808.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/848.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/848.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/849.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/849.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/850.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/850.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/851.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/851.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/852.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/852.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/853.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/853.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/855.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/855.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/856.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/856.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/857.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/857.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/858.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/858.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/859.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/859.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/860.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/860.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/861.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/861.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/862.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/862.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/863.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/863.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/864.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/864.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/865.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/865.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/866.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/866.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/867.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/867.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/869.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/869.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/872.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/872.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/895.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/895.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/899.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/899.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/991.ucp` & `monobit-0.43.1/monobit/encoding/tables/freedos/991.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/freedos/README.md` & `monobit-0.43.1/monobit/encoding/tables/freedos/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/iana/Amiga-1251` & `monobit-0.43.1/monobit/encoding/tables/iana/Amiga-1251`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/iana/PTCP154` & `monobit-0.43.1/monobit/encoding/tables/iana/PTCP154`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/ibm-cdra/037B34B0.UPMAP100` & `monobit-0.43.1/monobit/encoding/tables/ibm-cdra/037B34B0.UPMAP100`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/ibm-cdra/038834B0.UPMAP100` & `monobit-0.43.1/monobit/encoding/tables/ibm-cdra/038834B0.UPMAP100`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/ibm-cdra/039E44B0.UPMAP101` & `monobit-0.43.1/monobit/encoding/tables/ibm-cdra/039E44B0.UPMAP101`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/ibm-cdra/039F34B0.UPMAP100` & `monobit-0.43.1/monobit/encoding/tables/ibm-cdra/039F34B0.UPMAP100`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/ibm-cdra/readme.txt` & `monobit-0.43.1/monobit/encoding/tables/ibm-cdra/readme.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/icu/README.md` & `monobit-0.43.1/monobit/encoding/tables/icu/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/icu/aix-KSC5601.1987_0-4.3.6.ucm` & `monobit-0.43.1/monobit/encoding/tables/icu/aix-KSC5601.1987_0-4.3.6.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/icu/cns-11643-1992.ucm` & `monobit-0.43.1/monobit/encoding/tables/icu/cns-11643-1992.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/icu/ibm-1125_P100-1997.ucm` & `monobit-0.43.1/monobit/encoding/tables/icu/ibm-1125_P100-1997.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/icu/ibm-1375_P100-2008.ucm` & `monobit-0.43.1/monobit/encoding/tables/icu/ibm-1375_P100-2008.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/icu/ibm-720_P100-1997.ucm` & `monobit-0.43.1/monobit/encoding/tables/icu/ibm-720_P100-1997.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/icu/ibm-806_P100-1998.ucm` & `monobit-0.43.1/monobit/encoding/tables/icu/ibm-806_P100-1998.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/icu/ibm-851_P100-1995.ucm` & `monobit-0.43.1/monobit/encoding/tables/icu/ibm-851_P100-1995.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/icu/ibm-858_P100-1997.ucm` & `monobit-0.43.1/monobit/encoding/tables/icu/ibm-858_P100-1997.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/icu/ibm-868_P100-1995.ucm` & `monobit-0.43.1/monobit/encoding/tables/icu/ibm-868_P100-1995.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/icu/ibm-932_P120-1999.ucm` & `monobit-0.43.1/monobit/encoding/tables/icu/ibm-932_P120-1999.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/icu/windows-1361-2000.ucm` & `monobit-0.43.1/monobit/encoding/tables/icu/windows-1361-2000.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/icu/windows-936-2000.ucm` & `monobit-0.43.1/monobit/encoding/tables/icu/windows-936-2000.ucm`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-1.TXT` & `monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-10.TXT` & `monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-10.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-11.TXT` & `monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-11.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-13.TXT` & `monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-13.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-14.TXT` & `monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-14.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-15.TXT` & `monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-15.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-16.TXT` & `monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-16.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-2.TXT` & `monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-3.TXT` & `monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-3.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-4.TXT` & `monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-4.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-5.TXT` & `monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-5.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-6.TXT` & `monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-6.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-7.TXT` & `monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-7.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-8.TXT` & `monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-8.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/iso-8859/8859-9.TXT` & `monobit-0.43.1/monobit/encoding/tables/iso-8859/8859-9.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/iso-8859/ReadMe.txt` & `monobit-0.43.1/monobit/encoding/tables/iso-8859/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ADAMOS7.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/ADAMOS7.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ADAMSWTR.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/ADAMSWTR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/AMSCPC.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/AMSCPC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/AMSCPM.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/AMSCPM.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/APL2ALT1.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/APL2ALT1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/APL2ALT2.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/APL2ALT2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/APL2ICHG.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/APL2ICHG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/APL2PRIM.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/APL2PRIM.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ATARI8IG.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/ATARI8IG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ATARI8II.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/ATARI8II.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ATARI8VG.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/ATARI8VG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ATARI8VI.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/ATARI8VI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ATARISTI.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/ATARISTI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ATARISTV.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/ATARISTV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/C64IALT.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/C64IALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/C64IPRI.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/C64IPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/C64VALT.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/C64VALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/C64VPRI.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/C64VPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/COCOICHG.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/COCOICHG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/COCOSGR4.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/COCOSGR4.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/COCOSGR6.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/COCOSGR6.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/CPETIALT.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/CPETIALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/CPETIPRI.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/CPETIPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/CPETVALT.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/CPETVALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/CPETVPRI.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/CPETVPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/CVICIALT.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/CVICIALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/CVICIPRI.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/CVICIPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/CVICVALT.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/CVICVALT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/CVICVPRI.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/CVICVPRI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/IBMPCICH.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/IBMPCICH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/IBMPCVID.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/IBMPCVID.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/MINITLG0.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/MINITLG0.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/MINITLG1.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/MINITLG1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/MSX.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/MSX.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ORICG0.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/ORICG0.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ORICG1.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/ORICG1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/RISCEFF.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/RISCEFF.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/RISCOSB.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/RISCOSB.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/RISCOSI.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/RISCOSI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/RISCOSV.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/RISCOSV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ReadMe.txt` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/ReadMe.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/SINCLRQL.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/SINCLRQL.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TELTXTG0.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/TELTXTG0.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TELTXTG1.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/TELTXTG1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TELTXTG2.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/TELTXTG2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TELTXTG3.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/TELTXTG3.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TI994A.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/TI994A.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM1ICH.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM1ICH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM1ORG.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM1ORG.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM1REV.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM1REV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM3IIN.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM3IIN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM3IJP.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM3IJP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM3IRV.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM3IRV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM3VIN.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM3VIN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM3VJP.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM3VJP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM3VRV.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM3VRV.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM4AIA.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM4AIA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM4AIP.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM4AIP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM4AIR.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM4AIR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM4AVA.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM4AVA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM4AVP.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM4AVP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/TRSM4AVR.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/TRSM4AVR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZX80.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/ZX80.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZX81.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/ZX81.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZXDESKTP.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/ZXDESKTP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZXFZXKOI.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/ZXFZXKOI.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZXFZXLT1.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/ZXFZXLT1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZXFZXLT5.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/ZXFZXLT5.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZXFZXPUA.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/ZXFZXPUA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZXFZXSLT.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/ZXFZXSLT.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/kreativekorp/ZXSPCTRM.TXT` & `monobit-0.43.1/monobit/encoding/tables/kreativekorp/ZXSPCTRM.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/manual/README.md` & `monobit-0.43.1/monobit/encoding/tables/manual/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/manual/dec-vt100.ucp` & `monobit-0.43.1/monobit/encoding/tables/manual/dec-vt100.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/manual/hp48.txt` & `monobit-0.43.1/monobit/encoding/tables/manual/hp48.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/manual/ibm897graph.ucp` & `monobit-0.43.1/monobit/encoding/tables/manual/ibm897graph.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/manual/iso2047.txt` & `monobit-0.43.1/monobit/encoding/tables/manual/iso2047.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/manual/mac-system.ucp` & `monobit-0.43.1/monobit/encoding/tables/manual/mac-system.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/manual/russup3.ucp` & `monobit-0.43.1/monobit/encoding/tables/manual/russup3.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/manual/russup4ac.ucp` & `monobit-0.43.1/monobit/encoding/tables/manual/russup4ac.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/manual/russup4na.ucp` & `monobit-0.43.1/monobit/encoding/tables/manual/russup4na.ucp`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/manual/windows-1.0.txt` & `monobit-0.43.1/monobit/encoding/tables/manual/windows-1.0.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/manual/windows-2.0.txt` & `monobit-0.43.1/monobit/encoding/tables/manual/windows-2.0.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/manual/windows-3.1.txt` & `monobit-0.43.1/monobit/encoding/tables/manual/windows-3.1.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/EBCDIC/CP037.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/EBCDIC/CP037.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/EBCDIC/CP1026.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/EBCDIC/CP1026.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/EBCDIC/CP500.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/EBCDIC/CP500.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/EBCDIC/CP875.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/EBCDIC/CP875.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/MAC/CYRILLIC.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/MAC/CYRILLIC.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/MAC/GREEK.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/MAC/GREEK.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/MAC/ICELAND.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/MAC/ICELAND.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/MAC/LATIN2.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/MAC/LATIN2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/MAC/ROMAN.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/MAC/ROMAN.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/MAC/TURKISH.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/MAC/TURKISH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP437.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP437.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP737.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP737.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP775.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP775.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP850.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP850.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP852.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP852.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP855.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP855.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP857.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP857.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP860.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP860.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP861.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP861.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP862.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP862.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP863.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP863.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP864.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP864.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP865.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP865.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP866.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP866.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP869.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP869.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/PC/CP874.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/PC/CP874.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1250.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/WINDOWS/CP1250.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1251.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/WINDOWS/CP1251.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1252.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/WINDOWS/CP1252.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1253.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/WINDOWS/CP1253.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1254.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/WINDOWS/CP1254.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1255.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/WINDOWS/CP1255.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1256.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/WINDOWS/CP1256.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1257.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/WINDOWS/CP1257.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP1258.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/WINDOWS/CP1258.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP874.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/WINDOWS/CP874.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP932.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/WINDOWS/CP932.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP936.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/WINDOWS/CP936.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP949.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/WINDOWS/CP949.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/microsoft/WINDOWS/CP950.TXT` & `monobit-0.43.1/monobit/encoding/tables/microsoft/WINDOWS/CP950.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/misc/APL-ISO-IR-68.TXT` & `monobit-0.43.1/monobit/encoding/tables/misc/APL-ISO-IR-68.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/misc/ATARIST.TXT` & `monobit-0.43.1/monobit/encoding/tables/misc/ATARIST.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/misc/CP1006.TXT` & `monobit-0.43.1/monobit/encoding/tables/misc/CP1006.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/misc/CP424.TXT` & `monobit-0.43.1/monobit/encoding/tables/misc/CP424.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/misc/CP856.TXT` & `monobit-0.43.1/monobit/encoding/tables/misc/CP856.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/misc/GSM0338.TXT` & `monobit-0.43.1/monobit/encoding/tables/misc/GSM0338.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/misc/IBMGRAPH.TXT` & `monobit-0.43.1/monobit/encoding/tables/misc/IBMGRAPH.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/misc/JIS0208.TXT` & `monobit-0.43.1/monobit/encoding/tables/misc/JIS0208.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/misc/KOI8-R.TXT` & `monobit-0.43.1/monobit/encoding/tables/misc/KOI8-R.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/misc/KOI8-U.TXT` & `monobit-0.43.1/monobit/encoding/tables/misc/KOI8-U.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/misc/KPS9566.TXT` & `monobit-0.43.1/monobit/encoding/tables/misc/KPS9566.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/misc/KZ1048.TXT` & `monobit-0.43.1/monobit/encoding/tables/misc/KZ1048.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/misc/NEXTSTEP.TXT` & `monobit-0.43.1/monobit/encoding/tables/misc/NEXTSTEP.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/misc/SGML.TXT` & `monobit-0.43.1/monobit/encoding/tables/misc/SGML.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/misc/US-ASCII-QUOTES.TXT` & `monobit-0.43.1/monobit/encoding/tables/misc/US-ASCII-QUOTES.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/misc/dashen-map.txt` & `monobit-0.43.1/monobit/encoding/tables/misc/dashen-map.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/misc/ibm-ugl.txt` & `monobit-0.43.1/monobit/encoding/tables/misc/ibm-ugl.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/mleisher/ALTVAR.TXT` & `monobit-0.43.1/monobit/encoding/tables/mleisher/ALTVAR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/mleisher/ARMSCII-7.TXT` & `monobit-0.43.1/monobit/encoding/tables/mleisher/ARMSCII-7.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/mleisher/ARMSCII-8.TXT` & `monobit-0.43.1/monobit/encoding/tables/mleisher/ARMSCII-8.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/mleisher/ARMSCII-8A.TXT` & `monobit-0.43.1/monobit/encoding/tables/mleisher/ARMSCII-8A.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/mleisher/DECMCS.TXT` & `monobit-0.43.1/monobit/encoding/tables/mleisher/DECMCS.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/mleisher/GEO-ITA.TXT` & `monobit-0.43.1/monobit/encoding/tables/mleisher/GEO-ITA.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/mleisher/GEO-PS.TXT` & `monobit-0.43.1/monobit/encoding/tables/mleisher/GEO-PS.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/mleisher/IRANSYSTEM.TXT` & `monobit-0.43.1/monobit/encoding/tables/mleisher/IRANSYSTEM.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/mleisher/KOI8RU.TXT` & `monobit-0.43.1/monobit/encoding/tables/mleisher/KOI8RU.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/mleisher/OSNOVAR.TXT` & `monobit-0.43.1/monobit/encoding/tables/mleisher/OSNOVAR.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/mleisher/README.md` & `monobit-0.43.1/monobit/encoding/tables/mleisher/README.md`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/mleisher/TIS620.TXT` & `monobit-0.43.1/monobit/encoding/tables/mleisher/TIS620.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/moztw/big5_2003-b2u.txt` & `monobit-0.43.1/monobit/encoding/tables/moztw/big5_2003-b2u.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/moztw/eten.txt` & `monobit-0.43.1/monobit/encoding/tables/moztw/eten.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/python/TCVN5712-1.TXT` & `monobit-0.43.1/monobit/encoding/tables/python/TCVN5712-1.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/python/TCVN5712-2.TXT` & `monobit-0.43.1/monobit/encoding/tables/python/TCVN5712-2.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/python/TCVN5712-3.TXT` & `monobit-0.43.1/monobit/encoding/tables/python/TCVN5712-3.TXT`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/vietstd/unicode.html` & `monobit-0.43.1/monobit/encoding/tables/vietstd/unicode.html`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/vietstd/viscii1.1.txt` & `monobit-0.43.1/monobit/encoding/tables/vietstd/viscii1.1.txt`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/wikipedia/abicomp.html` & `monobit-0.43.1/monobit/encoding/tables/wikipedia/abicomp.html`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/wikipedia/brascii.html` & `monobit-0.43.1/monobit/encoding/tables/wikipedia/brascii.html`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/wikipedia/cp853.html` & `monobit-0.43.1/monobit/encoding/tables/wikipedia/cp853.html`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/wikipedia/cwi2.html` & `monobit-0.43.1/monobit/encoding/tables/wikipedia/cwi2.html`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/wikipedia/dec-special.html` & `monobit-0.43.1/monobit/encoding/tables/wikipedia/dec-special.html`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/wikipedia/dec-technical.html` & `monobit-0.43.1/monobit/encoding/tables/wikipedia/dec-technical.html`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/wikipedia/gem.html` & `monobit-0.43.1/monobit/encoding/tables/wikipedia/gem.html`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/wikipedia/kamenicky.html` & `monobit-0.43.1/monobit/encoding/tables/wikipedia/kamenicky.html`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/wikipedia/lics.html` & `monobit-0.43.1/monobit/encoding/tables/wikipedia/lics.html`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/wikipedia/mattel-aquarius.html` & `monobit-0.43.1/monobit/encoding/tables/wikipedia/mattel-aquarius.html`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/wikipedia/mazovia.html` & `monobit-0.43.1/monobit/encoding/tables/wikipedia/mazovia.html`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/wikipedia/pascii.html` & `monobit-0.43.1/monobit/encoding/tables/wikipedia/pascii.html`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/wikipedia/ventura.html` & `monobit-0.43.1/monobit/encoding/tables/wikipedia/ventura.html`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/wikipedia/windows-1252.html` & `monobit-0.43.1/monobit/encoding/tables/wikipedia/windows-1252.html`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/wikipedia/wingdings.html` & `monobit-0.43.1/monobit/encoding/tables/wikipedia/wingdings.html`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/wikipedia/wiscii.html` & `monobit-0.43.1/monobit/encoding/tables/wikipedia/wiscii.html`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/xfonts/mulearabic-1.enc` & `monobit-0.43.1/monobit/encoding/tables/xfonts/mulearabic-1.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/xfonts/mulearabic-2.enc` & `monobit-0.43.1/monobit/encoding/tables/xfonts/mulearabic-2.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/xfonts/mulelao-1.enc` & `monobit-0.43.1/monobit/encoding/tables/xfonts/mulelao-1.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/encoding/tables/xfonts/suneu-greek.enc` & `monobit-0.43.1/monobit/encoding/tables/xfonts/suneu-greek.enc`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/plumbing/args.py` & `monobit-0.43.1/monobit/plumbing/args.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/plumbing/help.py` & `monobit-0.43.1/monobit/plumbing/help.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/plumbing/history.py` & `monobit-0.43.1/monobit/plumbing/history.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/plumbing/scripting.py` & `monobit-0.43.1/monobit/plumbing/scripting.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/render/chart.py` & `monobit-0.43.1/monobit/render/chart.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/render/glyphmap.py` & `monobit-0.43.1/monobit/render/glyphmap.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/render/renderer.py` & `monobit-0.43.1/monobit/render/renderer.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/scripts/banner.py` & `monobit-0.43.1/monobit/scripts/banner.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/scripts/convert.py` & `monobit-0.43.1/monobit/scripts/convert.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/__init__.py` & `monobit-0.43.1/monobit/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/converters.py` & `monobit-0.43.1/monobit/storage/converters.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/magic.py` & `monobit-0.43.1/monobit/storage/magic.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/streams.py` & `monobit-0.43.1/monobit/storage/streams.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/containers/container.py` & `monobit-0.43.1/monobit/storage/containers/container.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/containers/directory.py` & `monobit-0.43.1/monobit/storage/containers/directory.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/containers/tar.py` & `monobit-0.43.1/monobit/storage/containers/tar.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/containers/zip.py` & `monobit-0.43.1/monobit/storage/containers/zip.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/amiga.py` & `monobit-0.43.1/monobit/storage/formats/amiga.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/bbc.py` & `monobit-0.43.1/monobit/storage/formats/bbc.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/common.py` & `monobit-0.43.1/monobit/storage/formats/common.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/cpi.py` & `monobit-0.43.1/monobit/storage/formats/cpi.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/daisydot.py` & `monobit-0.43.1/monobit/storage/formats/daisydot.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/dashen.py` & `monobit-0.43.1/monobit/storage/formats/dashen.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/dec.py` & `monobit-0.43.1/monobit/storage/formats/dec.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/dosstart.py` & `monobit-0.43.1/monobit/storage/formats/dosstart.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/figlet.py` & `monobit-0.43.1/monobit/storage/formats/figlet.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/fontx.py` & `monobit-0.43.1/monobit/storage/formats/fontx.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/fzx.py` & `monobit-0.43.1/monobit/storage/formats/fzx.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/gdos.py` & `monobit-0.43.1/monobit/storage/formats/gdos.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/geos.py` & `monobit-0.43.1/monobit/storage/formats/geos.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/nearlyraw.py` & `monobit-0.43.1/monobit/storage/formats/nearlyraw.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/pcl.py` & `monobit-0.43.1/monobit/storage/formats/pcl.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/pcpaint.py` & `monobit-0.43.1/monobit/storage/formats/pcpaint.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/pdf.py` & `monobit-0.43.1/monobit/storage/formats/pdf.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/pkfont.py` & `monobit-0.43.1/monobit/storage/formats/pkfont.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/prebuilt.py` & `monobit-0.43.1/monobit/storage/formats/prebuilt.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/printshop.py` & `monobit-0.43.1/monobit/storage/formats/printshop.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/psf.py` & `monobit-0.43.1/monobit/storage/formats/psf.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/raw.py` & `monobit-0.43.1/monobit/storage/formats/raw.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/signum.py` & `monobit-0.43.1/monobit/storage/formats/signum.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/vfont.py` & `monobit-0.43.1/monobit/storage/formats/vfont.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/xerox.py` & `monobit-0.43.1/monobit/storage/formats/xerox.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/apple/__init__.py` & `monobit-0.43.1/monobit/storage/formats/apple/__init__.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/apple/dfont.py` & `monobit-0.43.1/monobit/storage/formats/apple/dfont.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/apple/fond.py` & `monobit-0.43.1/monobit/storage/formats/apple/fond.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/apple/iigs.py` & `monobit-0.43.1/monobit/storage/formats/apple/iigs.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/apple/lisa.py` & `monobit-0.43.1/monobit/storage/formats/apple/lisa.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/apple/mgtk.py` & `monobit-0.43.1/monobit/storage/formats/apple/mgtk.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/apple/nfnt.py` & `monobit-0.43.1/monobit/storage/formats/apple/nfnt.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/apple/palm.py` & `monobit-0.43.1/monobit/storage/formats/apple/palm.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/fon/fon.py` & `monobit-0.43.1/monobit/storage/formats/fon/fon.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/fon/mz.py` & `monobit-0.43.1/monobit/storage/formats/fon/mz.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/fon/os2/__init__.py` & `monobit-0.43.1/monobit/storage/formats/fon/os2/__init__.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/fon/os2/gpifont.py` & `monobit-0.43.1/monobit/storage/formats/fon/os2/gpifont.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/fon/os2/lx.py` & `monobit-0.43.1/monobit/storage/formats/fon/os2/lx.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/fon/os2/ne.py` & `monobit-0.43.1/monobit/storage/formats/fon/os2/ne.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/fon/windows/LICENSE.md` & `monobit-0.43.1/monobit/storage/formats/fon/windows/LICENSE.md`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/fon/windows/__init__.py` & `monobit-0.43.1/monobit/storage/formats/fon/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/fon/windows/fnt.py` & `monobit-0.43.1/monobit/storage/formats/fon/windows/fnt.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/fon/windows/ne.py` & `monobit-0.43.1/monobit/storage/formats/fon/windows/ne.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/fon/windows/pe.py` & `monobit-0.43.1/monobit/storage/formats/fon/windows/pe.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/image/bmfont.py` & `monobit-0.43.1/monobit/storage/formats/image/bmfont.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/image/image.py` & `monobit-0.43.1/monobit/storage/formats/image/image.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/sfnt/sfnt.py` & `monobit-0.43.1/monobit/storage/formats/sfnt/sfnt.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/sfnt/sfnt_writer.py` & `monobit-0.43.1/monobit/storage/formats/sfnt/sfnt_writer.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/sfnt/fonttools/E_B_S_C_.py` & `monobit-0.43.1/monobit/storage/formats/sfnt/fonttools/E_B_S_C_.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/sfnt/fonttools/__init__.py` & `monobit-0.43.1/monobit/storage/formats/sfnt/fonttools/__init__.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/text/draw.py` & `monobit-0.43.1/monobit/storage/formats/text/draw.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/text/edwin.py` & `monobit-0.43.1/monobit/storage/formats/text/edwin.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/text/hex.py` & `monobit-0.43.1/monobit/storage/formats/text/hex.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/text/yaff.py` & `monobit-0.43.1/monobit/storage/formats/text/yaff.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/vector/borland.py` & `monobit-0.43.1/monobit/storage/formats/vector/borland.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/vector/hurt.py` & `monobit-0.43.1/monobit/storage/formats/vector/hurt.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/vector/svg.py` & `monobit-0.43.1/monobit/storage/formats/vector/svg.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/xlfd/bdf.py` & `monobit-0.43.1/monobit/storage/formats/xlfd/bdf.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/xlfd/hbf.py` & `monobit-0.43.1/monobit/storage/formats/xlfd/hbf.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/xlfd/pcf.py` & `monobit-0.43.1/monobit/storage/formats/xlfd/pcf.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/formats/xlfd/xlfd.py` & `monobit-0.43.1/monobit/storage/formats/xlfd/xlfd.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/wrappers/apple.py` & `monobit-0.43.1/monobit/storage/wrappers/apple.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/wrappers/binhex.py` & `monobit-0.43.1/monobit/storage/wrappers/binhex.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/wrappers/compressors.py` & `monobit-0.43.1/monobit/storage/wrappers/compressors.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/wrappers/macbinary.py` & `monobit-0.43.1/monobit/storage/wrappers/macbinary.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/monobit/storage/wrappers/source.py` & `monobit-0.43.1/monobit/storage/wrappers/source.py`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/LICENSE` & `monobit-0.43.1/LICENSE`

 * *Files identical despite different names*

### Comparing `monobit-0.43.0/README.md` & `monobit-0.43.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -263,14 +263,15 @@
 | monobit yaff               | `yaff`     | `.yaff`           |&check;|&check;|
 | SVG Fonts                  | `svg`      | `.svg`            |&check;|&check;|
 | Windows resource           | `win`      | `.fnt`            |&check;|&check;|
 | Windows font               | `fon`      | `.fon`            |&check;|&check; (NE) |
 | Borland Graphics Interface | `borland`  | `.chr`            |&check;|&check;|
 | Hershey fonts (Jim Hurt)   | `hurt`     | `.jhf`            |&check;|       |
 | DOSStart                   | `dosstart` | `.dsf`            |&check;|       |
+| GIMMS                      | `gimms`    | `.bin`            |&check;|       |
 
 
 Dependencies
 ------------
 
 Some formats require
 - **PIL** (`Pillow`)
```

### Comparing `monobit-0.43.0/pyproject.toml` & `monobit-0.43.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "monobit"
-version = "0.43.0"
+version = "0.43.1"
 authors = [
     { name = "Rob Hagemans", email = "rob.hagemans@hotmail.com" },
 ]
 description = "Tools for working with monochrome bitmap fonts."
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
```

### Comparing `monobit-0.43.0/PKG-INFO` & `monobit-0.43.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: monobit
-Version: 0.43.0
+Version: 0.43.1
 Summary: Tools for working with monochrome bitmap fonts.
 Project-URL: Homepage, https://github.com/robhagemans/monobit
 Author-email: Rob Hagemans <rob.hagemans@hotmail.com>
 License: MIT License
         
         Copyright (c) 2019--2023 Rob Hagemans
         
@@ -305,14 +305,15 @@
 | monobit yaff               | `yaff`     | `.yaff`           |&check;|&check;|
 | SVG Fonts                  | `svg`      | `.svg`            |&check;|&check;|
 | Windows resource           | `win`      | `.fnt`            |&check;|&check;|
 | Windows font               | `fon`      | `.fon`            |&check;|&check; (NE) |
 | Borland Graphics Interface | `borland`  | `.chr`            |&check;|&check;|
 | Hershey fonts (Jim Hurt)   | `hurt`     | `.jhf`            |&check;|       |
 | DOSStart                   | `dosstart` | `.dsf`            |&check;|       |
+| GIMMS                      | `gimms`    | `.bin`            |&check;|       |
 
 
 Dependencies
 ------------
 
 Some formats require
 - **PIL** (`Pillow`)
```

