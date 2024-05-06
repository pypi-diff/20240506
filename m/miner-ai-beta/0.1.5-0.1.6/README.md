# Comparing `tmp/miner_ai_beta-0.1.5.tar.gz` & `tmp/miner_ai_beta-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miner_ai_beta-0.1.5.tar", max compression
+gzip compressed data, was "miner_ai_beta-0.1.6.tar", max compression
```

## Comparing `miner_ai_beta-0.1.5.tar` & `miner_ai_beta-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2024-05-04 16:49:23.857900 miner_ai_beta-0.1.5/LICENSE
--rw-r--r--   0        0        0      242 2024-05-04 16:59:21.199649 miner_ai_beta-0.1.5/miner_ai_beta/loader/__init__.py
--rw-r--r--   0        0        0      473 2024-05-04 16:04:57.185499 miner_ai_beta-0.1.5/miner_ai_beta/loader/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     3042 2024-05-04 15:17:18.873214 miner_ai_beta-0.1.5/miner_ai_beta/loader/__pycache__/docs.cpython-311.pyc
--rw-r--r--   0        0        0     2372 2024-05-04 16:04:57.189700 miner_ai_beta-0.1.5/miner_ai_beta/loader/__pycache__/docs.cpython-312.pyc
--rw-r--r--   0        0        0     2299 2024-05-04 16:04:58.283790 miner_ai_beta-0.1.5/miner_ai_beta/loader/__pycache__/excels.cpython-312.pyc
--rw-r--r--   0        0        0     3252 2024-05-04 15:17:18.945722 miner_ai_beta-0.1.5/miner_ai_beta/loader/__pycache__/pages.cpython-311.pyc
--rw-r--r--   0        0        0     2566 2024-05-04 15:17:18.984762 miner_ai_beta-0.1.5/miner_ai_beta/loader/__pycache__/pages.cpython-312.pyc
--rw-r--r--   0        0        0     3161 2024-05-04 15:17:19.027542 miner_ai_beta-0.1.5/miner_ai_beta/loader/__pycache__/pdfs.cpython-311.pyc
--rw-r--r--   0        0        0     2309 2024-05-04 16:05:00.319553 miner_ai_beta-0.1.5/miner_ai_beta/loader/__pycache__/pdfs.cpython-312.pyc
--rw-r--r--   0        0        0     2165 2024-05-04 16:05:00.402279 miner_ai_beta-0.1.5/miner_ai_beta/loader/__pycache__/ppts.cpython-312.pyc
--rw-r--r--   0        0        0     2343 2024-05-04 16:05:00.331906 miner_ai_beta-0.1.5/miner_ai_beta/loader/__pycache__/tubes.cpython-312.pyc
--rw-r--r--   0        0        0      711 2024-05-04 16:05:00.626643 miner_ai_beta-0.1.5/miner_ai_beta/loader/__pycache__/union.cpython-312.pyc
--rw-r--r--   0        0        0     2455 2024-05-04 16:05:00.139759 miner_ai_beta-0.1.5/miner_ai_beta/loader/__pycache__/web_pages.cpython-312.pyc
--rw-r--r--   0        0        0     2928 2024-05-04 15:17:19.188416 miner_ai_beta-0.1.5/miner_ai_beta/loader/__pycache__/xlss.cpython-311.pyc
--rw-r--r--   0        0        0     2490 2024-05-04 15:17:19.226637 miner_ai_beta-0.1.5/miner_ai_beta/loader/__pycache__/xlss.cpython-312.pyc
--rw-r--r--   0        0        0     1737 2024-05-04 16:30:59.578915 miner_ai_beta-0.1.5/miner_ai_beta/loader/docs.py
--rw-r--r--   0        0        0     1731 2024-05-04 16:03:01.249647 miner_ai_beta-0.1.5/miner_ai_beta/loader/excels.py
--rw-r--r--   0        0        0     1697 2024-05-04 16:03:04.629094 miner_ai_beta-0.1.5/miner_ai_beta/loader/pdfs.py
--rw-r--r--   0        0        0     1782 2024-05-04 16:30:53.122384 miner_ai_beta-0.1.5/miner_ai_beta/loader/ppts.py
--rw-r--r--   0        0        0     1792 2024-05-04 16:03:14.578345 miner_ai_beta-0.1.5/miner_ai_beta/loader/tubes.py
--rw-r--r--   0        0        0      361 2024-05-04 15:52:12.917924 miner_ai_beta-0.1.5/miner_ai_beta/loader/union.py
--rw-r--r--   0        0        0     1857 2024-05-04 16:30:42.678525 miner_ai_beta-0.1.5/miner_ai_beta/loader/web_pages.py
--rw-r--r--   0        0        0      668 2024-05-05 08:53:16.437382 miner_ai_beta-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3966 2024-05-05 07:06:38.721971 miner_ai_beta-0.1.5/README.md
--rw-r--r--   0        0        0     4832 1970-01-01 00:00:00.000000 miner_ai_beta-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-04 16:49:23.857900 miner_ai_beta-0.1.6/LICENSE
+-rw-r--r--   0        0        0      242 2024-05-04 16:59:21.199649 miner_ai_beta-0.1.6/miner_ai_beta/loader/__init__.py
+-rw-r--r--   0        0        0      473 2024-05-04 16:04:57.185499 miner_ai_beta-0.1.6/miner_ai_beta/loader/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     3042 2024-05-04 15:17:18.873214 miner_ai_beta-0.1.6/miner_ai_beta/loader/__pycache__/docs.cpython-311.pyc
+-rw-r--r--   0        0        0     2372 2024-05-04 16:04:57.189700 miner_ai_beta-0.1.6/miner_ai_beta/loader/__pycache__/docs.cpython-312.pyc
+-rw-r--r--   0        0        0     2299 2024-05-04 16:04:58.283790 miner_ai_beta-0.1.6/miner_ai_beta/loader/__pycache__/excels.cpython-312.pyc
+-rw-r--r--   0        0        0     3252 2024-05-04 15:17:18.945722 miner_ai_beta-0.1.6/miner_ai_beta/loader/__pycache__/pages.cpython-311.pyc
+-rw-r--r--   0        0        0     2566 2024-05-04 15:17:18.984762 miner_ai_beta-0.1.6/miner_ai_beta/loader/__pycache__/pages.cpython-312.pyc
+-rw-r--r--   0        0        0     3161 2024-05-04 15:17:19.027542 miner_ai_beta-0.1.6/miner_ai_beta/loader/__pycache__/pdfs.cpython-311.pyc
+-rw-r--r--   0        0        0     2309 2024-05-04 16:05:00.319553 miner_ai_beta-0.1.6/miner_ai_beta/loader/__pycache__/pdfs.cpython-312.pyc
+-rw-r--r--   0        0        0     2165 2024-05-04 16:05:00.402279 miner_ai_beta-0.1.6/miner_ai_beta/loader/__pycache__/ppts.cpython-312.pyc
+-rw-r--r--   0        0        0     2343 2024-05-04 16:05:00.331906 miner_ai_beta-0.1.6/miner_ai_beta/loader/__pycache__/tubes.cpython-312.pyc
+-rw-r--r--   0        0        0      711 2024-05-04 16:05:00.626643 miner_ai_beta-0.1.6/miner_ai_beta/loader/__pycache__/union.cpython-312.pyc
+-rw-r--r--   0        0        0     2455 2024-05-04 16:05:00.139759 miner_ai_beta-0.1.6/miner_ai_beta/loader/__pycache__/web_pages.cpython-312.pyc
+-rw-r--r--   0        0        0     2928 2024-05-04 15:17:19.188416 miner_ai_beta-0.1.6/miner_ai_beta/loader/__pycache__/xlss.cpython-311.pyc
+-rw-r--r--   0        0        0     2490 2024-05-04 15:17:19.226637 miner_ai_beta-0.1.6/miner_ai_beta/loader/__pycache__/xlss.cpython-312.pyc
+-rw-r--r--   0        0        0     1753 2024-05-06 15:23:37.641122 miner_ai_beta-0.1.6/miner_ai_beta/loader/docs.py
+-rw-r--r--   0        0        0     1806 2024-05-06 15:23:41.336318 miner_ai_beta-0.1.6/miner_ai_beta/loader/excels.py
+-rw-r--r--   0        0        0     1713 2024-05-06 15:23:39.870469 miner_ai_beta-0.1.6/miner_ai_beta/loader/pdfs.py
+-rw-r--r--   0        0        0     1798 2024-05-06 15:23:36.444442 miner_ai_beta-0.1.6/miner_ai_beta/loader/ppts.py
+-rw-r--r--   0        0        0     1821 2024-05-06 15:23:35.159300 miner_ai_beta-0.1.6/miner_ai_beta/loader/tubes.py
+-rw-r--r--   0        0        0      361 2024-05-04 15:52:12.917924 miner_ai_beta-0.1.6/miner_ai_beta/loader/union.py
+-rw-r--r--   0        0        0     1873 2024-05-06 15:23:32.901218 miner_ai_beta-0.1.6/miner_ai_beta/loader/web_pages.py
+-rw-r--r--   0        0        0      668 2024-05-06 15:24:25.905772 miner_ai_beta-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3966 2024-05-05 07:06:38.721971 miner_ai_beta-0.1.6/README.md
+-rw-r--r--   0        0        0     4832 1970-01-01 00:00:00.000000 miner_ai_beta-0.1.6/PKG-INFO
```

### Comparing `miner_ai_beta-0.1.5/LICENSE` & `miner_ai_beta-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.5/miner_ai_beta/loader/__pycache__/docs.cpython-311.pyc` & `miner_ai_beta-0.1.6/miner_ai_beta/loader/__pycache__/docs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.5/miner_ai_beta/loader/__pycache__/docs.cpython-312.pyc` & `miner_ai_beta-0.1.6/miner_ai_beta/loader/__pycache__/docs.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.5/miner_ai_beta/loader/__pycache__/excels.cpython-312.pyc` & `miner_ai_beta-0.1.6/miner_ai_beta/loader/__pycache__/excels.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.5/miner_ai_beta/loader/__pycache__/pages.cpython-311.pyc` & `miner_ai_beta-0.1.6/miner_ai_beta/loader/__pycache__/pages.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.5/miner_ai_beta/loader/__pycache__/pages.cpython-312.pyc` & `miner_ai_beta-0.1.6/miner_ai_beta/loader/__pycache__/pages.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.5/miner_ai_beta/loader/__pycache__/pdfs.cpython-311.pyc` & `miner_ai_beta-0.1.6/miner_ai_beta/loader/__pycache__/pdfs.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.5/miner_ai_beta/loader/__pycache__/pdfs.cpython-312.pyc` & `miner_ai_beta-0.1.6/miner_ai_beta/loader/__pycache__/pdfs.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.5/miner_ai_beta/loader/__pycache__/ppts.cpython-312.pyc` & `miner_ai_beta-0.1.6/miner_ai_beta/loader/__pycache__/ppts.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.5/miner_ai_beta/loader/__pycache__/tubes.cpython-312.pyc` & `miner_ai_beta-0.1.6/miner_ai_beta/loader/__pycache__/tubes.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.5/miner_ai_beta/loader/__pycache__/union.cpython-312.pyc` & `miner_ai_beta-0.1.6/miner_ai_beta/loader/__pycache__/union.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.5/miner_ai_beta/loader/__pycache__/web_pages.cpython-312.pyc` & `miner_ai_beta-0.1.6/miner_ai_beta/loader/__pycache__/web_pages.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.5/miner_ai_beta/loader/__pycache__/xlss.cpython-311.pyc` & `miner_ai_beta-0.1.6/miner_ai_beta/loader/__pycache__/xlss.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.5/miner_ai_beta/loader/__pycache__/xlss.cpython-312.pyc` & `miner_ai_beta-0.1.6/miner_ai_beta/loader/__pycache__/xlss.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.5/miner_ai_beta/loader/docs.py` & `miner_ai_beta-0.1.6/miner_ai_beta/loader/docs.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,17 +29,17 @@
         doc = docx.Document(os.path.join(folder_path, doc_file))
         fullText = []
         for para in doc.paragraphs:
             fullText.append(para.text)
         super_text += '\n'.join(fullText)   
         print(f"Doc '{doc_file}' ingested")
 
