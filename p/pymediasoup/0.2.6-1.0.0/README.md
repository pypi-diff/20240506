# Comparing `tmp/pymediasoup-0.2.6.tar.gz` & `tmp/pymediasoup-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymediasoup-0.2.6.tar", max compression
+gzip compressed data, was "pymediasoup-1.0.0.tar", max compression
```

## Comparing `pymediasoup-0.2.6.tar` & `pymediasoup-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1066 2023-11-06 13:21:51.237035 pymediasoup-0.2.6/LICENSE
--rw-r--r--   0        0        0      840 2023-11-06 13:21:51.237094 pymediasoup-0.2.6/README.md
--rw-r--r--   0        0        0       77 2024-02-27 05:01:59.154794 pymediasoup-0.2.6/pymediasoup/__init__.py
--rw-r--r--   0        0        0       62 2024-02-27 05:04:38.095096 pymediasoup-0.2.6/pymediasoup/__version__.py
--rw-r--r--   0        0        0     5089 2024-02-27 05:01:59.155208 pymediasoup-0.2.6/pymediasoup/consumer.py
--rw-r--r--   0        0        0     4525 2024-02-27 05:01:59.155427 pymediasoup-0.2.6/pymediasoup/data_consumer.py
--rw-r--r--   0        0        0     5226 2024-02-27 05:01:59.155649 pymediasoup-0.2.6/pymediasoup/data_producer.py
--rw-r--r--   0        0        0     9254 2024-02-27 05:01:59.155937 pymediasoup-0.2.6/pymediasoup/device.py
--rw-r--r--   0        0        0      594 2024-02-27 05:01:59.156474 pymediasoup-0.2.6/pymediasoup/emitter.py
--rw-r--r--   0        0        0      277 2024-02-27 05:01:59.157135 pymediasoup-0.2.6/pymediasoup/errors.py
--rw-r--r--   0        0        0        0 2023-11-06 13:21:51.238168 pymediasoup-0.2.6/pymediasoup/handlers/__init__.py
--rw-r--r--   0        0        0    25662 2024-02-27 05:01:59.157641 pymediasoup-0.2.6/pymediasoup/handlers/aiortc_handler.py
--rw-r--r--   0        0        0     3812 2024-02-27 05:01:59.158032 pymediasoup-0.2.6/pymediasoup/handlers/handler_interface.py
--rw-r--r--   0        0        0        0 2023-11-06 13:21:51.238413 pymediasoup-0.2.6/pymediasoup/handlers/sdp/__init__.py
--rw-r--r--   0        0        0     5168 2024-02-27 05:01:59.158605 pymediasoup-0.2.6/pymediasoup/handlers/sdp/common_utils.py
--rw-r--r--   0        0        0    20334 2024-02-27 05:01:59.159395 pymediasoup-0.2.6/pymediasoup/handlers/sdp/media_section.py
--rw-r--r--   0        0        0    11880 2024-02-27 05:01:59.160027 pymediasoup-0.2.6/pymediasoup/handlers/sdp/remote_sdp.py
--rw-r--r--   0        0        0     3779 2024-02-27 05:01:59.160226 pymediasoup-0.2.6/pymediasoup/handlers/sdp/unified_plan_utils.py
--rw-r--r--   0        0        0        0 2023-11-06 13:21:51.238824 pymediasoup-0.2.6/pymediasoup/models/__init__.py
--rw-r--r--   0        0        0     2372 2024-02-27 05:01:59.160742 pymediasoup-0.2.6/pymediasoup/models/handler_interface.py
--rw-r--r--   0        0        0     2638 2024-02-27 05:01:59.161432 pymediasoup-0.2.6/pymediasoup/models/transport.py
--rw-r--r--   0        0        0    15037 2024-02-27 05:01:59.161721 pymediasoup-0.2.6/pymediasoup/ortc.py
--rw-r--r--   0        0        0     8895 2024-02-27 05:01:59.162294 pymediasoup-0.2.6/pymediasoup/producer.py
--rw-r--r--   0        0        0     9279 2024-02-27 05:01:59.163772 pymediasoup-0.2.6/pymediasoup/rtp_parameters.py
--rw-r--r--   0        0        0      513 2024-02-27 05:01:59.164322 pymediasoup-0.2.6/pymediasoup/scalability_modes.py
--rw-r--r--   0        0        0     1673 2024-02-27 05:01:59.164531 pymediasoup-0.2.6/pymediasoup/sctp_parameters.py
--rw-r--r--   0        0        0    18622 2024-02-27 05:01:59.164775 pymediasoup-0.2.6/pymediasoup/transport.py
--rw-r--r--   0        0        0      533 2024-02-27 05:02:28.052745 pymediasoup-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     1746 1970-01-01 00:00:00.000000 pymediasoup-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-06 07:50:25.191610 pymediasoup-1.0.0/LICENSE
+-rw-r--r--   0        0        0      840 2024-05-06 07:50:25.191610 pymediasoup-1.0.0/README.md
+-rw-r--r--   0        0        0      118 2024-05-06 07:50:25.191610 pymediasoup-1.0.0/pymediasoup/__init__.py
+-rw-r--r--   0        0        0       63 2024-05-06 07:50:25.191610 pymediasoup-1.0.0/pymediasoup/__version__.py
+-rw-r--r--   0        0        0     4954 2024-05-06 07:50:25.191610 pymediasoup-1.0.0/pymediasoup/consumer.py
+-rw-r--r--   0        0        0     4320 2024-05-06 07:50:25.191610 pymediasoup-1.0.0/pymediasoup/data_consumer.py
+-rw-r--r--   0        0        0     5013 2024-05-06 07:50:25.191610 pymediasoup-1.0.0/pymediasoup/data_producer.py
+-rw-r--r--   0        0        0     9361 2024-05-06 07:50:25.191610 pymediasoup-1.0.0/pymediasoup/device.py
+-rw-r--r--   0        0        0      577 2024-05-06 07:50:25.191610 pymediasoup-1.0.0/pymediasoup/emitter.py
+-rw-r--r--   0        0        0      281 2024-05-06 07:50:25.191610 pymediasoup-1.0.0/pymediasoup/errors.py
+-rw-r--r--   0        0        0        0 2024-05-06 07:50:25.191610 pymediasoup-1.0.0/pymediasoup/handlers/__init__.py
+-rw-r--r--   0        0        0    26304 2024-05-06 07:50:25.191610 pymediasoup-1.0.0/pymediasoup/handlers/aiortc_handler.py
+-rw-r--r--   0        0        0     3621 2024-05-06 07:50:25.191610 pymediasoup-1.0.0/pymediasoup/handlers/handler_interface.py
+-rw-r--r--   0        0        0        0 2024-05-06 07:50:25.191610 pymediasoup-1.0.0/pymediasoup/handlers/sdp/__init__.py
+-rw-r--r--   0        0        0     5286 2024-05-06 07:50:25.195610 pymediasoup-1.0.0/pymediasoup/handlers/sdp/common_utils.py
+-rw-r--r--   0        0        0    22045 2024-05-06 07:50:25.195610 pymediasoup-1.0.0/pymediasoup/handlers/sdp/media_section.py
+-rw-r--r--   0        0        0    11836 2024-05-06 07:50:25.195610 pymediasoup-1.0.0/pymediasoup/handlers/sdp/remote_sdp.py
+-rw-r--r--   0        0        0     3665 2024-05-06 07:50:25.195610 pymediasoup-1.0.0/pymediasoup/handlers/sdp/unified_plan_utils.py
+-rw-r--r--   0        0        0        0 2024-05-06 07:50:25.195610 pymediasoup-1.0.0/pymediasoup/models/__init__.py
+-rw-r--r--   0        0        0     2281 2024-05-06 07:50:25.195610 pymediasoup-1.0.0/pymediasoup/models/handler_interface.py
+-rw-r--r--   0        0        0     2480 2024-05-06 07:50:25.195610 pymediasoup-1.0.0/pymediasoup/models/transport.py
+-rw-r--r--   0        0        0    15797 2024-05-06 07:50:25.195610 pymediasoup-1.0.0/pymediasoup/ortc.py
+-rw-r--r--   0        0        0     8740 2024-05-06 07:50:25.195610 pymediasoup-1.0.0/pymediasoup/producer.py
+-rw-r--r--   0        0        0     9225 2024-05-06 07:50:25.195610 pymediasoup-1.0.0/pymediasoup/rtp_parameters.py
+-rw-r--r--   0        0        0      471 2024-05-06 07:50:25.195610 pymediasoup-1.0.0/pymediasoup/scalability_modes.py
+-rw-r--r--   0        0        0     1551 2024-05-06 07:50:25.195610 pymediasoup-1.0.0/pymediasoup/sctp_parameters.py
+-rw-r--r--   0        0        0    18506 2024-05-06 07:50:25.195610 pymediasoup-1.0.0/pymediasoup/transport.py
+-rw-r--r--   0        0        0      569 2024-05-06 07:50:25.195610 pymediasoup-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1738 1970-01-01 00:00:00.000000 pymediasoup-1.0.0/PKG-INFO
```

### Comparing `pymediasoup-0.2.6/LICENSE` & `pymediasoup-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymediasoup-0.2.6/README.md` & `pymediasoup-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `pymediasoup-0.2.6/pymediasoup/consumer.py` & `pymediasoup-1.0.0/pymediasoup/consumer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 import logging
 from typing import Optional, Any
 from aiortc import RTCRtpReceiver, MediaStreamTrack
 from pyee import AsyncIOEventEmitter
 from pydantic import BaseModel
-from .errors import InvalidStateError, UnsupportedError
+from .errors import InvalidStateError
 from .emitter import EnhancedEventEmitter
 from .rtp_parameters import MediaKind, RtpParameters
 
 
 logger = logging.getLogger(__name__)
 
 
 class ConsumerOptions(BaseModel):
     id: str
     producerId: str
     kind: MediaKind
     rtpParameters: RtpParameters
     appData: Optional[dict] = {}
 
+
 class Consumer(EnhancedEventEmitter):
     def __init__(
         self,
         id: str,
         localId: str,
         producerId: str,
         track: MediaStreamTrack,
         rtpParameters: RtpParameters,
         rtpReceiver: Optional[RTCRtpReceiver] = None,
         appData: Optional[dict] = {},
-        loop=None
+        loop=None,
     ):
         super(Consumer, self).__init__(loop=loop)
 
         # Closed flag.
         self._closed: bool = False
         # Observer instance.
         self._observer: AsyncIOEventEmitter = AsyncIOEventEmitter()
@@ -42,166 +43,165 @@
         self._producerId = producerId
         self._track = track
         # NOTE: 'AudioStreamTrack' object has no attribute 'enabled'
         self._paused: bool = False
         self._rtpParameters = rtpParameters
         self._rtpReceiver = rtpReceiver
         self._appData = appData
-        
+
         self._handleTrack()
-    
+
     # Consumer id.
     @property
     def id(self) -> str:
         return self._id
-    
+
     # Local id.
     @property
     def localId(self) -> str:
         return self._localId
 
     # Associated Producer id.
     @property
     def producerId(self) -> str:
         return self._producerId
-    
+
     # Whether the Consumer is closed.
     @property
     def closed(self) -> bool:
         return self._closed
-    
+
     # Media kind.
     @property
     def kind(self) -> MediaStreamTrack.kind:
         return self._track.kind
-    
+
     # Associated RTCRtpReceiver.
     @property
     def rtpReceiver(self) -> Optional[RTCRtpReceiver]:
         return self._rtpReceiver
-    
+
     # The associated track.
     @property
     def track(self) -> Optional[MediaStreamTrack]:
         return self._track
-    
+
     # RTP parameters.
     @property
     def rtpParameters(self) -> RtpParameters:
         return self._rtpParameters
-    
+
     # Whether the Consumer is paused.
     @property
     def paused(self) -> bool:
         return self._paused
-    
+
     # App custom data.
     @property
     def appData(self) -> Any:
         return self._appData
-    
+
     # Invalid setter.
     @appData.setter
     def appData(self, value):
-        raise Exception('cannot override appData object')
+        raise Exception("cannot override appData object")
 
-    
     # Observer.
     #
     # @emits close
     # @emits pause
     # @emits resume
     # @emits trackended
     @property
     def observer(self) -> AsyncIOEventEmitter:
         return self._observer
 
     async def close(self):
         if self._closed:
             return
-        
-        logger.debug('Consumer close()')
+
+        logger.debug("Consumer close()")
 
         self._closed = True
 
         self._destroyTrack()
 
-        await self.emit_for_results('@close')
+        await self.emit_for_results("@close")
 
         # Emit observer event.
-        self._observer.emit('close')
-  
+        self._observer.emit("close")
+
     # Transport was closed.
     def transportClosed(self):
         if self._closed:
             return
 
-        logger.debug('Consumer transportClosed()')
+        logger.debug("Consumer transportClosed()")
 
         self._closed = True
 
         self._destroyTrack()
 
-        self.emit('transportclose')
+        self.emit("transportclose")
+
+        self._observer.emit("close")
 
-        self._observer.emit('close')
-    
     # Get associated RTCRtpSender stats.
     async def getStats(self):
         if self._closed:
-            raise InvalidStateError('closed')
+            raise InvalidStateError("closed")
+
+        return await self.emit_for_results("@getstats")
 
-        return await self.emit_for_results('@getstats')
-    
     # Pauses sending media.
     def pause(self):
-        logger.debug('Consumer pause()')
+        logger.debug("Consumer pause()")
 
         if self._closed:
-            logger.debug('Consumer pause() | Consumer closed')
+            logger.debug("Consumer pause() | Consumer closed")
             return
-        
+
         self._paused = True
 
         if self._track and self._disableTrackOnPause:
             # TODO: MediaStreamTrack missing enable property
             # self._track.enabled = False
             pass
-        
-        self._observer.emit('pause')
-    
+
+        self._observer.emit("pause")
+
     # Resumes sending media.
     def resume(self):
-        logger.debug('Consumer resume()')
+        logger.debug("Consumer resume()")
 
         if self._closed:
-            logger.debug('Consumer resume() | Consumer closed')
+            logger.debug("Consumer resume() | Consumer closed")
             return
-        
+
         self._paused = False
 
         if self._track and self._disableTrackOnPause:
             # TODO: MediaStreamTrack missing enable property
             # self._track.enabled = True
             pass
-        
-        self._observer.emit('resume')
-    
+
+        self._observer.emit("resume")
+
     def _onTrackEnded(self):
         logger.debug('track "ended" event')
-        self.emit('trackended')
+        self.emit("trackended")
         # Emit observer event.
-        self._observer.emit('trackended')
-    
+        self._observer.emit("trackended")
+
     def _handleTrack(self):
         if not self._track:
             return
 
-        self._track.on('ended', self._onTrackEnded)
-    
+        self._track.on("ended", self._onTrackEnded)
+
     def _destroyTrack(self):
         if not self._track:
             return
 
-        self._track.remove_listener('ended', self._onTrackEnded)
+        self._track.remove_listener("ended", self._onTrackEnded)
 
         self._track.stop()
```

### Comparing `pymediasoup-0.2.6/pymediasoup/data_consumer.py` & `pymediasoup-1.0.0/pymediasoup/data_consumer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,8 @@
-import sys
-if sys.version_info >= (3, 8):
-    from typing import Optional, Any, Literal
-else:
-    from typing import Optional, Any
-    from typing_extensions import Literal
+from typing import Optional, Any, Literal
 
 import logging
 from pydantic import BaseModel
 from pyee import AsyncIOEventEmitter
 from aiortc import RTCDataChannel
 from .emitter import EnhancedEventEmitter
 from .sctp_parameters import SctpStreamParameters
@@ -20,23 +15,24 @@
     id: str
     dataProducerId: str
     sctpStreamParameters: SctpStreamParameters
     label: Optional[str]
     protocol: Optional[str]
     appData: Optional[dict] = {}
 
+
 class DataConsumer(EnhancedEventEmitter):
     def __init__(
         self,
         id: str,
         dataProducerId: str,
         dataChannel: RTCDataChannel,
         sctpStreamParameters: SctpStreamParameters,
         appData: Optional[dict] = {},
-        loop=None
+        loop=None,
     ):
         super(DataConsumer, self).__init__(loop=loop)
 
         # Closed flag.
         self._closed: bool = False
         # Observer instance.
         self._observer: AsyncIOEventEmitter = AsyncIOEventEmitter()
@@ -44,130 +40,130 @@
         self._id = id
         self._dataProducerId = dataProducerId
         self._dataChannel = dataChannel
         self._sctpStreamParameters = sctpStreamParameters
         self._appData = appData
 
         self._handleDataChannel()
-    
+
     # DataConsumer id.
     @property
     def id(self) -> str:
         return self._id
-    
+
     # Associated DataProducer id.
     @property
     def dataProducerId(self) -> str:
         return self._dataProducerId
-    
+
     # Whether the DataConsumer is closed.
     @property
     def closed(self) -> bool:
         return self._closed
-    
+
     # SCTP stream parameters.
     @property
     def sctpStreamParameters(self) -> SctpStreamParameters:
         return self._sctpStreamParameters
-    
+
     # DataChannel readyState.
     @property
     def readyState(self) -> Literal["closed", "closing", "connecting", "open"]:
         return self._dataChannel.readyState
-    
+
     # DataChannel label.
     @property
     def label(self) -> str:
         return self._dataChannel.label
-    
+
     # DataChannel protocol.
     @property
     def protocol(self) -> str:
         return self._dataChannel.protocol
 
     # DataChannel binaryType.
     @property
     def binaryType(self) -> str:
         return self._dataChannel.binaryType
-    
+
     @binaryType.setter
     def binaryType(self, binaryType: str):
         self._dataChannel.binaryType = binaryType
-    
+
     # App custom data.
     @property
     def appData(self) -> Any:
         return self._appData
-    
+
     # Invalid setter.
     @appData.setter
     def appData(self, value):
-        raise Exception('cannot override appData object')
-    
+        raise Exception("cannot override appData object")
+
     # Observer.
     @property
     def observer(self) -> AsyncIOEventEmitter:
         return self._observer
-    
+
     # Closes the DataConsumer.
     async def close(self):
         if self._closed:
             return
-        
-        logger.debug('DataConsumer close()')
+
+        logger.debug("DataConsumer close()")
 
         self._closed = True
 
         self._dataChannel.close()
 
-        await self.emit_for_results('@close')
+        await self.emit_for_results("@close")
 
         # Emit observer event.
-        self._observer.emit('close')
-    
+        self._observer.emit("close")
+
     # Transport was closed.
     def transportClosed(self):
         if self._closed:
             return
 
-        logger.debug('DataConsumer transportClosed()')
+        logger.debug("DataConsumer transportClosed()")
 
         self._closed = True
 
         self._dataChannel.close()
 
-        self.emit('transportclose')
+        self.emit("transportclose")
+
+        self._observer.emit("close")
 
-        self._observer.emit('close')
-    
     def _handleDataChannel(self):
-        @self._dataChannel.on('open')
+        @self._dataChannel.on("open")
         def on_open():
             if self._closed:
                 return
             logger.debug('DataConsumer DataChannel "open" event')
-            self.emit('open')
+            self.emit("open")
 
         # NOTE: aiortc.RTCDataChannel won't emit error event, here use pyee error event
-        @self._dataChannel.on('error')
+        @self._dataChannel.on("error")
         def on_error(message):
             if self._closed:
                 return
 
             logger.error(f'DataConsumer DataChannel "error" event: {message}')
-            
-            self.emit('error', message)
 
-        @self._dataChannel.on('close')
+            self.emit("error", message)
+
+        @self._dataChannel.on("close")
         def on_close():
             if self._closed:
                 return
             logger.warning('DataConsumer DataChannel "close" event')
             self._closed = True
-            self.emit('@close')
-            self._observer.emit('close')
+            self.emit("@close")
+            self._observer.emit("close")
 
-        @self._dataChannel.on('message')
+        @self._dataChannel.on("message")
         def on_message(message):
             if self._closed:
                 return
-            self.emit('message', message)
+            self.emit("message", message)
```

### Comparing `pymediasoup-0.2.6/pymediasoup/data_producer.py` & `pymediasoup-1.0.0/pymediasoup/data_producer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,8 @@
-import sys
-if sys.version_info >= (3, 8):
-    from typing import Optional, Any, Union, Literal
-else:
-    from typing import Optional, Any, Union
-    from typing_extensions import Literal
+from typing import Optional, Any, Union, Literal
 
 import logging
 from pyee import AsyncIOEventEmitter
 from aiortc import RTCDataChannel
 from pydantic import BaseModel
 from .errors import InvalidStateError
 from .emitter import EnhancedEventEmitter
@@ -21,170 +16,173 @@
     ordered: Optional[bool]
     maxPacketLifeTime: Optional[int]
     maxRetransmits: Optional[int]
     label: Optional[str]
     protocol: Optional[str]
     appData: Optional[dict] = {}
 
+
 class DataProducer(EnhancedEventEmitter):
     def __init__(
         self,
         id: str,
         dataChannel: RTCDataChannel,
         sctpStreamParameters: SctpStreamParameters,
         appData: Optional[dict] = None,
-        loop=None
+        loop=None,
     ):
         super(DataProducer, self).__init__(loop=loop)
 
         # Closed flag.
         self._closed: bool = False
         # Observer instance.
         self._observer: AsyncIOEventEmitter = AsyncIOEventEmitter()
 
         self._id = id
         self._dataChannel = dataChannel
         self._sctpStreamParameters = sctpStreamParameters
         self._appData = appData
-        
+
         self._handleDataChannel()
-    
+
     # DataProducer id.
     @property
     def id(self) -> str:
         return self._id
 
     # Whether the DataProducer is closed.
     @property
     def closed(self) -> bool:
         return self._closed
-    
+
     # SCTP stream parameters.
     @property
     def sctpStreamParameters(self) -> SctpStreamParameters:
         return self._sctpStreamParameters
-    
+
     # DataChannel readyState.
     @property
     def readyState(self) -> Literal["closed", "closing", "connecting", "open"]:
         return self._dataChannel.readyState
-    
+
     # DataChannel label.
     @property
     def label(self) -> str:
         return self._dataChannel.label
-    
+
     # DataChannel protocol.
     @property
     def protocol(self) -> str:
         return self._dataChannel.protocol
-    
+
     # DataChannel bufferedAmount.
     @property
     def bufferedAmount(self) -> int:
         return self._dataChannel.bufferedAmount
-    
+
     # DataChannel bufferedAmountLowThreshold.
     @property
     def bufferedAmountLowThreshold(self) -> int:
         return self._dataChannel.bufferedAmountLowThreshold
-    
+
     # Set DataChannel bufferedAmountLowThreshold.
     @bufferedAmountLowThreshold.setter
     def bufferedAmountLowThreshold(self, bufferedAmountLowThreshold: int):
         self._dataChannel.bufferedAmountLowThreshold = bufferedAmountLowThreshold
-    
+
     # App custom data.
     @property
     def appData(self) -> Any:
         return self._appData
-    
+
     # Invalid setter.
     @appData.setter
     def appData(self, value):
-        raise Exception('cannot override appData object')
-    
+        raise Exception("cannot override appData object")
+
     # Observer.
     @property
     def observer(self) -> AsyncIOEventEmitter:
         return self._observer
-    
+
     # Closes the DataProducer.
     async def close(self):
         if self._closed:
             return
-        
-        logger.debug('DataProducer close()')
+
+        logger.debug("DataProducer close()")
 
         self._closed = True
 
         self._dataChannel.close()
 
-        await self.emit_for_results('@close')
+        await self.emit_for_results("@close")
 
         # Emit observer event.
-        self._observer.emit('close')
-    
+        self._observer.emit("close")
+
     # Transport was closed.
     def transportClosed(self):
         if self._closed:
             return
 
-        logger.debug('DataProducer transportClosed()')
+        logger.debug("DataProducer transportClosed()")
 
         self._closed = True
 
         self._dataChannel.close()
 
-        self.emit('transportclose')
+        self.emit("transportclose")
+
+        self._observer.emit("close")
 
-        self._observer.emit('close')
-    
     # Send a message.
     def send(self, data: Union[bytes, str]):
-        logger.debug('DataProducer send()')
+        logger.debug("DataProducer send()")
 
         if self._closed:
-            raise InvalidStateError('closed')
-        
+            raise InvalidStateError("closed")
+
         self._dataChannel.send(data)
-    
+
     def _handleDataChannel(self):
-        @self._dataChannel.on('open')
+        @self._dataChannel.on("open")
         def on_open():
             if self._closed:
                 return
-            
+
             logger.debug('DataProducer DataChannel "open" event')
 
-            self.emit('open')
+            self.emit("open")
 
         # NOTE: aiortc.RTCDataChannel won't emit error event, here use pyee error event
-        @self._dataChannel.on('error')
+        @self._dataChannel.on("error")
         def on_error(message):
             if self._closed:
                 return
 
             logger.error(f'DataProducer DataChannel "error" event: {message}')
-            
-            self.emit('error', message)
 
-        @self._dataChannel.on('close')
+            self.emit("error", message)
+
+        @self._dataChannel.on("close")
         def on_close():
             if self._closed:
                 return
             logger.warning('DataProducer DataChannel "close" event')
             self._closed = True
-            self.emit('@close')
-            self._observer.emit('close')
+            self.emit("@close")
+            self._observer.emit("close")
 
-        @self._dataChannel.on('message')
+        @self._dataChannel.on("message")
         def on_message(message):
             if self._closed:
                 return
-            logger.warning(f'DataProducer DataChannel "message" event in a DataProducer, message discarded: {message}')
+            logger.warning(
+                f'DataProducer DataChannel "message" event in a DataProducer, message discarded: {message}'
+            )
 
-        @self._dataChannel.on('bufferedamountlow')
+        @self._dataChannel.on("bufferedamountlow")
         def on_bufferedamountlow():
             if self._closed:
                 return
