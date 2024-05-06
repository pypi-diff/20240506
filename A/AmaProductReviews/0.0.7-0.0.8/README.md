# Comparing `tmp/amaproductreviews-0.0.7.tar.gz` & `tmp/amaproductreviews-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amaproductreviews-0.0.7.tar", max compression
+gzip compressed data, was "amaproductreviews-0.0.8.tar", max compression
```

## Comparing `amaproductreviews-0.0.7.tar` & `amaproductreviews-0.0.8.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     4754 2024-04-28 19:51:19.925046 amaproductreviews-0.0.7/amaproductreviews.py
--rw-r--r--   0        0        0      371 2024-04-28 19:52:06.549611 amaproductreviews-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2245 2024-04-28 19:45:23.696166 amaproductreviews-0.0.7/README.md
--rw-r--r--   0        0        0     2850 1970-01-01 00:00:00.000000 amaproductreviews-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     5185 2024-05-06 11:54:51.242932 amaproductreviews-0.0.8/amaproductreviews.py
+-rw-r--r--   0        0        0      371 2024-05-06 11:55:52.837562 amaproductreviews-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2287 2024-04-28 20:00:17.667328 amaproductreviews-0.0.8/README.md
+-rw-r--r--   0        0        0     2892 1970-01-01 00:00:00.000000 amaproductreviews-0.0.8/PKG-INFO
```

### Comparing `amaproductreviews-0.0.7/amaproductreviews.py` & `amaproductreviews-0.0.8/amaproductreviews.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,8 +101,17 @@
 def comment_dataFrame(UrlProduct):
     reviews = extract_all_reviews(UrlProduct)
     reviews_cleaned = [clean_comment(review.replace("\n", " ")) for review in reviews]
     df = pd.DataFrame(reviews_cleaned, columns=['comment'])
     df['sentiment'] = df['comment'].apply(sentiment_analysis_textblob)
     return df
 def sentiemnt_by_comment(df):
-    return df.groupby('sentiment').count()['comment'].reset_index()
+    return df.groupby('sentiment').count()['comment'].reset_index()
+
+def get_reviews_images(UrlProduct):
+    driver.get(UrlProduct)
+    soup = BeautifulSoup(driver.page_source,'html.parser')
+    image_reviews = soup.find_all('div', class_='_Y3Itb_media-thumbnail-container_2MRZY')
+    image_reviews = str(image_reviews)
+    image_reviews = re.findall(r'src="(https.*?jpg)',image_reviews)
+    # Image_of_product = re.findall(r'src="https.*pg',str(Image_of_product))
+    return image_reviews
```

### Comparing `amaproductreviews-0.0.7/README.md` & `amaproductreviews-0.0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -134,8 +134,10 @@
 00000850: 0d0a 2d20 776f 7264 636c 6f75 640d 0a2d  ..- wordcloud..-
 00000860: 2077 6562 6472 6976 6572 5f6d 616e 6167   webdriver_manag
 00000870: 6572 0d0a 0d0a 2323 2054 6561 6d20 4d65  er....## Team Me
 00000880: 6d62 6572 733a 0d0a 0d0a 2d20 456c 204f  mbers:....- El O
 00000890: 7561 6e6b 7269 6d69 2041 6c69 0d0a 2d20  uankrimi Ali..- 
 000008a0: 4f6c 616d 696e 6520 5a61 6b61 7269 610d  Olamine Zakaria.
 000008b0: 0a2d 204f 7562 656c 6c61 2041 6264 616c  .- Oubella Abdal
-000008c0: 6c61 680d 0a                             lah..
+000008c0: 6c61 680d 0a23 0020 0041 006d 0061 0050  lah..#. .A.m.a.P
+000008d0: 0072 006f 0064 0075 0063 0074 0052 0065  .r.o.d.u.c.t.R.e
+000008e0: 0076 0069 0065 0077 0073 000d 000a 00    .v.i.e.w.s.....
```

### Comparing `amaproductreviews-0.0.7/PKG-INFO` & `amaproductreviews-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 416d 6150  : 2.1.Name: AmaP
 00000020: 726f 6475 6374 5265 7669 6577 730a 5665  roductReviews.Ve
-00000030: 7273 696f 6e3a 2030 2e30 2e37 0a53 756d  rsion: 0.0.7.Sum
+00000030: 7273 696f 6e3a 2030 2e30 2e38 0a53 756d  rsion: 0.0.8.Sum
 00000040: 6d61 7279 3a20 416e 616c 797a 6520 416d  mary: Analyze Am
 00000050: 617a 6f6e 2070 726f 6475 6374 2072 6576  azon product rev
 00000060: 6965 7773 0a41 7574 686f 723a 206f 6c61  iews.Author: ola
 00000070: 6d69 6e65 207a 616b 6172 6961 0a41 7574  mine zakaria.Aut
 00000080: 686f 722d 656d 6169 6c3a 206f 6c61 6d69  hor-email: olami
 00000090: 6e65 7a61 6b61 7269 6130 3340 676d 6169  nezakaria03@gmai
 000000a0: 6c2e 636f 6d0a 5265 7175 6972 6573 2d50  l.com.Requires-P
@@ -172,8 +172,10 @@
 00000ab0: 7565 7374 730a 2d20 776f 7264 636c 6f75  uests.- wordclou
 00000ac0: 640a 2d20 7765 6264 7269 7665 725f 6d61  d.- webdriver_ma
 00000ad0: 6e61 6765 720a 0a23 2320 5465 616d 204d  nager..## Team M
 00000ae0: 656d 6265 7273 3a0a 0a2d 2045 6c20 4f75  embers:..- El Ou
 00000af0: 616e 6b72 696d 6920 416c 690a 2d20 4f6c  ankrimi Ali.- Ol
 00000b00: 616d 696e 6520 5a61 6b61 7269 610a 2d20  amine Zakaria.- 
 00000b10: 4f75 6265 6c6c 6120 4162 6461 6c6c 6168  Oubella Abdallah
-00000b20: 0a0a                                     ..
+00000b20: 0a23 0020 0041 006d 0061 0050 0072 006f  .#. .A.m.a.P.r.o
+00000b30: 0064 0075 0063 0074 0052 0065 0076 0069  .d.u.c.t.R.e.v.i
+00000b40: 0065 0077 0073 000a 000a 000a            .e.w.s......
```