-    texts = text_splitter.split_text(super_text)
+        texts = text_splitter.split_text(super_text)
 
-    for text in texts:
-        document = Document(page_content=text, metadata={"title": doc_file, "link": "", "type": "document"})
-        documents.append(document)
+        for text in texts:
+            document = Document(page_content=text, metadata={"title": doc_file, "link": "", "type": "document"})
+            documents.append(document)
 
     # Store Embeddings in FAISS
     for i in tqdm(range(0,1), "Creating db from documents"):
         db = vectorstore.from_documents(documents, embeddings)
     return db
```

### Comparing `miner_ai_beta-0.1.5/miner_ai_beta/loader/excels.py` & `miner_ai_beta-0.1.6/miner_ai_beta/loader/excels.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from langchain.docstore.document import Document
 import pandas as pd
 from tqdm import tqdm
+import re
 
 def IndexFromXlss(folder_path: str, embeddings, vectorstore, chunk_size: int = 2000):
     """
     ## Load excel from folder
     This function loads documents from a folder and creates a Fass index (db).\n
     - folder_path: Path to folder containing PDFs\n
     - chunk_size: Chunk size in characters (default 2000)\n
@@ -18,27 +19,28 @@
     # Assuming your PDFs are in a folder named 'test_pdfs'
     xls_files = [f for f in os.listdir(folder_path) if f.endswith('.xlsx')]
 
     documents = []
     # Process each PDF file and split into chunks of 24000 characters
     text_splitter = RecursiveCharacterTextSplitter(chunk_size=chunk_size, chunk_overlap=0, length_function=len, is_separator_regex=False) # FIXED
 
-    super_text = ""
     documents = []
     # Process each PDF file
     for xls_file in tqdm(xls_files, "Parsing excels"):
+        super_text = ""
         sheets_dict = pd.read_excel(os.path.join(folder_path, xls_file), sheet_name=None)
         for sheet_name, df in sheets_dict.items():
             total_text = df.to_string()
             super_text += total_text   
-                
-    texts = text_splitter.split_text(super_text)
 
-    for text in texts:
-        document = Document(page_content=text, metadata={"title": xls_file, "link": "", "type": "document"})
-        documents.append(document)
+        super_text = re.sub('[\s+]', '', super_text)        
+        texts = text_splitter.split_text(super_text)
+
+        for text in texts:
+            document = Document(page_content=text, metadata={"title": xls_file, "link": "", "type": "document"})
+            documents.append(document)
 
 
     # Store Embeddings in FAISS
     for i in tqdm(range(0,1), "Creating db from documents"):  
         db = vectorstore.from_documents(documents, embeddings)
     return db
```

### Comparing `miner_ai_beta-0.1.5/miner_ai_beta/loader/pdfs.py` & `miner_ai_beta-0.1.6/miner_ai_beta/loader/pdfs.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,18 +25,18 @@
     # Process each PDF file
     for pdf_file in tqdm(pdf_files, "Parsing pdfs"):
         with pdfplumber.open(os.path.join(folder_path, pdf_file)) as pdf:
             total_text = ''
             for page in pdf.pages:
                 total_text += page.extract_text() or ''  # Extract text from each page
         
-    texts = text_splitter.split_text(total_text)
+        texts = text_splitter.split_text(total_text)
 
-    for text in texts:
-        document = Document(page_content=text, metadata={"title": pdf_file, "link": "", "type": "document"})
-        documents.append(document)
+        for text in texts:
+            document = Document(page_content=text, metadata={"title": pdf_file, "link": "", "type": "document"})
+            documents.append(document)
 
 
     # Store Embeddings in FAISS
     for i in tqdm(range(0,1), "Creating db from documents"):
         db = vectorstore.from_documents(documents, embeddings)
     return db
```

### Comparing `miner_ai_beta-0.1.5/miner_ai_beta/loader/ppts.py` & `miner_ai_beta-0.1.6/miner_ai_beta/loader/ppts.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,18 +27,18 @@
         prs = Presentation(ppt_file)
         total_text = ''
         for slide in prs.slides:
             for shape in slide.shapes:
                 if shape.has_text_frame:
                     total_text += str(shape.text) # Extract text from each page
         
-    texts = text_splitter.split_text(total_text)
+        texts = text_splitter.split_text(total_text)
 
-    for text in texts:
-        document = Document(page_content=text, metadata={"title": ppt_file, "link": "", "type": "document"})
-        documents.append(document)
+        for text in texts:
+            document = Document(page_content=text, metadata={"title": ppt_file, "link": "", "type": "document"})
+            documents.append(document)
 
 
     # Store Embeddings in FAISS
     for i in tqdm(range(0,1), "Creating db from documents"):
         db = vectorstore.from_documents(documents, embeddings)
     return db
```

### Comparing `miner_ai_beta-0.1.5/miner_ai_beta/loader/tubes.py` & `miner_ai_beta-0.1.6/miner_ai_beta/loader/tubes.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,18 +28,19 @@
         title = YouTube(tube).title
         tube_id = tube.split("https://www.youtube.com/watch?v=")[1] 
         transcripts = YouTubeTranscriptApi.get_transcript(tube_id)
         for transcript in transcripts:
             time = datetime.timedelta(0,transcript["start"])
             current_text = transcript["text"]
             total_text += f"text: {current_text}, at: {time}\n"
-    texts = text_splitter.split_text(total_text)
+            
+        texts = text_splitter.split_text(total_text)
 
-    for text in texts:
-        document = Document(page_content=text, metadata={"title": title, "link": tube, "type": "video"})
-        documents.append(document)
+        for text in texts:
+            document = Document(page_content=text, metadata={"title": title, "link": tube, "type": "video"})
+            documents.append(document)
 
 
     # Store Embeddings in FAISS
     for i in tqdm(range(0,1), "Creating db from documents"):
         db = vectorstore.from_documents(documents, embeddings)
     return db
```

### Comparing `miner_ai_beta-0.1.5/miner_ai_beta/loader/web_pages.py` & `miner_ai_beta-0.1.6/miner_ai_beta/loader/web_pages.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,17 +30,17 @@
             elements = soup.find_all("body") # Get all body elements (IMP) otherwise it retrieve all the html code
             for element in elements:
                 super_text += element.get_text()  
             print(f"Page '{title}' ingested")
         else:
             print(f"--> X '{page}' gave error")
     
-    texts = text_splitter.split_text(super_text)
+        texts = text_splitter.split_text(super_text)
 
-    for text in texts:
-        document = Document(page_content=text, metadata={"title": title, "link": page, "type": "site"})
-        documents.append(document)
+        for text in texts:
+            document = Document(page_content=text, metadata={"title": title, "link": page, "type": "site"})
+            documents.append(document)
 
     # Store Embeddings in FAISS
     for i in tqdm(range(0,1), "Creating db from documents"):
         db = vectorstore.from_documents(documents, embeddings)
     return db
```

### Comparing `miner_ai_beta-0.1.5/pyproject.toml` & `miner_ai_beta-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "miner-ai-beta"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 license = "MIT"
 authors = ["Valerio Domenici <valeriodomenici93@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Valerio357/miner-ai"
 keywords = ["langchain", "documents_mining", "web_scraping"]
```

### Comparing `miner_ai_beta-0.1.5/README.md` & `miner_ai_beta-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `miner_ai_beta-0.1.5/PKG-INFO` & `miner_ai_beta-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miner-ai-beta
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Home-page: https://github.com/Valerio357/miner-ai
 License: MIT
 Keywords: langchain,documents_mining,web_scraping
 Author: Valerio Domenici
 Author-email: valeriodomenici93@gmail.com
 Requires-Python: >=3.12,<4.0
```