-            self.emit('bufferedamountlow')
+            self.emit("bufferedamountlow")
```

### Comparing `pymediasoup-0.2.6/pymediasoup/device.py` & `pymediasoup-1.0.0/pymediasoup/device.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import sys
-if sys.version_info >= (3, 8):
-    from typing import Optional, Dict, Callable, Literal, List, Any, Union
-else:
-    from typing import Optional, Dict, Callable, List, Any, Union
-    from typing_extensions import Literal
+from typing import Optional, Dict, Callable, Literal, List, Any, Union
 
 import logging
 from pyee import AsyncIOEventEmitter
 from aiortc import RTCIceServer
 from .handlers.handler_interface import HandlerInterface
-from .ortc import ExtendedRtpCapabilities, getExtendedRtpCapabilities, canSend, getRecvRtpCapabilities
+from .ortc import (
+    ExtendedRtpCapabilities,
+    getExtendedRtpCapabilities,
+    canSend,
+    getRecvRtpCapabilities,
+)
 from .rtp_parameters import RtpCapabilities
 from .sctp_parameters import SctpCapabilities, SctpParameters
 from .errors import InvalidStateError
 from .transport import InternalTransportOptions, Transport
 from .models.transport import IceParameters, IceCandidate, DtlsParameters
 
 
@@ -30,195 +30,216 @@
 
         # Extended RTP capabilities.
         self._extendedRtpCapabilities: Optional[ExtendedRtpCapabilities] = None
         # Local RTP capabilities for receiving media.
         self._recvRtpCapabilities: Optional[RtpCapabilities] = None
         # Whether we can produce audio/video based on computed extended RTP
         # capabilities.
-        self._canProduceByKind: Dict[str, bool] = {
-            'audio': False,
-            'video': False
-        }
+        self._canProduceByKind: Dict[str, bool] = {"audio": False, "video": False}
         self._sctpCapabilities: Optional[SctpCapabilities] = None
 
     # The RTC handler name.
     @property
     def handlerName(self) -> str:
         if not self._loaded:
-            raise InvalidStateError('not loaded')
+            raise InvalidStateError("not loaded")
         return self._handlerName
-    
+
     # Whether the Device is loaded.
     @property
     def loaded(self) -> bool:
         return self._loaded
-    
+
     # RTP capabilities of the Device for receiving media.
     # @raise {InvalidStateError} if not loaded.
     @property
     def rtpCapabilities(self) -> Optional[RtpCapabilities]:
         if not self._loaded:
-            raise InvalidStateError('not loaded')
+            raise InvalidStateError("not loaded")
         return self._recvRtpCapabilities
-    
+
     # SCTP capabilities of the Device.
     # @raise {InvalidStateError} if not loaded.
     @property
     def sctpCapabilities(self) -> Optional[SctpCapabilities]:
         if not self._loaded:
-            raise InvalidStateError('not loaded')
+            raise InvalidStateError("not loaded")
         return self._sctpCapabilities
-    
+
     # Observer.
     # @emits newtransport - (Transport)
     @property
     def observer(self):
         return self._observer
-    
+
     # Initialize the Device.
     async def load(self, routerRtpCapabilities: Union[RtpCapabilities, dict]):
-        logger.debug(f'Device load() [routerRtpCapabilities:{routerRtpCapabilities}]')
+        logger.debug(f"Device load() [routerRtpCapabilities:{routerRtpCapabilities}]")
         if isinstance(routerRtpCapabilities, dict):
-            routerRtpCapabilities:RtpCapabilities = RtpCapabilities(**routerRtpCapabilities)
+            routerRtpCapabilities: RtpCapabilities = RtpCapabilities(
+                **routerRtpCapabilities
+            )
         else:
-            routerRtpCapabilities:RtpCapabilities = routerRtpCapabilities.copy(deep=True)
+            routerRtpCapabilities: RtpCapabilities = routerRtpCapabilities.copy(
+                deep=True
+            )
         # Temporal handler to get its capabilities.
         if self._loaded:
-            logger.warning('already loaded')
+            logger.warning("already loaded")
             return
         handler: HandlerInterface = self._handlerFactory()
         nativeRtpCapabilities = await handler.getNativeRtpCapabilities()
-        logger.debug(f'Device load() | got native RTP capabilities:{nativeRtpCapabilities}')
+        logger.debug(
+            f"Device load() | got native RTP capabilities:{nativeRtpCapabilities}"
+        )
         # Get extended RTP capabilities.
-        self._extendedRtpCapabilities = getExtendedRtpCapabilities(nativeRtpCapabilities, routerRtpCapabilities)
-        logger.debug(f'Device load() | got extended RTP capabilities:{self._extendedRtpCapabilities}')
+        self._extendedRtpCapabilities = getExtendedRtpCapabilities(
+            nativeRtpCapabilities, routerRtpCapabilities
+        )
+        logger.debug(
+            f"Device load() | got extended RTP capabilities:{self._extendedRtpCapabilities}"
+        )
         # Check whether we can produce audio/video.
-        self._canProduceByKind['audio'] = canSend('audio', self._extendedRtpCapabilities)
-        self._canProduceByKind['video'] = canSend('video', self._extendedRtpCapabilities)
+        self._canProduceByKind["audio"] = canSend(
+            "audio", self._extendedRtpCapabilities
+        )
+        self._canProduceByKind["video"] = canSend(
+            "video", self._extendedRtpCapabilities
+        )
         # Generate our receiving RTP capabilities for receiving media.
-        self._recvRtpCapabilities = getRecvRtpCapabilities(self._extendedRtpCapabilities)
-        logger.debug(f'Device load() | got receiving RTP capabilities:{self._recvRtpCapabilities}')
+        self._recvRtpCapabilities = getRecvRtpCapabilities(
+            self._extendedRtpCapabilities
+        )
+        logger.debug(
+            f"Device load() | got receiving RTP capabilities:{self._recvRtpCapabilities}"
+        )
         # Generate our SCTP capabilities.
         self._sctpCapabilities = await handler.getNativeSctpCapabilities()
-        logger.debug(f'Device load() | got native SCTP capabilities:{self._sctpCapabilities}')
-        logger.debug('Device load() succeeded')
+        logger.debug(
+            f"Device load() | got native SCTP capabilities:{self._sctpCapabilities}"
+        )
+        logger.debug("Device load() succeeded")
         self._loaded = True
         self._handlerName = handler.name
         await handler.close()
 
     # Whether we can produce audio/video.
     # @raise {InvalidStateError} if not loaded.
     # @raise {TypeError} if wrong arguments.
-    def canProduce(self, kind: Literal['video', 'audio']):
+    def canProduce(self, kind: Literal["video", "audio"]):
         if not self._loaded:
-            raise InvalidStateError('not loaded')
-        elif kind not in ['video', 'audio']:
-            raise TypeError(f'invalid kind {kind}')
+            raise InvalidStateError("not loaded")
+        elif kind not in ["video", "audio"]:
+            raise TypeError(f"invalid kind {kind}")
         return self._canProduceByKind[kind]
-    
+
     # Creates a Transport for sending media.
     # @raise {InvalidStateError} if not loaded.
     # @raise {TypeError} if wrong arguments.
     def createSendTransport(
         self,
         id: str,
         iceParameters: IceParameters,
         iceCandidates: List[IceCandidate],
         dtlsParameters: DtlsParameters,
         sctpParameters: Optional[SctpParameters],
         iceServers: Optional[List[RTCIceServer]] = None,
-        iceTransportPolicy: Optional[Literal['all', 'relay']] = None,
+        iceTransportPolicy: Optional[Literal["all", "relay"]] = None,
         additionalSettings: Optional[dict] = None,
         proprietaryConstraints: Any = None,
-        appData: Optional[dict] = {}
+        appData: Optional[dict] = {},
     ) -> Transport:
-        logger.debug('createSendTransport()')
+        logger.debug("createSendTransport()")
         return self._createTransport(
-            direction='send',
+            direction="send",
             id=id,
             iceParameters=iceParameters,
             iceCandidates=iceCandidates,
             dtlsParameters=dtlsParameters,
             sctpParameters=sctpParameters,
             iceServers=iceServers,
             iceTransportPolicy=iceTransportPolicy,
             additionalSettings=additionalSettings,
             proprietaryConstraints=proprietaryConstraints,
-            appData=appData
+            appData=appData,
         )
-    
+
     # Creates a Transport for receiving media.
     # @raise {InvalidStateError} if not loaded.
     # @raise {TypeError} if wrong arguments.
     def createRecvTransport(
         self,
         id: str,
         iceParameters: Union[IceParameters, dict],
         iceCandidates: List[Union[IceCandidate, dict]],
         dtlsParameters: Union[DtlsParameters, dict],
         sctpParameters: Optional[Union[SctpParameters, dict]] = None,
         iceServers: Optional[List[RTCIceServer]] = None,
-        iceTransportPolicy: Optional[Literal['all', 'relay']] = None,
+        iceTransportPolicy: Optional[Literal["all", "relay"]] = None,
         additionalSettings: Optional[dict] = None,
         proprietaryConstraints: Any = None,
-        appData: Optional[dict] = {}
+        appData: Optional[dict] = {},
     ) -> Transport:
-        logger.debug('createRecvTransport()')
+        logger.debug("createRecvTransport()")
         if isinstance(iceParameters, dict):
             iceParameters: IceParameters = IceParameters(**iceParameters)
-        
-        iceCandidates = [IceCandidate(**c) if isinstance(c, dict) else c for c in iceCandidates]
-        
+
+        iceCandidates = [
+            IceCandidate(**c) if isinstance(c, dict) else c for c in iceCandidates
+        ]
+
         if isinstance(dtlsParameters, dict):
             dtlsParameters: DtlsParameters = DtlsParameters(**dtlsParameters)
-        
+
         if isinstance(sctpParameters, dict):
             sctpParameters: SctpParameters = SctpParameters(**sctpParameters)
-        
+
         return self._createTransport(
-            direction='recv',
+            direction="recv",
             id=id,
             iceParameters=iceParameters,
             iceCandidates=iceCandidates,
             dtlsParameters=dtlsParameters,
             sctpParameters=sctpParameters,
             iceServers=iceServers,
             iceTransportPolicy=iceTransportPolicy,
             additionalSettings=additionalSettings,
             proprietaryConstraints=proprietaryConstraints,
-            appData=appData
+            appData=appData,
         )
-    
+
     def _createTransport(
         self,
-        direction: Literal['send', 'recv'],
+        direction: Literal["send", "recv"],
         id: str,
         iceParameters: IceParameters,
         iceCandidates: List[IceCandidate],
         dtlsParameters: DtlsParameters,
         sctpParameters: Optional[SctpParameters],
         iceServers: Optional[List[RTCIceServer]] = None,
-        iceTransportPolicy: Optional[Literal['all', 'relay']] = None,
+        iceTransportPolicy: Optional[Literal["all", "relay"]] = None,
         additionalSettings: Optional[dict] = None,
         proprietaryConstraints: Any = None,
-        appData: Optional[dict] = {}
+        appData: Optional[dict] = {},
     ) -> Transport:
         if not self._loaded:
-            raise InvalidStateError('not loaded')
-        transport = Transport(options=InternalTransportOptions(
-            direction=direction,
-            handlerFactory=self._handlerFactory,
-            extendedRtpCapabilities=self._extendedRtpCapabilities,
-            canProduceByKind=self._canProduceByKind,
-            id=id,
-            iceParameters=iceParameters,
-            iceCandidates=iceCandidates,
-            dtlsParameters=dtlsParameters,
-            sctpParameters=sctpParameters,
-            iceServers=iceServers,
-            iceTransportPolicy=iceTransportPolicy,
-            additionalSettings=additionalSettings,
-            proprietaryConstraints=proprietaryConstraints,
-            appData=appData
-        ))
-    
+            raise InvalidStateError("not loaded")
+        transport = Transport(
+            options=InternalTransportOptions(
+                direction=direction,
+                handlerFactory=self._handlerFactory,
+                extendedRtpCapabilities=self._extendedRtpCapabilities,
+                canProduceByKind=self._canProduceByKind,
+                id=id,
+                iceParameters=iceParameters,
+                iceCandidates=iceCandidates,
+                dtlsParameters=dtlsParameters,
+                sctpParameters=sctpParameters,
+                iceServers=iceServers,
+                iceTransportPolicy=iceTransportPolicy,
+                additionalSettings=additionalSettings,
+                proprietaryConstraints=proprietaryConstraints,
+                appData=appData,
+            )
+        )
+
         return transport
```

### Comparing `pymediasoup-0.2.6/pymediasoup/emitter.py` & `pymediasoup-1.0.0/pymediasoup/emitter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-import inspect
 from pyee import AsyncIOEventEmitter
 
+
 class EnhancedEventEmitter(AsyncIOEventEmitter):
     def __init__(self, loop=None):
         super(EnhancedEventEmitter, self).__init__(loop=loop)
-    
+
     async def emit_for_results(self, event, *args, **kwargs):
         results = []
         for f in list(self._events[event].values()):
             try:
                 result = await f(*args, **kwargs)
             except Exception as exc:
-                self.emit('error', exc)
+                self.emit("error", exc)
             else:
                 if result:
                     results.append(result)
-        return results
+        return results
```

### Comparing `pymediasoup-0.2.6/pymediasoup/handlers/aiortc_handler.py` & `pymediasoup-1.0.0/pymediasoup/handlers/aiortc_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,59 @@
-import sys
-if sys.version_info >= (3, 8):
-    from typing import Dict, Literal, List, Optional, Any
-else:
-    from typing import Dict, List, Optional, Any
-    from typing_extensions import Literal
+from typing import Dict, Literal, List, Optional, Any
 
 import logging
-from aiortc import RTCIceServer, RTCPeerConnection, RTCSessionDescription, RTCRtpTransceiver, MediaStreamTrack
+from aiortc import (
+    RTCIceServer,
+    RTCPeerConnection,
+    RTCSessionDescription,
+    RTCRtpTransceiver,
+    MediaStreamTrack,
+)
 import sdp_transform
 from .sdp import common_utils
 from .sdp.remote_sdp import RemoteSdp
 from .sdp.unified_plan_utils import addLegacySimulcast, getRtpEncodings
 from .sdp.common_utils import applyCodecParameters, extractDtlsParameters
 from .handler_interface import HandlerInterface
 from ..ortc import ExtendedRtpCapabilities
-from ..rtp_parameters import MediaKind, RtpParameters, RtpCapabilities, RtpCodecCapability, RtpEncodingParameters, RtcpParameters
+from ..rtp_parameters import (
+    MediaKind,
+    RtpParameters,
+    RtpCapabilities,
+    RtpCodecCapability,
+    RtpEncodingParameters,
+    RtcpParameters,
+)
 from ..sctp_parameters import SctpCapabilities, SctpParameters, SctpStreamParameters
 from ..ortc import getSendingRtpParameters, getSendingRemoteRtpParameters, reduceCodecs
 from ..scalability_modes import parse as smParse
 from ..models.transport import IceCandidate, IceParameters, DtlsParameters, DtlsRole
-from ..models.handler_interface import HandlerRunOptions, HandlerSendOptions, HandlerSendResult, HandlerSendDataChannelResult, HandlerReceiveDataChannelResult, HandlerReceiveOptions, HandlerReceiveResult, HandlerReceiveDataChannelOptions
+from ..models.handler_interface import (
+    HandlerRunOptions,
+    HandlerSendOptions,
+    HandlerSendResult,
+    HandlerSendDataChannelResult,
+    HandlerReceiveDataChannelResult,
+    HandlerReceiveOptions,
+    HandlerReceiveResult,
+    HandlerReceiveDataChannelOptions,
+)
 from ..producer import ProducerCodecOptions
 
 
 logger = logging.getLogger(__name__)
-SCTP_NUM_STREAMS = { 'OS': 1024, 'MIS': 1024 }
+SCTP_NUM_STREAMS = {"OS": 1024, "MIS": 1024}
+
 
 class AiortcHandler(HandlerInterface):
 
-    def __init__(self, tracks: List[MediaStreamTrack]=[], loop=None):
+    def __init__(self, tracks: List[MediaStreamTrack] = [], loop=None):
         super(AiortcHandler, self).__init__(loop=loop)
         # Handler direction.
-        self._direction: Optional[Literal['send', 'recv']] = None
+        self._direction: Optional[Literal["send", "recv"]] = None
         # Remote SDP handler.
         self._remoteSdp: Optional[RemoteSdp] = None
         # Generic sending RTP parameters for audio and video.
         self._sendingRtpParametersByKind: Dict[str, RtpParameters] = {}
         # Generic sending RTP parameters for audio and video suitable for the SDP
         # remote answer.
         self._sendingRemoteRtpParametersByKind: Dict[str, RtpParameters] = {}
@@ -48,218 +66,246 @@
         # Sending DataChannel id value counter. Incremented for each new DataChannel.
         self._nextSendSctpStreamId = 0
         # Got transport local and remote parameters.
         self._transportReady = False
         self._tracks = tracks
 
     @classmethod
-    def createFactory(cls, tracks: List[MediaStreamTrack]=[], loop=None):
+    def createFactory(cls, tracks: List[MediaStreamTrack] = [], loop=None):
         return lambda: cls(tracks, loop)
 
     @property
     def name(self) -> str:
-        return 'aiortc'
-    
+        return "aiortc"
+
     @property
     def pc(self) -> RTCPeerConnection:
         if self._pc:
             return self._pc
         else:
-            raise Exception('PeerConnection not ready')
-    
+            raise Exception("PeerConnection not ready")
+
     @property
     def remoteSdp(self) -> RemoteSdp:
         if self._remoteSdp:
             return self._remoteSdp
         else:
-            raise Exception('Remote SDP not ready')
-    
+            raise Exception("Remote SDP not ready")
+
     async def close(self):
-        logger.debug('close()')
+        logger.debug("close()")
 
         if self._pc:
             await self._pc.close()
 
     async def getNativeRtpCapabilities(self) -> RtpCapabilities:
-        logger.debug('getNativeRtpCapabilities()')
+        logger.debug("getNativeRtpCapabilities()")
 
         pc = RTCPeerConnection()
         for track in self._tracks:
             pc.addTrack(track)
-        pc.addTransceiver('audio')
-        pc.addTransceiver('video')
+        pc.addTransceiver("audio")
+        pc.addTransceiver("video")
 
         offer: RTCSessionDescription = await pc.createOffer()
         await pc.close()
 
         sdpDict: dict = sdp_transform.parse(offer.sdp)
-        nativeRtpCapabilities:RtpCapabilities = common_utils.extractRtpCapabilities(sdpDict)
+        nativeRtpCapabilities: RtpCapabilities = common_utils.extractRtpCapabilities(
+            sdpDict
+        )
 
         return nativeRtpCapabilities
-    
+
     async def getNativeSctpCapabilities(self) -> SctpCapabilities:
-        logger.debug('getNativeSctpCapabilities()')
-        return SctpCapabilities.parse_obj({
-            'numStreams': SCTP_NUM_STREAMS
-        })
-    
+        logger.debug("getNativeSctpCapabilities()")
+        return SctpCapabilities.parse_obj({"numStreams": SCTP_NUM_STREAMS})
+
     def run(
         self,
-        direction: Literal['send', 'recv'],
+        direction: Literal["send", "recv"],
         iceParameters: IceParameters,
         iceCandidates: List[IceCandidate],
         dtlsParameters: DtlsParameters,
         extendedRtpCapabilities: ExtendedRtpCapabilities,
-        sctpParameters: Optional[SctpParameters]=None,
-        iceServers: Optional[RTCIceServer]=None,
-        iceTransportPolicy: Optional[Literal['all', 'relay']]=None,
-        additionalSettings: Optional[Any]=None,
-        proprietaryConstraints: Optional[Any]=None
+        sctpParameters: Optional[SctpParameters] = None,
+        iceServers: Optional[RTCIceServer] = None,
+        iceTransportPolicy: Optional[Literal["all", "relay"]] = None,
+        additionalSettings: Optional[Any] = None,
+        proprietaryConstraints: Optional[Any] = None,
     ):
-        logger.debug('AiortcHandler run()')
+        logger.debug("AiortcHandler run()")
         options = HandlerRunOptions(
             direction=direction,
             iceParameters=iceParameters,
             iceCandidates=iceCandidates,
             dtlsParameters=dtlsParameters,
             sctpParameters=sctpParameters,
             iceServers=iceServers,
             iceTransportPolicy=iceTransportPolicy,
             additionalSettings=additionalSettings,
             proprietaryConstraints=proprietaryConstraints,
-            extendedRtpCapabilities=extendedRtpCapabilities
+            extendedRtpCapabilities=extendedRtpCapabilities,
         )
         self._direction = options.direction
         self._remoteSdp = RemoteSdp(
             iceParameters=options.iceParameters,
             iceCandidates=options.iceCandidates,
             dtlsParameters=options.dtlsParameters,
-            sctpParameters=options.sctpParameters
+            sctpParameters=options.sctpParameters,
         )
         self._sendingRtpParametersByKind = {
-            'audio': getSendingRtpParameters('audio', options.extendedRtpCapabilities),
-            'video': getSendingRtpParameters('video', options.extendedRtpCapabilities)
+            "audio": getSendingRtpParameters("audio", options.extendedRtpCapabilities),
+            "video": getSendingRtpParameters("video", options.extendedRtpCapabilities),
         }
         self._sendingRemoteRtpParametersByKind = {
-            'audio': getSendingRemoteRtpParameters('audio', options.extendedRtpCapabilities),
-            'video': getSendingRemoteRtpParameters('video', options.extendedRtpCapabilities)
+            "audio": getSendingRemoteRtpParameters(
+                "audio", options.extendedRtpCapabilities
+            ),
+            "video": getSendingRemoteRtpParameters(
+                "video", options.extendedRtpCapabilities
+            ),
         }
         self._pc = RTCPeerConnection()
 
-        @self._pc.on('iceconnectionstatechange')
+        @self._pc.on("iceconnectionstatechange")
         def on_iceconnectionstatechange():
-            if self._pc.iceConnectionState == 'checking':
-                self.emit('@connectionstatechange', 'connecting')
-            elif self._pc.iceConnectionState in ['connected', 'completed']:
-                self.emit('@connectionstatechange', 'connected')
-            elif self._pc.iceConnectionState == 'failed':
-                self.emit('@connectionstatechange', 'failed')
-            elif self._pc.iceConnectionState == 'disconnected':
-                self.emit('@connectionstatechange', 'disconnected')
-            elif self._pc.iceConnectionState == 'closed':
-                self.emit('@connectionstatechange', 'closed')
-        
+            if self._pc.iceConnectionState == "checking":
+                self.emit("@connectionstatechange", "connecting")
+            elif self._pc.iceConnectionState in ["connected", "completed"]:
+                self.emit("@connectionstatechange", "connected")
+            elif self._pc.iceConnectionState == "failed":
+                self.emit("@connectionstatechange", "failed")
+            elif self._pc.iceConnectionState == "disconnected":
+                self.emit("@connectionstatechange", "disconnected")
+            elif self._pc.iceConnectionState == "closed":
+                self.emit("@connectionstatechange", "closed")
+
     async def updateIceServers(self, iceServers):
-        logger.warning('updateIceServers() not implemented')
+        logger.warning("updateIceServers() not implemented")
         # TODO: aiortc can not update iceServers
-    
+
     async def restartIce(self, iceParameters):
-        logger.debug('restartIce()')
+        logger.debug("restartIce()")
         self._remoteSdp.updateIceParameters(iceParameters)
         if not self._transportReady:
             return
-        if self._direction == 'send':
+        if self._direction == "send":
             # NOTE: aiortc RTCPeerConnection createOffer do not have iceRestart options
             offer = await self._pc.createOffer()
-            logger.debug(f'restartIce() | calling pc.setLocalDescription() [offer:{offer}]')
+            logger.debug(
+                f"restartIce() | calling pc.setLocalDescription() [offer:{offer}]"
+            )
             await self._pc.setLocalDescription(offer)
             answer: RTCSessionDescription = RTCSessionDescription(
-                type='answer',
-                sdp=self._remoteSdp.getSdp()
+                type="answer", sdp=self._remoteSdp.getSdp()
+            )
+            logger.debug(
+                f"restartIce() | calling pc.setRemoteDescription() [answer:{answer}]"
             )
-            logger.debug(f'restartIce() | calling pc.setRemoteDescription() [answer:{answer}]')
             await self._pc.setRemoteDescription(answer)
         else:
             offer: RTCSessionDescription = RTCSessionDescription(
-                type='offer',
-                sdp=self._remoteSdp.getSdp()
+                type="offer", sdp=self._remoteSdp.getSdp()
+            )
+            logger.debug(
+                f"restartIce() | calling pc.setRemoteDescription() [offer:{offer}]"
             )
-            logger.debug(f'restartIce() | calling pc.setRemoteDescription() [offer:{offer}]')
             await self._pc.setRemoteDescription(offer)
             answer = await self._pc.createAnswer()
-            logger.debug(f'restartIce() | calling pc.setLocalDescription() [answer:{answer}]')
+            logger.debug(
+                f"restartIce() | calling pc.setLocalDescription() [answer:{answer}]"
+            )
             await self._pc.setLocalDescription(answer)
-        
+
     async def getTransportStats(self):
         return self._pc.getStats()
 
     async def send(
         self,
         track: MediaStreamTrack,
-        encodings: List[RtpEncodingParameters]=[],
-        codecOptions: Optional[ProducerCodecOptions]=None,
-        codec: Optional[RtpCodecCapability]=None
+        encodings: List[RtpEncodingParameters] = [],
+        codecOptions: Optional[ProducerCodecOptions] = None,
+        codec: Optional[RtpCodecCapability] = None,
     ) -> HandlerSendResult:
         options = HandlerSendOptions(
-            track=track,
-            encodings=encodings,
-            codecOptions=codecOptions,
-            codec=codec
+            track=track, encodings=encodings, codecOptions=codecOptions, codec=codec
         )
         self._assertSendDirection()
