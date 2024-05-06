# Comparing `tmp/twelvelabs-0.1.22.tar.gz` & `tmp/twelvelabs-0.1.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twelvelabs-0.1.22.tar", last modified: Wed Apr 24 08:07:45 2024, max compression
+gzip compressed data, was "twelvelabs-0.1.23.tar", last modified: Mon May  6 14:49:00 2024, max compression
```

## Comparing `twelvelabs-0.1.22.tar` & `twelvelabs-0.1.23.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 zini       (501) staff       (20)        0 2024-04-24 08:07:45.642258 twelvelabs-0.1.22/
--rw-r--r--   0 zini       (501) staff       (20)    10306 2024-04-09 04:06:21.000000 twelvelabs-0.1.22/LICENSE
--rw-r--r--   0 zini       (501) staff       (20)    14535 2024-04-24 08:07:45.641589 twelvelabs-0.1.22/PKG-INFO
--rw-r--r--   0 zini       (501) staff       (20)    14147 2024-04-09 04:06:21.000000 twelvelabs-0.1.22/README.md
--rw-r--r--   0 zini       (501) staff       (20)       38 2024-04-24 08:07:45.642308 twelvelabs-0.1.22/setup.cfg
--rw-r--r--   0 zini       (501) staff       (20)      700 2024-04-24 08:07:20.000000 twelvelabs-0.1.22/setup.py
-drwxr-xr-x   0 zini       (501) staff       (20)        0 2024-04-24 08:07:45.636607 twelvelabs-0.1.22/twelvelabs/
--rw-r--r--   0 zini       (501) staff       (20)      768 2024-02-02 15:17:34.000000 twelvelabs-0.1.22/twelvelabs/__init__.py
--rw-r--r--   0 zini       (501) staff       (20)     3955 2024-02-02 15:17:34.000000 twelvelabs-0.1.22/twelvelabs/base_client.py
--rw-r--r--   0 zini       (501) staff       (20)     1371 2024-02-02 15:17:34.000000 twelvelabs-0.1.22/twelvelabs/client.py
--rw-r--r--   0 zini       (501) staff       (20)      313 2024-02-02 15:17:34.000000 twelvelabs-0.1.22/twelvelabs/constants.py
--rw-r--r--   0 zini       (501) staff       (20)     2069 2024-02-02 15:17:34.000000 twelvelabs-0.1.22/twelvelabs/exceptions.py
-drwxr-xr-x   0 zini       (501) staff       (20)        0 2024-04-24 08:07:45.638799 twelvelabs-0.1.22/twelvelabs/models/
--rw-r--r--   0 zini       (501) staff       (20)     1034 2024-02-02 15:17:34.000000 twelvelabs-0.1.22/twelvelabs/models/__init__.py
--rw-r--r--   0 zini       (501) staff       (20)      459 2024-02-02 15:17:34.000000 twelvelabs-0.1.22/twelvelabs/models/_base.py
--rw-r--r--   0 zini       (501) staff       (20)      164 2024-04-09 04:06:21.000000 twelvelabs-0.1.22/twelvelabs/models/engine.py
--rw-r--r--   0 zini       (501) staff       (20)      782 2024-02-02 15:17:34.000000 twelvelabs-0.1.22/twelvelabs/models/generate.py
--rw-r--r--   0 zini       (501) staff       (20)     7060 2024-03-07 05:18:58.000000 twelvelabs-0.1.22/twelvelabs/models/index.py
--rw-r--r--   0 zini       (501) staff       (20)     2066 2024-03-07 07:44:40.000000 twelvelabs-0.1.22/twelvelabs/models/search.py
--rw-r--r--   0 zini       (501) staff       (20)     2888 2024-04-09 04:06:21.000000 twelvelabs-0.1.22/twelvelabs/models/task.py
--rw-r--r--   0 zini       (501) staff       (20)     4408 2024-04-09 04:15:10.000000 twelvelabs-0.1.22/twelvelabs/models/video.py
--rw-r--r--   0 zini       (501) staff       (20)      505 2024-03-04 08:47:21.000000 twelvelabs-0.1.22/twelvelabs/resource.py
-drwxr-xr-x   0 zini       (501) staff       (20)        0 2024-04-24 08:07:45.640358 twelvelabs-0.1.22/twelvelabs/resources/
--rw-r--r--   0 zini       (501) staff       (20)      228 2024-02-02 15:17:34.000000 twelvelabs-0.1.22/twelvelabs/resources/__init__.py
--rw-r--r--   0 zini       (501) staff       (20)      424 2024-02-02 15:17:34.000000 twelvelabs-0.1.22/twelvelabs/resources/engine.py
--rw-r--r--   0 zini       (501) staff       (20)     1551 2024-03-07 05:51:31.000000 twelvelabs-0.1.22/twelvelabs/resources/generate.py
--rw-r--r--   0 zini       (501) staff       (20)     4737 2024-03-07 05:40:16.000000 twelvelabs-0.1.22/twelvelabs/resources/index.py
--rw-r--r--   0 zini       (501) staff       (20)     2671 2024-02-24 15:37:49.000000 twelvelabs-0.1.22/twelvelabs/resources/search.py
--rw-r--r--   0 zini       (501) staff       (20)     7380 2024-04-24 08:05:51.000000 twelvelabs-0.1.22/twelvelabs/resources/task.py
--rw-r--r--   0 zini       (501) staff       (20)     7646 2024-03-07 07:39:37.000000 twelvelabs-0.1.22/twelvelabs/resources/video.py
-drwxr-xr-x   0 zini       (501) staff       (20)        0 2024-04-24 08:07:45.640958 twelvelabs-0.1.22/twelvelabs/types/
--rw-r--r--   0 zini       (501) staff       (20)       58 2024-02-02 15:17:34.000000 twelvelabs-0.1.22/twelvelabs/types/__init__.py
--rw-r--r--   0 zini       (501) staff       (20)      104 2024-02-02 15:17:34.000000 twelvelabs-0.1.22/twelvelabs/types/index.py
--rw-r--r--   0 zini       (501) staff       (20)      885 2024-03-07 07:39:37.000000 twelvelabs-0.1.22/twelvelabs/util.py
-drwxr-xr-x   0 zini       (501) staff       (20)        0 2024-04-24 08:07:45.641212 twelvelabs-0.1.22/twelvelabs.egg-info/
--rw-r--r--   0 zini       (501) staff       (20)    14535 2024-04-24 08:07:45.000000 twelvelabs-0.1.22/twelvelabs.egg-info/PKG-INFO
--rw-r--r--   0 zini       (501) staff       (20)      851 2024-04-24 08:07:45.000000 twelvelabs-0.1.22/twelvelabs.egg-info/SOURCES.txt
--rw-r--r--   0 zini       (501) staff       (20)        1 2024-04-24 08:07:45.000000 twelvelabs-0.1.22/twelvelabs.egg-info/dependency_links.txt
--rw-r--r--   0 zini       (501) staff       (20)       30 2024-04-24 08:07:45.000000 twelvelabs-0.1.22/twelvelabs.egg-info/requires.txt
--rw-r--r--   0 zini       (501) staff       (20)       11 2024-04-24 08:07:45.000000 twelvelabs-0.1.22/twelvelabs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:49:00.338317 twelvelabs-0.1.23/
+-rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16749 2024-05-06 14:49:00.338317 twelvelabs-0.1.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14147 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 14:49:00.338317 twelvelabs-0.1.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:49:00.334317 twelvelabs-0.1.23/twelvelabs/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3985 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:49:00.338317 twelvelabs-0.1.23/twelvelabs/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/models/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/models/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/models/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7099 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/models/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/models/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/models/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:49:00.338317 twelvelabs-0.1.23/twelvelabs/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/resources/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/resources/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/resources/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/resources/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7466 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/resources/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7783 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/resources/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:49:00.338317 twelvelabs-0.1.23/twelvelabs/types/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/types/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-06 14:48:50.000000 twelvelabs-0.1.23/twelvelabs/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 14:49:00.338317 twelvelabs-0.1.23/twelvelabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16749 2024-05-06 14:49:00.000000 twelvelabs-0.1.23/twelvelabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-06 14:49:00.000000 twelvelabs-0.1.23/twelvelabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 14:49:00.000000 twelvelabs-0.1.23/twelvelabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-06 14:49:00.000000 twelvelabs-0.1.23/twelvelabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 14:49:00.000000 twelvelabs-0.1.23/twelvelabs.egg-info/top_level.txt
```

### Comparing `twelvelabs-0.1.22/LICENSE` & `twelvelabs-0.1.23/LICENSE`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.22/PKG-INFO` & `twelvelabs-0.1.23/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: twelvelabs
-Version: 0.1.22
-Summary: SDK for Twelve Labs API
-Home-page: https://github.com/twelvelabs-io/twelvelabs-python
-Author: Twelve Labs
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pydantic==2.4.2
-Requires-Dist: httpx==0.25.2
-
 # TwelveLabs Python SDK
 
 This SDK provides a convenient way to interact with the Twelve Labs Video Understanding Platform from an application written in the Python language. The SDK equips you with a set of intuitive classes and methods that streamline the process of interacting with the platform, minimizing the need for boilerplate code.
 
 # Prerequisites
 
 Ensure that the following prerequisites are met before using the SDK:
```