-        logger.debug(f'send() [kind:{options.track.kind}, track.id:{options.track.id}]')
+        logger.debug(f"send() [kind:{options.track.kind}, track.id:{options.track.id}]")
         if options.encodings:
             for idx in range(len(options.encodings)):
-                options.encodings[idx].rid = f'r{idx}'
+                options.encodings[idx].rid = f"r{idx}"
 
-        sendingRtpParameters: RtpParameters = self._sendingRtpParametersByKind[options.track.kind].copy(deep=True)
-        sendingRtpParameters.codecs = reduceCodecs(sendingRtpParameters.codecs, options.codec)
+        sendingRtpParameters: RtpParameters = self._sendingRtpParametersByKind[
+            options.track.kind
+        ].copy(deep=True)
+        sendingRtpParameters.codecs = reduceCodecs(
+            sendingRtpParameters.codecs, options.codec
+        )
 
-        sendingRemoteRtpParameters: RtpParameters = self._sendingRemoteRtpParametersByKind[options.track.kind].copy(deep=True)
-        sendingRemoteRtpParameters.codecs = reduceCodecs(sendingRemoteRtpParameters.codecs, options.codec)
+        sendingRemoteRtpParameters: RtpParameters = (
+            self._sendingRemoteRtpParametersByKind[options.track.kind].copy(deep=True)
+        )
+        sendingRemoteRtpParameters.codecs = reduceCodecs(
+            sendingRemoteRtpParameters.codecs, options.codec
+        )
 
         mediaSectionIdx = self.remoteSdp.getNextMediaSectionIdx()
-        transceiver = self.pc.addTransceiver(options.track, direction='sendonly')
+        transceiver = self.pc.addTransceiver(options.track, direction="sendonly")
 
-        offer: RTCSessionDescription  = await self.pc.createOffer()
+        offer: RTCSessionDescription = await self.pc.createOffer()
         offerMediaDict: dict
         localSdpDict = sdp_transform.parse(offer.sdp)
         if not self._transportReady:
-            await self._setupTransport(localDtlsRole='server', localSdpDict=localSdpDict)
+            await self._setupTransport(
+                localDtlsRole="server", localSdpDict=localSdpDict
+            )
         # Special case for VP9 with SVC.
         hackVp9Svc = False
         if options.encodings:
-            layers=smParse(options.encodings[0].scalabilityMode if options.encodings[0].scalabilityMode else '')
+            layers = smParse(
+                options.encodings[0].scalabilityMode
+                if options.encodings[0].scalabilityMode
+                else ""
+            )
         else:
-            layers=smParse('')
-        if len(options.encodings) == 1 and layers.spatialLayers > 1 and sendingRtpParameters.codecs[0].mimeType.lower() == 'video/vp9':
-            logger.debug('send() | enabling legacy simulcast for VP9 SVC')
+            layers = smParse("")
+        if (
+            len(options.encodings) == 1
+            and layers.spatialLayers > 1
+            and sendingRtpParameters.codecs[0].mimeType.lower() == "video/vp9"
+        ):
+            logger.debug("send() | enabling legacy simulcast for VP9 SVC")
             hackVp9Svc = True
             localSdpDict = sdp_transform.parse
-            offerMediaDict = localSdpDict['media'][mediaSectionIdx.idx]
-            addLegacySimulcast(offerMediaDict=offerMediaDict, numStreams=layers.spatialLayers)
+            offerMediaDict = localSdpDict["media"][mediaSectionIdx.idx]
+            addLegacySimulcast(
+                offerMediaDict=offerMediaDict, numStreams=layers.spatialLayers
+            )
             offer = RTCSessionDescription(
-                type='offer',
-                sdp=sdp_transform.write(localSdpDict)
+                type="offer", sdp=sdp_transform.write(localSdpDict)
             )
-        
-        logger.debug(f'send() | calling pc.setLocalDescription() [offer:{offer}]')
+
+        logger.debug(f"send() | calling pc.setLocalDescription() [offer:{offer}]")
 
         await self.pc.setLocalDescription(offer)
         # We can now get the transceiver.mid.
         localId = transceiver.mid
         # Set MID.
         sendingRtpParameters.mid = localId
         localSdpDict = sdp_transform.parse(self.pc.localDescription.sdp)
 
-        offerMediaDict = localSdpDict['media'][mediaSectionIdx.idx]
+        offerMediaDict = localSdpDict["media"][mediaSectionIdx.idx]
 
-        logger.debug(f"send() | get offerMediaDict {offerMediaDict} \n from localSdpDict {localSdpDict['media']} index {mediaSectionIdx.idx}")
+        logger.debug(
+            f"send() | get offerMediaDict {offerMediaDict} \n from localSdpDict {localSdpDict['media']} index {mediaSectionIdx.idx}"  # noqa
+        )
         # Set RTCP CNAME.
-        if sendingRtpParameters.rtcp == None:
+        if sendingRtpParameters.rtcp is None:
             sendingRtpParameters.rtcp = RtcpParameters()
         sendingRtpParameters.rtcp.cname = common_utils.getCname(offerMediaDict)
         # Set RTP encodings by parsing the SDP offer if no encodings are given.
         if not options.encodings:
             sendingRtpParameters.encodings = getRtpEncodings(offerMediaDict)
         # Set RTP encodings by parsing the SDP offer and complete them with given
         # one if just a single encoding has been given.
@@ -274,37 +320,39 @@
                     newEncodings = [newEncodings[0]]
             sendingRtpParameters.encodings = newEncodings
         # Otherwise if more than 1 encoding are given use them verbatim.
         else:
             sendingRtpParameters.encodings = options.encodings
         # If VP8 or H264 and there is effective simulcast, add scalabilityMode to
         # each encoding.
-        if len(sendingRtpParameters.encodings) > 1 and (sendingRtpParameters.codecs[0].mimeType.lower() == 'video/vp8' or sendingRtpParameters.codecs[0].mimeType.lower() == 'video/h264'):
+        if len(sendingRtpParameters.encodings) > 1 and (
+            sendingRtpParameters.codecs[0].mimeType.lower() == "video/vp8"
+            or sendingRtpParameters.codecs[0].mimeType.lower() == "video/h264"
+        ):
             for encoding in sendingRtpParameters.encodings:
-                encoding.scalabilityMode = 'S1T3'
+                encoding.scalabilityMode = "S1T3"
         self.remoteSdp.send(
             offerMediaDict=offerMediaDict,
             reuseMid=mediaSectionIdx.reuseMid,
             offerRtpParameters=sendingRtpParameters,
             answerRtpParameters=sendingRemoteRtpParameters,
             codecOptions=options.codecOptions,
-            extmapAllowMixed=True
+            extmapAllowMixed=True,
         )
         answer: RTCSessionDescription = RTCSessionDescription(
-            type='answer',
-            sdp=self.remoteSdp.getSdp()
+            type="answer", sdp=self.remoteSdp.getSdp()
         )
-        logger.debug(f'send() | calling pc.setRemoteDescription() [answer:{answer}]')
+        logger.debug(f"send() | calling pc.setRemoteDescription() [answer:{answer}]")
         await self.pc.setRemoteDescription(answer)
         # Store in the map.
         self._mapMidTransceiver[localId] = transceiver
         return HandlerSendResult(
             localId=localId,
             rtpParameters=sendingRtpParameters,
-            rtpSender=transceiver.sender
+            rtpSender=transceiver.sender,
         )
 
     async def stopSending(self, localId):
         pass
         # self._assertSendDirection()
         # logger.debug(f'stopSending() [localId:{localId}]')
         # transceiver = self._mapMidTransceiver.get(localId)
@@ -320,243 +368,266 @@
         # answer: RTCSessionDescription = RTCSessionDescription(
         #     type='answer',
         #     sdp=self._remoteSdp.getSdp()
         # )
         # logger.debug(f'stopSending() | calling pc.setRemoteDescription() [answer:{answer}]')
         # await self._pc.setRemoteDescription(answer)
         # self._mapMidTransceiver.pop(localId, None)
-    
+
     async def replaceTrack(self, localId, track=None):
         self._assertSendDirection()
         if track:
-            logger.debug(f'replaceTrack() [localId:{localId}, track.id:{track.id}]')
+            logger.debug(f"replaceTrack() [localId:{localId}, track.id:{track.id}]")
         else:
-            logger.debug(f'replaceTrack() [localId:{localId}, no track]')
+            logger.debug(f"replaceTrack() [localId:{localId}, no track]")
         transceiver = self._mapMidTransceiver.get(localId)
         if not transceiver:
-            raise Exception('associated RTCRtpTransceiver not found')
+            raise Exception("associated RTCRtpTransceiver not found")
 
         await transceiver.sender.replaceTrack(track)
-    
+
     async def setMaxSpatialLayer(self, localId: str, spatialLayer: int):
-        logger.warning('setMaxSpatialLayer() not implemented')
+        logger.warning("setMaxSpatialLayer() not implemented")
         # NOTE: RTCRtpSender do not have getParameters()
         # self._assertSendDirection()
         # logger.debug(f'setMaxSpatialLayer() [localId:{localId}, spatialLayer:{spatialLayer}]')
         # transceiver = self._mapMidTransceiver.get(localId)
         # if not transceiver:
         #     raise Exception('associated RTCRtpTransceiver not found')
         # parameters = transceiver.sender.getParameters()
-    
+
     async def setRtpEncodingParameters(self, localId: str, params: Any):
-        logger.warning('setRtpEncodingParameters() not implemented')
+        logger.warning("setRtpEncodingParameters() not implemented")
         # NOTE: RTCRtpSender do not have getParameters()
-    
+
     async def getSenderStats(self, localId: str):
         self._assertSendDirection()
         transceiver = self._mapMidTransceiver.get(localId)
         if not transceiver:
-            raise Exception('associated RTCRtpTransceiver not found')
+            raise Exception("associated RTCRtpTransceiver not found")
         return await transceiver.sender.getStats()
-    
+
     async def sendDataChannel(
         self,
-        streamId: Optional[int]=None,
-        ordered: Optional[bool]=True,
-        maxPacketLifeTime: Optional[int]=None,
-        maxRetransmits: Optional[int]=None,
-        label: Optional[str]=None,
-        protocol: Optional[str]=None
+        streamId: Optional[int] = None,
+        ordered: Optional[bool] = True,
+        maxPacketLifeTime: Optional[int] = None,
+        maxRetransmits: Optional[int] = None,
+        label: Optional[str] = None,
+        protocol: Optional[str] = None,
     ) -> HandlerSendDataChannelResult:
-        if streamId == None:
+        if streamId is None:
             streamId = self._nextSendSctpStreamId
-        options=SctpStreamParameters(
+        options = SctpStreamParameters(
             streamId=streamId,
             ordered=ordered,
             maxPacketLifeTime=maxPacketLifeTime,
             maxRetransmits=maxRetransmits,
             label=label,
-            protocol=protocol
+            protocol=protocol,
         )
         self._assertSendDirection()
-        logger.debug('sendDataChannel()')
+        logger.debug("sendDataChannel()")
         dataChannel = self.pc.createDataChannel(
             label=options.label,
             maxPacketLifeTime=options.maxPacketLifeTime,
             ordered=options.ordered,
             protocol=options.protocol,
             negotiated=True,
-            id=self._nextSendSctpStreamId
+            id=self._nextSendSctpStreamId,
         )
         # Increase next id.
-        self._nextSendSctpStreamId = (self._nextSendSctpStreamId + 1) % SCTP_NUM_STREAMS.get('MIS', 1)
+        self._nextSendSctpStreamId = (
+            self._nextSendSctpStreamId + 1
+        ) % SCTP_NUM_STREAMS.get("MIS", 1)
         # If this is the first DataChannel we need to create the SDP answer with
         # m=application section.
         if not self._hasDataChannelMediaSection:
             offer: RTCSessionDescription = await self.pc.createOffer()
             localSdpDict = sdp_transform.parse(offer.sdp)
-            offerMediaDicts = [m for m in localSdpDict.get('media') if m.get('type') == 'application']
+            offerMediaDicts = [
+                m for m in localSdpDict.get("media") if m.get("type") == "application"
+            ]
             if not offerMediaDicts:
-                raise Exception('No datachannel')
+                raise Exception("No datachannel")
             offerMediaDict = offerMediaDicts[0]
 
             if not self._transportReady:
-                await self._setupTransport(localDtlsRole='server', localSdpDict=localSdpDict)
-            
-            logger.debug(f'sendDataChannel() | calling pc.setLocalDescription() [offer:{offer}]')
+                await self._setupTransport(
+                    localDtlsRole="server", localSdpDict=localSdpDict
+                )
+
+            logger.debug(
+                f"sendDataChannel() | calling pc.setLocalDescription() [offer:{offer}]"
+            )
             await self.pc.setLocalDescription(offer)
             self.remoteSdp.sendSctpAssociation(offerMediaDict=offerMediaDict)
             answer: RTCSessionDescription = RTCSessionDescription(
-                type='answer',
-                sdp=self.remoteSdp.getSdp()
+                type="answer", sdp=self.remoteSdp.getSdp()
             )
 
-            logger.debug(f'sendDataChannel() | calling pc.setRemoteDescription() [answer:{answer}]')
+            logger.debug(
+                f"sendDataChannel() | calling pc.setRemoteDescription() [answer:{answer}]"
+            )
             await self.pc.setRemoteDescription(answer)
             self._hasDataChannelMediaSection = True
-        
+
         return HandlerSendDataChannelResult(
-            dataChannel=dataChannel,
-            sctpStreamParameters=options
+            dataChannel=dataChannel, sctpStreamParameters=options
         )
-    
+
     async def receive(
-        self,
-        trackId: str,
-        kind: MediaKind,
-        rtpParameters: RtpParameters
+        self, trackId: str, kind: MediaKind, rtpParameters: RtpParameters
     ) -> HandlerReceiveResult:
         options = HandlerReceiveOptions(
-            trackId=trackId,
-            kind=kind,
-            rtpParameters=rtpParameters
+            trackId=trackId, kind=kind, rtpParameters=rtpParameters
         )
         self._assertRecvDirection()
-        logger.debug(f'receive() [trackId:{options.trackId}, kind:{options.kind}]')
-        localId = options.rtpParameters.mid if options.rtpParameters.mid != None else str(len(self._mapMidTransceiver))
+        logger.debug(f"receive() [trackId:{options.trackId}, kind:{options.kind}]")
+        localId = (
+            options.rtpParameters.mid
+            if options.rtpParameters.mid is not None
+            else str(len(self._mapMidTransceiver))
+        )
         self.remoteSdp.receive(
             mid=localId,
             kind=options.kind,
             offerRtpParameters=options.rtpParameters,
             streamId=options.rtpParameters.rtcp.cname,
-            trackId=options.trackId
+            trackId=options.trackId,
         )
         offer: RTCSessionDescription = RTCSessionDescription(
-            type='offer',
-            sdp=self.remoteSdp.getSdp()
+            type="offer", sdp=self.remoteSdp.getSdp()
         )
-        logger.debug(f'receive() | calling pc.setRemoteDescription() [offer:{offer}]')
+        logger.debug(f"receive() | calling pc.setRemoteDescription() [offer:{offer}]")
         await self.pc.setRemoteDescription(offer)
         answer: RTCSessionDescription = await self.pc.createAnswer()
         localSdpDict = sdp_transform.parse(answer.sdp)
-        answerMediaDict = [m for m in localSdpDict.get('media') if str(m.get('mid')) == localId][0]
+        answerMediaDict = [
+            m for m in localSdpDict.get("media") if str(m.get("mid")) == localId
+        ][0]
         # May need to modify codec parameters in the answer based on codec
         # parameters in the offer.
-        applyCodecParameters(offerRtpParameters=options.rtpParameters, answerMediaDict=answerMediaDict)
+        applyCodecParameters(
+            offerRtpParameters=options.rtpParameters, answerMediaDict=answerMediaDict
+        )
         answer = RTCSessionDescription(
-            type='answer',
-            sdp=sdp_transform.write(localSdpDict)
+            type="answer", sdp=sdp_transform.write(localSdpDict)
         )
         if not self._transportReady:
-            await self._setupTransport(localDtlsRole='client', localSdpDict=localSdpDict)
-        logger.debug(f'receive() | calling pc.setLocalDescription() [answer:{answer}]')
+            await self._setupTransport(
+                localDtlsRole="client", localSdpDict=localSdpDict
+            )
+        logger.debug(f"receive() | calling pc.setLocalDescription() [answer:{answer}]")
         await self.pc.setLocalDescription(answer)
         transceivers = [t for t in self.pc.getTransceivers() if t.mid == localId]
         if not transceivers:
-            raise Exception('new RTCRtpTransceiver not found')
+            raise Exception("new RTCRtpTransceiver not found")
         # Store in the map.
         transceiver = transceivers[0]
         self._mapMidTransceiver[localId] = transceiver
 
         return HandlerReceiveResult(
             localId=localId,
             track=transceiver.receiver.track,
-            rtpReceiver=transceiver.receiver
+            rtpReceiver=transceiver.receiver,
         )
-        
+
     async def stopReceiving(self, localId: str):
         self._assertRecvDirection()
-        logger.debug(f'stopReceiving() [localId:{localId}]')
+        logger.debug(f"stopReceiving() [localId:{localId}]")
         transceiver = self._mapMidTransceiver.get(localId)
         if not transceiver:
-            raise Exception('associated RTCRtpTransceiver not found')
+            raise Exception("associated RTCRtpTransceiver not found")
         self.remoteSdp.closeMediaSection(transceiver.mid)
         offer: RTCSessionDescription = RTCSessionDescription(
-            type='offer',
-            sdp=self.remoteSdp.getSdp()
+            type="offer", sdp=self.remoteSdp.getSdp()
+        )
+        logger.debug(
+            f"stopReceiving() | calling pc.setRemoteDescription() [offer:{offer}]"
         )
-        logger.debug(f'stopReceiving() | calling pc.setRemoteDescription() [offer:{offer}]')
         await self.pc.setRemoteDescription(offer)
         answer = await self.pc.createAnswer()
-        logger.debug(f'stopReceiving() | calling pc.setLocalDescription() [answer:{answer}]')
+        logger.debug(
+            f"stopReceiving() | calling pc.setLocalDescription() [answer:{answer}]"
+        )
         await self.pc.setLocalDescription(answer)
         self._mapMidTransceiver.pop(localId, None)
-    
+
     async def getReceiverStats(self, localId: str):
         self._assertRecvDirection()
         transceiver = self._mapMidTransceiver.get(localId)
         if not transceiver:
-            raise Exception('associated RTCRtpTransceiver not found')
+            raise Exception("associated RTCRtpTransceiver not found")
         return await transceiver.receiver.getStats()
-    
+
     async def receiveDataChannel(
         self,
         sctpStreamParameters: SctpStreamParameters,
-        label: Optional[str]=None,
-        protocol: Optional[str]=None
+        label: Optional[str] = None,
+        protocol: Optional[str] = None,
     ) -> HandlerReceiveDataChannelResult:
         options = HandlerReceiveDataChannelOptions(
-            sctpStreamParameters=sctpStreamParameters,
-            label=label,
-            protocol=protocol
+            sctpStreamParameters=sctpStreamParameters, label=label, protocol=protocol
         )
         self._assertRecvDirection()
-        logger.debug(f'[receiveDataChannel() [options:{options.sctpStreamParameters}]]')
+        logger.debug(f"[receiveDataChannel() [options:{options.sctpStreamParameters}]]")
         dataChannel = self.pc.createDataChannel(
             label=options.label,
             maxPacketLifeTime=options.sctpStreamParameters.maxPacketLifeTime,
             maxRetransmits=options.sctpStreamParameters.maxRetransmits,
             ordered=options.sctpStreamParameters.ordered,
             protocol=options.protocol,
             negotiated=True,
-            id=options.sctpStreamParameters.streamId
+            id=options.sctpStreamParameters.streamId,
         )
 
         # If this is the first DataChannel we need to create the SDP offer with
         # m=application section.
         if not self._hasDataChannelMediaSection:
             self.remoteSdp.receiveSctpAssociation()
             offer: RTCSessionDescription = RTCSessionDescription(
-                type='offer',
-                sdp=self.remoteSdp.getSdp()
+                type="offer", sdp=self.remoteSdp.getSdp()
+            )
+            logger.debug(
+                f"receiveDataChannel() | calling pc.setRemoteDescription() [offer:{offer}]"
             )
-            logger.debug(f'receiveDataChannel() | calling pc.setRemoteDescription() [offer:{offer}]')
             await self.pc.setRemoteDescription(offer)
             answer = await self.pc.createAnswer()
             if not self._transportReady:
                 localSdpDict = sdp_transform.parse(answer.sdp)
-                await self._setupTransport(localDtlsRole='client', localSdpDict=localSdpDict)
-            logger.debug(f'receiveDataChannel() | calling pc.setRemoteDescription() [answer:{answer}]')
+                await self._setupTransport(
+                    localDtlsRole="client", localSdpDict=localSdpDict
+                )
+            logger.debug(
+                f"receiveDataChannel() | calling pc.setRemoteDescription() [answer:{answer}]"
+            )
             await self.pc.setLocalDescription(answer)
             self._hasDataChannelMediaSection = True
         return HandlerReceiveDataChannelResult(dataChannel=dataChannel)
-    
-    async def _setupTransport(self, localDtlsRole: DtlsRole, localSdpDict: dict={}):
+
+    async def _setupTransport(self, localDtlsRole: DtlsRole, localSdpDict: dict = {}):
         if localSdpDict == {}:
             localSdpDict = sdp_transform.parse(self.pc.localDescription.sdp)
         # Get our local DTLS parameters.
         dtlsParameters: DtlsParameters = extractDtlsParameters(localSdpDict)
         # Set our DTLS role.
         dtlsParameters.role = localDtlsRole
         # Update the remote DTLS role in the SDP.
-        self.remoteSdp.updateDtlsRole('server' if localDtlsRole == 'client' else 'client')
+        self.remoteSdp.updateDtlsRole(
+            "server" if localDtlsRole == "client" else "client"
+        )
         # Need to tell the remote transport about our parameters.
-        await self.emit_for_results('@connect', dtlsParameters)
+        await self.emit_for_results("@connect", dtlsParameters)
         self._transportReady = True
-    
+
     def _assertSendDirection(self):
-        if self._direction != 'send':
-            raise Exception('method can just be called for handlers with "send" direction')
-    
+        if self._direction != "send":
+            raise Exception(
+                'method can just be called for handlers with "send" direction'
+            )
+
     def _assertRecvDirection(self):
-        if self._direction != 'recv':
-            raise Exception('method can just be called for handlers with "recv" direction')
+        if self._direction != "recv":
+            raise Exception(
+                'method can just be called for handlers with "recv" direction'
+            )
```

### Comparing `pymediasoup-0.2.6/pymediasoup/handlers/sdp/media_section.py` & `pymediasoup-1.0.0/pymediasoup/handlers/sdp/media_section.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,435 +1,492 @@
-import sys
-if sys.version_info >= (3, 8):
-    from typing import List, Optional, Literal
-else:
-    from typing import List, Optional
-    from typing_extensions import Literal
+from typing import List, Optional, Literal
 
 import re
 import logging
 from aiortc import RTCIceParameters, RTCIceCandidate, RTCDtlsParameters
 from ...producer import ProducerCodecOptions
 from ...rtp_parameters import RtpParameters, RtpCodecParameters, RtpEncodingParameters
 from ...sctp_parameters import SctpParameters
 from ...models.transport import PlainRtpParameters, IceCandidate
 
 
 logger = logging.getLogger(__name__)
 
 
 def getCodecName(codec: RtpCodecParameters):
-    pattern = re.compile(r'^(audio|video)/(.+)', re.I)
+    pattern = re.compile(r"^(audio|video)/(.+)", re.I)
     match = pattern.match(codec.mimeType)
     if match:
         return match.group(2)
     else:
-        raise TypeError('invalid codec.mimeType')
+        raise TypeError("invalid codec.mimeType")
+
 
 class MediaSection:
     def __init__(
         self,
-        iceParameters: Optional[RTCIceParameters]=None,
-        iceCandidates: List[IceCandidate]=[],
-        dtlsParameters: Optional[RTCDtlsParameters]=None,
-        planB:bool=False
+        iceParameters: Optional[RTCIceParameters] = None,
+        iceCandidates: List[IceCandidate] = [],
+        dtlsParameters: Optional[RTCDtlsParameters] = None,
+        planB: bool = False,
     ):
-        self._mediaDict: dict={}
-        self._planB=planB
+        self._mediaDict: dict = {}
+        self._planB = planB
         if iceParameters:
             self.setIceParameters(iceParameters)
         if iceCandidates:
-            self._mediaDict['candidates'] = []
+            self._mediaDict["candidates"] = []
             for candidate in iceCandidates:
                 c_dict = candidate.dict()
-                c_dict['component'] = 1
-                self._mediaDict['candidates'].append(c_dict)
-            self._mediaDict['endOfCandidates'] = 'end-of-candidates'
-            self._mediaDict['iceOptions'] = 'renomination'
+                c_dict["component"] = 1
+                self._mediaDict["candidates"].append(c_dict)
+            self._mediaDict["endOfCandidates"] = "end-of-candidates"
+            self._mediaDict["iceOptions"] = "renomination"
         if dtlsParameters:
             self.setDtlsRole(dtlsParameters.role)
-    
+
     @property
     def mid(self) -> str:
-        return str(self._mediaDict.get('mid', ''))
-    
+        return str(self._mediaDict.get("mid", ""))
+
     @property
     def closed(self):
-        return self._mediaDict.get('port') == 0
-    
+        return self._mediaDict.get("port") == 0
+
     def getDict(self):
         return self._mediaDict
-    
+
     def setIceParameters(self, iceParameters: RTCIceParameters):
-        self._mediaDict['iceUfrag'] = iceParameters.usernameFragment
-        self._mediaDict['icePwd'] = iceParameters.password
-    
+        self._mediaDict["iceUfrag"] = iceParameters.usernameFragment
+        self._mediaDict["icePwd"] = iceParameters.password
+
     def disable(self):
-        self._mediaDict['direction'] = 'inactive'
-        self._mediaDict.pop('ext', None)
-        self._mediaDict.pop('ssrcs', None)
-        self._mediaDict.pop('ssrcGroups', None)
-        self._mediaDict.pop('simulcast', None)
-        self._mediaDict.pop('simulcast_03', None)
-        self._mediaDict.pop('rids', None)
-    
+        self._mediaDict["direction"] = "inactive"
+        self._mediaDict.pop("ext", None)
+        self._mediaDict.pop("ssrcs", None)
+        self._mediaDict.pop("ssrcGroups", None)
+        self._mediaDict.pop("simulcast", None)
+        self._mediaDict.pop("simulcast_03", None)
+        self._mediaDict.pop("rids", None)
+
     def close(self):
-        self._mediaDict['direction'] = 'inactive'
-        self._mediaDict['port'] = 0
-        self._mediaDict.pop('ext', None)
-        self._mediaDict.pop('ssrcs', None)
-        self._mediaDict.pop('ssrcGroups', None)
-        self._mediaDict.pop('simulcast', None)
-        self._mediaDict.pop('simulcast_03', None)
-        self._mediaDict.pop('rids', None)
-        self._mediaDict.pop('extmapAllowMixed', None)
-    
+        self._mediaDict["direction"] = "inactive"
+        self._mediaDict["port"] = 0
+        self._mediaDict.pop("ext", None)
+        self._mediaDict.pop("ssrcs", None)
+        self._mediaDict.pop("ssrcGroups", None)
+        self._mediaDict.pop("simulcast", None)
+        self._mediaDict.pop("simulcast_03", None)
+        self._mediaDict.pop("rids", None)
+        self._mediaDict.pop("extmapAllowMixed", None)
+
     def setDtlsRole(self, role: str):
-        logger.warning('MediaSection setDtlsRole() not implement')
+        logger.warning("MediaSection setDtlsRole() not implement")
+
+    def planBReceive(
+        self, offerRtpParameters: RtpParameters, streamId: str, trackId: str
+    ):
+        logger.warning("MediaSection planBReceive() not implement")
 
-    def planBReceive(self, offerRtpParameters: RtpParameters, streamId: str, trackId: str):
-        logger.warning('MediaSection planBReceive() not implement')
-    
     def planBStopReceiving(self, offerRtpParameters: RtpParameters):
-        logger.warning('MediaSection planBStopReceiving() not implement')
-    
+        logger.warning("MediaSection planBStopReceiving() not implement")
+
+
 class AnswerMediaSection(MediaSection):
-    def __init__(
+    def __init__(  # noqa
         self,
         offerMediaDict: dict,
-        sctpParameters: Optional[SctpParameters]=None,
-        offerRtpParameters: Optional[RtpParameters]=None,
-        answerRtpParameters: Optional[RtpParameters]=None,
-        codecOptions: Optional[ProducerCodecOptions]=None,
-        iceParameters: Optional[RTCIceParameters]=None,
-        iceCandidates: List[RTCIceCandidate]=[],
-        dtlsParameters: Optional[RTCDtlsParameters]=None,
-        plainRtpParameters: Optional[PlainRtpParameters]=None,
-        planB: bool=False,
-        extmapAllowMixed: bool=False
+        sctpParameters: Optional[SctpParameters] = None,
+        offerRtpParameters: Optional[RtpParameters] = None,
+        answerRtpParameters: Optional[RtpParameters] = None,
+        codecOptions: Optional[ProducerCodecOptions] = None,
+        iceParameters: Optional[RTCIceParameters] = None,
+        iceCandidates: List[RTCIceCandidate] = [],
+        dtlsParameters: Optional[RTCDtlsParameters] = None,
+        plainRtpParameters: Optional[PlainRtpParameters] = None,
+        planB: bool = False,
+        extmapAllowMixed: bool = False,
     ):
-        super(AnswerMediaSection, self).__init__(iceParameters, iceCandidates, dtlsParameters, planB)
-        self._mediaDict['mid'] = offerMediaDict.get('mid')
-        self._mediaDict['type'] = offerMediaDict.get('type')
-        self._mediaDict['protocol'] = offerMediaDict.get('protocol')
+        super(AnswerMediaSection, self).__init__(
+            iceParameters, iceCandidates, dtlsParameters, planB
+        )
+        self._mediaDict["mid"] = offerMediaDict.get("mid")
+        self._mediaDict["type"] = offerMediaDict.get("type")
+        self._mediaDict["protocol"] = offerMediaDict.get("protocol")
 
         if not plainRtpParameters:
-            self._mediaDict['connection'] = {
-                'ip': '127.0.0.1',
-                'version': 4
-            }
-            self._mediaDict['port'] = 7
+            self._mediaDict["connection"] = {"ip": "127.0.0.1", "version": 4}
+            self._mediaDict["port"] = 7
         else:
-            self._mediaDict['connection'] = {
-                'ip': plainRtpParameters.ip,
-                'version': plainRtpParameters.ipVersion
+            self._mediaDict["connection"] = {
+                "ip": plainRtpParameters.ip,
+                "version": plainRtpParameters.ipVersion,
             }
-            self._mediaDict['port'] = plainRtpParameters.port
-        
-        if offerMediaDict.get('type') in ['audio', 'video']:
-            self._mediaDict['direction'] = 'recvonly'
-            self._mediaDict['rtp'] = []
-            self._mediaDict['rtcpFb'] = []
-            self._mediaDict['fmtp'] = []
+            self._mediaDict["port"] = plainRtpParameters.port
+
+        if offerMediaDict.get("type") in ["audio", "video"]:
+            self._mediaDict["direction"] = "recvonly"
+            self._mediaDict["rtp"] = []
+            self._mediaDict["rtcpFb"] = []
+            self._mediaDict["fmtp"] = []
             if answerRtpParameters:
                 for codec in answerRtpParameters.codecs:
                     rtp = {
-                        'payload': codec.payloadType,
-                        'codec': getCodecName(codec),
-                        'rate': codec.clockRate
+                        "payload": codec.payloadType,
+                        "codec": getCodecName(codec),
+                        "rate": codec.clockRate,
                     }
                     if codec.channels:
-                        if (codec.channels > 1):
-                            rtp['encoding'] = codec.channels
-                    self._mediaDict['rtp'].append(rtp)
+                        if codec.channels > 1:
+                            rtp["encoding"] = codec.channels
+                    self._mediaDict["rtp"].append(rtp)
                     codecParameters = codec.parameters
                     if codecOptions:
                         if offerRtpParameters:
-                            offerCodecs = [offerRtpCodec for offerRtpCodec in offerRtpParameters.codecs if offerRtpCodec.payloadType == codec.payloadType]
+                            offerCodecs = [
+                                offerRtpCodec
+                                for offerRtpCodec in offerRtpParameters.codecs
+                                if offerRtpCodec.payloadType == codec.payloadType
+                            ]
                             if offerCodecs:
-                                offerCodec:RtpCodecParameters = offerCodecs[0]
-                                if codec.mimeType.lower() == 'audio/opus':
-                                    if codecOptions.opusStereo != None:
-                                        offerCodec.parameters['sprop-stereo'] = 1 if codecOptions.opusStereo else 0
-                                        codecParameters['stereo'] = 1 if codecOptions.opusStereo else 0
-                                    if codecOptions.opusFec != None:
-                                        offerCodec.parameters['useinbandfec'] = 1 if codecOptions.opusFec else 0
-                                        codecParameters['useinbandfec'] = 1 if codecOptions.opusFec else 0
-                                    if codecOptions.opusDtx != None:
-                                        offerCodec.parameters['usedtx'] = 1 if codecOptions.opusDtx else 0
-                                        codecParameters['usedtx'] = 1 if codecOptions.opusDtx else 0
-                                    if codecOptions.opusMaxPlaybackRate != None:
-                                        codecParameters['maxplaybackrate'] = codecOptions.opusMaxPlaybackRate
-                                    if codecOptions.opusMaxAverageBitrate != None:
-                                        codecParameters['maxaveragebitrate'] = codecOptions.opusMaxAverageBitrate
-                                    if codecOptions.opusPtime != None:
-                                        offerCodec.parameters['ptime'] = codecOptions.opusPtime
-                                        codecParameters['ptime'] = codecOptions.opusPtime
-                                elif codec.mimeType.lower() in ['video/vp8', 'video/vp9', 'video/h264', 'video/h265']:
-                                    if codecOptions.videoGoogleStartBitrate != None:
-                                        codecParameters['x-google-start-bitrate'] = codecOptions.videoGoogleStartBitrate
-                                    if codecOptions.videoGoogleMaxBitrate != None:
-                                        codecParameters['x-google-max-bitrate'] = codecOptions.videoGoogleMaxBitrate
-                                    if codecOptions.videoGoogleMinBitrate != None:
-                                        codecParameters['x-google-min-bitrate'] = codecOptions.videoGoogleMinBitrate
-                        
+                                offerCodec: RtpCodecParameters = offerCodecs[0]
+                                if codec.mimeType.lower() == "audio/opus":
+                                    if codecOptions.opusStereo is not None:
+                                        offerCodec.parameters["sprop-stereo"] = (
+                                            1 if codecOptions.opusStereo else 0
+                                        )
+                                        codecParameters["stereo"] = (
+                                            1 if codecOptions.opusStereo else 0
+                                        )
+                                    if codecOptions.opusFec is not None:
+                                        offerCodec.parameters["useinbandfec"] = (
+                                            1 if codecOptions.opusFec else 0
+                                        )
+                                        codecParameters["useinbandfec"] = (
+                                            1 if codecOptions.opusFec else 0
+                                        )
+                                    if codecOptions.opusDtx is not None:
+                                        offerCodec.parameters["usedtx"] = (
+                                            1 if codecOptions.opusDtx else 0
+                                        )
+                                        codecParameters["usedtx"] = (
+                                            1 if codecOptions.opusDtx else 0
+                                        )
+                                    if codecOptions.opusMaxPlaybackRate is not None:
+                                        codecParameters["maxplaybackrate"] = (
+                                            codecOptions.opusMaxPlaybackRate
+                                        )
+                                    if codecOptions.opusMaxAverageBitrate is not None:
+                                        codecParameters["maxaveragebitrate"] = (
+                                            codecOptions.opusMaxAverageBitrate
+                                        )
+                                    if codecOptions.opusPtime is not None:
+                                        offerCodec.parameters["ptime"] = (
+                                            codecOptions.opusPtime
+                                        )
+                                        codecParameters["ptime"] = (
+                                            codecOptions.opusPtime
+                                        )
+                                elif codec.mimeType.lower() in [
+                                    "video/vp8",
+                                    "video/vp9",
+                                    "video/h264",
+                                    "video/h265",
+                                ]:
+                                    if codecOptions.videoGoogleStartBitrate is not None:
+                                        codecParameters["x-google-start-bitrate"] = (
+                                            codecOptions.videoGoogleStartBitrate
+                                        )
+                                    if codecOptions.videoGoogleMaxBitrate is not None:
+                                        codecParameters["x-google-max-bitrate"] = (
+                                            codecOptions.videoGoogleMaxBitrate
+                                        )
+                                    if codecOptions.videoGoogleMinBitrate is not None:
+                                        codecParameters["x-google-min-bitrate"] = (
+                                            codecOptions.videoGoogleMinBitrate
+                                        )
+
                     fmtp = {
-                        'payload': codec.payloadType,
-                        'config': ';'.join([f'{key}={value}' for key, value in codecParameters.items()])
+                        "payload": codec.payloadType,
+                        "config": ";".join(
+                            [f"{key}={value}" for key, value in codecParameters.items()]
+                        ),
                     }
-                    if fmtp['config']:
-                        self._mediaDict['fmtp'].append(fmtp)
+                    if fmtp["config"]:
+                        self._mediaDict["fmtp"].append(fmtp)
                     for fb in codec.rtcpFeedback:
-                        self._mediaDict['rtcpFb'].append({
-                            'payload': codec.payloadType,
-                            'type': fb.type,
-                            'subtype': fb.parameter
-                        })
-                
-                self._mediaDict['payloads'] = ' '.join([str(codec.payloadType) for codec in answerRtpParameters.codecs])
-                self._mediaDict['ext'] = []
+                        self._mediaDict["rtcpFb"].append(
+                            {
+                                "payload": codec.payloadType,
+                                "type": fb.type,
+                                "subtype": fb.parameter,
+                            }
+                        )
+
+                self._mediaDict["payloads"] = " ".join(
+                    [str(codec.payloadType) for codec in answerRtpParameters.codecs]
+                )
+                self._mediaDict["ext"] = []
                 for ext in answerRtpParameters.headerExtensions:
                     # Don't add a header extension if not present in the offer.
-                    if ext.uri in [localExt['uri'] for localExt in offerMediaDict['ext']]:
-                        self._mediaDict['ext'].append({
-                            'uri': ext.uri,
-                            'value': ext.id
-                        })
+                    if ext.uri in [
+                        localExt["uri"] for localExt in offerMediaDict["ext"]
+                    ]:
+                        self._mediaDict["ext"].append({"uri": ext.uri, "value": ext.id})
             # Allow both 1 byte and 2 bytes length header extensions.
-            if extmapAllowMixed and offerMediaDict.get('extmapAllowMixed') == 'extmap-allow-mixed':
-                self._mediaDict['extmapAllowMixed'] = 'extmap-allow-mixed'
+            if (
+                extmapAllowMixed
+                and offerMediaDict.get("extmapAllowMixed") == "extmap-allow-mixed"
+            ):
+                self._mediaDict["extmapAllowMixed"] = "extmap-allow-mixed"
             # Simulcast.
-            if offerMediaDict.get('simulcast'):
-                simulcast: dict = offerMediaDict.get('simulcast', {})
-                self._mediaDict['simulcast'] = {
-                    'dir1': 'recv',
-                    'list1': simulcast.get('list1')
+            if offerMediaDict.get("simulcast"):
+                simulcast: dict = offerMediaDict.get("simulcast", {})
+                self._mediaDict["simulcast"] = {
+                    "dir1": "recv",
+                    "list1": simulcast.get("list1"),
                 }
-                self._mediaDict['rids'] = []
-                if offerMediaDict.get('rids'):
-                    rids: list = offerMediaDict.get('rids', [])
+                self._mediaDict["rids"] = []
+                if offerMediaDict.get("rids"):
+                    rids: list = offerMediaDict.get("rids", [])
                     for rid in rids:
-                        if rid.get('direction') == 'send':
-                            self._mediaDict['rids'].append({
-                                'id': rid.get('id'),
-                                'direction': 'recv'
-                            })
+                        if rid.get("direction") == "send":
+                            self._mediaDict["rids"].append(
+                                {"id": rid.get("id"), "direction": "recv"}
+                            )
             # Simulcast (draft version 03).
-            elif offerMediaDict.get('simulcast_03'):
-                simulcast_03: dict = offerMediaDict.get('simulcast_03', {})
-                self._mediaDict['simulcast_03'] = {
-                    'value': simulcast_03.get('value', '').replace('send', 'recv')
+            elif offerMediaDict.get("simulcast_03"):
+                simulcast_03: dict = offerMediaDict.get("simulcast_03", {})
+                self._mediaDict["simulcast_03"] = {
+                    "value": simulcast_03.get("value", "").replace("send", "recv")
                 }
-                self._mediaDict['rids'] = []
-                if offerMediaDict.get('rids'):
-                    rids_03: list = offerMediaDict.get('rids', [])
+                self._mediaDict["rids"] = []
+                if offerMediaDict.get("rids"):
+                    rids_03: list = offerMediaDict.get("rids", [])
                     for rid in rids_03:
-                        if rid.get('direction') == 'send':
-                            self._mediaDict['rids'].append({
-                                'id': rid.get('id'),
-                                'direction': 'recv'
-                            })
-            self._mediaDict['rtcpMux'] = 'rtcp-mux'
-            self._mediaDict['rtcpRsize'] = 'rtcp-rsize'
-            if self._planB and self._mediaDict.get('type') == 'video':
-                self._mediaDict['xGoogleFlag'] = 'conference'
-            
-        elif offerMediaDict.get('type') == 'application':
+                        if rid.get("direction") == "send":
+                            self._mediaDict["rids"].append(
+                                {"id": rid.get("id"), "direction": "recv"}
+                            )
+            self._mediaDict["rtcpMux"] = "rtcp-mux"
+            self._mediaDict["rtcpRsize"] = "rtcp-rsize"
+            if self._planB and self._mediaDict.get("type") == "video":
+                self._mediaDict["xGoogleFlag"] = "conference"
+
+        elif offerMediaDict.get("type") == "application":
             # New spec.
             if sctpParameters:
-                if offerMediaDict.get('sctpPort'):
-                    self._mediaDict['payloads'] = 'webrtc-datachannel'
-                    self._mediaDict['sctpPort'] = sctpParameters.port
-                    self._mediaDict['maxMessageSize'] = sctpParameters.maxMessageSize
+                if offerMediaDict.get("sctpPort"):
+                    self._mediaDict["payloads"] = "webrtc-datachannel"
+                    self._mediaDict["sctpPort"] = sctpParameters.port
+                    self._mediaDict["maxMessageSize"] = sctpParameters.maxMessageSize
                 # Old spec.
-                elif offerMediaDict.get('sctpmap'):
-                    self._mediaDict['payloads'] = sctpParameters.port
-                    self._mediaDict['sctpmap'] = {
-                        'app': 'webrtc-datachannel',
-                        'sctpmapNumber': sctpParameters.port,
-                        'maxMessageSize': sctpParameters.maxMessageSize
+                elif offerMediaDict.get("sctpmap"):
+                    self._mediaDict["payloads"] = sctpParameters.port
+                    self._mediaDict["sctpmap"] = {
+                        "app": "webrtc-datachannel",
+                        "sctpmapNumber": sctpParameters.port,
+                        "maxMessageSize": sctpParameters.maxMessageSize,
                     }
+
     def setDtlsRole(self, role: str):
-        if role == 'client':
-            self._mediaDict['setup'] = 'active'
-        elif role == 'server':
-            self._mediaDict['setup'] = 'passive'
-        elif role == 'auto':
-            self._mediaDict['setup'] = 'actpass'
+        if role == "client":
+            self._mediaDict["setup"] = "active"
+        elif role == "server":
+            self._mediaDict["setup"] = "passive"
+        elif role == "auto":
+            self._mediaDict["setup"] = "actpass"
+
 
 class OfferMediaSection(MediaSection):
     def __init__(
         self,
         mid: str,
-        kind: Literal['audio', 'video', 'application'],
-        streamId: Optional[str]=None,
-        trackId: Optional[str]=None,
-        oldDataChannelSpec: Optional[bool]=False,
-        sctpParameters: Optional[SctpParameters]=None,
-        offerRtpParameters: Optional[RtpParameters]=None,
-        iceParameters: Optional[RTCIceParameters]=None,
-        iceCandidates: List[RTCIceCandidate]=[],
-        dtlsParameters: Optional[RTCDtlsParameters]=None,
-        plainRtpParameters: Optional[PlainRtpParameters]=None,
-        planB: bool=False,    
+        kind: Literal["audio", "video", "application"],
+        streamId: Optional[str] = None,
+        trackId: Optional[str] = None,
+        oldDataChannelSpec: Optional[bool] = False,
+        sctpParameters: Optional[SctpParameters] = None,
+        offerRtpParameters: Optional[RtpParameters] = None,
+        iceParameters: Optional[RTCIceParameters] = None,
+        iceCandidates: List[RTCIceCandidate] = [],
+        dtlsParameters: Optional[RTCDtlsParameters] = None,
+        plainRtpParameters: Optional[PlainRtpParameters] = None,
+        planB: bool = False,
     ):
-        super(OfferMediaSection, self).__init__(iceParameters, iceCandidates, dtlsParameters, planB)
-        self._mediaDict['mid'] = mid
-        self._mediaDict['type'] = kind
+        super(OfferMediaSection, self).__init__(
+            iceParameters, iceCandidates, dtlsParameters, planB
+        )
+        self._mediaDict["mid"] = mid
+        self._mediaDict["type"] = kind
         if not plainRtpParameters:
-            self._mediaDict['connection'] = {
-                'ip': '127.0.0.1',
-                'version': 4
-            }
+            self._mediaDict["connection"] = {"ip": "127.0.0.1", "version": 4}
             if not sctpParameters:
-                self._mediaDict['protocol'] = 'UDP/TLS/RTP/SAVPF'
+                self._mediaDict["protocol"] = "UDP/TLS/RTP/SAVPF"
             else:
-                self._mediaDict['protocol'] = 'UDP/DTLS/SCTP'
-            self._mediaDict['port'] = 7
+                self._mediaDict["protocol"] = "UDP/DTLS/SCTP"
+            self._mediaDict["port"] = 7
         else:
-            self._mediaDict['connection'] = {
-                'ip': plainRtpParameters.ip,
-                'version': plainRtpParameters.ipVersion
+            self._mediaDict["connection"] = {
+                "ip": plainRtpParameters.ip,
+                "version": plainRtpParameters.ipVersion,
             }
-            self._mediaDict['protocol'] = 'RTP/AVP'
-            self._mediaDict['port'] = plainRtpParameters.port
-        
-        if kind in ['audio', 'video']:
-            self._mediaDict['direction'] = 'sendonly'
-            self._mediaDict['rtp'] = []
-            self._mediaDict['rtcpFb'] = []
-            self._mediaDict['fmtp'] = []
+            self._mediaDict["protocol"] = "RTP/AVP"
+            self._mediaDict["port"] = plainRtpParameters.port
+
+        if kind in ["audio", "video"]:
+            self._mediaDict["direction"] = "sendonly"
+            self._mediaDict["rtp"] = []
+            self._mediaDict["rtcpFb"] = []
+            self._mediaDict["fmtp"] = []
             if not self._planB:
-                self._mediaDict['msid'] = f"{streamId if streamId else '-'} {trackId}"
+                self._mediaDict["msid"] = f"{streamId if streamId else '-'} {trackId}"
             if offerRtpParameters:
                 for codec in offerRtpParameters.codecs:
                     rtp = {
-                        'payload': codec.payloadType,
-                        'codec': getCodecName(codec),
-                        'rate': codec.clockRate
+                        "payload": codec.payloadType,
+                        "codec": getCodecName(codec),
+                        "rate": codec.clockRate,
                     }
                     if codec.channels:
                         if codec.channels > 1:
-                            rtp['encoding'] = codec.channels
-                    self._mediaDict['rtp'].append(rtp)
+                            rtp["encoding"] = codec.channels
+                    self._mediaDict["rtp"].append(rtp)
                     fmtp = {
-                        'payload': codec.payloadType,
-                        'config': ';'.join([f'{key}={value}' for key, value in codec.parameters.items()])
+                        "payload": codec.payloadType,
+                        "config": ";".join(
+                            [
+                                f"{key}={value}"
+                                for key, value in codec.parameters.items()
+                            ]
+                        ),
                     }
-                    if fmtp['config']:
-                        self._mediaDict['fmtp'].append(fmtp)
+                    if fmtp["config"]:
+                        self._mediaDict["fmtp"].append(fmtp)
                     for fb in codec.rtcpFeedback:
-                        self._mediaDict['rtcpFb'].append({
-                            'payload': codec.payloadType,
-                            'type': fb.type,
-                            'subtype': fb.parameter
-                        })
-                
-                self._mediaDict['payloads'] = ' '.join([str(codec.payloadType) for codec in offerRtpParameters.codecs])
-                self._mediaDict['ext'] = []
+                        self._mediaDict["rtcpFb"].append(
+                            {
+                                "payload": codec.payloadType,
+                                "type": fb.type,
+                                "subtype": fb.parameter,
+                            }
+                        )
+
+                self._mediaDict["payloads"] = " ".join(
+                    [str(codec.payloadType) for codec in offerRtpParameters.codecs]
+                )
+                self._mediaDict["ext"] = []
                 for ext in offerRtpParameters.headerExtensions:
-                    self._mediaDict['ext'].append({
-                        'uri': ext.uri,
-                        'value': ext.id
-                    })
-                
-                self._mediaDict['rtcpMux'] = 'rtcp-mux'
-                self._mediaDict['rtcpRsize'] = 'rtcp-rsize'
+                    self._mediaDict["ext"].append({"uri": ext.uri, "value": ext.id})
+
+                self._mediaDict["rtcpMux"] = "rtcp-mux"
+                self._mediaDict["rtcpRsize"] = "rtcp-rsize"
                 encoding: RtpEncodingParameters = offerRtpParameters.encodings[0]
                 ssrc = encoding.ssrc
-                rtxSsrc = encoding.rtx.ssrc if encoding.rtx and encoding.rtx.ssrc else None
-                self._mediaDict['ssrcs'] = []
-                self._mediaDict['ssrcGroups'] = []
+                rtxSsrc = (
+                    encoding.rtx.ssrc if encoding.rtx and encoding.rtx.ssrc else None
+                )
+                self._mediaDict["ssrcs"] = []
+                self._mediaDict["ssrcGroups"] = []
                 cname = None
                 if offerRtpParameters.rtcp:
                     if offerRtpParameters.rtcp.cname:
                         cname = offerRtpParameters.rtcp.cname
                 if cname:
-                    self._mediaDict['ssrcs'].append({
-                        'id': ssrc,
-                        'attribute': 'cname',
-                        'value': cname
-                    })
+                    self._mediaDict["ssrcs"].append(
+                        {"id": ssrc, "attribute": "cname", "value": cname}
+                    )
                 if self._planB:
-                    self._mediaDict['ssrcs'].append({
-                        'id': ssrc,
-                        'attribute': 'msid',
-                        'value': f"{streamId if streamId else '-'} {trackId}"
-                    })
+                    self._mediaDict["ssrcs"].append(
+                        {
+                            "id": ssrc,
+                            "attribute": "msid",
+                            "value": f"{streamId if streamId else '-'} {trackId}",
+                        }
+                    )
                 if rtxSsrc:
                     if cname:
-                        self._mediaDict['ssrcs'].append({
-                            'id': rtxSsrc,
-                            'attribute': 'cname',
-                            'value': cname
-                        })
+                        self._mediaDict["ssrcs"].append(
+                            {"id": rtxSsrc, "attribute": "cname", "value": cname}
+                        )
                     if self._planB:
-                        self._mediaDict['ssrcs'].append({
-                            'id': rtxSsrc,
-                            'attribute': 'msid',
-                            'value': f"{streamId if streamId else '-'} {trackId}"
-                        })
-                    self._mediaDict['ssrcGroups'].append({
-                        'semantics': 'FID',
-                        'ssrcs': f'{ssrc} {rtxSsrc}'
-                    })
-        elif kind == 'application':
+                        self._mediaDict["ssrcs"].append(
+                            {
+                                "id": rtxSsrc,
+                                "attribute": "msid",
+                                "value": f"{streamId if streamId else '-'} {trackId}",
+                            }
+                        )
+                    self._mediaDict["ssrcGroups"].append(
+                        {"semantics": "FID", "ssrcs": f"{ssrc} {rtxSsrc}"}
+                    )
+        elif kind == "application":
             if sctpParameters:
                 # New spec.
                 if not oldDataChannelSpec:
-                    self._mediaDict['payloads'] = 'webrtc-datachannel'
-                    self._mediaDict['sctpPort'] = sctpParameters.port
-                    self._mediaDict['maxMessageSize'] = sctpParameters.maxMessageSize
+                    self._mediaDict["payloads"] = "webrtc-datachannel"
+                    self._mediaDict["sctpPort"] = sctpParameters.port
+                    self._mediaDict["maxMessageSize"] = sctpParameters.maxMessageSize
                 # Old spec.
                 else:
-                    self._mediaDict['payloads'] = sctpParameters.port
-                    self._mediaDict['sctpmap'] = {
-                        'app': 'webrtc-datachannel',
-                        'sctpmapNumber': sctpParameters.port,
-                        'maxMessageSize': sctpParameters.maxMessageSize
+                    self._mediaDict["payloads"] = sctpParameters.port
+                    self._mediaDict["sctpmap"] = {
+                        "app": "webrtc-datachannel",
+                        "sctpmapNumber": sctpParameters.port,
+                        "maxMessageSize": sctpParameters.maxMessageSize,
                     }
+
     def setDtlsRole(self, _):
         # Always 'actpass'.
-        self._mediaDict['setup'] = 'actpass'
-    
-    def planBReceive(self, offerRtpParameters: RtpParameters, streamId: str, trackId: str):
+        self._mediaDict["setup"] = "actpass"
+
+    def planBReceive(
+        self, offerRtpParameters: RtpParameters, streamId: str, trackId: str
+    ):
         encoding = offerRtpParameters.encodings[0]
         ssrc = encoding.ssrc
         rtxSsrc = encoding.rtx.ssrc if encoding.rtx and encoding.rtx.ssrc else None
         if offerRtpParameters.rtcp:
             if offerRtpParameters.rtcp.cname:
                 cname = offerRtpParameters.rtcp.cname
         if cname:
-            self._mediaDict['ssrcs'].append({
-                'id': ssrc,
-                'attribute': 'cname',
-                'value': cname
-            })
-        self._mediaDict['ssrcs'].append({
-            'id': ssrc,
-            'attribute': 'msid',
-            'value': f"{streamId if streamId else '-'} {trackId}"
-        })
+            self._mediaDict["ssrcs"].append(
+                {"id": ssrc, "attribute": "cname", "value": cname}
+            )
+        self._mediaDict["ssrcs"].append(
+            {
+                "id": ssrc,
+                "attribute": "msid",
+                "value": f"{streamId if streamId else '-'} {trackId}",
+            }
+        )
         if rtxSsrc:
             if cname:
-                self._mediaDict['ssrcs'].append({
-                    'id': rtxSsrc,
-                    'attribute': 'cname',
-                    'value': cname
-                })
-            self._mediaDict['ssrcs'].append({
-                'id': rtxSsrc,
-                'attribute': 'msid',
-                'value': f"{streamId if streamId else '-'} {trackId}"
-            })
-            self._mediaDict['ssrcGroups'].append({
-                'semantics': 'FID',
-                'ssrcs': f'{ssrc} {rtxSsrc}'
-            })
-    
+                self._mediaDict["ssrcs"].append(
+                    {"id": rtxSsrc, "attribute": "cname", "value": cname}
+                )
+            self._mediaDict["ssrcs"].append(
+                {
+                    "id": rtxSsrc,
+                    "attribute": "msid",
+                    "value": f"{streamId if streamId else '-'} {trackId}",
+                }
+            )
+            self._mediaDict["ssrcGroups"].append(
+                {"semantics": "FID", "ssrcs": f"{ssrc} {rtxSsrc}"}
+            )
+
     def planBStopReceiving(self, offerRtpParameters: RtpParameters):
         encoding = offerRtpParameters.encodings[0]
         ssrc = encoding.ssrc
         rtxSsrc = encoding.rtx.ssrc if encoding.rtx and encoding.rtx.ssrc else None
-        self._mediaDict['ssrcs'] = [s for s in self._mediaDict['ssrcs'] if s['id'] != ssrc and s['id'] != rtxSsrc]
+        self._mediaDict["ssrcs"] = [
+            s
+            for s in self._mediaDict["ssrcs"]
+            if s["id"] != ssrc and s["id"] != rtxSsrc
+        ]
         if rtxSsrc:
-            self._mediaDict['ssrcGroups'] = [group for group in self._mediaDict['ssrcGroups'] if group['ssrcs'] != f'{ssrc} {rtxSsrc}']
+            self._mediaDict["ssrcGroups"] = [
+                group
+                for group in self._mediaDict["ssrcGroups"]
+                if group["ssrcs"] != f"{ssrc} {rtxSsrc}"
+            ]
```

### Comparing `pymediasoup-0.2.6/pymediasoup/handlers/sdp/remote_sdp.py` & `pymediasoup-1.0.0/pymediasoup/handlers/sdp/remote_sdp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,156 +1,162 @@
-import sys
-if sys.version_info >= (3, 8):
-    from typing import List, Optional, Literal, Dict
-else:
-    from typing import List, Optional, Dict
-    from typing_extensions import Literal
+from typing import List, Optional, Literal, Dict
 
 import logging
 from pydantic import BaseModel
 from aiortc import RTCIceCandidate
 import sdp_transform
 from .media_section import MediaSection, AnswerMediaSection, OfferMediaSection
-from ...models.transport import IceCandidate, IceParameters, DtlsParameters, DtlsRole, PlainRtpParameters, DtlsRole
+from ...models.transport import (
+    IceCandidate,
+    IceParameters,
+    DtlsParameters,
+    DtlsRole,
+    PlainRtpParameters,
+)
 from ...producer import ProducerCodecOptions
-from ...rtp_parameters import MediaKind, RtpParameters
+from ...rtp_parameters import RtpParameters
 from ...sctp_parameters import SctpParameters
 
 
 logger = logging.getLogger(__name__)
 
 
 class MediaSectionIdx(BaseModel):
     idx: int
     reuseMid: Optional[str]
 
+
 class RemoteSdp:
     def __init__(
         self,
         iceParameters: Optional[IceParameters] = None,
         iceCandidates: List[IceCandidate] = [],
         dtlsParameters: Optional[DtlsParameters] = None,
         sctpParameters: SctpParameters = None,
         plainRtpParameters: Optional[PlainRtpParameters] = None,
-        planB: bool = False
+        planB: bool = False,
     ):
         self._iceParameters: Optional[IceParameters] = iceParameters
         self._iceCandidates: List[RTCIceCandidate] = iceCandidates
         self._dtlsParameters: Optional[DtlsParameters] = dtlsParameters
         self._sctpParameters: Optional[SctpParameters] = sctpParameters
         self._plainRtpParameters: Optional[PlainRtpParameters] = plainRtpParameters
         self._planB: bool = planB
         self._mediaSections: List[MediaSection] = []
         self._midToIndex: Dict[str, int] = {}
         self._firstMid: Optional[str] = None
         self._sdpDict: dict = {
-            'version': 0,
-            'origin': {
-                'address': '0.0.0.0',
-                'ipVer': 4,
-                'netType': 'IN',
-                'sessionId': 10000,
-                'sessionVersion': 0,
-                'username': 'mediasoup-client'
+            "version": 0,
+            "origin": {
+                "address": "0.0.0.0",
+                "ipVer": 4,
+                "netType": "IN",
+                "sessionId": 10000,
+                "sessionVersion": 0,
+                "username": "mediasoup-client",
             },
-            'name': '-',
-            'timing': { 'start': 0, 'stop': 0 },
-            'media': []
+            "name": "-",
+            "timing": {"start": 0, "stop": 0},
+            "media": [],
         }
 
         # If ICE parameters are given, add ICE-Lite indicator.
         if iceParameters:
             if iceParameters.iceLite:
-                self._sdpDict['icelite'] = 'ice-lite'
-        
+                self._sdpDict["icelite"] = "ice-lite"
+
         # If DTLS parameters are given, assume WebRTC and BUNDLE.
         if dtlsParameters:
-            self._sdpDict['msidSemantic'] = { 'semantic': 'WMS', 'token': '*' }
+            self._sdpDict["msidSemantic"] = {"semantic": "WMS", "token": "*"}
             # NOTE: aiortc currently only support sha-256
             for fingerprint in dtlsParameters.fingerprints:
-                if fingerprint.algorithm == 'sha-256':
+                if fingerprint.algorithm == "sha-256":
 
-                    self._sdpDict['fingerprint'] = {
-                        'type': fingerprint.algorithm,
-                        'hash': fingerprint.value
+                    self._sdpDict["fingerprint"] = {
+                        "type": fingerprint.algorithm,
+                        "hash": fingerprint.value,
                     }
             # # NOTE: Mediasoup Client take the latest fingerprint.
             # self._sdpDict['fingerprint'] = {
             #     'type': dtlsParameters.fingerprints[-1].algorithm,
             #     'hash': dtlsParameters.fingerprints[-1].value
             # }
-            self._sdpDict['groups'] = [{ 'type': 'BUNDLE', 'mids': '' }]
-        
+            self._sdpDict["groups"] = [{"type": "BUNDLE", "mids": ""}]
+
         # If there are plain RPT parameters, override SDP origin.
         if plainRtpParameters:
-            self._sdpDict['origin']['address'] = plainRtpParameters.ip
-            self._sdpDict['origin']['ipVer'] = plainRtpParameters.ipVersion
-    
+            self._sdpDict["origin"]["address"] = plainRtpParameters.ip
+            self._sdpDict["origin"]["ipVer"] = plainRtpParameters.ipVersion
+
     def updateIceParameters(self, iceParameters: IceParameters):
-        logger.debug(f'updateIceParameters() [iceParameters:{iceParameters}]')
+        logger.debug(f"updateIceParameters() [iceParameters:{iceParameters}]")
         self._iceParameters = iceParameters
-        self._sdpDict['icelite'] = 'ice-lite' if iceParameters.iceLite else None
-    
+        self._sdpDict["icelite"] = "ice-lite" if iceParameters.iceLite else None
+
     def updateDtlsRole(self, role: DtlsRole):
-        logger.debug(f'updateDtlsRole() [role:{role}]')
+        logger.debug(f"updateDtlsRole() [role:{role}]")
         if self._dtlsParameters:
             self._dtlsParameters.role = role
             for mediaSection in self._mediaSections:
                 mediaSection.setDtlsRole(role)
-        
+
     def getNextMediaSectionIdx(self):
         # If a closed media section is found, return its index.
         for idx, mediaSection in enumerate(self._mediaSections):
             if mediaSection.closed:
-                logger.debug(f'remoteSdp | getNextMediaSectionIdx() Closed media sections found { mediaSection}')
+                logger.debug(
+                    f"remoteSdp | getNextMediaSectionIdx() Closed media sections found { mediaSection}"
+                )
                 return MediaSectionIdx(idx=idx, reuseMid=mediaSection.mid)
         # If no closed media section is found, return next one.
-        logger.debug(f'remoteSdp | getNextMediaSectionIdx() No closed media sections found, return next {len(self._mediaSections)}')
+        logger.debug(
+            f"remoteSdp | getNextMediaSectionIdx() No closed media sections found, return next {len(self._mediaSections)}"
+        )
         return MediaSectionIdx(idx=len(self._mediaSections))
-    
+
     def send(
         self,
         offerMediaDict: dict,
         offerRtpParameters: RtpParameters,
         answerRtpParameters: RtpParameters,
-        codecOptions: Optional[ProducerCodecOptions]=None,
-        reuseMid: Optional[str]=None,
-        extmapAllowMixed = False
+        codecOptions: Optional[ProducerCodecOptions] = None,
+        reuseMid: Optional[str] = None,
+        extmapAllowMixed=False,
     ):
-        logger.debug(f'remoteSdp | send() offerMediaDict {offerMediaDict}')
+        logger.debug(f"remoteSdp | send() offerMediaDict {offerMediaDict}")
         mediaSection = AnswerMediaSection(
             sctpParameters=self._sctpParameters,
             iceParameters=self._iceParameters,
             iceCandidates=self._iceCandidates,
             dtlsParameters=self._dtlsParameters,
             plainRtpParameters=self._plainRtpParameters,
             planB=self._planB,
             offerMediaDict=offerMediaDict,
             offerRtpParameters=offerRtpParameters,
             answerRtpParameters=answerRtpParameters,
             codecOptions=codecOptions,
-            extmapAllowMixed=extmapAllowMixed
+            extmapAllowMixed=extmapAllowMixed,
         )
         # Unified-Plan with closed media section replacement.
         if reuseMid:
             self._replaceMediaSection(mediaSection, reuseMid)
         # Unified-Plan or Plan-B with different media kind.
         elif mediaSection.mid not in self._midToIndex.keys():
             self._addMediaSection(mediaSection)
         # Plan-B with same media kind.
         else:
             self._replaceMediaSection(mediaSection)
-        
+
     def receive(
         self,
         mid: str,
-        kind: Literal['audio', 'video', 'application'],
+        kind: Literal["audio", "video", "application"],
         offerRtpParameters: RtpParameters,
         streamId: str,
-        trackId: str
+        trackId: str,
     ):
         idx: int = self._midToIndex.get(str(mid), -1)
         if idx != -1:
             mediaSection = self._mediaSections[idx]
             # Plan-B.
             mediaSection.planBReceive(offerRtpParameters, streamId, trackId)
             self._replaceMediaSection(mediaSection)
@@ -162,117 +168,125 @@
                 dtlsParameters=self._dtlsParameters,
                 plainRtpParameters=self._plainRtpParameters,
                 planB=self._planB,
                 mid=mid,
                 kind=kind,
                 offerRtpParameters=offerRtpParameters,
                 streamId=streamId,
-                trackId=trackId
+                trackId=trackId,
             )
             # Let's try to recycle a closed media section (if any).
             # NOTE: Yes, we can recycle a closed m=audio section with a new m=video.
             closedMediaSections = [ms for ms in self._mediaSections if ms.closed]
             if closedMediaSections:
                 self._replaceMediaSection(mediaSection, closedMediaSections[0].mid)
             else:
                 self._addMediaSection(mediaSection)
-            
+
     def disableMediaSection(self, mid: str):
         idx: int = self._midToIndex.get(str(mid), -1)
         if idx == -1:
             raise Exception(f"no media section found with mid '{mid}'")
         mediaSection = self._mediaSections[idx]
         mediaSection.disable()
-    
+
     def closeMediaSection(self, mid: str):
         idx: int = self._midToIndex.get(str(mid), -1)
         if idx == -1:
             raise Exception(f"no media section found with mid '{mid}'")
         mediaSection = self._mediaSections[idx]
         # NOTE: Closing the first m section is a pain since it invalidates the
         # bundled transport, so let's avoid it.
         if mid == self._firstMid:
-            logger.debug(f'closeMediaSection() | cannot close first media section, disabling it instead [mid:{mid}]')
+            logger.debug(
+                f"closeMediaSection() | cannot close first media section, disabling it instead [mid:{mid}]"
+            )
             self.disableMediaSection(mid)
             return
         mediaSection.close()
         # Regenerate BUNDLE mids.
         self._regenerateBundleMids()
-    
+
     def planBStopReceiving(self, mid: str, offerRtpParameters: RtpParameters):
         idx: int = self._midToIndex.get(str(mid), -1)
         if idx == -1:
             raise Exception(f"no media section found with mid '{mid}'")
         mediaSection = self._mediaSections[idx]
         mediaSection.planBStopReceiving(offerRtpParameters)
         self._replaceMediaSection(mediaSection)
-    
+
     def sendSctpAssociation(self, offerMediaDict: dict):
         mediaSection = AnswerMediaSection(
             iceParameters=self._iceParameters,
             iceCandidates=self._iceCandidates,
             dtlsParameters=self._dtlsParameters,
             sctpParameters=self._sctpParameters,
             plainRtpParameters=self._plainRtpParameters,
-            offerMediaDict=offerMediaDict
+            offerMediaDict=offerMediaDict,
         )
         self._addMediaSection(mediaSection)
-    
+
     def receiveSctpAssociation(self, oldDataChannelSpec: bool = False):
         mediaSection = OfferMediaSection(
             iceParameters=self._iceParameters,
             iceCandidates=self._iceCandidates,
             dtlsParameters=self._dtlsParameters,
             sctpParameters=self._sctpParameters,
             plainRtpParameters=self._plainRtpParameters,
-            mid='datachannel',
-            kind='application',
-            oldDataChannelSpec=oldDataChannelSpec
+            mid="datachannel",
+            kind="application",
+            oldDataChannelSpec=oldDataChannelSpec,
         )
         self._addMediaSection(mediaSection)
-    
+
     def getSdp(self) -> str:
         # Increase SDP version.
-        self._sdpDict['origin']['sessionVersion'] += 1
+        self._sdpDict["origin"]["sessionVersion"] += 1
         return sdp_transform.write(self._sdpDict)
-    
+
     def _addMediaSection(self, newMediaSection: MediaSection):
-        if self._firstMid == None:
+        if self._firstMid is None:
             self._firstMid = newMediaSection.mid
         # Add to the list.
         self._mediaSections.append(newMediaSection)
         # Add to the map.
         self._midToIndex[newMediaSection.mid] = len(self._mediaSections) - 1
         # Add to the SDP object.
-        self._sdpDict['media'].append(newMediaSection.getDict())
+        self._sdpDict["media"].append(newMediaSection.getDict())
         # Regenerate BUNDLE mids.
         self._regenerateBundleMids()
 
-    def _replaceMediaSection(self, newMediaSection: MediaSection, reuseMid: Optional[str]=None):
+    def _replaceMediaSection(
+        self, newMediaSection: MediaSection, reuseMid: Optional[str] = None
+    ):
         # Store it in the map.
         if reuseMid:
             idx = self._midToIndex.get(str(reuseMid), -1)
             if idx == -1:
                 raise Exception(f"no media section found with mid '{reuseMid}'")
             oldMediaSection = self._mediaSections[idx]
             # Replace the index in the vector with the new media section.
             self._mediaSections[idx] = newMediaSection
             # Update the map.
             del self._midToIndex[oldMediaSection.mid]
             self._midToIndex[newMediaSection.mid] = idx
             # Update the SDP object.
-            self._sdpDict['media'][idx] = newMediaSection.getDict()
+            self._sdpDict["media"][idx] = newMediaSection.getDict()
             # Regenerate BUNDLE mids.
             self._regenerateBundleMids()
         else:
             idx = self._midToIndex.get(newMediaSection.mid, -1)
             if idx == -1:
-                raise Exception(f"no media section found with mid '{newMediaSection.mid}'")
+                raise Exception(
+                    f"no media section found with mid '{newMediaSection.mid}'"
+                )
             # Replace the index in the vector with the new media section.
             self._mediaSections[idx] = newMediaSection
             # Update the SDP object.
-            self._sdpDict['media'][idx] = newMediaSection.getDict()
-    
+            self._sdpDict["media"][idx] = newMediaSection.getDict()
+
     def _regenerateBundleMids(self):
         if not self._dtlsParameters:
             return
-        self._sdpDict['groups'][0]['mids'] = ' '.join([ms.mid for ms in self._mediaSections if not ms.closed])
+        self._sdpDict["groups"][0]["mids"] = " ".join(
+            [ms.mid for ms in self._mediaSections if not ms.closed]
+        )
```

### Comparing `pymediasoup-0.2.6/pymediasoup/handlers/sdp/unified_plan_utils.py` & `pymediasoup-1.0.0/pymediasoup/handlers/sdp/unified_plan_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,128 +1,122 @@
 import re
 from typing import List
 from ...rtp_parameters import RtpEncodingParameters, RTX
 
 
 def getRtpEncodings(offerMediaDict: dict) -> List[RtpEncodingParameters]:
     ssrcs = set()
-    for line in offerMediaDict.get('ssrcs', []):
-        ssrc = line.get('id')
+    for line in offerMediaDict.get("ssrcs", []):
+        ssrc = line.get("id")
         ssrcs.add(ssrc)
-    
+
     if len(ssrcs) == 0:
-        raise Exception('no a=ssrc lines found')
+        raise Exception("no a=ssrc lines found")
 
     ssrcToRtxSsrc = {}
 
     # First assume RTX is used.
-    for line in offerMediaDict.get('ssrcGroups', []):
-        if line.get('semantics') != 'FID':
+    for line in offerMediaDict.get("ssrcGroups", []):
+        if line.get("semantics") != "FID":
             continue
-        ssrc, rtxSsrc = re.split('\s', line.get('ssrcs'))
+        ssrc, rtxSsrc = re.split(r"\s", line.get("ssrcs"))
 
         ssrc = int(ssrc)
         rtxSsrc = int(rtxSsrc)
 
         if ssrc in ssrcs:
             # Remove both the SSRC and RTX SSRC from the set so later we know that they
             # are already handled.
             ssrcs.remove(ssrc)
             ssrcs.remove(rtxSsrc)
 
             # Add to the map.
             ssrcToRtxSsrc[ssrc] = rtxSsrc
-    
+
     # If the set of SSRCs is not empty it means that RTX is not being used, so take
     # media SSRCs from there.
     for ssrc in ssrcs:
         ssrcToRtxSsrc[ssrc] = None
-    
+
     encodings: List[RtpEncodingParameters] = []
     for ssrc, rtxSsrc in ssrcToRtxSsrc.items():
         encoding = RtpEncodingParameters(ssrc=ssrc)
-        if rtxSsrc != None:
+        if rtxSsrc is not None:
             encoding.rtx = RTX(ssrc=rtxSsrc)
         encodings.append(encoding)
     return encodings
 
+
 # Adds multi-ssrc based simulcast into the given SDP media section offer.
 def addLegacySimulcast(offerMediaDict: dict, numStreams: int):
     if numStreams <= 1:
-        raise Exception('numStreams must be greater than 1')
+        raise Exception("numStreams must be greater than 1")
 
     # Get the SSRC.
-    ssrcMsidLines = [line for line in offerMediaDict.get('ssrcs', []) if line.get('attribute') == 'msid']
+    ssrcMsidLines = [
+        line
+        for line in offerMediaDict.get("ssrcs", [])
+        if line.get("attribute") == "msid"
+    ]
     if not ssrcMsidLines:
-        raise Exception('a=ssrc line with msid information not found')
-    
+        raise Exception("a=ssrc line with msid information not found")
+
     ssrcMsidLine = ssrcMsidLines[0]
 
-    streamId, trackId = ssrcMsidLine.get('value').split(' ')
-    firstSsrc = ssrcMsidLine.get('id')
+    streamId, trackId = ssrcMsidLine.get("value").split(" ")
+    firstSsrc = ssrcMsidLine.get("id")
 
     firstRtxSsrc = None
 
     # Get the SSRC for RTX.
-    for line in offerMediaDict.get('ssrcGroups', []):
-        if line.get('semantics') != 'FID':
+    for line in offerMediaDict.get("ssrcGroups", []):
+        if line.get("semantics") != "FID":
             # False
             continue
-        ssrcs = re.split('\s', line.get('ssrcs'))
+        ssrcs = re.split(r"\s", line.get("ssrcs"))
         if int(ssrcs[0]) == firstSsrc:
             firstRtxSsrc = int(ssrcs[1])
             # True
-    
-    ssrcCnameLine = [line for line in offerMediaDict.get('ssrcs', []) if line.get('attribute') == 'cname']
+
+    ssrcCnameLine = [
+        line
+        for line in offerMediaDict.get("ssrcs", [])
+        if line.get("attribute") == "cname"
+    ]
 
     if not ssrcCnameLine:
-        raise Exception('a=ssrc line with cname information not found')
-    
-    cname = ssrcCnameLine.get('value')
+        raise Exception("a=ssrc line with cname information not found")
+
+    cname = ssrcCnameLine.get("value")
 
     ssrcs = []
     rtxSsrcs = []
 
     for i in range(numStreams):
         ssrcs.append(firstSsrc + i)
-        if firstRtxSsrc != None:
+        if firstRtxSsrc is not None:
             rtxSsrcs.append(firstRtxSsrc + i)
-    
-    offerMediaDict['ssrcGroups'] = []
-    offerMediaDict['ssrcs'] = []
-
-    offerMediaDict['ssrcGroups'].append({
-        'semantics': 'SIM',
-        'ssrc': ' '.join(ssrcs)
-    })
+
+    offerMediaDict["ssrcGroups"] = []
+    offerMediaDict["ssrcs"] = []
+
+    offerMediaDict["ssrcGroups"].append({"semantics": "SIM", "ssrc": " ".join(ssrcs)})
 
     for ssrc in ssrcs:
-        offerMediaDict['ssrcs'].append({
-            'id': ssrc,
-            'attribute': 'cname',
-            'value': cname
-        })
-        offerMediaDict['ssrcs'].append({
-            'id': ssrc,
-            'attribute': 'msid',
-            'value': f'{streamId} {trackId}'
-        })
-    
+        offerMediaDict["ssrcs"].append(
+            {"id": ssrc, "attribute": "cname", "value": cname}
+        )
+        offerMediaDict["ssrcs"].append(
+            {"id": ssrc, "attribute": "msid", "value": f"{streamId} {trackId}"}
+        )
+
     for i in range(len(rtxSsrcs)):
         ssrc = ssrcs[i]
         rtxSsrc = rtxSsrcs[i]
 
-        offerMediaDict['ssrc'].append({
-            'id': rtxSsrc,
-            'attribute': 'cname',
-            'value': cname
-        })
-        offerMediaDict['ssrc'].append({
-            'id': rtxSsrc,
-            'attribute': 'msid',
-            'value': f'{streamId} {trackId}'
-        })
-        offerMediaDict['ssrc'].append({
-            'id': 'FID',
-            'ssrcs': f'{ssrc} {rtxSsrc}'
-        })
-
+        offerMediaDict["ssrc"].append(
+            {"id": rtxSsrc, "attribute": "cname", "value": cname}
+        )
+        offerMediaDict["ssrc"].append(
+            {"id": rtxSsrc, "attribute": "msid", "value": f"{streamId} {trackId}"}
+        )
+        offerMediaDict["ssrc"].append({"id": "FID", "ssrcs": f"{ssrc} {rtxSsrc}"})
```

### Comparing `pymediasoup-0.2.6/pymediasoup/models/handler_interface.py` & `pymediasoup-1.0.0/pymediasoup/models/handler_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,78 +1,91 @@
-import sys
-if sys.version_info >= (3, 8):
-    from typing import Callable, Literal, List, Optional, Any
-else:
-    from typing import Callable, List, Optional, Any
-    from typing_extensions import Literal
+from typing import Literal, List, Optional, Any
 
 from pydantic import BaseModel
-from aiortc import RTCIceServer, RTCRtpSender, RTCRtpReceiver, RTCDataChannel, MediaStreamTrack
+from aiortc import (
+    RTCIceServer,
+    RTCRtpSender,
+    RTCRtpReceiver,
+    RTCDataChannel,
+    MediaStreamTrack,
+)
 from .transport import IceCandidate, IceParameters, DtlsParameters
 from ..ortc import ExtendedRtpCapabilities
 from ..sctp_parameters import SctpParameters, SctpStreamParameters
 from ..producer import ProducerCodecOptions
-from ..rtp_parameters import RtpCodecCapability, RtpParameters, MediaKind, RtpEncodingParameters
+from ..rtp_parameters import (
+    RtpCodecCapability,
+    RtpParameters,
+    MediaKind,
+    RtpEncodingParameters,
+)
 
 
 class HandlerRunOptions(BaseModel):
-    direction: Literal['send', 'recv']
+    direction: Literal["send", "recv"]
     iceParameters: IceParameters
     iceCandidates: List[IceCandidate]
     dtlsParameters: DtlsParameters
     sctpParameters: Optional[SctpParameters]
     iceServers: Optional[RTCIceServer]
-    iceTransportPolicy: Optional[Literal['all', 'relay']]
+    iceTransportPolicy: Optional[Literal["all", "relay"]]
     additionalSettings: Optional[Any]
     proprietaryConstraints: Optional[Any]
     extendedRtpCapabilities: ExtendedRtpCapabilities
 
     class Config:
-        arbitrary_types_allowed=True
+        arbitrary_types_allowed = True
+
 
 class HandlerSendOptions(BaseModel):
     track: MediaStreamTrack
     encodings: List[RtpEncodingParameters] = []
     codecOptions: Optional[ProducerCodecOptions]
     codec: Optional[RtpCodecCapability]
 
     class Config:
-        arbitrary_types_allowed=True
+        arbitrary_types_allowed = True
+
 
 class HandlerSendResult(BaseModel):
     localId: str
     rtpParameters: RtpParameters
     rtpSender: Optional[RTCRtpSender]
 
     class Config:
-        arbitrary_types_allowed=True
+        arbitrary_types_allowed = True
+
 
 class HandlerReceiveOptions(BaseModel):
     trackId: str
     kind: MediaKind
     rtpParameters: RtpParameters
 
+
 class HandlerReceiveResult(BaseModel):
     localId: str
     track: MediaStreamTrack
     rtpReceiver: Optional[RTCRtpReceiver]
 
     class Config:
-        arbitrary_types_allowed=True
+        arbitrary_types_allowed = True
+
 
 class HandlerSendDataChannelResult(BaseModel):
     dataChannel: RTCDataChannel
     sctpStreamParameters: SctpStreamParameters
 
     class Config:
-        arbitrary_types_allowed=True
+        arbitrary_types_allowed = True
+
 
 class HandlerReceiveDataChannelOptions(BaseModel):
     sctpStreamParameters: SctpStreamParameters
     label: Optional[str]
     protocol: Optional[str]
 
+
 class HandlerReceiveDataChannelResult(BaseModel):
     dataChannel: RTCDataChannel
 
     class Config:
-        arbitrary_types_allowed=True
+        arbitrary_types_allowed = True
```

### Comparing `pymediasoup-0.2.6/pymediasoup/models/transport.py` & `pymediasoup-1.0.0/pymediasoup/models/transport.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,85 +1,91 @@
-import sys
-if sys.version_info >= (3, 8):
-    from typing import Optional, Literal, List, Any, Callable, Dict
-else:
-    from typing import Optional, List, Any, Callable, Dict
-    from typing_extensions import Literal
+from typing import Optional, Literal, List, Any, Callable, Dict
 
 from enum import IntEnum
 from aiortc import RTCIceServer
 from pydantic import BaseModel
 from ..ortc import ExtendedRtpCapabilities
-from ..sctp_parameters import SctpParameters, SctpStreamParameters
+from ..sctp_parameters import SctpParameters
 
 
 class IceParameters(BaseModel):
     # ICE username fragment.
     usernameFragment: str
     # ICE password.
     password: str
     # ICE Lite.
     iceLite: Optional[bool]
 
+
 class IceCandidate(BaseModel):
     # Unique identifier that allows ICE to correlate candidates that appear on
     # multiple transports.
     foundation: str
     # The assigned priority of the candidate.
     priority: int
     # The IP address of the candidate.
     ip: str
     # The protocol of the candidate.
-    protocol: Literal['udp', 'tcp']
+    protocol: Literal["udp", "tcp"]
     # The port for the candidate.
     port: int
     # The type of candidate..
-    type: Literal['host', 'srflx', 'prflx', 'relay']
+    type: Literal["host", "srflx", "prflx", "relay"]
     # The type of TCP candidate.
-    tcpType: Optional[Literal['active', 'passive', 'so']]
+    tcpType: Optional[Literal["active", "passive", "so"]]
+
 
 # The hash function algorithm (as defined in the "Hash function Textual Names"
 # registry initially specified in RFC 4572 Section 8) and its corresponding
 # certificate fingerprint value (in lowercase hex string as expressed utilizing
 # the syntax of "fingerprint" in RFC 4572 Section 5).
 class DtlsFingerprint(BaseModel):
     algorithm: str
     value: str
 
-DtlsRole = Literal['auto', 'client', 'server']
+
+DtlsRole = Literal["auto", "client", "server"]
+
 
 class DtlsParameters(BaseModel):
     # DTLS role. Default 'auto'.
-    role: DtlsRole = 'auto'
+    role: DtlsRole = "auto"
     fingerprints: List[DtlsFingerprint]
 
-ConnectionState = Literal['new', 'connecting', 'connected', 'failed', 'disconnected', 'closed']
+
+ConnectionState = Literal[
+    "new", "connecting", "connected", "failed", "disconnected", "closed"
+]
+
 
 class IpVersion(IntEnum):
     ipv4 = 4
     ipv6 = 6
 
+
 class PlainRtpParameters(BaseModel):
     ip: str
     ipVersion: IpVersion
     port: int
 
+
 class TransportOptions(BaseModel):
     id: str
     iceParameters: IceParameters
     iceCandidates: List[IceCandidate]
     dtlsParameters: DtlsParameters
     sctpParameters: Optional[SctpParameters]
     iceServers: Optional[List[RTCIceServer]]
-    iceTransportPolicy: Optional[Literal['all', 'relay']]
+    iceTransportPolicy: Optional[Literal["all", "relay"]]
     additionalSettings: Optional[dict] = None
     proprietaryConstraints: Any = None
     appData: Optional[dict] = {}
 
     class Config:
-        arbitrary_types_allowed=True
+        arbitrary_types_allowed = True
+
 
 class InternalTransportOptions(TransportOptions):
-    direction: Literal['send', 'recv']
+    direction: Literal["send", "recv"]
     handlerFactory: Callable
     extendedRtpCapabilities: Optional[ExtendedRtpCapabilities] = None
     canProduceByKind: Dict[str, bool]
```

### Comparing `pymediasoup-0.2.6/pymediasoup/ortc.py` & `pymediasoup-1.0.0/pymediasoup/ortc.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,96 +1,128 @@
 from typing import List, Optional
-from .rtp_parameters import RtpCodec, RtcpFeedback, RtpHeaderExtension, RtpCapabilities, ExtendedRtpCapabilities, ExtendedCodec, ExtendedHeaderExtension, RtpCodecCapability, RtpHeaderExtension, MediaKind, RtpParameters, RtpCodecParameters, RtpHeaderExtensionParameters, RtpEncodingParameters, RtcpParameters
+from .rtp_parameters import (
+    RtpCodec,
+    RtcpFeedback,
+    RtpHeaderExtension,
+    RtpCapabilities,
+    ExtendedRtpCapabilities,
+    ExtendedCodec,
+    ExtendedHeaderExtension,
+    RtpCodecCapability,
+    MediaKind,
+    RtpParameters,
+    RtpCodecParameters,
+    RtpHeaderExtensionParameters,
+    RtpEncodingParameters,
+    RtcpParameters,
+)
 import h264_profile_level_id as h264
 
 
-RTP_PROBATOR_MID = 'probator'
+RTP_PROBATOR_MID = "probator"
 RTP_PROBATOR_SSRC = 1234
 RTP_PROBATOR_CODEC_PAYLOAD_TYPE = 127
 
-def matchCodecs(aCodec: RtpCodec, bCodec: RtpCodec, strict: bool = False, modify: bool = False) -> bool:
+
+def matchCodecs(
+    aCodec: RtpCodec, bCodec: RtpCodec, strict: bool = False, modify: bool = False
+) -> bool:
     aMimeType = aCodec.mimeType.lower()
     bMimeType = bCodec.mimeType.lower()
     if aMimeType != bMimeType:
         return False
     if aCodec.clockRate != bCodec.clockRate:
         return False
     if aCodec.channels != bCodec.channels:
         return False
 
-    if aMimeType == 'video/h264':
-        aPacketizationMode = aCodec.parameters.get('packetization-mode', 0)
-        bPacketizationMode = bCodec.parameters.get('packetization-mode', 0)
+    if aMimeType == "video/h264":
+        aPacketizationMode = aCodec.parameters.get("packetization-mode", 0)
+        bPacketizationMode = bCodec.parameters.get("packetization-mode", 0)
         if aPacketizationMode != bPacketizationMode:
             return False
         if strict:
             if not h264.isSameProfile(aCodec.parameters, bCodec.parameters):
                 return False
 
             if modify:
                 try:
                     selectedProfileLevelId = h264.generateProfileLevelIdForAnswer(
-                        aCodec.parameters, bCodec.parameters)
+                        aCodec.parameters, bCodec.parameters
+                    )
                 except TypeError:
                     return False
                 else:
                     if selectedProfileLevelId:
-                        aCodec.parameters['profile-level-id'] = selectedProfileLevelId
+                        aCodec.parameters["profile-level-id"] = selectedProfileLevelId
                     else:
-                        del aCodec.parameters['profile-level-id']
+                        del aCodec.parameters["profile-level-id"]
 
-    elif aMimeType == 'video/vp9':
+    elif aMimeType == "video/vp9":
         if strict:
-            aProfileId = aCodec.parameters.get('profile-id', 0)
-            bProfileId = bCodec.parameters.get('profile-id', 0)
+            aProfileId = aCodec.parameters.get("profile-id", 0)
+            bProfileId = bCodec.parameters.get("profile-id", 0)
             if aProfileId != bProfileId:
                 return False
 
     else:
         pass
 
     return True
 
 
 def isRtxCodec(codec: RtpCodec) -> bool:
     if not codec:
         return False
-    return codec.mimeType.endswith('/rtx')
+    return codec.mimeType.endswith("/rtx")
 
 
 def reduceRtcpFeedback(codecA: RtpCodec, codecB: RtpCodec) -> List[RtcpFeedback]:
     reducedRtcpFeedback: List[RtcpFeedback] = []
     for aFb in codecA.rtcpFeedback:
-        matchingBFbs = [bFb for bFb in codecB.rtcpFeedback if bFb.type == aFb.type and (
-            bFb.parameter == aFb.parameter or (not bFb.parameter and not aFb.parameter))]
+        matchingBFbs = [
+            bFb
+            for bFb in codecB.rtcpFeedback
+            if bFb.type == aFb.type
+            and (
+                bFb.parameter == aFb.parameter
+                or (not bFb.parameter and not aFb.parameter)
+            )
+        ]
         if matchingBFbs:
             reducedRtcpFeedback.append(matchingBFbs[0])
 
     return reducedRtcpFeedback
 
 
 def matchHeaderExtensions(aExt: RtpHeaderExtension, bExt: RtpHeaderExtension) -> bool:
     if aExt.kind != bExt.kind:
         return False
     if aExt.uri != bExt.uri:
         return False
     return True
 
+
 # Generate extended RTP capabilities for sending and receiving.
 
 
-def getExtendedRtpCapabilities(localCaps: RtpCapabilities, remoteCaps: RtpCapabilities) -> ExtendedRtpCapabilities:
+def getExtendedRtpCapabilities(
+    localCaps: RtpCapabilities, remoteCaps: RtpCapabilities
+) -> ExtendedRtpCapabilities:
     extendedRtpCapabilities: ExtendedRtpCapabilities = ExtendedRtpCapabilities()
     # Match media codecs and keep the order preferred by remoteCaps.
     for remoteCodec in remoteCaps.codecs:
         if isRtxCodec(remoteCodec):
             continue
 
-        matchingLocalCodecs = [localCodec for localCodec in localCaps.codecs if matchCodecs(
-            localCodec, remoteCodec, strict=True, modify=True)]
+        matchingLocalCodecs = [
+            localCodec
+            for localCodec in localCaps.codecs
+            if matchCodecs(localCodec, remoteCodec, strict=True, modify=True)
+        ]
 
         if not matchingLocalCodecs:
             continue
 
         matchingLocalCodec = matchingLocalCodecs[0]
 
         extendedCodec: ExtendedCodec = ExtendedCodec(
@@ -98,280 +130,346 @@
             kind=matchingLocalCodec.kind,
             clockRate=matchingLocalCodec.clockRate,
             channels=matchingLocalCodec.channels,
             localPayloadType=matchingLocalCodec.preferredPayloadType,
             remotePayloadType=remoteCodec.preferredPayloadType,
             localParameters=matchingLocalCodec.parameters,
             remoteParameters=remoteCodec.parameters,
-            rtcpFeedback=reduceRtcpFeedback(matchingLocalCodec, remoteCodec)
+            rtcpFeedback=reduceRtcpFeedback(matchingLocalCodec, remoteCodec),
         )
         extendedRtpCapabilities.codecs.append(extendedCodec)
 
     # Match RTX codecs.
     for extendedCodec in extendedRtpCapabilities.codecs:
-        matchingLocalRtxCodecs = [localCodec for localCodec in localCaps.codecs if isRtxCodec(
-            localCodec) and localCodec.parameters.get('apt') == extendedCodec.localPayloadType]
-        matchingRemoteRtxCodecs = [remoteCodec for remoteCodec in remoteCaps.codecs if isRtxCodec(
-            remoteCodec) and remoteCodec.parameters.get('apt') == extendedCodec.remotePayloadType]
+        matchingLocalRtxCodecs = [
+            localCodec
+            for localCodec in localCaps.codecs
+            if isRtxCodec(localCodec)
+            and localCodec.parameters.get("apt") == extendedCodec.localPayloadType
+        ]
+        matchingRemoteRtxCodecs = [
+            remoteCodec
+            for remoteCodec in remoteCaps.codecs
+            if isRtxCodec(remoteCodec)
+            and remoteCodec.parameters.get("apt") == extendedCodec.remotePayloadType
+        ]
         if matchingLocalRtxCodecs and matchingRemoteRtxCodecs:
-            extendedCodec.localRtxPayloadType = matchingLocalRtxCodecs[0].preferredPayloadType
-            extendedCodec.remoteRtxPayloadType = matchingRemoteRtxCodecs[0].preferredPayloadType
+            extendedCodec.localRtxPayloadType = matchingLocalRtxCodecs[
+                0
+            ].preferredPayloadType
+            extendedCodec.remoteRtxPayloadType = matchingRemoteRtxCodecs[
+                0
+            ].preferredPayloadType
 
     # Match header extensions.
     for remoteExt in remoteCaps.headerExtensions:
         matchingLocalExts = [
-            localExt for localExt in localCaps.headerExtensions if matchHeaderExtensions(localExt, remoteExt)]
+            localExt
+            for localExt in localCaps.headerExtensions
+            if matchHeaderExtensions(localExt, remoteExt)
+        ]
 
         if not matchingLocalExts:
             continue
 
         matchingLocalExt = matchingLocalExts[0]
 
         extendedExt: ExtendedHeaderExtension = ExtendedHeaderExtension(
             kind=remoteExt.kind,
             uri=remoteExt.uri,
             sendId=matchingLocalExt.preferredId,
             recvId=remoteExt.preferredId,
             encrypt=matchingLocalExt.preferredEncrypt,
-            direction='sendrecv'
+            direction="sendrecv",
         )
 
-        if remoteExt.direction == 'sendrecv':
-            extendedExt.direction = 'sendrecv'
-        elif remoteExt.direction == 'recvonly':
-            extendedExt.direction = 'sendonly'
-        elif remoteExt.direction == 'sendonly':
-            extendedExt.direction = 'recvonly'
-        elif remoteExt.direction == 'inactive':
-            extendedExt.direction = 'inactive'
+        if remoteExt.direction == "sendrecv":
+            extendedExt.direction = "sendrecv"
+        elif remoteExt.direction == "recvonly":
+            extendedExt.direction = "sendonly"
+        elif remoteExt.direction == "sendonly":
+            extendedExt.direction = "recvonly"
+        elif remoteExt.direction == "inactive":
+            extendedExt.direction = "inactive"
         else:
             pass
 
         extendedRtpCapabilities.headerExtensions.append(extendedExt)
 
     return extendedRtpCapabilities
 
+
 # Generate RTP capabilities for receiving media based on the given extended
 # RTP capabilities.
 
 
-def getRecvRtpCapabilities(extendedRtpCapabilities: ExtendedRtpCapabilities) -> RtpCapabilities:
+def getRecvRtpCapabilities(
+    extendedRtpCapabilities: ExtendedRtpCapabilities,
+) -> RtpCapabilities:
     rtpCapabilities: RtpCapabilities = RtpCapabilities()
     for extendedCodec in extendedRtpCapabilities.codecs:
 
         codec: RtpCodecCapability = RtpCodecCapability(
             mimeType=extendedCodec.mimeType,
             kind=extendedCodec.kind,
             preferredPayloadType=extendedCodec.remotePayloadType,
             clockRate=extendedCodec.clockRate,
             channels=extendedCodec.channels,
             parameters=extendedCodec.localParameters,
-            rtcpFeedback=extendedCodec.rtcpFeedback
+            rtcpFeedback=extendedCodec.rtcpFeedback,
         )
 
         rtpCapabilities.codecs.append(codec)
 
         # Add RTX codec.
         if not extendedCodec.remoteRtxPayloadType:
             continue
 
         rtxCodec: RtpCodecCapability = RtpCodecCapability(
-            mimeType=f'{extendedCodec.kind}/rtx',
+            mimeType=f"{extendedCodec.kind}/rtx",
             kind=extendedCodec.kind,
             preferredPayloadType=extendedCodec.remoteRtxPayloadType,
             clockRate=extendedCodec.clockRate,
-            parameters={
-                'apt': extendedCodec.remotePayloadType
-            },
-            rtcpFeedback=[]
+            parameters={"apt": extendedCodec.remotePayloadType},
+            rtcpFeedback=[],
         )
 
         rtpCapabilities.codecs.append(rtxCodec)
 
         # TODO: In the future, we need to add FEC, CN, etc, codecs.
 
     for extendedExtension in extendedRtpCapabilities.headerExtensions:
         # Ignore RTP extensions not valid for receiving.
-        if extendedExtension.direction != 'sendrecv' and extendedExtension.direction != 'recvonly':
+        if (
+            extendedExtension.direction != "sendrecv"
+            and extendedExtension.direction != "recvonly"
+        ):
             continue
 
         ext: RtpHeaderExtension = RtpHeaderExtension(
             kind=extendedExtension.kind,
             uri=extendedExtension.uri,
             preferredId=extendedExtension.recvId,
             preferredEncrypt=extendedExtension.encrypt,
-            direction=extendedExtension.direction
+            direction=extendedExtension.direction,
         )
 
         rtpCapabilities.headerExtensions.append(ext)
 
     return rtpCapabilities
 
+
 # Generate RTP parameters of the given kind for sending media.
 # NOTE: mid, encodings and rtcp fields are left empty.
 
 
-def getSendingRtpParameters(kind: MediaKind, extendedRtpCapabilities: ExtendedRtpCapabilities) -> RtpParameters:
+def getSendingRtpParameters(
+    kind: MediaKind, extendedRtpCapabilities: ExtendedRtpCapabilities
+) -> RtpParameters:
     rtpParameters: RtpParameters = RtpParameters()
     for extendedCodec in extendedRtpCapabilities.codecs:
         if extendedCodec.kind != kind:
             continue
 
         codec: RtpCodecParameters = RtpCodecParameters(
             mimeType=extendedCodec.mimeType,
             payloadType=extendedCodec.localPayloadType,
             clockRate=extendedCodec.clockRate,
             channels=extendedCodec.channels,
             parameters=extendedCodec.localParameters,
-            rtcpFeedback=extendedCodec.rtcpFeedback
+            rtcpFeedback=extendedCodec.rtcpFeedback,
         )
 
         rtpParameters.codecs.append(codec)
 
         # Add RTX codec.
         if extendedCodec.localRtxPayloadType:
             rtxCodec: RtpCodecParameters = RtpCodecParameters(
-                mimeType=f'{extendedCodec.kind}/rtx',
+                mimeType=f"{extendedCodec.kind}/rtx",
                 payloadType=extendedCodec.localRtxPayloadType,
                 clockRate=extendedCodec.clockRate,
-                parameters={'apt': extendedCodec.localPayloadType},
-                rtcpFeedback=[]
+                parameters={"apt": extendedCodec.localPayloadType},
+                rtcpFeedback=[],
             )
 
             rtpParameters.codecs.append(rtxCodec)
 
     for extendedExtension in extendedRtpCapabilities.headerExtensions:
-        if extendedExtension.kind != kind or (extendedExtension.direction not in ['sendrecv', 'sendonly']):
+        if extendedExtension.kind != kind or (
+            extendedExtension.direction not in ["sendrecv", "sendonly"]
+        ):
             continue
 
         ext: RtpHeaderExtensionParameters = RtpHeaderExtensionParameters(
             uri=extendedExtension.uri,
             id=extendedExtension.sendId,
             encrypt=extendedExtension.encrypt,
-            parameters={}
+            parameters={},
         )
 
         rtpParameters.headerExtensions.append(ext)
-    
+
     return rtpParameters
 
+
 # Generate RTP parameters of the given kind suitable for the remote SDP answer.
-def getSendingRemoteRtpParameters(kind: MediaKind, extendedRtpCapabilities: ExtendedRtpCapabilities) -> RtpParameters:
+def getSendingRemoteRtpParameters(
+    kind: MediaKind, extendedRtpCapabilities: ExtendedRtpCapabilities
+) -> RtpParameters:
     rtpParameters: RtpParameters = RtpParameters()
     for extendedCodec in extendedRtpCapabilities.codecs:
         if extendedCodec.kind != kind:
             continue
 
         codec = RtpCodecParameters(
             mimeType=extendedCodec.mimeType,
             payloadType=extendedCodec.localPayloadType,
             clockRate=extendedCodec.clockRate,
             channels=extendedCodec.channels,
             parameters=extendedCodec.remoteParameters,
-            rtcpFeedback=extendedCodec.rtcpFeedback
+            rtcpFeedback=extendedCodec.rtcpFeedback,
         )
 
         rtpParameters.codecs.append(codec)
 
         # Add RTX codec.
         if extendedCodec.localRtxPayloadType:
             rtxCodec: RtpCodecParameters = RtpCodecParameters(
-                mimeType=f'{extendedCodec.kind}/rtx',
+                mimeType=f"{extendedCodec.kind}/rtx",
                 payloadType=extendedCodec.localRtxPayloadType,
                 clockRate=extendedCodec.clockRate,
-                parameters={'apt': extendedCodec.localPayloadType},
-                rtcpFeedback=[]
+                parameters={"apt": extendedCodec.localPayloadType},
+                rtcpFeedback=[],
             )
 
             rtpParameters.codecs.append(rtxCodec)
-    
+
     for extendedExtension in extendedRtpCapabilities.headerExtensions:
-        if extendedExtension.kind != kind or (extendedExtension.direction not in ['sendrecv', 'sendonly']):
+        if extendedExtension.kind != kind or (
+            extendedExtension.direction not in ["sendrecv", "sendonly"]
+        ):
             continue
 
         ext: RtpHeaderExtensionParameters = RtpHeaderExtensionParameters(
             uri=extendedExtension.uri,
             id=extendedExtension.sendId,
             encrypt=extendedExtension.encrypt,
-            parameters={}
+            parameters={},
         )
 
         rtpParameters.headerExtensions.append(ext)
-    
+
     # Reduce codecs' RTCP feedback. Use Transport-CC if available, REMB otherwise.
-    if [ext for ext in rtpParameters.headerExtensions if ext.uri == 'http://www.ietf.org/id/draft-holmer-rmcat-transport-wide-cc-extensions-01']:
+    if [
+        ext
+        for ext in rtpParameters.headerExtensions
+        if ext.uri
+        == "http://www.ietf.org/id/draft-holmer-rmcat-transport-wide-cc-extensions-01"
+    ]:
         for codec in rtpParameters.codecs:
-            codec.rtcpFeedback = [fb for fb in codec.rtcpFeedback if fb.type != 'goog-remb']
-        
-    elif [ext for ext in rtpParameters.headerExtensions if ext.uri == 'http://www.webrtc.org/experiments/rtp-hdrext/abs-send-time']:
+            codec.rtcpFeedback = [
+                fb for fb in codec.rtcpFeedback if fb.type != "goog-remb"
+            ]
+
+    elif [
+        ext
+        for ext in rtpParameters.headerExtensions
+        if ext.uri == "http://www.webrtc.org/experiments/rtp-hdrext/abs-send-time"
+    ]:
         for codec in rtpParameters.codecs:
-            codec.rtcpFeedback = [fb for fb in codec.rtcpFeedback if fb.type != 'transport-cc']
-    
+            codec.rtcpFeedback = [
+                fb for fb in codec.rtcpFeedback if fb.type != "transport-cc"
+            ]
+
     else:
         for codec in rtpParameters.codecs:
-            codec.rtcpFeedback = [fb for fb in codec.rtcpFeedback if fb.type not in ['transport-cc', 'goog-remb']]
-        
+            codec.rtcpFeedback = [
+                fb
+                for fb in codec.rtcpFeedback
+                if fb.type not in ["transport-cc", "goog-remb"]
+            ]
+
     return rtpParameters
 
+
 # Reduce given codecs by returning an array of codecs "compatible" with the
 # given capability codec. If no capability codec is given, take the first
 # one(s).
 #
 # Given codecs must be generated by ortc.getSendingRtpParameters() or
 # ortc.getSendingRemoteRtpParameters().
 #
 # The returned array of codecs also include a RTX codec if available.
-def reduceCodecs(codecs: List[RtpCodecParameters], capCodec: Optional[RtpCodecCapability]=None):
+def reduceCodecs(
+    codecs: List[RtpCodecParameters], capCodec: Optional[RtpCodecCapability] = None
+):
     filteredCodecs: List[RtpCodecParameters] = []
 
     # If no capability codec is given, take the first one (and RTX).
     if not capCodec:
         filteredCodecs.append(codecs[0])
-        if len(codecs) >=2:
+        if len(codecs) >= 2:
             if isRtxCodec(codecs[1]):
                 filteredCodecs.append(codecs[1])
 
     # Otherwise look for a compatible set of codecs.
     else:
         for idx in range(len(codecs)):
             if matchCodecs(codecs[idx], capCodec):
                 filteredCodecs.append(codecs[idx])
 
                 if idx + 1 < len(codecs):
                     if isRtxCodec(codecs[idx + 1]):
                         filteredCodecs.append(codecs[idx + 1])
                         break
-        
+
         if not filteredCodecs:
-            raise TypeError('no matching codec found')
-    
+            raise TypeError("no matching codec found")
+
     return filteredCodecs
 
+
 # Create RTP parameters for a Consumer for the RTP probator.
 def generateProbatorRtpParameters(videoRtpParameters: RtpParameters) -> RtpParameters:
     videoRtpParameters = videoRtpParameters.copy(deep=True)
 
     rtpParameters: RtpParameters = RtpParameters(
         mid=RTP_PROBATOR_MID,
         encodings=[RtpEncodingParameters(ssrc=RTP_PROBATOR_SSRC)],
-        rtcp=RtcpParameters(cname='probator')
+        rtcp=RtcpParameters(cname="probator"),
     )
 
     rtpParameters.codecs.append(videoRtpParameters.codecs[0])
     rtpParameters.codecs[0].payloadType = RTP_PROBATOR_CODEC_PAYLOAD_TYPE
     rtpParameters.headerExtensions = videoRtpParameters.headerExtensions
 
     return rtpParameters
 
+
 # Whether media can be sent based on the given RTP capabilities.
 def canSend(kind: MediaKind, extendedRtpCapabilities: ExtendedRtpCapabilities) -> bool:
-    return len([codec for codec in extendedRtpCapabilities.codecs if codec.kind == kind]) > 0
+    return (
+        len([codec for codec in extendedRtpCapabilities.codecs if codec.kind == kind])
+        > 0
+    )
+
 
 # Whether the given RTP parameters can be received with the given RTP
 # capabilities.
-def canReceive(rtpParameters: RtpParameters, extendedRtpCapabilities: ExtendedRtpCapabilities) -> bool:
+def canReceive(
+    rtpParameters: RtpParameters, extendedRtpCapabilities: ExtendedRtpCapabilities
+) -> bool:
     if not rtpParameters.codecs:
         return False
-    
+
     firstMediaCodec = rtpParameters.codecs[0]
 
-    return len([codec for codec in extendedRtpCapabilities.codecs if codec.remotePayloadType == firstMediaCodec.payloadType]) > 0
+    return (
+        len(
+            [
+                codec
+                for codec in extendedRtpCapabilities.codecs
+                if codec.remotePayloadType == firstMediaCodec.payloadType
+            ]
+        )
+        > 0
+    )
```

### Comparing `pymediasoup-0.2.6/pymediasoup/producer.py` & `pymediasoup-1.0.0/pymediasoup/producer.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,40 +19,42 @@
     opusMaxPlaybackRate: Optional[int]
     opusMaxAverageBitrate: Optional[int]
     opusPtime: Optional[int]
     videoGoogleStartBitrate: Optional[int]
     videoGoogleMaxBitrate: Optional[int]
     videoGoogleMinBitrate: Optional[int]
 
+
 class ProducerOptions(BaseModel):
     track: Optional[MediaStreamTrack] = None
     encodings: Optional[List[RtpEncodingParameters]] = []
     codecOptions: Optional[ProducerCodecOptions] = None
     codec: Optional[RtpCodecCapability] = None
     stopTracks: bool = True
     disableTrackOnPause: bool = True
     zeroRtpOnPause: bool = False
     appData: Optional[Any] = {}
 
     class Config:
-        arbitrary_types_allowed=True
+        arbitrary_types_allowed = True
+
 
 class Producer(EnhancedEventEmitter):
     def __init__(
         self,
         id: str,
         localId: str,
         track: MediaStreamTrack,
         rtpParameters: RtpParameters,
         stopTracks: bool,
         disableTrackOnPause: bool,
         zeroRtpOnPause: bool,
         rtpSender: Optional[RTCRtpSender] = None,
         appData: Optional[dict] = None,
-        loop=None
+        loop=None,
     ):
         super(Producer, self).__init__(loop=loop)
 
         # Closed flag.
         self._closed: bool = False
         # Observer instance.
         self._observer: AsyncIOEventEmitter = AsyncIOEventEmitter()
@@ -73,176 +75,180 @@
 
         self._handleTrack()
 
     # Producer id.
     @property
     def id(self) -> str:
         return self._id
-    
+
     # Local id.
     @property
     def localId(self) -> str:
         return self._localId
-    
+
     # Whether the Producer is closed.
     @property
     def closed(self) -> bool:
         return self._closed
-    
+
     # Media kind.
     @property
     def kind(self) -> MediaStreamTrack.kind:
         return self._track.kind
-    
+
     # Associated RTCRtpSender.
     @property
     def rtpSender(self) -> Optional[RTCRtpSender]:
         return self._rtpSender
-    
+
     # The associated track.
     @property
     def track(self) -> Optional[MediaStreamTrack]:
         return self._track
-    
+
     # RTP parameters.
     @property
     def rtpParameters(self) -> RtpParameters:
         return self._rtpParameters
-    
+
     # Whether the Producer is paused.
     @property
     def paused(self) -> bool:
         return self._paused
-    
+
     # Max spatial layer.
     @property
     def maxSpatialLayer(self) -> Optional[int]:
         return self._maxSpatialLayer
-    
+
     # App custom data.
     @property
     def appData(self) -> Any:
         return self._appData
-    
+
     # Invalid setter.
     @appData.setter
     def appData(self, value):
-        raise Exception('cannot override appData object')
-    
+        raise Exception("cannot override appData object")
+
     # Observer.
     #
     # @emits close
     # @emits pause
     # @emits resume
     # @emits trackended
     @property
     def observer(self) -> AsyncIOEventEmitter:
         return self._observer
 
     async def close(self):
         if self._closed:
             return
-        
-        logger.debug('Producer close()')
+
+        logger.debug("Producer close()")
 
         self._closed = True
 
         self._destroyTrack()
 
-        await self.emit_for_results('@close')
+        await self.emit_for_results("@close")
 
         # Emit observer event.
-        self._observer.emit('close')
-    
+        self._observer.emit("close")
+
     # Transport was closed.
     def transportClosed(self):
         if self._closed:
             return
 
-        logger.debug('Producer transportClosed()')
+        logger.debug("Producer transportClosed()")
 
         self._closed = True
 
         self._destroyTrack()
 
-        self.emit('transportclose')
+        self.emit("transportclose")
+
+        self._observer.emit("close")
 
-        self._observer.emit('close')
-    
     # Get associated RTCRtpSender stats.
     async def getStats(self):
         if self._closed:
-            raise InvalidStateError('closed')
+            raise InvalidStateError("closed")
+
+        return await self.emit_for_results("@getstats")
 
-        return await self.emit_for_results('@getstats')
-    
     # Pauses sending media.
     def pause(self):
-        logger.warning("Producer pause() | 'AudioStreamTrack' object has no attribute 'enabled' pause() won't work")
-        logger.debug('Producer pause()')
+        logger.warning(
+            "Producer pause() | 'AudioStreamTrack' object has no attribute 'enabled' pause() won't work"
+        )
+        logger.debug("Producer pause()")
 
         if self._closed:
-            logger.debug('Producer pause() | Producer closed')
+            logger.debug("Producer pause() | Producer closed")
             return
-        
+
         self._paused = True
 
         if self._track and self._disableTrackOnPause:
             # TODO: MediaStreamTrack missing enable property
             # self._track.enabled = False
             pass
-        
+
         if self._zeroRtpOnPause:
-            self.emit('@replacetrack')
-        
-        self._observer.emit('pause')
-    
+            self.emit("@replacetrack")
+
+        self._observer.emit("pause")
+
     # Resumes sending media.
     def resume(self):
-        logger.warning("Producer pause() | 'AudioStreamTrack' object has no attribute 'enabled' resume() may not work")
-        logger.debug('Producer resume()')
+        logger.warning(
+            "Producer pause() | 'AudioStreamTrack' object has no attribute 'enabled' resume() may not work"
+        )
+        logger.debug("Producer resume()")
 
         if self._closed:
-            logger.debug('Producer resume() | Producer closed')
+            logger.debug("Producer resume() | Producer closed")
             return
-        
+
         self._paused = False
 
         if self._track and self._disableTrackOnPause:
             # TODO: MediaStreamTrack missing enable property
             # self._track.enabled = True
             pass
-        
+
         if self._zeroRtpOnPause:
-            self.emit('@replacetrack')
-        
-        self._observer.emit('resume')
+            self.emit("@replacetrack")
+
+        self._observer.emit("resume")
 
     # Replaces the current track with a new one or null.
     async def replaceTrack(self, track: MediaStreamTrack):
-        logger.debug(f'replaceTrack() [track: {track}]')
+        logger.debug(f"replaceTrack() [track: {track}]")
 
         if self._closed:
             # This must be done here. Otherwise there is no chance to stop the given
             # track.
             if self._stopTracks:
                 track.stop()
 
-            raise InvalidStateError('closed')
-    
-        elif track.readyState == 'ended':
-            raise InvalidStateError('ended')
-        
+            raise InvalidStateError("closed")
+
+        elif track.readyState == "ended":
+            raise InvalidStateError("ended")
+
         # Do nothing if this is the same track as the current handled one.
         if track == self._track:
-            logger.debug('Producer replaceTrack() | same track, ignored')
+            logger.debug("Producer replaceTrack() | same track, ignored")
             return
-        
+
         if not self._zeroRtpOnPause or not self._paused:
-            await self.emit_for_results('@replacetrack', track)
+            await self.emit_for_results("@replacetrack", track)
 
         # Destroy the previous track.
         self._destroyTrack()
 
         self._track = track
 
         # If this Producer was paused/resumed and the state of the new
@@ -252,55 +258,55 @@
                 # TODO: MediaStreamTrack missing enable property
                 # self._track.enabled = True
                 pass
             elif self._paused:
                 # TODO: MediaStreamTrack missing enable property
                 # self._track.enabled = False
                 pass
-        
+
         self._handleTrack()
 
     # Sets the video max spatial layer to be sent.
     async def setMaxSpatialLayer(self, spatialLayer: int):
         if self._closed:
-            raise InvalidStateError('closed')
-        
-        elif self._kind != 'video':
-            raise UnsupportedError('not a video Producer')
-        
+            raise InvalidStateError("closed")
+
+        elif self._kind != "video":
+            raise UnsupportedError("not a video Producer")
+
         if spatialLayer == self._maxSpatialLayer:
             return
-        
-        await self.emit_for_results('@setmaxspatiallayer', spatialLayer)
+
+        await self.emit_for_results("@setmaxspatiallayer", spatialLayer)
 
         self._maxSpatialLayer = spatialLayer
-    
+
     # Sets the DSCP value.
     # TODO: RTCRtpEncodingParameters
     async def setRtpEncodingParameters(self, params):
         if self._closed:
-            raise InvalidStateError('closed')
-        
-        await self.emit_for_results('@setrtpencodingparameters', params)
-    
+            raise InvalidStateError("closed")
+
+        await self.emit_for_results("@setrtpencodingparameters", params)
+
     def _onTrackEnded(self):
-            logger.debug('Producer track "ended" event')
-            self.emit('trackended')
-            self._observer.emit('trackended')
-    
+        logger.debug('Producer track "ended" event')
+        self.emit("trackended")
+        self._observer.emit("trackended")
+
     def _handleTrack(self):
         if not self._track:
             return
 
-        self._track.on('ended', self._onTrackEnded)
-    
+        self._track.on("ended", self._onTrackEnded)
+
     def _destroyTrack(self):
         if not self._track:
             return
 
-        if self._track.readyState == 'ended':
+        if self._track.readyState == "ended":
             return
 
-        self._track.remove_listener('ended', self._onTrackEnded)
+        self._track.remove_listener("ended", self._onTrackEnded)
 
         if self._stopTracks:
             self._track.stop()
```

### Comparing `pymediasoup-0.2.6/pymediasoup/rtp_parameters.py` & `pymediasoup-1.0.0/pymediasoup/rtp_parameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-import sys
-if sys.version_info >= (3, 8):
-    from typing import Optional, List, Any, Literal
-else:
-    from typing import Optional, List, Any
-    from typing_extensions import Literal
+from typing import Optional, List, Literal
 
 from pydantic import BaseModel
 
 
 # Media kind ('audio' or 'video').
-MediaKind = Literal['audio', 'video']
+MediaKind = Literal["audio", "video"]
+
 
 # Provides information on RTCP feedback messages for a specific codec. Those
 # messages can be transport layer feedback messages or codec-specific feedback
 # messages. The list of RTCP feedbacks supported by mediasoup is defined in the
 # supportedRtpCapabilities.ts file.
 class RtcpFeedback(BaseModel):
     type: str
-    parameter: str = ''
+    parameter: str = ""
+
 
 class Codec(BaseModel):
     # The codec MIME media type/subtype (e.g. 'audio/opus', 'video/VP8').
     mimeType: str
     # Codec clock rate expressed in Hertz.
     clockRate: int
     # The number of channels supported (e.g. two for stereo). Just for audio.
-	# Default 1.
+    # Default 1.
     channels: Optional[int] = None
     # Transport layer and codec-specific feedback messages for this codec.
     rtcpFeedback: List[RtcpFeedback] = []
 
+
 class RtpCodec(Codec):
     # Codec specific parameters. Some parameters (such as 'packetization-mode'
     # and 'profile-level-id' in H264 or 'profile-id' in VP9) are critical for
     # codec matching.
     parameters: dict = {}
 
+
 class ExtendedCodec(Codec):
     kind: MediaKind
     localPayloadType: int
     localRtxPayloadType: Optional[int]
     remotePayloadType: int
     remoteRtxPayloadType: Optional[int]
     localParameters: dict = {}
     remoteParameters: dict = {}
 
+
 # Provides information on the capabilities of a codec within the RTP
 # capabilities. The list of media codecs supported by mediasoup and their
 # settings is defined in the supportedRtpCapabilities.ts file.
 #
 # Exactly one RtpCodecCapability will be present for each supported combination
 # of parameters that requires a distinct value of preferredPayloadType. For
 # example:
@@ -62,95 +62,106 @@
 # one). If given, make sure it's in the 96-127 range.
 class RtpCodecCapability(RtpCodec):
     # Media kind.
     kind: MediaKind
     # The preferred RTP payload type.
     preferredPayloadType: Optional[int]
 
+
 # Provides information on codec settings within the RTP parameters. The list
 # of media codecs supported by mediasoup and their settings is defined in the
 # supportedRtpCapabilities.ts file.
 class RtpCodecParameters(RtpCodec):
     # The value that goes in the RTP Payload Type Field. Must be unique.
     payloadType: int
 
+
 # Provides information relating to supported header extensions. The list of
 # RTP header extensions supported by mediasoup is defined in the
 # supportedRtpCapabilities.ts file.
 #
 # mediasoup does not currently support encrypted RTP header extensions. The
 # direction field is just present in mediasoup RTP capabilities (retrieved via
 # router.rtpCapabilities or mediasoup.getSupportedRtpCapabilities()). It's
 # ignored if present in endpoints' RTP capabilities.
 class RtpHeaderExtension(BaseModel):
     # Media kind. If empty string, it's valid for all kinds.
-	# Default any media kind.
+    # Default any media kind.
     kind: Optional[MediaKind] = None
     # The URI of the RTP header extension, as defined in RFC 5285.
     uri: str
     # The preferred numeric identifier that goes in the RTP packet. Must be
-	# unique.
+    # unique.
     preferredId: int
     # If True, it is preferred that the value in the header be encrypted as per
-	# RFC 6904. Default False.
+    # RFC 6904. Default False.
     preferredEncrypt: Optional[bool] = False
     # If 'sendrecv', mediasoup supports sending and receiving this RTP extension.
-	# 'sendonly' means that mediasoup can send (but not receive) it. 'recvonly'
-	# means that mediasoup can receive (but not send) it.
-    direction: Optional[Literal['sendrecv', 'sendonly', 'recvonly', 'inactive']] = 'sendrecv'
+    # 'sendonly' means that mediasoup can send (but not receive) it. 'recvonly'
+    # means that mediasoup can receive (but not send) it.
+    direction: Optional[Literal["sendrecv", "sendonly", "recvonly", "inactive"]] = (
+        "sendrecv"
+    )
+
 
 class ExtendedHeaderExtension(BaseModel):
     kind: Optional[MediaKind] = None
     uri: str
     sendId: int
     recvId: int
     encrypt: bool
-    direction: Optional[Literal['sendrecv', 'sendonly', 'recvonly', 'inactive']] = 'sendrecv'
+    direction: Optional[Literal["sendrecv", "sendonly", "recvonly", "inactive"]] = (
+        "sendrecv"
+    )
+
 
 # The RTP capabilities define what mediasoup or an endpoint can receive at
 # media level.
 class RtpCapabilities(BaseModel):
     # Supported media and RTX codecs.
     codecs: List[RtpCodecCapability] = []
     # Supported RTP header extensions.
     headerExtensions: List[RtpHeaderExtension] = []
     # Supported FEC mechanisms.
     fecMechanisms: List[str] = []
 
+
 class RTX(BaseModel):
     ssrc: int
 
+
 # Provides information relating to an encoding, which represents a media RTP
 # stream and its associated RTX stream (if any).
 class RtpEncodingParameters(BaseModel):
     # The media SSRC.
     ssrc: Optional[int]
     # The RID RTP extension value. Must be unique.
     rid: Optional[str]
     # Codec payload type this encoding affects. If unset, first media codec is
-	# chosen.
+    # chosen.
     codecPayloadType: Optional[int]
     # RTX stream information. It must contain a numeric ssrc field indicating
-	# the RTX SSRC.
+    # the RTX SSRC.
     rtx: Optional[RTX]
     # It indicates whether discontinuous RTP transmission will be used. Useful
-	# for audio (if the codec supports it) and for video screen sharing (when
-	# static content is being transmitted, this option disables the RTP
-	# inactivity checks in mediasoup). Default False.
+    # for audio (if the codec supports it) and for video screen sharing (when
+    # static content is being transmitted, this option disables the RTP
+    # inactivity checks in mediasoup). Default False.
     dtx: Optional[bool] = False
     # Number of spatial and temporal layers in the RTP stream (e.g. 'L1T3').
-	# See webrtc-svc.
+    # See webrtc-svc.
     scalabilityMode: Optional[str]
     # Others.
     scaleResolutionDownBy: Optional[int]
     maxBitrate: Optional[int]
     maxFramerate: Optional[int]
     adaptivePtime: Optional[bool]
-    priority: Optional[Literal['very-low','low','medium','high']]
-    networkPriority: Optional[Literal['very-low','low','medium','high']]
+    priority: Optional[Literal["very-low", "low", "medium", "high"]]
+    networkPriority: Optional[Literal["very-low", "low", "medium", "high"]]
+
 
 # Defines a RTP header extension within the RTP parameters. The list of RTP
 # header extensions supported by mediasoup is defined in the
 # supportedRtpCapabilities.ts file.
 #
 # mediasoup does not currently support encrypted RTP header extensions and no
 # parameters are currently considered.
@@ -160,23 +171,25 @@
     # The numeric identifier that goes in the RTP packet. Must be unique.
     id: int
     # If True, the value in the header is encrypted as per RFC 6904. Default False.
     encrypt: Optional[bool] = False
     # Configuration parameters for the header extension.
     parameters: Optional[dict] = {}
 
+
 class RtcpParameters(BaseModel):
     # The Canonical Name (CNAME) used by RTCP (e.g. in SDES messages).
     cname: Optional[str]
     # Whether reduced size RTCP RFC 5506 is configured (if True) or compound RTCP
-	# as specified in RFC 3550 (if False). Default True.
+    # as specified in RFC 3550 (if False). Default True.
     reducedSize: Optional[bool] = True
     # Whether RTCP-mux is used. Default True.
     mux: Optional[bool]
 
+
 # The RTP send parameters describe a media stream received by mediasoup from
 # an endpoint through its corresponding mediasoup Producer. These parameters
 # may include a mid value that the mediasoup transport will use to match
 # received RTP packets based on their MID RTP extension value.
 #
 # mediasoup allows RTP send parameters with a single encoding and with multiple
 # encodings (simulcast). In the latter case, each entry in the encodings array
@@ -209,11 +222,12 @@
     codecs: List[RtpCodecParameters] = []
     # RTP header extensions in use.
     headerExtensions: List[RtpHeaderExtensionParameters] = []
     # Transmitted RTP streams and their settings.
     encodings: List[RtpEncodingParameters] = []
     # Parameters used for RTCP.
     rtcp: Optional[RtcpParameters]
-    
+
+
 class ExtendedRtpCapabilities(BaseModel):
     codecs: List[ExtendedCodec] = []
     headerExtensions: List[ExtendedHeaderExtension] = []
```

### Comparing `pymediasoup-0.2.6/pymediasoup/sctp_parameters.py` & `pymediasoup-1.0.0/pymediasoup/sctp_parameters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,48 @@
-import sys
-if sys.version_info >= (3, 8):
-    from typing import Optional, Literal
-else:
-    from typing import Optional
-    from typing_extensions import Literal
+from typing import Optional
 
 from pydantic import BaseModel
 
 
 class NumSctpStreams(BaseModel):
     # Initially requested number of outgoing SCTP streams.
     OS: int
     # Maximum number of incoming SCTP streams.
     MIS: int
 
+
 class SctpCapabilities(BaseModel):
     numStreams: NumSctpStreams
 
+
 class SctpParameters(BaseModel):
     # Must always equal 5000.
     port: int
     # Initially requested number of outgoing SCTP streams.
     OS: int
     # Maximum number of incoming SCTP streams.
     MIS: int
     # Maximum allowed size for SCTP messages.
     maxMessageSize: int
 
+
 # SCTP stream parameters describe the reliability of a certain SCTP stream.
 # If ordered is True then maxPacketLifeTime and maxRetransmits must be
 # False.
 # If ordered if False, only one of maxPacketLifeTime or maxRetransmits
 # can be True.
 class SctpStreamParameters(BaseModel):
     # SCTP stream id.
     streamId: Optional[int]
     # Whether data messages must be received in order. if True the messages will
-	# be sent reliably. Default True.
+    # be sent reliably. Default True.
     ordered: Optional[bool] = True
     # When ordered is False indicates the time (in milliseconds) after which a
-	# SCTP packet will stop being retransmitted.
+    # SCTP packet will stop being retransmitted.
     maxPacketLifeTime: Optional[int]
     # When ordered is False indicates the maximum number of times a packet will
-	# be retransmitted.
+    # be retransmitted.
     maxRetransmits: Optional[int]
     # A label which can be used to distinguish this DataChannel from others.
     label: Optional[str]
     # Name of the sub-protocol used by this DataChannel.
-    protocol: Optional[str]
+    protocol: Optional[str]
```

### Comparing `pymediasoup-0.2.6/pymediasoup/transport.py` & `pymediasoup-1.0.0/pymediasoup/transport.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,60 @@
-import sys
-if sys.version_info >= (3, 8):
-    from typing import Optional, Literal, List, Any, Callable, Dict, Union
-else:
-    from typing import Optional, List, Any, Callable, Dict, Union
-    from typing_extensions import Literal
+from typing import Optional, Literal, List, Any, Dict, Union
 
 import logging
 from pyee import AsyncIOEventEmitter
 from aiortc import RTCIceServer, MediaStreamTrack
 from .ortc import canReceive, generateProbatorRtpParameters, ExtendedRtpCapabilities
 from .errors import InvalidStateError, UnsupportedError
 from .emitter import EnhancedEventEmitter
 from .handlers.handler_interface import HandlerInterface
-from .models.handler_interface import HandlerReceiveOptions, HandlerSendResult, HandlerReceiveResult, SctpStreamParameters, HandlerSendDataChannelResult, HandlerReceiveDataChannelOptions, HandlerReceiveDataChannelResult
-from .models.transport import ConnectionState, IceParameters, InternalTransportOptions, DtlsParameters
+from .models.handler_interface import (
+    HandlerSendResult,
+    HandlerReceiveResult,
+    SctpStreamParameters,
+    HandlerSendDataChannelResult,
+    HandlerReceiveDataChannelResult,
+)
+from .models.transport import (
+    ConnectionState,
+    IceParameters,
+    InternalTransportOptions,
+    DtlsParameters,
+)
 from .consumer import Consumer, ConsumerOptions
 from .producer import Producer, ProducerOptions
 from .data_consumer import DataConsumer, DataConsumerOptions
 from .data_producer import DataProducer, DataProducerOptions
 from .producer import ProducerCodecOptions
-from .rtp_parameters import RtpParameters, RtpCodecCapability, RtpEncodingParameters, MediaKind
+from .rtp_parameters import (
+    RtpParameters,
+    RtpCodecCapability,
+    RtpEncodingParameters,
+    MediaKind,
+)
 
 
 logger = logging.getLogger(__name__)
 
 
 class Transport(EnhancedEventEmitter):
-    def __init__(
-        self,
-        options: InternalTransportOptions,
-        loop=None
-    ):
+    def __init__(self, options: InternalTransportOptions, loop=None):
         super(Transport, self).__init__(loop=loop)
 
-        logger.debug(f'constructor() [id:{options.id}, direction:{options.direction}]')
+        logger.debug(f"constructor() [id:{options.id}, direction:{options.direction}]")
 
         # Closed flag.
         self._closed: bool = False
         # Whether we can produce audio/video based on computed extended RTP
         # capabilities.
         self._canProduceByKind: Dict[str, bool]
         # App custom data.
         self._appData: Optional[dict]
         # Transport connection state.
-        self._connectionState: ConnectionState = 'new'
+        self._connectionState: ConnectionState = "new"
         # Producers indexed by id
         self._producers: Dict[str, Producer] = {}
         # Consumers indexed by id.
         self._consumers: Dict[str, Consumer] = {}
         # DataProducers indexed by id
         self._dataProducers: Dict[str, DataProducer] = {}
         # DataConsumers indexed by id.
@@ -56,27 +63,31 @@
         self._probatorConsumerCreated: bool = False
         # Observer instance.
         self._observer: AsyncIOEventEmitter = AsyncIOEventEmitter()
 
         # Id.
         self._id: str = options.id
         # Direction.
-        self._direction: Literal['send', 'recv'] = options.direction
+        self._direction: Literal["send", "recv"] = options.direction
         # Extended RTP capabilities.
-        self._extendedRtpCapabilities: ExtendedRtpCapabilities = options.extendedRtpCapabilities
+        self._extendedRtpCapabilities: ExtendedRtpCapabilities = (
+            options.extendedRtpCapabilities
+        )
         self._canProduceByKind: Dict[str, bool] = options.canProduceByKind
-        self._maxSctpMessageSize = options.sctpParameters.maxMessageSize if options.sctpParameters else None
+        self._maxSctpMessageSize = (
+            options.sctpParameters.maxMessageSize if options.sctpParameters else None
+        )
 
         if options.additionalSettings:
             additionalSettings = options.additionalSettings.copy(deep=True)
-            del additionalSettings['iceServers']
-            del additionalSettings['iceTransportPolicy']
-            del additionalSettings['bundlePolicy']
-            del additionalSettings['rtcpMuxPolicy']
-            del additionalSettings['sdpSemantics']
+            del additionalSettings["iceServers"]
+            del additionalSettings["iceTransportPolicy"]
+            del additionalSettings["bundlePolicy"]
+            del additionalSettings["rtcpMuxPolicy"]
+            del additionalSettings["sdpSemantics"]
         else:
             additionalSettings = None
 
         self._handler: HandlerInterface = options.handlerFactory()
 
         self._handler.run(
             direction=options.direction,
@@ -84,55 +95,55 @@
             iceCandidates=options.iceCandidates,
             dtlsParameters=options.dtlsParameters,
             sctpParameters=options.sctpParameters,
             iceServers=options.iceServers,
             iceTransportPolicy=options.iceTransportPolicy,
             additionalSettings=additionalSettings,
             proprietaryConstraints=options.proprietaryConstraints,
-            extendedRtpCapabilities=options.extendedRtpCapabilities
+            extendedRtpCapabilities=options.extendedRtpCapabilities,
         )
 
         self._appData = options.appData
 
         self._handleHandler()
-    
+
     # Producer id.
     @property
     def id(self) -> str:
         return self._id
-    
+
     # Whether the Producer is closed.
     @property
     def closed(self) -> bool:
         return self._closed
-    
+
     # Transport direction.
     @property
-    def direction(self) -> Literal['send', 'recv']:
+    def direction(self) -> Literal["send", "recv"]:
         return self._direction
-    
+
     # RTC handler instance.
     @property
     def handler(self) -> HandlerInterface:
         return self._handler
-    
+
     # Connection state.
     @property
     def connectionState(self) -> ConnectionState:
         return self._connectionState
-    
+
     # App custom data.
     @property
     def appData(self) -> Any:
         return self._appData
-    
+
     # Invalid setter.
     @appData.setter
     def appData(self, value):
-        raise Exception('cannot override appData object')
+        raise Exception("cannot override appData object")
 
     # Observer.
     #
     # @emits close
     # @emits newproducer - (producer: Producer)
     # @emits newconsumer - (producer: Producer)
     # @emits newdataproducer - (dataProducer: DataProducer)
@@ -141,367 +152,377 @@
     def observer(self) -> AsyncIOEventEmitter:
         return self._observer
 
     # Close the Transport.
     async def close(self):
         if self._closed:
             return
-        
-        logger.debug('Transport close()')
+
+        logger.debug("Transport close()")
 
         self._closed = True
 
         # Close the handler.
         await self._handler.close()
 
         # Close all Process.
-        for process_dict in [self._producers, self._consumers, self._dataProducers, self._dataConsumers]:
+        for process_dict in [
+            self._producers,
+            self._consumers,
+            self._dataProducers,
+            self._dataConsumers,
+        ]:
             for process in process_dict.values():
                 process.transportClosed()
             process_dict.clear()
-        
-        self._observer.emit('close')
-    
+
+        self._observer.emit("close")
+
     # Get associated Transport (RTCPeerConnection) stats.
     #
     # @returns {RTCStatsReport}
     async def getStats(self):
         if self._closed:
-            raise InvalidStateError('closed')
+            raise InvalidStateError("closed")
 
         return await self._handler.getTransportStats()
 
     # Restart ICE connection.
     async def restartIce(self, iceParameters: IceParameters):
         if self._closed:
-            raise InvalidStateError('closed')
-        
+            raise InvalidStateError("closed")
+
         return await self._handler.restartIce(iceParameters)
-    
+
     # Update ICE servers.
     async def updateIceServers(self, iceServers: List[RTCIceServer]):
         if self._closed:
-            raise InvalidStateError('closed')
+            raise InvalidStateError("closed")
 
         return await self._handler.updateIceServers(iceServers)
-    
+
     # Create a Producer.
     async def produce(
         self,
         track: Optional[MediaStreamTrack] = None,
         encodings: Optional[List[RtpEncodingParameters]] = [],
         codecOptions: Optional[ProducerCodecOptions] = None,
         codec: Optional[RtpCodecCapability] = None,
         stopTracks: bool = True,
         disableTrackOnPause: bool = True,
         zeroRtpOnPause: bool = False,
-        appData: Optional[Any] = {}
+        appData: Optional[Any] = {},
     ) -> Producer:
         options: ProducerOptions = ProducerOptions(
             track=track,
             encodings=encodings,
             codecOptions=codecOptions,
             codec=codec,
             stopTracks=stopTracks,
             disableTrackOnPause=disableTrackOnPause,
             zeroRtpOnPause=zeroRtpOnPause,
-            appData=appData
+            appData=appData,
         )
-        logger.debug(f'Transport produce() [track:{options.track}]')
+        logger.debug(f"Transport produce() [track:{options.track}]")
         if not options.track:
-            raise TypeError('missing track')
-        elif self._direction != 'send':
-            raise UnsupportedError('not a sending Transport')
+            raise TypeError("missing track")
+        elif self._direction != "send":
+            raise UnsupportedError("not a sending Transport")
         elif not self._canProduceByKind.get(options.track.kind):
-            raise UnsupportedError(f'cannot produce {options.track.kind}')
-        elif options.track.readyState == 'ended':
-            raise InvalidStateError('track ended')
-        elif len(self.listeners('connect')) == 0 and self._connectionState == 'new':
+            raise UnsupportedError(f"cannot produce {options.track.kind}")
+        elif options.track.readyState == "ended":
+            raise InvalidStateError("track ended")
+        elif len(self.listeners("connect")) == 0 and self._connectionState == "new":
             raise TypeError('no "connect" listener set into this transport')
-        elif len(self.listeners('connect')) == 0:
+        elif len(self.listeners("connect")) == 0:
             raise TypeError('no "produce" listener set into this transport')
-        
+
         # NOTE: Mediasoup client enqueue command here.
         handlerSendResult: HandlerSendResult = await self._handler.send(
             track=options.track,
             encodings=options.encodings,
             codecOptions=options.codecOptions,
-            codec=options.codec
+            codec=options.codec,
         )
 
         ids = await self.emit_for_results(
-            'produce',
+            "produce",
             options.track.kind,
             handlerSendResult.rtpParameters,
-            options.appData
+            options.appData,
         )
 
         producer = Producer(
             id=ids[0],
             localId=handlerSendResult.localId,
             rtpSender=handlerSendResult.rtpSender,
             track=options.track,
             rtpParameters=handlerSendResult.rtpParameters,
             stopTracks=options.stopTracks,
             disableTrackOnPause=options.disableTrackOnPause,
             zeroRtpOnPause=options.zeroRtpOnPause,
-            appData=options.appData
+            appData=options.appData,
         )
 
         self._producers[producer.id] = producer
         self._handleProducer(producer)
 
         # Emit observer event.
-        self._observer.emit('newproducer', producer)
+        self._observer.emit("newproducer", producer)
 
         return producer
-    
+
         # TODO: stop the given track if the command above failed due to closed Transport.
-    
+
     async def consume(
         self,
         id: str,
         producerId: str,
         kind: MediaKind,
         rtpParameters: Union[RtpParameters, dict],
-        appData: Optional[dict] = {}
+        appData: Optional[dict] = {},
     ) -> Consumer:
 
         if isinstance(rtpParameters, dict):
             rtpParameters: RtpParameters = RtpParameters(**rtpParameters)
 
         options: ConsumerOptions = ConsumerOptions(
             id=id,
             producerId=producerId,
             kind=kind,
             rtpParameters=rtpParameters,
-            appData=appData
+            appData=appData,
         )
-        logger.debug('Transport consume()')
-        rtpParameters:  RtpParameters = options.rtpParameters.copy(deep=True)
+        logger.debug("Transport consume()")
+        rtpParameters: RtpParameters = options.rtpParameters.copy(deep=True)
         if self._closed:
-            raise InvalidStateError('closed')
-        elif self._direction != 'recv':
-            raise UnsupportedError('not a receiving Transport')
-        elif len(self.listeners('connect')) == 0 and self._connectionState == 'new':
+            raise InvalidStateError("closed")
+        elif self._direction != "recv":
+            raise UnsupportedError("not a receiving Transport")
+        elif len(self.listeners("connect")) == 0 and self._connectionState == "new":
             raise TypeError('no "connect" listener set into this transport')
 
         # NOTE: Mediasoup client enqueue command here.
-        if not canReceive(rtpParameters=rtpParameters, extendedRtpCapabilities=self._extendedRtpCapabilities):
-            raise UnsupportedError('cannot consume this Producer')
+        if not canReceive(
+            rtpParameters=rtpParameters,
+            extendedRtpCapabilities=self._extendedRtpCapabilities,
+        ):
+            raise UnsupportedError("cannot consume this Producer")
 
         handlerReceiveResult: HandlerReceiveResult = await self._handler.receive(
-            trackId=options.id,
-            kind=options.kind,
-            rtpParameters=rtpParameters
+            trackId=options.id, kind=options.kind, rtpParameters=rtpParameters
         )
 
         consumer: Consumer = Consumer(
             id=options.id,
             localId=handlerReceiveResult.localId,
             producerId=options.producerId,
             track=handlerReceiveResult.track,
             rtpParameters=rtpParameters,
-            appData=options.appData
+            appData=options.appData,
         )
 
         self._consumers[consumer.id] = consumer
         self._handleConsumer(consumer)
 
         # If this is the first video Consumer and the Consumer for RTP probation
         # has not yet been created, create it now.
-        if not self._probatorConsumerCreated and options.kind == 'video':
-            probatorRtpParameters = generateProbatorRtpParameters(consumer.rtpParameters)
+        if not self._probatorConsumerCreated and options.kind == "video":
+            probatorRtpParameters = generateProbatorRtpParameters(
+                consumer.rtpParameters
+            )
             await self._handler.receive(
-                trackId='probator',
-                kind='video',
-                rtpParameters=probatorRtpParameters
+                trackId="probator", kind="video", rtpParameters=probatorRtpParameters
             )
 
-            logger.debug('Transport consume() | Consumer for RTP probation created')
+            logger.debug("Transport consume() | Consumer for RTP probation created")
 
             self._probatorConsumerCreated = True
-        
-        self._observer.emit('newconsumer', consumer)
+
+        self._observer.emit("newconsumer", consumer)
 
         return consumer
-    
+
     # Create a DataProducer
     async def produceData(
         self,
-        ordered: Optional[bool]=None,
-        maxPacketLifeTime: Optional[int]=None,
-        maxRetransmits: Optional[int]=None,
-        label: Optional[str]=None,
-        protocol: Optional[str]=None,
-        appData: Optional[dict] = {}
+        ordered: Optional[bool] = None,
+        maxPacketLifeTime: Optional[int] = None,
+        maxRetransmits: Optional[int] = None,
+        label: Optional[str] = None,
+        protocol: Optional[str] = None,
+        appData: Optional[dict] = {},
     ) -> DataProducer:
         options: DataProducerOptions = DataProducerOptions(
             ordered=ordered,
             maxPacketLifeTime=maxPacketLifeTime,
             maxRetransmits=maxRetransmits,
             label=label,
             protocol=protocol,
-            appData=appData
+            appData=appData,
         )
-        logger.debug('Transport produceData()')
-        if self._direction != 'send':
-            raise UnsupportedError('not a sending Transport')
+        logger.debug("Transport produceData()")
+        if self._direction != "send":
+            raise UnsupportedError("not a sending Transport")
 
         elif not self._maxSctpMessageSize:
-            raise UnsupportedError('SCTP not enabled by remote Transport')
+            raise UnsupportedError("SCTP not enabled by remote Transport")
 
-        elif len(self.listeners('connect')) == 0 and self._connectionState == 'new':
+        elif len(self.listeners("connect")) == 0 and self._connectionState == "new":
             raise TypeError('no "connect" listener set into this transport')
 
-        elif len(self.listeners('producedata')) == 0:
+        elif len(self.listeners("producedata")) == 0:
             raise TypeError('no "producedata" listener set into this transport')
 
         if options.maxPacketLifeTime or options.maxRetransmits:
             options.ordered = False
-        
+
         # NOTE: Mediasoup client enqueue command here.
-        handlerSendDataChannelResult: HandlerSendDataChannelResult = await self._handler.sendDataChannel(
-            ordered=options.ordered,
-            maxPacketLifeTime=options.maxPacketLifeTime,
-            maxRetransmits=options.maxRetransmits,
-            label=options.label,
-            protocol=options.protocol
+        handlerSendDataChannelResult: HandlerSendDataChannelResult = (
+            await self._handler.sendDataChannel(
+                ordered=options.ordered,
+                maxPacketLifeTime=options.maxPacketLifeTime,
+                maxRetransmits=options.maxRetransmits,
+                label=options.label,
+                protocol=options.protocol,
+            )
         )
 
         ids = await self.emit_for_results(
-            'producedata',
+            "producedata",
             sctpStreamParameters=handlerSendDataChannelResult.sctpStreamParameters,
             label=options.label,
             protocol=options.protocol,
-            appData=options.appData
+            appData=options.appData,
         )
 
         dataProducer = DataProducer(
             id=ids[0],
             dataChannel=handlerSendDataChannelResult.dataChannel,
             sctpStreamParameters=handlerSendDataChannelResult.sctpStreamParameters,
-            appData=options.appData
+            appData=options.appData,
         )
 
         self._dataProducers[dataProducer.id] = dataProducer
         self._handleDataProducer(dataProducer)
 
         # Emit observer event.
-        self._observer.emit('newdataproducer', dataProducer)
+        self._observer.emit("newdataproducer", dataProducer)
 
         return dataProducer
 
     # Create a DataConsumer
     async def consumeData(
         self,
         id: str,
         dataProducerId: str,
         sctpStreamParameters: SctpStreamParameters,
-        label: Optional[str]=None,
-        protocol: Optional[str]=None,
-        appData: Optional[dict]={}
+        label: Optional[str] = None,
+        protocol: Optional[str] = None,
+        appData: Optional[dict] = {},
     ) -> DataConsumer:
         options: DataConsumerOptions = DataConsumerOptions(
             id=id,
             dataProducerId=dataProducerId,
             sctpStreamParameters=sctpStreamParameters,
             label=label,
             protocol=protocol,
-            appData=appData
+            appData=appData,
         )
-        logger.debug('Transport consumeData()')
+        logger.debug("Transport consumeData()")
         if self._closed:
-            raise InvalidStateError('closed')
-        elif self._direction != 'recv':
-            raise UnsupportedError('not a receiving Transport')
-        elif len(self.listeners('connect')) == 0 and self._connectionState == 'new':
+            raise InvalidStateError("closed")
+        elif self._direction != "recv":
+            raise UnsupportedError("not a receiving Transport")
+        elif len(self.listeners("connect")) == 0 and self._connectionState == "new":
             raise TypeError('no "connect" listener set into this transport')
-        
+
         # NOTE: Mediasoup client enqueue command here.
-        handlerReceiveDataChannelResult: HandlerReceiveDataChannelResult = await self._handler.receiveDataChannel(
-            sctpStreamParameters=options.sctpStreamParameters,
-            label=options.label,
-            protocol=options.protocol
+        handlerReceiveDataChannelResult: HandlerReceiveDataChannelResult = (
+            await self._handler.receiveDataChannel(
+                sctpStreamParameters=options.sctpStreamParameters,
+                label=options.label,
+                protocol=options.protocol,
+            )
         )
 
         dataConsumer: DataConsumer = DataConsumer(
             id=options.id,
             dataProducerId=options.dataProducerId,
             dataChannel=handlerReceiveDataChannelResult.dataChannel,
             sctpStreamParameters=options.sctpStreamParameters,
-            appData=options.appData
+            appData=options.appData,
         )
 
         self._dataConsumers[dataConsumer.id] = dataConsumer
         self._handleDataConsumer(dataConsumer)
 
         # Emit observer event.
-        self._observer.emit('newdataconsumer', dataConsumer)
+        self._observer.emit("newdataconsumer", dataConsumer)
 
         return dataConsumer
 
     def _handleHandler(self):
         handler = self._handler
 
-        @handler.on('@connect')
+        @handler.on("@connect")
         async def on_connect(dtlsParameters: DtlsParameters):
             if self._closed:
-                raise InvalidStateError('closed')
+                raise InvalidStateError("closed")
             else:
-                self.emit('connect', dtlsParameters)
+                self.emit("connect", dtlsParameters)
 
-        @handler.on('@connectionstatechange')
+        @handler.on("@connectionstatechange")
         def on_connectionstatechange(connectionState: ConnectionState):
             self._connectionState = connectionState
             if not self._closed:
-                self.emit('connectionstatechange', connectionState)
-    
+                self.emit("connectionstatechange", connectionState)
+
     def _handleProducer(self, producer: Producer):
-        @producer.on('@close')
+        @producer.on("@close")
         async def on_close():
             del self._producers[producer.id]
             if self._closed:
                 return
             await self._handler.stopSending(producer.localId)
-        
-        @producer.on('@replacetrack')
+
+        @producer.on("@replacetrack")
         async def on_replacetrack(track):
             await self._handler.replaceTrack(producer.localId, track)
-        
-        @producer.on('@setmaxspatiallayer')
+
+        @producer.on("@setmaxspatiallayer")
         async def on_setmaxspatiallayer(spatialLayer):
             await self._handler.setMaxSpatialLayer(producer.localId, spatialLayer)
-        
-        @producer.on('@setrtpencodingparameters')
+
+        @producer.on("@setrtpencodingparameters")
         async def on_setrtpencodingparameters(params):
             await self._handler.setRtpEncodingParameters(producer.localId, params)
-        
-        @producer.on('@getstats')
+
+        @producer.on("@getstats")
         async def on_getstats():
             if self._closed:
-                return InvalidStateError('closed')
+                return InvalidStateError("closed")
             return await self._handler.getSenderStats(producer.localId)
-    
+
     def _handleConsumer(self, consumer: Consumer):
-        @consumer.on('@close')
+        @consumer.on("@close")
         async def on_close():
             del self._consumers[consumer.id]
             if self._closed:
                 return
             await self._handler.stopReceiving(consumer.localId)
 
-        @consumer.on('@getstats')
+        @consumer.on("@getstats")
         async def on_getstats():
             if self._closed:
-                return InvalidStateError('closed')
+                return InvalidStateError("closed")
             return await self._handler.getReceiverStats(consumer.localId)
-        
+
     def _handleDataProducer(self, dataProducer: DataProducer):
-        @dataProducer.on('@close')
+        @dataProducer.on("@close")
         async def on_close():
             del self._dataProducers[dataProducer.id]
-        
+
     def _handleDataConsumer(self, dataConsumer: DataConsumer):
-        @dataConsumer.on('@close')
+        @dataConsumer.on("@close")
         async def on_close():
-            del self._dataConsumers[dataConsumer.id]
+            del self._dataConsumers[dataConsumer.id]
```

### Comparing `pymediasoup-0.2.6/pyproject.toml` & `pymediasoup-1.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tool.poetry]
 name = "pymediasoup"
-version = "0.2.6"
+version = "1.0.0"
 description = "mediasoup python client"
 authors = ["Jiang Yue <maze1024@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/skymaze/pymediasoup"
 
 [tool.poetry.dependencies]
-python = ">=3.7, <3.12"
+python = "^3.8.1"
 pydantic = "^1.8.1"
 aiortc = "^1.5.0"
 h264-profile-level-id = "^1.0.0"
-sdp-transform = "^1.0.6"
-pyee = "^9.0.4"
+sdp-transform = "^1.1.0"
+pyee = "^11.1.0"
+av = "^11.0.0"
 
-[tool.poetry.dev-dependencies]
-mypy = "^0.990"
+[tool.poetry.group.dev.dependencies]
+flake8 = "^7.0.0"
+black = "^24.4.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pymediasoup-0.2.6/PKG-INFO` & `pymediasoup-1.0.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: pymediasoup
-Version: 0.2.6
+Version: 1.0.0
 Summary: mediasoup python client
 Home-page: https://github.com/skymaze/pymediasoup
 License: MIT
 Author: Jiang Yue
 Author-email: maze1024@gmail.com
-Requires-Python: >=3.7,<3.12
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiortc (>=1.5.0,<2.0.0)
+Requires-Dist: av (>=11.0.0,<12.0.0)
 Requires-Dist: h264-profile-level-id (>=1.0.0,<2.0.0)
 Requires-Dist: pydantic (>=1.8.1,<2.0.0)
-Requires-Dist: pyee (>=9.0.4,<10.0.0)
-Requires-Dist: sdp-transform (>=1.0.6,<2.0.0)
+Requires-Dist: pyee (>=11.1.0,<12.0.0)
+Requires-Dist: sdp-transform (>=1.1.0,<2.0.0)
 Project-URL: Repository, https://github.com/skymaze/pymediasoup
 Description-Content-Type: text/markdown
 
 # PyMediasoup
 [![Python](https://img.shields.io/pypi/pyversions/pymediasoup)](https://www.python.org/)
 [![Pypi](https://img.shields.io/pypi/v/pymediasoup)](https://pypi.org/project/pymediasoup/)
 [![License](https://img.shields.io/pypi/l/pymediasoup)](https://github.com/skymaze/pymediasoup/blob/main/LICENSE)
```