### Comparing `twelvelabs-0.1.22/README.md` & `twelvelabs-0.1.23/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,281 +1,293 @@
-# TwelveLabs Python SDK
-
-This SDK provides a convenient way to interact with the Twelve Labs Video Understanding Platform from an application written in the Python language. The SDK equips you with a set of intuitive classes and methods that streamline the process of interacting with the platform, minimizing the need for boilerplate code.
-
-# Prerequisites
-
-Ensure that the following prerequisites are met before using the SDK:
-
--  [Python](https://www.python.org) 3.7 or newer must be installed on your machine.
--  You have an API key. If you don't have an account, please [sign up](https://api.twelvelabs.io/) for a free account. Then, to retrieve your API key, go to the [Dashboard](https://api.twelvelabs.io/dashboard) page, and select the **Copy** icon to the right of the key to copy it to your clipboard.
-
-# Install the SDK
-
-Install the `twelvelabs` package:
-
- ```sh
- pip install twelvelabs
- ```
-
-
-# Initialize the SDK
-
-1. Import the SDK into your application:
-
-   ```py
-   from twelvelabs import TwelveLabs
-   ```
-
-2.  Instantiate the SDK client with your API key. This example code assumes that your API key is stored in an environment variable named `TL_API_KEY`:
-
-    ```py
-    client = TwelveLabs(api_key=os.getenv('TL_API_KEY'))
-    ```
-
-# Use the SDK
-
-To get started with the SDK, follow these basic steps:
-
-1. Create an index.
-2. Upload videos.
-3. Perform downstream tasks, such as searching or generating text from video.
-
-## Create an index
-
-To create an index, use the example code below, replacing "<YOUR_INDEX_NAME>" with the desired name for your index:
-
-```py
-from twelvelabs import APIStatusError
-
-index_obj = None
-try:
-    index_obj = client.index.create(
-        name = "<YOUR_INDEX_NAME>",
-        engines =[
-            {
-                "name": "marengo2.6",
-                "options": ["visual", "conversation", "text_in_video"],
-            },
-            {
-                "name": "pegasus1",
-                "options": ["visual", "conversation"],
-            },
-        ],
-    )
-    print(index_obj)
-except APIStatusError as e:
-    print('API Status Error, 4xx or 5xx')
-    print(e)
-except Exception as e:
-    print(e)
-```
-
-Note the following about this example:
-- The platform provides two distinct engine types - embedding and generative, each serving unique purposes in multimodal video understanding.
-  - **Embedding engines (Marengo)**: These engines are proficient at performing tasks such as search and classification, enabling enhanced video understanding.
-  - **Generative engines (Pegasus)**: These engines generate text based on your videos.
-  For your index, both Marengo and Pegasus are enabled.
-- The `engines.options` fields specify the types of information each video understanding engine will process.
-- The engines and the engine options specified when you create an index apply to all the videos you upload to that index and cannot be changed. For details, see the [Engine options](https://docs.twelvelabs.io/v1.2/docs/engine-options) page.
-
-The output should look similar to the following:
-
-```
-Index(id='65b1b926560f741da96836d7', created_at='2024-01-25T01:28:06.061Z', updated_at='2024-01-25T01:28:06.061Z', name='test-index-to-researchers1', engines=[Engine(name='marengo2.6', options=['visual', 'conversation', 'text_in_video'], addons=None), Engine(name='pegasus1', options=['visual', 'conversation'], addons=None)], video_count=0, total_duration=0.0, expires_at='2024-04-24T01:28:06.061Z')
-```
-
-Note that the API returns, among other information, a field named `id`, representing the unique identifier of your new index.
-
-For a description of each field in the request and response, see the [Create an index](https://docs.twelvelabs.io/v1.2/reference/create-index) page.
-
-
-## Upload videos
-
-Before you upload a video to the platform, ensure that it meets the following requirements:
-
-- **Video resolution**: Must be greater or equal than 360p and less or equal than 4K. For consistent search results, Twelve Labs recommends you upload 360p videos.
-- **Video and audio formats**:  The video files you wish to upload must be encoded in the video and audio formats listed on the [FFmpeg Formats Documentation](https://ffmpeg.org/ffmpeg-formats.html) page. For videos in other formats, contact us at [support@twelvelabs.io](mailto:support@twelvelabs.io).
-- **Duration**: For Marengo, it must be between 4 seconds and 2 hours (7,200s). For Pegasus, it must be between 4 seconds and 20 minutes (1200s).
-- **File size**: Must not exceed 2 GB. If you require different options, send us an email at support@twelvelabs.io.
-- **Audio track**: If the `conversation` [engine option](https://docs.twelvelabs.io/v1.2/docs/engine-options) is selected, the video you're uploading must contain an audio track.
-
-To upload videos, use the example code below, replacing the following:
-
-- **`<YOUR_VIDEO_PATH>`**: with a string representing the path to the directory containing the video files you wish to upload.
-- **`<YOUR_INDEX_ID>`**: with a string representing the unique identifier of the index to which you want to upload your video.
-
-
-```py
-from glob import glob
-from twelvelabs.models.task import Task
-
-video_files = glob("<YOUR_VIDEO_PATH>") # Example: "/videos/*.mp4
-for video_file in video_files:
-  print(f"Uploading {video_file}")
-  task = client.task.create(index_id="<YOUR_INDEX_ID>", file=video_file, language="en")
-  print(f"Task id={task.id}")
-
-  # (Optional) Monitor the video indexing process
-  # Utility function to print the status of a video indexing task
-  def on_task_update(task: Task):
-          print(f"  Status={task.status}")
-  task.wait_for_done(callback=on_task_update)
-  if task.status != "ready":
-      raise RuntimeError(f"Indexing failed with status {task.status}")
-  print(f"Uploaded {video_file}. The unique identifer of your video is {task.video_id}.")
-```
-
-Note that once a video has been successfully uploaded and indexed, the response will contain a field named `video_id`, representing the unique identifier of your video.
-
-For a description of each field in the request and response, see the [Create a video indexing task](https://docs.twelvelabs.io/reference/create-video-indexing-task) page.
-
-## Perform downstream tasks
-
-The sections below show how you can perform the most common downstream tasks. See [our documentation](https://docs.twelvelabs.io/docs) for a complete list of all the features the Twelve Labs Understanding Platform provides.
-
-### Search
-
-To perform a search request, use the example code below, replacing the following:
-
-- **`<YOUR_INDEX_ID>`**: with a string representing the unique identifier of your index.
-- **`<YOUR_QUERY>`**: with a string representing your search query. Note that the API supports full natural language-based search. The following examples are valid queries: "birds flying near a castle," "sun shining on water," and "an officer holding a child's hand."
-- **`[<YOUR_SEARCH_OPTIONS>]`**: with an array of strings that specifies the sources of information the platform uses when performing a search. For example, to search based on visual and conversation cues, use `["visual", "conversation"]`. Note that the search options you specify must be a subset of the engine options used when you created the index. For more details, see the [Search options](https://docs.twelvelabs.io/docs/search-options) page. 
-
-```py
-search_results = client.search.query("<YOUR_INDEX_ID>", "<YOUR_QUERY>", ["<YOUR_SEARCH_OPTIONS>"])
-
-# Utility function to print a specific page
-def print_page(page):
-  for clip in page:
-    print(
-        f" video_id={clip.video_id} score={clip.score} start={clip.start} end={clip.end} confidence={clip.confidence}"
-    )
-
-print_page(search_results.data)
-
-while True:
-    try:
-        print_page(next(search_results))
-    except StopIteration:
-        break
-```
-
-The results are returned one page at a time, with a default limit of 10 results on each page. The `next ` method returns the next page of results. When you've reached the end of the dataset, a `StopIteration` exception is raised.
-
-```
- video_id=65ca2bce48db9fa780cb3fa4 score=84.9 start=104.9375 end=111.90625 confidence=high
- video_id=65ca2bce48db9fa780cb3fa4 score=84.82 start=160.46875 end=172.75 confidence=high
- video_id=65ca2bce48db9fa780cb3fa4 score=84.77 start=55.375 end=72.46875 confidence=high
-```
-
-
-Note that the response contains, among other information, the following fields:
-- `video_id`: The unique identifier of the video that matched your search terms.
-- `score`: A quantitative value determined by the AI engine representing the level of confidence that the results match your search terms.
-- `start`: The start time of the matching video clip, expressed in seconds.
-- `end`: The end time of the matching video clip, expressed in seconds.
-- `confidence`: A qualitative indicator based on the value of the score field. This field can take one of the following values:
-  - `high`
-  - `medium`
-  - `low`
-  - `extremely low`
-
-
-For a description of each field in the request and response, see the [Make a search request](https://docs.twelvelabs.io/v1.2/reference/make-search-request) page.
-
-### Generate text from video
-
-The Twelve Labs Video Understanding Platform offers three distinct endpoints tailored to meet various requirements. Each endpoint has been designed with specific levels of flexibility and customization to accommodate different needs.
-
-Note the following about using these endpoints:
-- The Pegasus video understanding engine must be enabled for the index to which your video has been uploaded.
-- Your prompts must be instructive or descriptive, and you should not phrase them as questions.
-- The maximum length of a prompt is 300 characters.
-
-#### Topics, titles, and hashtags
-
-To generate topics, titles, and hashtags, use the example code below, replacing the following:
-
-- **`<YOUR_VIDEO_ID>`**: with a string representing the unique identifier of your video.
-- **`[<TYPES>]`**: with an array of strings representing the type of text the platform should generate. Example: `["title", "topic", "hashtag"]`.
-
-```py
-res = client.generate.gist("<YOUR_VIDEO_ID>", types=["<TYPES>"])
-print(f"Title = {res.title}\nTopics = {res.topics}\nHashtags = {res.hashtags}")
-```
-
-For a description of each field in the request and response, see the [Titles, topics, or hashtags](https://docs.twelvelabs.io/v1.2/reference/generate-gist) page.
-
-#### Summaries, chapters, and highlights
-
-To generate summaries, chapters, and highlights, use the example code below, replacing the following:
-
-- **`<YOUR_VIDEO_ID>`**: with a string representing the unique identifier of your video.
-- **`<TYPE>`**: with a string representing the type of text the platform should generate. This parameter can take one of the following values: "summary", "chapter", or "highlight".
-- _(Optional)_ **`<YOUR_PROMPT>`**: with a string that provides context for the summarization task, such as the target audience, style, tone of voice, and purpose. Example:  "Generate a summary in no more than 5 bullet points."
-
-
-```py
-res = client.generate.summarize("<YOUR_VIDEO_ID>", type="<TYPE>", prompt="<YOUR_PROMPT>")
-print(f"{res.summary}")
-```
-
-For a description of each field in the request and response, see the [Summaries, chapters, or highlights](https://docs.twelvelabs.io/v1.2/docs/generate-summaries-chapters-highlights) page.
-
-#### Open-ended texts
-
-To generate open-ended texts, use the example code below, replacing the following:
-- **`<YOUR_VIDEO_ID>`**: with a string representing the unique identifier of your video.
-- **`<YOUR_PROMPT>`**: with a string that guides the model on the desired format or content. The maximum length of the prompt is 500 tokens or roughly 350 words. Example:  "I want to generate a description for my video with the following format: Title of the video, followed by a summary in 2-3 sentences, highlighting the main topic, key events, and concluding remarks."
-
-```py
-res = client.generate.text(video_id="<YOUR_VIDEO_ID>", prompt="<YOUR_PROMPT>")
-print(f"{res.data}")
-```
-
-## Error Handling
-
-The SDK includes a set of exceptions that are mapped to specific HTTP status codes, as shown in the table below:
-
-| Exception | HTTP Status Code |
-|----------|----------|
-| BadRequestError| 400 |
-| AuthenticationError | 401 |
-| PermissionDeniedError  | 403 |
-| NotFoundError | 404 |
-| ConflictError | 409 |
-| UnprocessableEntityError | 422 |
-| RateLimitError | 429 |
-| InternalServerError | 5xx |
-
-The following example shows how you can handle specific HTTP errors in your application:
-
-```python
-import os
-from twelvelabs import TwelveLabs
-
-client = TwelveLabs(os.getenv("TWELVELABS_API_KEY"))
-try:
-    engines = client.engines.list()
-    print(engines)
-except twelvelabs.APIConnectionError as e:
-    print("Cannot connect to API server")
-except twelvelabs.BadRequestError as e:
-    print("Bad request.")
-except twelvelabs.APIStatusError as e:
-    print(f"Status code {e.status_code} received")
-    print(e.response)
-```
-
-# License
-
-We use the Developer Certificate of Origin (DCO) in lieu of a Contributor License Agreement for all contributions to Twelve Labs' open-source projects. We request that contributors agree to the terms of the DCO and indicate that agreement by signing all commits made to Twelve Labs' projects by adding a line with your name and email address to every Git commit message contributed, as shown in the example below:
-
-```
-Signed-off-by: Jane Doe <jane.doe@example.com>
-```
-
-You can sign your commit automatically with Git by using `git commit -s` if you have your `user.name` and `user.email` set as part of your Git configuration.
-We ask that you use your real name (please, no anonymous contributions or pseudonyms). By signing your commitment, you are certifying that you have the right have the right to submit it under the open-source license used by that particular project. You must use your real name (no pseudonyms or anonymous contributions are allowed.)
-We use the Probot DCO GitHub app to check for DCO signoffs of every commit.
-If you forget to sign your commits, the DCO bot will remind you and give you detailed instructions for how to amend your commits to add a signature.
+Metadata-Version: 2.1
+Name: twelvelabs
+Version: 0.1.23
+Summary: SDK for Twelve Labs API
+Home-page: https://github.com/twelvelabs-io/twelvelabs-python
+Author: Twelve Labs
+License: UNKNOWN
+Description: # TwelveLabs Python SDK
+        
+        This SDK provides a convenient way to interact with the Twelve Labs Video Understanding Platform from an application written in the Python language. The SDK equips you with a set of intuitive classes and methods that streamline the process of interacting with the platform, minimizing the need for boilerplate code.
+        
+        # Prerequisites
+        
+        Ensure that the following prerequisites are met before using the SDK:
+        
+        -  [Python](https://www.python.org) 3.7 or newer must be installed on your machine.
+        -  You have an API key. If you don't have an account, please [sign up](https://api.twelvelabs.io/) for a free account. Then, to retrieve your API key, go to the [Dashboard](https://api.twelvelabs.io/dashboard) page, and select the **Copy** icon to the right of the key to copy it to your clipboard.
+        
+        # Install the SDK
+        
+        Install the `twelvelabs` package:
+        
+         ```sh
+         pip install twelvelabs
+         ```
+        
+        
+        # Initialize the SDK
+        
+        1. Import the SDK into your application:
+        
+           ```py
+           from twelvelabs import TwelveLabs
+           ```
+        
+        2.  Instantiate the SDK client with your API key. This example code assumes that your API key is stored in an environment variable named `TL_API_KEY`:
+        
+            ```py
+            client = TwelveLabs(api_key=os.getenv('TL_API_KEY'))
+            ```
+        
+        # Use the SDK
+        
+        To get started with the SDK, follow these basic steps:
+        
+        1. Create an index.
+        2. Upload videos.
+        3. Perform downstream tasks, such as searching or generating text from video.
+        
+        ## Create an index
+        
+        To create an index, use the example code below, replacing "<YOUR_INDEX_NAME>" with the desired name for your index:
+        
+        ```py
+        from twelvelabs import APIStatusError
+        
+        index_obj = None
+        try:
+            index_obj = client.index.create(
+                name = "<YOUR_INDEX_NAME>",
+                engines =[
+                    {
+                        "name": "marengo2.6",
+                        "options": ["visual", "conversation", "text_in_video"],
+                    },
+                    {
+                        "name": "pegasus1",
+                        "options": ["visual", "conversation"],
+                    },
+                ],
+            )
+            print(index_obj)
+        except APIStatusError as e:
+            print('API Status Error, 4xx or 5xx')
+            print(e)
+        except Exception as e:
+            print(e)
+        ```
+        
+        Note the following about this example:
+        - The platform provides two distinct engine types - embedding and generative, each serving unique purposes in multimodal video understanding.
+          - **Embedding engines (Marengo)**: These engines are proficient at performing tasks such as search and classification, enabling enhanced video understanding.
+          - **Generative engines (Pegasus)**: These engines generate text based on your videos.
+          For your index, both Marengo and Pegasus are enabled.
+        - The `engines.options` fields specify the types of information each video understanding engine will process.
+        - The engines and the engine options specified when you create an index apply to all the videos you upload to that index and cannot be changed. For details, see the [Engine options](https://docs.twelvelabs.io/v1.2/docs/engine-options) page.
+        
+        The output should look similar to the following:
+        
+        ```
+        Index(id='65b1b926560f741da96836d7', created_at='2024-01-25T01:28:06.061Z', updated_at='2024-01-25T01:28:06.061Z', name='test-index-to-researchers1', engines=[Engine(name='marengo2.6', options=['visual', 'conversation', 'text_in_video'], addons=None), Engine(name='pegasus1', options=['visual', 'conversation'], addons=None)], video_count=0, total_duration=0.0, expires_at='2024-04-24T01:28:06.061Z')
+        ```
+        
+        Note that the API returns, among other information, a field named `id`, representing the unique identifier of your new index.
+        
+        For a description of each field in the request and response, see the [Create an index](https://docs.twelvelabs.io/v1.2/reference/create-index) page.
+        
+        
+        ## Upload videos
+        
+        Before you upload a video to the platform, ensure that it meets the following requirements:
+        
+        - **Video resolution**: Must be greater or equal than 360p and less or equal than 4K. For consistent search results, Twelve Labs recommends you upload 360p videos.
+        - **Video and audio formats**:  The video files you wish to upload must be encoded in the video and audio formats listed on the [FFmpeg Formats Documentation](https://ffmpeg.org/ffmpeg-formats.html) page. For videos in other formats, contact us at [support@twelvelabs.io](mailto:support@twelvelabs.io).
+        - **Duration**: For Marengo, it must be between 4 seconds and 2 hours (7,200s). For Pegasus, it must be between 4 seconds and 20 minutes (1200s).
+        - **File size**: Must not exceed 2 GB. If you require different options, send us an email at support@twelvelabs.io.
+        - **Audio track**: If the `conversation` [engine option](https://docs.twelvelabs.io/v1.2/docs/engine-options) is selected, the video you're uploading must contain an audio track.
+        
+        To upload videos, use the example code below, replacing the following:
+        
+        - **`<YOUR_VIDEO_PATH>`**: with a string representing the path to the directory containing the video files you wish to upload.
+        - **`<YOUR_INDEX_ID>`**: with a string representing the unique identifier of the index to which you want to upload your video.
+        
+        
+        ```py
+        from glob import glob
+        from twelvelabs.models.task import Task
+        
+        video_files = glob("<YOUR_VIDEO_PATH>") # Example: "/videos/*.mp4
+        for video_file in video_files:
+          print(f"Uploading {video_file}")
+          task = client.task.create(index_id="<YOUR_INDEX_ID>", file=video_file, language="en")
+          print(f"Task id={task.id}")
+        
+          # (Optional) Monitor the video indexing process
+          # Utility function to print the status of a video indexing task
+          def on_task_update(task: Task):
+                  print(f"  Status={task.status}")
+          task.wait_for_done(callback=on_task_update)
+          if task.status != "ready":
+              raise RuntimeError(f"Indexing failed with status {task.status}")
+          print(f"Uploaded {video_file}. The unique identifer of your video is {task.video_id}.")
+        ```
+        
+        Note that once a video has been successfully uploaded and indexed, the response will contain a field named `video_id`, representing the unique identifier of your video.
+        
+        For a description of each field in the request and response, see the [Create a video indexing task](https://docs.twelvelabs.io/reference/create-video-indexing-task) page.
+        
+        ## Perform downstream tasks
+        
+        The sections below show how you can perform the most common downstream tasks. See [our documentation](https://docs.twelvelabs.io/docs) for a complete list of all the features the Twelve Labs Understanding Platform provides.
+        
+        ### Search
+        
+        To perform a search request, use the example code below, replacing the following:
+        
+        - **`<YOUR_INDEX_ID>`**: with a string representing the unique identifier of your index.
+        - **`<YOUR_QUERY>`**: with a string representing your search query. Note that the API supports full natural language-based search. The following examples are valid queries: "birds flying near a castle," "sun shining on water," and "an officer holding a child's hand."
+        - **`[<YOUR_SEARCH_OPTIONS>]`**: with an array of strings that specifies the sources of information the platform uses when performing a search. For example, to search based on visual and conversation cues, use `["visual", "conversation"]`. Note that the search options you specify must be a subset of the engine options used when you created the index. For more details, see the [Search options](https://docs.twelvelabs.io/docs/search-options) page. 
+        
+        ```py
+        search_results = client.search.query("<YOUR_INDEX_ID>", "<YOUR_QUERY>", ["<YOUR_SEARCH_OPTIONS>"])
+        
+        # Utility function to print a specific page
+        def print_page(page):
+          for clip in page:
+            print(
+                f" video_id={clip.video_id} score={clip.score} start={clip.start} end={clip.end} confidence={clip.confidence}"
+            )
+        
+        print_page(search_results.data)
+        
+        while True:
+            try:
+                print_page(next(search_results))
+            except StopIteration:
+                break
+        ```
+        
+        The results are returned one page at a time, with a default limit of 10 results on each page. The `next ` method returns the next page of results. When you've reached the end of the dataset, a `StopIteration` exception is raised.
+        
+        ```
+         video_id=65ca2bce48db9fa780cb3fa4 score=84.9 start=104.9375 end=111.90625 confidence=high
+         video_id=65ca2bce48db9fa780cb3fa4 score=84.82 start=160.46875 end=172.75 confidence=high
+         video_id=65ca2bce48db9fa780cb3fa4 score=84.77 start=55.375 end=72.46875 confidence=high
+        ```
+        
+        
+        Note that the response contains, among other information, the following fields:
+        - `video_id`: The unique identifier of the video that matched your search terms.
+        - `score`: A quantitative value determined by the AI engine representing the level of confidence that the results match your search terms.
+        - `start`: The start time of the matching video clip, expressed in seconds.
+        - `end`: The end time of the matching video clip, expressed in seconds.
+        - `confidence`: A qualitative indicator based on the value of the score field. This field can take one of the following values:
+          - `high`
+          - `medium`
+          - `low`
+          - `extremely low`
+        
+        
+        For a description of each field in the request and response, see the [Make a search request](https://docs.twelvelabs.io/v1.2/reference/make-search-request) page.
+        
+        ### Generate text from video
+        
+        The Twelve Labs Video Understanding Platform offers three distinct endpoints tailored to meet various requirements. Each endpoint has been designed with specific levels of flexibility and customization to accommodate different needs.
+        
+        Note the following about using these endpoints:
+        - The Pegasus video understanding engine must be enabled for the index to which your video has been uploaded.
+        - Your prompts must be instructive or descriptive, and you should not phrase them as questions.
+        - The maximum length of a prompt is 300 characters.
+        
+        #### Topics, titles, and hashtags
+        
+        To generate topics, titles, and hashtags, use the example code below, replacing the following:
+        
+        - **`<YOUR_VIDEO_ID>`**: with a string representing the unique identifier of your video.
+        - **`[<TYPES>]`**: with an array of strings representing the type of text the platform should generate. Example: `["title", "topic", "hashtag"]`.
+        
+        ```py
+        res = client.generate.gist("<YOUR_VIDEO_ID>", types=["<TYPES>"])
+        print(f"Title = {res.title}\nTopics = {res.topics}\nHashtags = {res.hashtags}")
+        ```
+        
+        For a description of each field in the request and response, see the [Titles, topics, or hashtags](https://docs.twelvelabs.io/v1.2/reference/generate-gist) page.
+        
+        #### Summaries, chapters, and highlights
+        
+        To generate summaries, chapters, and highlights, use the example code below, replacing the following:
+        
+        - **`<YOUR_VIDEO_ID>`**: with a string representing the unique identifier of your video.
+        - **`<TYPE>`**: with a string representing the type of text the platform should generate. This parameter can take one of the following values: "summary", "chapter", or "highlight".
+        - _(Optional)_ **`<YOUR_PROMPT>`**: with a string that provides context for the summarization task, such as the target audience, style, tone of voice, and purpose. Example:  "Generate a summary in no more than 5 bullet points."
+        
+        
+        ```py
+        res = client.generate.summarize("<YOUR_VIDEO_ID>", type="<TYPE>", prompt="<YOUR_PROMPT>")
+        print(f"{res.summary}")
+        ```
+        
+        For a description of each field in the request and response, see the [Summaries, chapters, or highlights](https://docs.twelvelabs.io/v1.2/docs/generate-summaries-chapters-highlights) page.
+        
+        #### Open-ended texts
+        
+        To generate open-ended texts, use the example code below, replacing the following:
+        - **`<YOUR_VIDEO_ID>`**: with a string representing the unique identifier of your video.
+        - **`<YOUR_PROMPT>`**: with a string that guides the model on the desired format or content. The maximum length of the prompt is 500 tokens or roughly 350 words. Example:  "I want to generate a description for my video with the following format: Title of the video, followed by a summary in 2-3 sentences, highlighting the main topic, key events, and concluding remarks."
+        
+        ```py
+        res = client.generate.text(video_id="<YOUR_VIDEO_ID>", prompt="<YOUR_PROMPT>")
+        print(f"{res.data}")
+        ```
+        
+        ## Error Handling
+        
+        The SDK includes a set of exceptions that are mapped to specific HTTP status codes, as shown in the table below:
+        
+        | Exception | HTTP Status Code |
+        |----------|----------|
+        | BadRequestError| 400 |
+        | AuthenticationError | 401 |
+        | PermissionDeniedError  | 403 |
+        | NotFoundError | 404 |
+        | ConflictError | 409 |
+        | UnprocessableEntityError | 422 |
+        | RateLimitError | 429 |
+        | InternalServerError | 5xx |
+        
+        The following example shows how you can handle specific HTTP errors in your application:
+        
+        ```python
+        import os
+        from twelvelabs import TwelveLabs
+        
+        client = TwelveLabs(os.getenv("TWELVELABS_API_KEY"))
+        try:
+            engines = client.engines.list()
+            print(engines)
+        except twelvelabs.APIConnectionError as e:
+            print("Cannot connect to API server")
+        except twelvelabs.BadRequestError as e:
+            print("Bad request.")
+        except twelvelabs.APIStatusError as e:
+            print(f"Status code {e.status_code} received")
+            print(e.response)
+        ```
+        
+        # License
+        
+        We use the Developer Certificate of Origin (DCO) in lieu of a Contributor License Agreement for all contributions to Twelve Labs' open-source projects. We request that contributors agree to the terms of the DCO and indicate that agreement by signing all commits made to Twelve Labs' projects by adding a line with your name and email address to every Git commit message contributed, as shown in the example below:
+        
+        ```
+        Signed-off-by: Jane Doe <jane.doe@example.com>
+        ```
+        
+        You can sign your commit automatically with Git by using `git commit -s` if you have your `user.name` and `user.email` set as part of your Git configuration.
+        We ask that you use your real name (please, no anonymous contributions or pseudonyms). By signing your commitment, you are certifying that you have the right have the right to submit it under the open-source license used by that particular project. You must use your real name (no pseudonyms or anonymous contributions are allowed.)
+        We use the Probot DCO GitHub app to check for DCO signoffs of every commit.
+        If you forget to sign your commits, the DCO bot will remind you and give you detailed instructions for how to amend your commits to add a signature.
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
```

### Comparing `twelvelabs-0.1.22/setup.py` & `twelvelabs-0.1.23/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from setuptools import setup, find_packages
 from pathlib import Path
+import os
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
+version_file = os.path.join(os.path.dirname(__file__), "VERSION")
+with open(version_file, "r") as f:
+    version = f.read().strip()
 
 with open("requirements.txt") as f:
     required = f.read().splitlines()
 
 setup(
     name="twelvelabs",
-    version="0.1.22",
+    version=version,
     author="Twelve Labs",
     description="SDK for Twelve Labs API",
     url="https://github.com/twelvelabs-io/twelvelabs-python",
     packages=find_packages(),
     install_requires=required,
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `twelvelabs-0.1.22/twelvelabs/__init__.py` & `twelvelabs-0.1.23/twelvelabs/__init__.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.22/twelvelabs/base_client.py` & `twelvelabs-0.1.23/twelvelabs/base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             raise exceptions.APIConnectionError(request=response._request)
 
         try:
             response.raise_for_status()
         except httpx.HTTPStatusError as e:
             raise self._make_status_error(e.response)
 
-        if "application/json" in response.headers.get("Content-Type", ""):
+        if len(response.content) > 0 and "application/json" in response.headers.get("Content-Type", ""):
             return response.json()
         return response.text
 
     def _make_status_error(self, response: httpx.Response) -> APIStatusError:
         if response.is_closed and not response.is_stream_consumed:
             body = None
             err_msg = f"Error code: {response.status_code}"
```

### Comparing `twelvelabs-0.1.22/twelvelabs/client.py` & `twelvelabs-0.1.23/twelvelabs/client.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.22/twelvelabs/exceptions.py` & `twelvelabs-0.1.23/twelvelabs/exceptions.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.22/twelvelabs/models/__init__.py` & `twelvelabs-0.1.23/twelvelabs/models/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from ._base import Object, ObjectWithTimestamp, PageInfo
+from ._base import Object, ObjectWithTimestamp, PageInfo, RootModelList
 from .engine import Engine
 from .index import Index, IndexListWithPagination
 from .task import Task, TaskStatus, TaskListWithPagination
 from .video import Video, VideoValue, VideoListWithPagination
-from .search import SearchData, SearchPageInfo, SearchResult, CombinedSearchResult
+from .search import SearchData, SearchPageInfo, SearchResult, CombinedSearchResult, GroupByVideoSearchData
 from .generate import (
     GenerateOpenEndedTextResult,
     GenerateSummarizeChapterResult,
     GenerateSummarizeHighlightResult,
     GenerateSummarizeResult,
     GenerateGistResult,
 )
@@ -30,8 +30,9 @@
     "SearchResult",
     "CombinedSearchResult",
     "GenerateOpenEndedTextResult",
     "GenerateSummarizeChapterResult",
     "GenerateSummarizeHighlightResult",
     "GenerateSummarizeResult",
     "GenerateGistResult",
+    "RootModelList",
 ]
```

### Comparing `twelvelabs-0.1.22/twelvelabs/models/generate.py` & `twelvelabs-0.1.23/twelvelabs/models/generate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import List, Optional
 
-from ._base import BaseModel
+from ._base import BaseModel, RootModelList
 
 
 class GenerateOpenEndedTextResult(BaseModel):
     id: str
     data: str
 
 
@@ -21,16 +21,16 @@
     end: int
     highlight: str
 
 
 class GenerateSummarizeResult(BaseModel):
     id: str
     summary: Optional[str] = None
-    chapters: Optional[List[GenerateSummarizeChapterResult]] = None
-    highlights: Optional[List[GenerateSummarizeHighlightResult]] = None
+    chapters: Optional[RootModelList[GenerateSummarizeChapterResult]] = None
+    highlights: Optional[RootModelList[GenerateSummarizeHighlightResult]] = None
 
 
 class GenerateGistResult(BaseModel):
     id: str
     title: Optional[str] = None
     topics: Optional[List[str]] = None
     hashtags: Optional[List[str]] = None
```

### Comparing `twelvelabs-0.1.22/twelvelabs/models/index.py` & `twelvelabs-0.1.23/twelvelabs/models/index.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from typing import List, Optional, TYPE_CHECKING, Union, BinaryIO, Literal, Dict, Any
 from pydantic import Field, PrivateAttr
 
-from ._base import ModelMixin, BaseModel, ObjectWithTimestamp, PageInfo
+from ._base import ModelMixin, BaseModel, ObjectWithTimestamp, PageInfo, RootModelList
 
 if TYPE_CHECKING:
     from ..resources import Index as IndexResource
     from . import Task, TaskStatus, SearchResult, Video, VideoListWithPagination
 
 
 class Engine(BaseModel):
@@ -16,15 +16,15 @@
     addons: Optional[List[str]] = None
 
 
 class Index(ObjectWithTimestamp):
     _resource: IndexResource = PrivateAttr()
     name: str = Field(alias="index_name")
     # engine_id: str # v1.1
-    engines: List[Engine]
+    engines: RootModelList[Engine]
     # options: List[str] = Field(alias="index_options") # v1.1
     # addons: Optional[List[str]] # v1.1
     video_count: int
     total_duration: float
     expires_at: Optional[str] = None
 
     def __init__(self, resource: IndexResource, **data):
@@ -86,15 +86,15 @@
         updated_at: Optional[Union[str, Dict[str, str]]] = None,
         indexed_at: Optional[Union[str, Dict[str, str]]] = None,
         page: Optional[int] = None,
         page_limit: Optional[int] = None,
         sort_by: Optional[str] = None,
         sort_option: Optional[str] = None,
         **kwargs,
-    ) -> Video:
+    ) -> RootModelList[Video]:
         return self._resource.video.list(
             self.id,
             id=id,
             filename=filename,
             size=size,
             width=width,
             height=height,
```

### Comparing `twelvelabs-0.1.22/twelvelabs/models/search.py` & `twelvelabs-0.1.23/twelvelabs/models/search.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from typing import List, Optional, TYPE_CHECKING, Dict, Any, Union, Literal
 from pydantic import Field, PrivateAttr
 
-from ._base import BaseModel, ModelMixin
+from ._base import BaseModel, ModelMixin, RootModelList
 
 if TYPE_CHECKING:
     from ..resources import Search as SearchResource
 
 
 class SearchPool(BaseModel):
     total_count: int
@@ -25,55 +25,55 @@
     start: float
     end: float
     video_id: str
     metadata: Optional[List[Dict[str, Any]]] = None
     confidence: str
     thumbnail_url: Optional[str] = None
     module_confidence: Optional[Dict[str, Any]] = None
-    modules: Optional[List[SearchModule]] = None
+    modules: Optional[RootModelList[SearchModule]] = None
 
 
 class GroupByVideoSearchData(BaseModel):
-    clips: Optional[List[SearchData]] = None
+    clips: Optional[RootModelList[SearchData]] = None
     id: str
 
 
 class SearchPageInfo(BaseModel):
     limit_per_page: int
     total_results: int
     page_expired_at: str
     next_page_token: Optional[str] = None
     prev_page_token: Optional[str] = None
 
 
 class SearchResult(ModelMixin, BaseModel):
     _resource: SearchResource = PrivateAttr()
     pool: SearchPool = Field(alias="search_pool")
-    data: List[Union[SearchData, GroupByVideoSearchData]]
+    data: RootModelList[Union[SearchData, GroupByVideoSearchData]]
     page_info: SearchPageInfo
 
     def __init__(self, resource: SearchResource, **data):
         super().__init__(**data)
         self._resource = resource
 
     def __iter__(self):
         return self
 
-    def __next__(self) -> List[SearchData]:
+    def __next__(self) -> RootModelList[Union[SearchData, GroupByVideoSearchData]]:
         next_page_token = self.page_info.next_page_token
         if not next_page_token:
             raise StopIteration
 
         res = self._resource.by_page_token(next_page_token)
         self.page_info = res.page_info
         return res.data
 
 
 class CombinedSearchResult(SearchResult):
-    def __next__(self) -> List[SearchData]:
+    def __next__(self) -> RootModelList[SearchData]:
         next_page_token = self.page_info.next_page_token
         if not next_page_token:
             raise StopIteration
 
         res = self._resource.combined_by_page_token(next_page_token)
         self.page_info = res.page_info
         return res.data
```

### Comparing `twelvelabs-0.1.22/twelvelabs/models/task.py` & `twelvelabs-0.1.23/twelvelabs/models/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from typing import Optional, Dict, Any, Callable, List, TYPE_CHECKING
 from pydantic import PrivateAttr
 
-from ._base import ObjectWithTimestamp, BaseModel, ModelMixin, PageInfo
+from ._base import ObjectWithTimestamp, BaseModel, ModelMixin, PageInfo, RootModelList
 
 if TYPE_CHECKING:
     from ..resources import Task as TaskResource
 
 
 class TaskHLS(BaseModel):
     video_url: Optional[str] = None
@@ -67,26 +67,26 @@
                 callback(self)
         return self
 
 
 class TaskListWithPagination(ModelMixin, BaseModel):
     _resource: TaskResource = PrivateAttr()
     _origin_params: Dict[str, Any] = PrivateAttr()
-    data: List[Task] = []
+    data: RootModelList[Task] = []
     page_info: PageInfo
 
     def __init__(self, resource: TaskResource, origin_params: Dict[str, Any], **data):
         super().__init__(**data)
         self._resource = resource
         self._origin_params = origin_params
 
     def __iter__(self):
         return self
 
-    def __next__(self) -> List[Task]:
+    def __next__(self) -> RootModelList[Task]:
         if self.page_info.page >= self.page_info.total_page:
             raise StopIteration
         params = self._origin_params
         params["page"] = self.page_info.page + 1
         res = self._resource.list_pagination(**params)
         self.page_info = res.page_info
         return res.data
```

### Comparing `twelvelabs-0.1.22/twelvelabs/models/video.py` & `twelvelabs-0.1.23/twelvelabs/models/video.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from typing import Optional, TYPE_CHECKING, Dict, Any, List, Union, Literal
 from pydantic import PrivateAttr, Extra
 
-from ._base import ObjectWithTimestamp, BaseModel, ModelMixin, PageInfo
+from ._base import ObjectWithTimestamp, BaseModel, ModelMixin, PageInfo, RootModelList
 
 if TYPE_CHECKING:
     from ..resources import Video as VideoResource
     from . import (
         GeneratorGistResult,
         GenerateSummarizeResult,
         GenerateOpenEndedTextResult,
@@ -69,34 +69,34 @@
     ) -> None:
         return self._resource._client.index.video.delete(
             self._index_id, self.id, **kwargs
         )
 
     def transcription(
         self, *, start: Optional[float] = None, end: Optional[float] = None, **kwargs
-    ) -> List[VideoValue]:
+    ) -> RootModelList[VideoValue]:
         return self._resource._client.index.video.transcription(
             self._index_id, self.id, start=start, end=end, **kwargs
         )
 
     def text_in_video(
         self, *, start: Optional[float] = None, end: Optional[float] = None, **kwargs
-    ) -> List[VideoValue]:
+    ) -> RootModelList[VideoValue]:
         return self._resource._client.index.video.text_in_video(
             self._index_id, self.id, start=start, end=end, **kwargs
         )
 
     def logo(
         self, *, start: Optional[float] = None, end: Optional[float] = None, **kwargs
-    ) -> List[VideoValue]:
+    ) -> RootModelList[VideoValue]:
         return self._resource._client.index.video.logo(
             self._index_id, self.id, start=start, end=end, **kwargs
         )
 
-    def thumbnail(self, *, time: Optional[float] = None, **kwargs) -> List[VideoValue]:
+    def thumbnail(self, *, time: Optional[float] = None, **kwargs) -> str:
         return self._resource._client.index.video.thumbnail(
             self._index_id, self.id, time=time, **kwargs
         )
 
     # Generate relate methods
 
     def generate_gist(
@@ -124,26 +124,26 @@
             self.id, type, prompt=prompt, **kwargs
         )
 
 
 class VideoListWithPagination(ModelMixin, BaseModel):
     _resource: VideoResource = PrivateAttr()
     _origin_params: Dict[str, Any] = PrivateAttr()
-    data: List[Video] = []
+    data: RootModelList[Video] = []
     page_info: PageInfo
 
     def __init__(self, resource: VideoResource, origin_params: Dict[str, Any], **data):
         super().__init__(**data)
         self._resource = resource
         self._origin_params = origin_params
 
     def __iter__(self):
         return self
 
-    def __next__(self) -> List[Video]:
+    def __next__(self) -> RootModelList[Video]:
         if self.page_info.page >= self.page_info.total_page:
             raise StopIteration
         params = self._origin_params
         params["page"] = self.page_info.page + 1
         res = self._resource.list_pagination(**params)
         self.page_info = res.page_info
         return res.data
```

### Comparing `twelvelabs-0.1.22/twelvelabs/resources/generate.py` & `twelvelabs-0.1.23/twelvelabs/resources/generate.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.22/twelvelabs/resources/index.py` & `twelvelabs-0.1.23/twelvelabs/resources/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     Optional,
     Union,
     Literal,
     Dict,
     TYPE_CHECKING,
 )
 
+from ..models import RootModelList
 from ..resource import APIResource
 from .. import models
 from .. import types
 from ..util import remove_none_values, get_local_params, handle_comparison_params
 from .video import Video
 
 if TYPE_CHECKING:
@@ -41,15 +42,15 @@
         page: Optional[int] = 1,
         page_limit: Optional[int] = 10,
         sort_by: Optional[str] = "created_at",
         sort_option: Optional[str] = "desc",
         created_at: Optional[Union[str, Dict[str, str]]] = None,
         updated_at: Optional[Union[str, Dict[str, str]]] = None,
         **kwargs,
-    ) -> List[models.Index]:
+    ) -> RootModelList[models.Index]:
         params = {
             "_id": id,
             "index_name": name,
             "engine_options": engine_options,
             "engine_family": engine_family,
             "page": page,
             "page_limit": page_limit,
@@ -58,15 +59,15 @@
             "created_at": created_at,
             "updated_at": updated_at,
         }
         handle_comparison_params(params, "created_at", created_at)
         handle_comparison_params(params, "updated_at", updated_at)
         res = self._get("indexes", params=remove_none_values(params), **kwargs)
 
-        return [models.Index(self, **index) for index in res["data"]]
+        return RootModelList([models.Index(self, **index) for index in res["data"]])
 
     def list_pagination(
         self,
         *,
         id: Optional[str] = None,
         name: Optional[str] = None,
         engine_options: Optional[
```

### Comparing `twelvelabs-0.1.22/twelvelabs/resources/search.py` & `twelvelabs-0.1.23/twelvelabs/resources/search.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.22/twelvelabs/resources/task.py` & `twelvelabs-0.1.23/twelvelabs/resources/task.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Optional, Union, BinaryIO, List, Dict
 
+from ..models import RootModelList
 from ..resource import APIResource
 from .. import models
 from ..util import remove_none_values, get_local_params, handle_comparison_params
 
 
 class Task(APIResource):
     def retrieve(self, id: str, **kwargs) -> models.Task:
@@ -23,15 +24,15 @@
         updated_at: Optional[Union[str, Dict[str, str]]] = None,
         estimated_time: Optional[str] = None,
         page: Optional[int] = None,
         page_limit: Optional[int] = None,
         sort_by: Optional[str] = None,
         sort_option: Optional[str] = None,
         **kwargs,
-    ) -> List[models.Task]:
+    ) -> RootModelList[models.Task]:
         params = {
             "_id": id,
             "index_id": index_id,
             "filename": filename,
             "duration": duration,
             "width": width,
             "height": height,
@@ -42,15 +43,15 @@
             "page_limit": page_limit,
             "sort_by": sort_by,
             "sort_option": sort_option,
         }
         handle_comparison_params(params, "created_at", created_at)
         handle_comparison_params(params, "updated_at", updated_at)
         res = self._get("tasks", params=remove_none_values(params), **kwargs)
-        return [models.Task(self, **task) for task in res["data"]]
+        return RootModelList(   [models.Task(self, **task) for task in res["data"]])
 
     def list_pagination(
         self,
         *,
         id: Optional[str] = None,
         index_id: Optional[str] = None,
         filename: Optional[str] = None,
@@ -148,15 +149,15 @@
         index_id: str,
         *,
         files: Optional[List[Union[str, BinaryIO, None]]] = None,
         urls: Optional[List[str]] = None,
         language: Optional[str] = None,
         disable_video_stream: Optional[bool] = None,
         **kwargs,
-    ) -> List[models.Task]:
+    ) -> RootModelList[models.Task]:
         if not files and not urls:
             raise ValueError("Either files or urls must be provided")
 
         tasks = []
         if files:
             for file in files:
                 try:
@@ -183,15 +184,15 @@
                         **kwargs,
                     )
                     tasks.append(task)
                 except Exception as e:
                     print(f"Error processing url {url}: {e}")
                     continue
 
-        return tasks
+        return RootModelList(tasks)
 
     def delete(self, id: str, **kwargs) -> None:
         self._delete(f"tasks/{id}", **kwargs)
 
     def status(self, index_id: str, **kwargs) -> models.TaskStatus:
         params = {"index_id": index_id}
         res = self._get("tasks/status", params=params, **kwargs)
```

### Comparing `twelvelabs-0.1.22/twelvelabs/resources/video.py` & `twelvelabs-0.1.23/twelvelabs/resources/video.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Optional, List, Dict, Any, Union
 
+from ..models._base import RootModelList
 from ..resource import APIResource
 from .. import models
 from ..util import (
     remove_none_values,
     get_data_with_default,
     get_local_params,
     handle_comparison_params,
@@ -31,15 +32,15 @@
         updated_at: Optional[Union[str, Dict[str, str]]] = None,
         indexed_at: Optional[Union[str, Dict[str, str]]] = None,
         page: Optional[int] = None,
         page_limit: Optional[int] = None,
         sort_by: Optional[str] = None,
         sort_option: Optional[str] = None,
         **kwargs,
-    ) -> List[models.Video]:
+    ) -> RootModelList[models.Video]:
         params = {
             "_id": id,
             "filename": filename,
             "size": size,
             "width": width,
             "height": height,
             "duration": duration,
@@ -60,15 +61,15 @@
         handle_comparison_params(params, "duration", duration)
         handle_comparison_params(params, "created_at", created_at)
         handle_comparison_params(params, "updated_at", updated_at)
         handle_comparison_params(params, "indexed_at", indexed_at)
         res = self._get(
             f"indexes/{index_id}/videos", params=remove_none_values(params), **kwargs
         )
-        return [models.Video(self, index_id, **video) for video in res["data"]]
+        return RootModelList([models.Video(self, index_id, **video) for video in res["data"]])
 
     def list_pagination(
         self,
         index_id: str,
         *,
         id: Optional[str] = None,
         filename: Optional[str] = None,
@@ -151,74 +152,74 @@
         self,
         index_id: str,
         id: str,
         *,
         start: Optional[float] = None,
         end: Optional[float] = None,
         **kwargs,
-    ) -> List[models.VideoValue]:
+    ) -> RootModelList[models.VideoValue]:
         params = {
             "start": start,
             "end": end,
         }
         res = self._get(
             f"indexes/{index_id}/videos/{id}/transcription",
             params=remove_none_values(params),
             **kwargs,
         )
-        return [
+        return RootModelList([
             models.VideoValue(**value)
             for value in get_data_with_default(res, "data", [])
-        ]
+        ])
 
     def text_in_video(
         self,
         index_id: str,
         id: str,
         *,
         start: Optional[float] = None,
         end: Optional[float] = None,
         **kwargs,
-    ) -> List[models.VideoValue]:
+    ) -> RootModelList[models.VideoValue]:
         params = {
             "start": start,
             "end": end,
         }
         res = self._get(
             f"indexes/{index_id}/videos/{id}/text-in-video",
             params=remove_none_values(params),
             **kwargs,
         )
-        return [
+        return RootModelList([
             models.VideoValue(**value)
             for value in get_data_with_default(res, "data", [])
-        ]
+        ])
 
     def logo(
         self,
         index_id: str,
         id: str,
         *,
         start: Optional[float] = None,
         end: Optional[float] = None,
         **kwargs,
-    ) -> List[models.VideoValue]:
+    ) -> RootModelList[models.VideoValue]:
         params = {
             "start": start,
             "end": end,
         }
         res = self._get(
             f"indexes/{index_id}/videos/{id}/logo",
             params=remove_none_values(params),
             **kwargs,
         )
-        return [
+        return RootModelList([
             models.VideoValue(**value)
             for value in get_data_with_default(res, "data", [])
-        ]
+        ])
 
     def thumbnail(
         self,
         index_id: str,
         id: str,
         *,
         time: Optional[float] = None,
```

### Comparing `twelvelabs-0.1.22/twelvelabs/util.py` & `twelvelabs-0.1.23/twelvelabs/util.py`

 * *Files identical despite different names*

### Comparing `twelvelabs-0.1.22/twelvelabs.egg-info/PKG-INFO` & `twelvelabs-0.1.23/twelvelabs.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,294 +1,293 @@
 Metadata-Version: 2.1
 Name: twelvelabs
-Version: 0.1.22
+Version: 0.1.23
 Summary: SDK for Twelve Labs API
 Home-page: https://github.com/twelvelabs-io/twelvelabs-python
 Author: Twelve Labs
+License: UNKNOWN
+Description: # TwelveLabs Python SDK
+        
+        This SDK provides a convenient way to interact with the Twelve Labs Video Understanding Platform from an application written in the Python language. The SDK equips you with a set of intuitive classes and methods that streamline the process of interacting with the platform, minimizing the need for boilerplate code.
+        
+        # Prerequisites
+        
+        Ensure that the following prerequisites are met before using the SDK:
+        
+        -  [Python](https://www.python.org) 3.7 or newer must be installed on your machine.
+        -  You have an API key. If you don't have an account, please [sign up](https://api.twelvelabs.io/) for a free account. Then, to retrieve your API key, go to the [Dashboard](https://api.twelvelabs.io/dashboard) page, and select the **Copy** icon to the right of the key to copy it to your clipboard.
+        
+        # Install the SDK
+        
+        Install the `twelvelabs` package:
+        
+         ```sh
+         pip install twelvelabs
+         ```
+        
+        
+        # Initialize the SDK
+        
+        1. Import the SDK into your application:
+        
+           ```py
+           from twelvelabs import TwelveLabs
+           ```
+        
+        2.  Instantiate the SDK client with your API key. This example code assumes that your API key is stored in an environment variable named `TL_API_KEY`:
+        
+            ```py
+            client = TwelveLabs(api_key=os.getenv('TL_API_KEY'))
+            ```
+        
+        # Use the SDK
+        
+        To get started with the SDK, follow these basic steps:
+        
+        1. Create an index.
+        2. Upload videos.
+        3. Perform downstream tasks, such as searching or generating text from video.
+        
+        ## Create an index
+        
+        To create an index, use the example code below, replacing "<YOUR_INDEX_NAME>" with the desired name for your index:
+        
+        ```py
+        from twelvelabs import APIStatusError
+        
+        index_obj = None
+        try:
+            index_obj = client.index.create(
+                name = "<YOUR_INDEX_NAME>",
+                engines =[
+                    {
+                        "name": "marengo2.6",
+                        "options": ["visual", "conversation", "text_in_video"],
+                    },
+                    {
+                        "name": "pegasus1",
+                        "options": ["visual", "conversation"],
+                    },
+                ],
+            )
+            print(index_obj)
+        except APIStatusError as e:
+            print('API Status Error, 4xx or 5xx')
+            print(e)
+        except Exception as e:
+            print(e)
+        ```
+        
+        Note the following about this example:
+        - The platform provides two distinct engine types - embedding and generative, each serving unique purposes in multimodal video understanding.
+          - **Embedding engines (Marengo)**: These engines are proficient at performing tasks such as search and classification, enabling enhanced video understanding.
+          - **Generative engines (Pegasus)**: These engines generate text based on your videos.
+          For your index, both Marengo and Pegasus are enabled.
+        - The `engines.options` fields specify the types of information each video understanding engine will process.
+        - The engines and the engine options specified when you create an index apply to all the videos you upload to that index and cannot be changed. For details, see the [Engine options](https://docs.twelvelabs.io/v1.2/docs/engine-options) page.
+        
+        The output should look similar to the following:
+        
+        ```
+        Index(id='65b1b926560f741da96836d7', created_at='2024-01-25T01:28:06.061Z', updated_at='2024-01-25T01:28:06.061Z', name='test-index-to-researchers1', engines=[Engine(name='marengo2.6', options=['visual', 'conversation', 'text_in_video'], addons=None), Engine(name='pegasus1', options=['visual', 'conversation'], addons=None)], video_count=0, total_duration=0.0, expires_at='2024-04-24T01:28:06.061Z')
+        ```
+        
+        Note that the API returns, among other information, a field named `id`, representing the unique identifier of your new index.
+        
+        For a description of each field in the request and response, see the [Create an index](https://docs.twelvelabs.io/v1.2/reference/create-index) page.
+        
+        
+        ## Upload videos
+        
+        Before you upload a video to the platform, ensure that it meets the following requirements:
+        
+        - **Video resolution**: Must be greater or equal than 360p and less or equal than 4K. For consistent search results, Twelve Labs recommends you upload 360p videos.
+        - **Video and audio formats**:  The video files you wish to upload must be encoded in the video and audio formats listed on the [FFmpeg Formats Documentation](https://ffmpeg.org/ffmpeg-formats.html) page. For videos in other formats, contact us at [support@twelvelabs.io](mailto:support@twelvelabs.io).
+        - **Duration**: For Marengo, it must be between 4 seconds and 2 hours (7,200s). For Pegasus, it must be between 4 seconds and 20 minutes (1200s).
+        - **File size**: Must not exceed 2 GB. If you require different options, send us an email at support@twelvelabs.io.
+        - **Audio track**: If the `conversation` [engine option](https://docs.twelvelabs.io/v1.2/docs/engine-options) is selected, the video you're uploading must contain an audio track.
+        
+        To upload videos, use the example code below, replacing the following:
+        
+        - **`<YOUR_VIDEO_PATH>`**: with a string representing the path to the directory containing the video files you wish to upload.
+        - **`<YOUR_INDEX_ID>`**: with a string representing the unique identifier of the index to which you want to upload your video.
+        
+        
+        ```py
+        from glob import glob
+        from twelvelabs.models.task import Task
+        
+        video_files = glob("<YOUR_VIDEO_PATH>") # Example: "/videos/*.mp4
+        for video_file in video_files:
+          print(f"Uploading {video_file}")
+          task = client.task.create(index_id="<YOUR_INDEX_ID>", file=video_file, language="en")
+          print(f"Task id={task.id}")
+        
+          # (Optional) Monitor the video indexing process
+          # Utility function to print the status of a video indexing task
+          def on_task_update(task: Task):
+                  print(f"  Status={task.status}")
+          task.wait_for_done(callback=on_task_update)
+          if task.status != "ready":
+              raise RuntimeError(f"Indexing failed with status {task.status}")
+          print(f"Uploaded {video_file}. The unique identifer of your video is {task.video_id}.")
+        ```
+        
+        Note that once a video has been successfully uploaded and indexed, the response will contain a field named `video_id`, representing the unique identifier of your video.
+        
+        For a description of each field in the request and response, see the [Create a video indexing task](https://docs.twelvelabs.io/reference/create-video-indexing-task) page.
+        
+        ## Perform downstream tasks
+        
+        The sections below show how you can perform the most common downstream tasks. See [our documentation](https://docs.twelvelabs.io/docs) for a complete list of all the features the Twelve Labs Understanding Platform provides.
+        
+        ### Search
+        
+        To perform a search request, use the example code below, replacing the following:
+        
+        - **`<YOUR_INDEX_ID>`**: with a string representing the unique identifier of your index.
+        - **`<YOUR_QUERY>`**: with a string representing your search query. Note that the API supports full natural language-based search. The following examples are valid queries: "birds flying near a castle," "sun shining on water," and "an officer holding a child's hand."
+        - **`[<YOUR_SEARCH_OPTIONS>]`**: with an array of strings that specifies the sources of information the platform uses when performing a search. For example, to search based on visual and conversation cues, use `["visual", "conversation"]`. Note that the search options you specify must be a subset of the engine options used when you created the index. For more details, see the [Search options](https://docs.twelvelabs.io/docs/search-options) page. 
+        
+        ```py
+        search_results = client.search.query("<YOUR_INDEX_ID>", "<YOUR_QUERY>", ["<YOUR_SEARCH_OPTIONS>"])
+        
+        # Utility function to print a specific page
+        def print_page(page):
+          for clip in page:
+            print(
+                f" video_id={clip.video_id} score={clip.score} start={clip.start} end={clip.end} confidence={clip.confidence}"
+            )
+        
+        print_page(search_results.data)
+        
+        while True:
+            try:
+                print_page(next(search_results))
+            except StopIteration:
+                break
+        ```
+        
+        The results are returned one page at a time, with a default limit of 10 results on each page. The `next ` method returns the next page of results. When you've reached the end of the dataset, a `StopIteration` exception is raised.
+        
+        ```
+         video_id=65ca2bce48db9fa780cb3fa4 score=84.9 start=104.9375 end=111.90625 confidence=high
+         video_id=65ca2bce48db9fa780cb3fa4 score=84.82 start=160.46875 end=172.75 confidence=high
+         video_id=65ca2bce48db9fa780cb3fa4 score=84.77 start=55.375 end=72.46875 confidence=high
+        ```
+        
+        
+        Note that the response contains, among other information, the following fields:
+        - `video_id`: The unique identifier of the video that matched your search terms.
+        - `score`: A quantitative value determined by the AI engine representing the level of confidence that the results match your search terms.
+        - `start`: The start time of the matching video clip, expressed in seconds.
+        - `end`: The end time of the matching video clip, expressed in seconds.
+        - `confidence`: A qualitative indicator based on the value of the score field. This field can take one of the following values:
+          - `high`
+          - `medium`
+          - `low`
+          - `extremely low`
+        
+        
+        For a description of each field in the request and response, see the [Make a search request](https://docs.twelvelabs.io/v1.2/reference/make-search-request) page.
+        
+        ### Generate text from video
+        
+        The Twelve Labs Video Understanding Platform offers three distinct endpoints tailored to meet various requirements. Each endpoint has been designed with specific levels of flexibility and customization to accommodate different needs.
+        
+        Note the following about using these endpoints:
+        - The Pegasus video understanding engine must be enabled for the index to which your video has been uploaded.
+        - Your prompts must be instructive or descriptive, and you should not phrase them as questions.
+        - The maximum length of a prompt is 300 characters.
+        
+        #### Topics, titles, and hashtags
+        
+        To generate topics, titles, and hashtags, use the example code below, replacing the following:
+        
+        - **`<YOUR_VIDEO_ID>`**: with a string representing the unique identifier of your video.
+        - **`[<TYPES>]`**: with an array of strings representing the type of text the platform should generate. Example: `["title", "topic", "hashtag"]`.
+        
+        ```py
+        res = client.generate.gist("<YOUR_VIDEO_ID>", types=["<TYPES>"])
+        print(f"Title = {res.title}\nTopics = {res.topics}\nHashtags = {res.hashtags}")
+        ```
+        
+        For a description of each field in the request and response, see the [Titles, topics, or hashtags](https://docs.twelvelabs.io/v1.2/reference/generate-gist) page.
+        
+        #### Summaries, chapters, and highlights
+        
+        To generate summaries, chapters, and highlights, use the example code below, replacing the following:
+        
+        - **`<YOUR_VIDEO_ID>`**: with a string representing the unique identifier of your video.
+        - **`<TYPE>`**: with a string representing the type of text the platform should generate. This parameter can take one of the following values: "summary", "chapter", or "highlight".
+        - _(Optional)_ **`<YOUR_PROMPT>`**: with a string that provides context for the summarization task, such as the target audience, style, tone of voice, and purpose. Example:  "Generate a summary in no more than 5 bullet points."
+        
+        
+        ```py
+        res = client.generate.summarize("<YOUR_VIDEO_ID>", type="<TYPE>", prompt="<YOUR_PROMPT>")
+        print(f"{res.summary}")
+        ```
+        
+        For a description of each field in the request and response, see the [Summaries, chapters, or highlights](https://docs.twelvelabs.io/v1.2/docs/generate-summaries-chapters-highlights) page.
+        
+        #### Open-ended texts
+        
+        To generate open-ended texts, use the example code below, replacing the following:
+        - **`<YOUR_VIDEO_ID>`**: with a string representing the unique identifier of your video.
+        - **`<YOUR_PROMPT>`**: with a string that guides the model on the desired format or content. The maximum length of the prompt is 500 tokens or roughly 350 words. Example:  "I want to generate a description for my video with the following format: Title of the video, followed by a summary in 2-3 sentences, highlighting the main topic, key events, and concluding remarks."
+        
+        ```py
+        res = client.generate.text(video_id="<YOUR_VIDEO_ID>", prompt="<YOUR_PROMPT>")
+        print(f"{res.data}")
+        ```
+        
+        ## Error Handling
+        
+        The SDK includes a set of exceptions that are mapped to specific HTTP status codes, as shown in the table below:
+        
+        | Exception | HTTP Status Code |
+        |----------|----------|
+        | BadRequestError| 400 |
+        | AuthenticationError | 401 |
+        | PermissionDeniedError  | 403 |
+        | NotFoundError | 404 |
+        | ConflictError | 409 |
+        | UnprocessableEntityError | 422 |
+        | RateLimitError | 429 |
+        | InternalServerError | 5xx |
+        
+        The following example shows how you can handle specific HTTP errors in your application:
+        
+        ```python
+        import os
+        from twelvelabs import TwelveLabs
+        
+        client = TwelveLabs(os.getenv("TWELVELABS_API_KEY"))
+        try:
+            engines = client.engines.list()
+            print(engines)
+        except twelvelabs.APIConnectionError as e:
+            print("Cannot connect to API server")
+        except twelvelabs.BadRequestError as e:
+            print("Bad request.")
+        except twelvelabs.APIStatusError as e:
+            print(f"Status code {e.status_code} received")
+            print(e.response)
+        ```
+        
+        # License
+        
+        We use the Developer Certificate of Origin (DCO) in lieu of a Contributor License Agreement for all contributions to Twelve Labs' open-source projects. We request that contributors agree to the terms of the DCO and indicate that agreement by signing all commits made to Twelve Labs' projects by adding a line with your name and email address to every Git commit message contributed, as shown in the example below:
+        
+        ```
+        Signed-off-by: Jane Doe <jane.doe@example.com>
+        ```
+        
+        You can sign your commit automatically with Git by using `git commit -s` if you have your `user.name` and `user.email` set as part of your Git configuration.
+        We ask that you use your real name (please, no anonymous contributions or pseudonyms). By signing your commitment, you are certifying that you have the right have the right to submit it under the open-source license used by that particular project. You must use your real name (no pseudonyms or anonymous contributions are allowed.)
+        We use the Probot DCO GitHub app to check for DCO signoffs of every commit.
+        If you forget to sign your commits, the DCO bot will remind you and give you detailed instructions for how to amend your commits to add a signature.
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pydantic==2.4.2
-Requires-Dist: httpx==0.25.2
-
-# TwelveLabs Python SDK
-
-This SDK provides a convenient way to interact with the Twelve Labs Video Understanding Platform from an application written in the Python language. The SDK equips you with a set of intuitive classes and methods that streamline the process of interacting with the platform, minimizing the need for boilerplate code.
-
-# Prerequisites
-
-Ensure that the following prerequisites are met before using the SDK:
-
--  [Python](https://www.python.org) 3.7 or newer must be installed on your machine.
--  You have an API key. If you don't have an account, please [sign up](https://api.twelvelabs.io/) for a free account. Then, to retrieve your API key, go to the [Dashboard](https://api.twelvelabs.io/dashboard) page, and select the **Copy** icon to the right of the key to copy it to your clipboard.
-
-# Install the SDK
-
-Install the `twelvelabs` package:
-
- ```sh
- pip install twelvelabs
- ```
-
-
-# Initialize the SDK
-
-1. Import the SDK into your application:
-
-   ```py
-   from twelvelabs import TwelveLabs
-   ```
-
-2.  Instantiate the SDK client with your API key. This example code assumes that your API key is stored in an environment variable named `TL_API_KEY`:
-
-    ```py
-    client = TwelveLabs(api_key=os.getenv('TL_API_KEY'))
-    ```
-
-# Use the SDK
-
-To get started with the SDK, follow these basic steps:
-
-1. Create an index.
-2. Upload videos.
-3. Perform downstream tasks, such as searching or generating text from video.
-
-## Create an index
-
-To create an index, use the example code below, replacing "<YOUR_INDEX_NAME>" with the desired name for your index:
-
-```py
-from twelvelabs import APIStatusError
-
-index_obj = None
-try:
-    index_obj = client.index.create(
-        name = "<YOUR_INDEX_NAME>",
-        engines =[
-            {
-                "name": "marengo2.6",
-                "options": ["visual", "conversation", "text_in_video"],
-            },
-            {
-                "name": "pegasus1",
-                "options": ["visual", "conversation"],
-            },
-        ],
-    )
-    print(index_obj)
-except APIStatusError as e:
-    print('API Status Error, 4xx or 5xx')
-    print(e)
-except Exception as e:
-    print(e)
-```
-
-Note the following about this example:
-- The platform provides two distinct engine types - embedding and generative, each serving unique purposes in multimodal video understanding.
-  - **Embedding engines (Marengo)**: These engines are proficient at performing tasks such as search and classification, enabling enhanced video understanding.
-  - **Generative engines (Pegasus)**: These engines generate text based on your videos.
-  For your index, both Marengo and Pegasus are enabled.
-- The `engines.options` fields specify the types of information each video understanding engine will process.
-- The engines and the engine options specified when you create an index apply to all the videos you upload to that index and cannot be changed. For details, see the [Engine options](https://docs.twelvelabs.io/v1.2/docs/engine-options) page.
-
-The output should look similar to the following:
-
-```
-Index(id='65b1b926560f741da96836d7', created_at='2024-01-25T01:28:06.061Z', updated_at='2024-01-25T01:28:06.061Z', name='test-index-to-researchers1', engines=[Engine(name='marengo2.6', options=['visual', 'conversation', 'text_in_video'], addons=None), Engine(name='pegasus1', options=['visual', 'conversation'], addons=None)], video_count=0, total_duration=0.0, expires_at='2024-04-24T01:28:06.061Z')
-```
-
-Note that the API returns, among other information, a field named `id`, representing the unique identifier of your new index.
-
-For a description of each field in the request and response, see the [Create an index](https://docs.twelvelabs.io/v1.2/reference/create-index) page.
-
-
-## Upload videos
-
-Before you upload a video to the platform, ensure that it meets the following requirements:
-
-- **Video resolution**: Must be greater or equal than 360p and less or equal than 4K. For consistent search results, Twelve Labs recommends you upload 360p videos.
-- **Video and audio formats**:  The video files you wish to upload must be encoded in the video and audio formats listed on the [FFmpeg Formats Documentation](https://ffmpeg.org/ffmpeg-formats.html) page. For videos in other formats, contact us at [support@twelvelabs.io](mailto:support@twelvelabs.io).
-- **Duration**: For Marengo, it must be between 4 seconds and 2 hours (7,200s). For Pegasus, it must be between 4 seconds and 20 minutes (1200s).
-- **File size**: Must not exceed 2 GB. If you require different options, send us an email at support@twelvelabs.io.
-- **Audio track**: If the `conversation` [engine option](https://docs.twelvelabs.io/v1.2/docs/engine-options) is selected, the video you're uploading must contain an audio track.
-
-To upload videos, use the example code below, replacing the following:
-
-- **`<YOUR_VIDEO_PATH>`**: with a string representing the path to the directory containing the video files you wish to upload.
-- **`<YOUR_INDEX_ID>`**: with a string representing the unique identifier of the index to which you want to upload your video.
-
-
-```py
-from glob import glob
-from twelvelabs.models.task import Task
-
-video_files = glob("<YOUR_VIDEO_PATH>") # Example: "/videos/*.mp4
-for video_file in video_files:
-  print(f"Uploading {video_file}")
-  task = client.task.create(index_id="<YOUR_INDEX_ID>", file=video_file, language="en")
-  print(f"Task id={task.id}")
-
-  # (Optional) Monitor the video indexing process
-  # Utility function to print the status of a video indexing task
-  def on_task_update(task: Task):
-          print(f"  Status={task.status}")
-  task.wait_for_done(callback=on_task_update)
-  if task.status != "ready":
-      raise RuntimeError(f"Indexing failed with status {task.status}")
-  print(f"Uploaded {video_file}. The unique identifer of your video is {task.video_id}.")
-```
-
-Note that once a video has been successfully uploaded and indexed, the response will contain a field named `video_id`, representing the unique identifier of your video.
-
-For a description of each field in the request and response, see the [Create a video indexing task](https://docs.twelvelabs.io/reference/create-video-indexing-task) page.
-
-## Perform downstream tasks
-
-The sections below show how you can perform the most common downstream tasks. See [our documentation](https://docs.twelvelabs.io/docs) for a complete list of all the features the Twelve Labs Understanding Platform provides.
-
-### Search
-
-To perform a search request, use the example code below, replacing the following:
-
-- **`<YOUR_INDEX_ID>`**: with a string representing the unique identifier of your index.
-- **`<YOUR_QUERY>`**: with a string representing your search query. Note that the API supports full natural language-based search. The following examples are valid queries: "birds flying near a castle," "sun shining on water," and "an officer holding a child's hand."
-- **`[<YOUR_SEARCH_OPTIONS>]`**: with an array of strings that specifies the sources of information the platform uses when performing a search. For example, to search based on visual and conversation cues, use `["visual", "conversation"]`. Note that the search options you specify must be a subset of the engine options used when you created the index. For more details, see the [Search options](https://docs.twelvelabs.io/docs/search-options) page. 
-
-```py
-search_results = client.search.query("<YOUR_INDEX_ID>", "<YOUR_QUERY>", ["<YOUR_SEARCH_OPTIONS>"])
-
-# Utility function to print a specific page
-def print_page(page):
-  for clip in page:
-    print(
-        f" video_id={clip.video_id} score={clip.score} start={clip.start} end={clip.end} confidence={clip.confidence}"
-    )
-
-print_page(search_results.data)
-
-while True:
-    try:
-        print_page(next(search_results))
-    except StopIteration:
-        break
-```
-
-The results are returned one page at a time, with a default limit of 10 results on each page. The `next ` method returns the next page of results. When you've reached the end of the dataset, a `StopIteration` exception is raised.
-
-```
- video_id=65ca2bce48db9fa780cb3fa4 score=84.9 start=104.9375 end=111.90625 confidence=high
- video_id=65ca2bce48db9fa780cb3fa4 score=84.82 start=160.46875 end=172.75 confidence=high
- video_id=65ca2bce48db9fa780cb3fa4 score=84.77 start=55.375 end=72.46875 confidence=high
-```
-
-
-Note that the response contains, among other information, the following fields:
-- `video_id`: The unique identifier of the video that matched your search terms.
-- `score`: A quantitative value determined by the AI engine representing the level of confidence that the results match your search terms.
-- `start`: The start time of the matching video clip, expressed in seconds.
-- `end`: The end time of the matching video clip, expressed in seconds.
-- `confidence`: A qualitative indicator based on the value of the score field. This field can take one of the following values:
-  - `high`
-  - `medium`
-  - `low`
-  - `extremely low`
-
-
-For a description of each field in the request and response, see the [Make a search request](https://docs.twelvelabs.io/v1.2/reference/make-search-request) page.
-
-### Generate text from video
-
-The Twelve Labs Video Understanding Platform offers three distinct endpoints tailored to meet various requirements. Each endpoint has been designed with specific levels of flexibility and customization to accommodate different needs.
-
-Note the following about using these endpoints:
-- The Pegasus video understanding engine must be enabled for the index to which your video has been uploaded.
-- Your prompts must be instructive or descriptive, and you should not phrase them as questions.
-- The maximum length of a prompt is 300 characters.
-
-#### Topics, titles, and hashtags
-
-To generate topics, titles, and hashtags, use the example code below, replacing the following:
-
-- **`<YOUR_VIDEO_ID>`**: with a string representing the unique identifier of your video.
-- **`[<TYPES>]`**: with an array of strings representing the type of text the platform should generate. Example: `["title", "topic", "hashtag"]`.
-
-```py
-res = client.generate.gist("<YOUR_VIDEO_ID>", types=["<TYPES>"])
-print(f"Title = {res.title}\nTopics = {res.topics}\nHashtags = {res.hashtags}")
-```
-
-For a description of each field in the request and response, see the [Titles, topics, or hashtags](https://docs.twelvelabs.io/v1.2/reference/generate-gist) page.
-
-#### Summaries, chapters, and highlights
-
-To generate summaries, chapters, and highlights, use the example code below, replacing the following:
-
-- **`<YOUR_VIDEO_ID>`**: with a string representing the unique identifier of your video.
-- **`<TYPE>`**: with a string representing the type of text the platform should generate. This parameter can take one of the following values: "summary", "chapter", or "highlight".
-- _(Optional)_ **`<YOUR_PROMPT>`**: with a string that provides context for the summarization task, such as the target audience, style, tone of voice, and purpose. Example:  "Generate a summary in no more than 5 bullet points."
-
-
-```py
-res = client.generate.summarize("<YOUR_VIDEO_ID>", type="<TYPE>", prompt="<YOUR_PROMPT>")
-print(f"{res.summary}")
-```
-
-For a description of each field in the request and response, see the [Summaries, chapters, or highlights](https://docs.twelvelabs.io/v1.2/docs/generate-summaries-chapters-highlights) page.
-
-#### Open-ended texts
-
-To generate open-ended texts, use the example code below, replacing the following:
-- **`<YOUR_VIDEO_ID>`**: with a string representing the unique identifier of your video.
-- **`<YOUR_PROMPT>`**: with a string that guides the model on the desired format or content. The maximum length of the prompt is 500 tokens or roughly 350 words. Example:  "I want to generate a description for my video with the following format: Title of the video, followed by a summary in 2-3 sentences, highlighting the main topic, key events, and concluding remarks."
-
-```py
-res = client.generate.text(video_id="<YOUR_VIDEO_ID>", prompt="<YOUR_PROMPT>")
-print(f"{res.data}")
-```
-
-## Error Handling
-
-The SDK includes a set of exceptions that are mapped to specific HTTP status codes, as shown in the table below:
-
-| Exception | HTTP Status Code |
-|----------|----------|
-| BadRequestError| 400 |
-| AuthenticationError | 401 |
-| PermissionDeniedError  | 403 |
-| NotFoundError | 404 |
-| ConflictError | 409 |
-| UnprocessableEntityError | 422 |
-| RateLimitError | 429 |
-| InternalServerError | 5xx |
-
-The following example shows how you can handle specific HTTP errors in your application:
-
-```python
-import os
-from twelvelabs import TwelveLabs
-
-client = TwelveLabs(os.getenv("TWELVELABS_API_KEY"))
-try:
-    engines = client.engines.list()
-    print(engines)
-except twelvelabs.APIConnectionError as e:
-    print("Cannot connect to API server")
-except twelvelabs.BadRequestError as e:
-    print("Bad request.")
-except twelvelabs.APIStatusError as e:
-    print(f"Status code {e.status_code} received")
-    print(e.response)
-```
-
-# License
-
-We use the Developer Certificate of Origin (DCO) in lieu of a Contributor License Agreement for all contributions to Twelve Labs' open-source projects. We request that contributors agree to the terms of the DCO and indicate that agreement by signing all commits made to Twelve Labs' projects by adding a line with your name and email address to every Git commit message contributed, as shown in the example below:
-
-```
-Signed-off-by: Jane Doe <jane.doe@example.com>
-```
-
-You can sign your commit automatically with Git by using `git commit -s` if you have your `user.name` and `user.email` set as part of your Git configuration.
-We ask that you use your real name (please, no anonymous contributions or pseudonyms). By signing your commitment, you are certifying that you have the right have the right to submit it under the open-source license used by that particular project. You must use your real name (no pseudonyms or anonymous contributions are allowed.)
-We use the Probot DCO GitHub app to check for DCO signoffs of every commit.
-If you forget to sign your commits, the DCO bot will remind you and give you detailed instructions for how to amend your commits to add a signature.
```

### Comparing `twelvelabs-0.1.22/twelvelabs.egg-info/SOURCES.txt` & `twelvelabs-0.1.23/twelvelabs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

