# Comparing `tmp/opclabs_mqttnet-5.80.191.tar.gz` & `tmp/opclabs_mqttnet-5.80.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opclabs_mqttnet-5.80.191.tar", last modified: Mon May  6 14:40:57 2024, max compression
+gzip compressed data, was "opclabs_mqttnet-5.80.75.tar", last modified: Fri Feb 16 19:21:03 2024, max compression
```

## Comparing `opclabs_mqttnet-5.80.191.tar` & `opclabs_mqttnet-5.80.75.tar`

### file list

```diff
@@ -1,318 +1,318 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 14:40:57.151687 opclabs_mqttnet-5.80.191/
--rw-rw-rw-   0        0        0      168 2024-02-20 15:46:20.000000 opclabs_mqttnet-5.80.191/MANIFEST.in
--rw-rw-rw-   0        0        0    18761 2024-05-06 14:40:57.151687 opclabs_mqttnet-5.80.191/PKG-INFO
--rw-rw-rw-   0        0        0      726 2024-02-20 15:46:16.000000 opclabs_mqttnet-5.80.191/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 14:40:56.042306 opclabs_mqttnet-5.80.191/opclabs_mqttnet/
-drwxrwxrwx   0        0        0        0 2024-05-06 14:40:56.511056 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/
--rw-rw-rw-   0        0        0     2442 2024-05-06 14:34:25.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/MQTTnet.Extensions.ManagedClient_4.3.3.952.html
--rw-rw-rw-   0        0        0     2442 2024-05-06 14:34:24.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/MQTTnet_4.3.3.952.html
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:21.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Platforms_1.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:20.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Platforms_1.1.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:21.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Platforms_1.1.1.txt
--rw-rw-rw-   0        0        0     1116 2024-05-06 14:34:22.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Platforms_2.0.0.txt
--rw-rw-rw-   0        0        0     1116 2024-05-06 14:34:22.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Platforms_2.1.0.txt
--rw-rw-rw-   0        0        0     1116 2024-05-06 14:34:22.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Platforms_2.1.2.txt
--rw-rw-rw-   0        0        0     9323 2024-05-06 14:34:22.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Portable.Compatibility_1.0.2.txt
--rw-rw-rw-   0        0        0     9211 2024-05-06 14:34:22.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Runtime.CoreCLR_1.0.2.txt
--rw-rw-rw-   0        0        0     9211 2024-05-06 14:34:22.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Runtime.CoreCLR_1.0.3.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:23.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Targets_1.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:22.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Targets_1.1.0.txt
--rw-rw-rw-   0        0        0    11228 2024-05-06 14:34:23.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.UniversalWindowsPlatform_6.2.10.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:20.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore_5.0.2.txt
--rw-rw-rw-   0        0        0    11228 2024-05-06 14:34:19.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.Net.Native.Compiler_1.7.6.txt
--rw-rw-rw-   0        0        0    11228 2024-05-06 14:34:19.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.Net.Native.Compiler_2.2.8-rel-28605-00.txt
--rw-rw-rw-   0        0        0    11228 2024-05-06 14:34:20.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.Net.UWPCoreRuntimeSdk_2.2.10.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:23.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.Win32.Primitives_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:23.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.Win32.Primitives_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:25.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/NETStandard.Library_1.6.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:28.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.AppContext_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:28.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Buffers_4.3.0.txt
--rw-rw-rw-   0        0        0     1116 2024-05-06 14:34:28.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Buffers_4.4.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:28.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections.Concurrent_4.0.12.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:28.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections.Concurrent_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:28.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections.Immutable_1.2.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:28.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections.NonGeneric_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:28.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections.NonGeneric_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:29.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections.Specialized_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:29.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections.Specialized_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:28.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections_4.0.11.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:28.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:29.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.ComponentModel.EventBasedAsync_4.0.11.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:29.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.ComponentModel.EventBasedAsync_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:29.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Console_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:29.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Data.Common_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:29.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.Contracts_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:30.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.Debug_4.0.11.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:29.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.Debug_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:30.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.DiagnosticSource_4.0.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:30.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.DiagnosticSource_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:30.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.StackTrace_4.0.2.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:30.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.Tools_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:31.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.Tracing_4.1.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:30.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.Tracing_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:31.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Globalization.Calendars_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:31.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Globalization.Calendars_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:31.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Globalization.Extensions_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:31.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Globalization.Extensions_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:31.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Globalization_4.0.11.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:31.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Globalization_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:32.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.Compression.ZipFile_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:32.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.Compression_4.1.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:32.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.Compression_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:32.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.FileSystem.Primitives_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:32.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.FileSystem.Primitives_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:32.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.FileSystem_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:32.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.FileSystem_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:33.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.IsolatedStorage_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:32.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.IO_4.1.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:31.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.IO_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:33.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Linq.Expressions_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:33.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Linq.Queryable_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:33.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Linq_4.1.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:33.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Linq_4.3.0.txt
--rw-rw-rw-   0        0        0     1116 2024-05-06 14:34:33.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Memory_4.5.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:34.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Http.Rtc_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:34.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Http_4.1.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:33.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Http_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:34.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Http_4.3.4.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:34.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.NameResolution_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:35.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Primitives_4.0.11.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:35.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Primitives_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:35.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Requests_4.0.11.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:35.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Requests_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:35.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Security_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:35.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Security_4.3.2.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:35.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Sockets_4.1.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:35.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Sockets_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:35.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.WebHeaderCollection_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:36.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.WebSockets.Client_4.3.2.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:36.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.WebSockets_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:36.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Numerics.Vectors.WindowsRuntime_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:36.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Numerics.Vectors_4.3.0.txt
--rw-rw-rw-   0        0        0     1116 2024-05-06 14:34:36.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Numerics.Vectors_4.4.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:37.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.ObjectModel_4.0.12.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:36.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.ObjectModel_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:37.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Private.DataContractSerialization_4.1.2.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:37.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Private.DataContractSerialization_4.3.0.txt
--rw-rw-rw-   0        0        0     1116 2024-05-06 14:34:37.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Private.ServiceModel_4.5.3.txt
--rw-rw-rw-   0        0        0     2442 2024-05-06 14:34:37.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Private.ServiceModel_4.6.0.html
--rw-rw-rw-   0        0        0     2442 2024-05-06 14:34:38.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Context_7.0.0.html
--rw-rw-rw-   0        0        0     1116 2024-05-06 14:34:38.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.DispatchProxy_4.5.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:39.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Emit.ILGeneration_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:39.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Emit.ILGeneration_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:39.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Emit.Lightweight_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:39.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Emit.Lightweight_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:39.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Emit_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:38.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Emit_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:39.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Extensions_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:39.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Extensions_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:39.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Metadata_1.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:40.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Primitives_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:39.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Primitives_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:40.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.TypeExtensions_4.1.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:40.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.TypeExtensions_4.3.0.txt
--rw-rw-rw-   0        0        0     1116 2024-05-06 14:34:40.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.TypeExtensions_4.4.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:38.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection_4.1.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:38.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:40.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Resources.ResourceManager_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:40.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Resources.ResourceManager_4.3.0.txt
--rw-rw-rw-   0        0        0     1116 2024-05-06 14:34:41.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.CompilerServices.Unsafe_4.5.0.txt
--rw-rw-rw-   0        0        0     1116 2024-05-06 14:34:41.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.CompilerServices.Unsafe_4.5.2.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:41.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Extensions_4.1.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:41.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Extensions_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:41.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Handles_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:41.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Handles_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:41.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.InteropServices.RuntimeInformation_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:42.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.InteropServices.WindowsRuntime_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:41.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.InteropServices.WindowsRuntime_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:41.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.InteropServices_4.1.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:41.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.InteropServices_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:42.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Numerics_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:42.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Numerics_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:42.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Serialization.Json_4.0.3.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:42.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Serialization.Primitives_4.1.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:43.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Serialization.Primitives_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:43.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Serialization.Xml_4.1.2.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:43.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Serialization.Xml_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:44.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.WindowsRuntime.UI.Xaml_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:43.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.WindowsRuntime_4.0.11.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:43.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.WindowsRuntime_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:40.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime_4.1.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:40.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime_4.3.0.txt
--rw-rw-rw-   0        0        0     1116 2024-05-06 14:34:44.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.AccessControl_4.5.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:44.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Claims_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:44.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Algorithms_4.2.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:44.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Algorithms_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:45.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Cng_4.2.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:44.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Cng_4.3.0.txt
--rw-rw-rw-   0        0        0     1116 2024-05-06 14:34:45.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Cng_4.4.0.txt
--rw-rw-rw-   0        0        0     1116 2024-05-06 14:34:45.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Cng_4.5.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:45.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Csp_4.0.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:45.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Csp_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:45.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Encoding_4.0.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:45.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Encoding_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:45.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.OpenSsl_4.0.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:45.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.OpenSsl_4.3.0.txt
--rw-rw-rw-   0        0        0     1116 2024-05-06 14:34:45.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Pkcs_4.5.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:46.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Primitives_4.0.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:45.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Primitives_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:46.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.X509Certificates_4.1.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:46.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.X509Certificates_4.3.0.txt
--rw-rw-rw-   0        0        0     1116 2024-05-06 14:34:46.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Xml_4.5.0.txt
--rw-rw-rw-   0        0        0     1116 2024-05-06 14:34:46.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Permissions_4.5.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:46.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Principal.Windows_4.3.0.txt
--rw-rw-rw-   0        0        0     1116 2024-05-06 14:34:46.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Principal.Windows_4.5.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:46.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Principal_4.3.0.txt
--rw-rw-rw-   0        0        0     2442 2024-05-06 14:34:46.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.ServiceModel.Duplex_4.6.0.html
--rw-rw-rw-   0        0        0     2442 2024-05-06 14:34:47.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.ServiceModel.Http_4.6.0.html
--rw-rw-rw-   0        0        0     2442 2024-05-06 14:34:47.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.ServiceModel.NetTcp_4.6.0.html
--rw-rw-rw-   0        0        0     1116 2024-05-06 14:34:47.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.ServiceModel.Primitives_4.5.3.txt
--rw-rw-rw-   0        0        0     2442 2024-05-06 14:34:47.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.ServiceModel.Primitives_4.6.0.html
--rw-rw-rw-   0        0        0     2442 2024-05-06 14:34:47.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.ServiceModel.Security_4.6.0.html
--rw-rw-rw-   0        0        0     1116 2024-05-06 14:34:48.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Text.Encoding.CodePages_4.5.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:48.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Text.Encoding.Extensions_4.0.11.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:48.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Text.Encoding.Extensions_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:48.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Text.Encoding_4.0.11.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:47.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Text.Encoding_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:48.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Text.RegularExpressions_4.1.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:48.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Text.RegularExpressions_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:48.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.Overlapped_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:49.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.Tasks.Extensions_4.0.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:49.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.Tasks.Extensions_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:49.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.Tasks_4.0.11.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:49.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.Tasks_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:49.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.ThreadPool_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:49.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.Thread_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:49.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.Timer_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:48.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading_4.0.11.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:48.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:49.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Xml.ReaderWriter_4.0.11.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:49.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Xml.ReaderWriter_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:50.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Xml.XDocument_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:50.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Xml.XmlDocument_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:50.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Xml.XmlDocument_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:50.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Xml.XmlSerializer_4.0.11.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:50.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Xml.XmlSerializer_4.3.0.txt
-drwxrwxrwx   0        0        0        0 2024-05-06 14:40:56.698568 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/
--rw-rw-rw-   0        0        0  2875392 2024-02-20 15:44:28.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/BoxedAppSDK.Managed.dll
--rw-rw-rw-   0        0        0    44032 2023-12-08 17:10:46.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/MQTTnet.Extensions.ManagedClient.dll
--rw-rw-rw-   0        0        0   329728 2023-12-08 17:10:22.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/MQTTnet.dll
--rw-rw-rw-   0        0        0    22144 2021-10-22 23:42:08.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Bcl.AsyncInterfaces.dll
--rw-rw-rw-   0        0        0    27264 2021-10-22 23:47:34.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Caching.Abstractions.dll
--rw-rw-rw-   0        0        0    38000 2021-10-22 23:53:04.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Caching.Memory.dll
--rw-rw-rw-   0        0        0    25200 2021-10-22 23:47:32.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.Abstractions.dll
--rw-rw-rw-   0        0        0    34432 2021-10-22 23:47:42.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.Binder.dll
--rw-rw-rw-   0        0        0    23152 2021-10-22 23:51:02.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.CommandLine.dll
--rw-rw-rw-   0        0        0    18560 2021-10-22 23:51:12.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.EnvironmentVariables.dll
--rw-rw-rw-   0        0        0    26224 2021-10-22 23:49:04.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.FileExtensions.dll
--rw-rw-rw-   0        0        0    25728 2021-10-22 23:49:20.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.Json.dll
--rw-rw-rw-   0        0        0    24688 2021-10-22 23:49:30.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.UserSecrets.dll
--rw-rw-rw-   0        0        0    36464 2021-10-22 23:47:44.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.dll
--rw-rw-rw-   0        0        0    47216 2021-10-22 23:48:04.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.DependencyInjection.Abstractions.dll
--rw-rw-rw-   0        0        0    84608 2021-10-22 23:48:22.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.DependencyInjection.dll
--rw-rw-rw-   0        0        0    21120 2021-10-22 23:47:34.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.FileProviders.Abstractions.dll
--rw-rw-rw-   0        0        0    42608 2021-10-22 23:48:22.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.FileProviders.Physical.dll
--rw-rw-rw-   0        0        0    44160 2021-10-22 23:48:18.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.FileSystemGlobbing.dll
--rw-rw-rw-   0        0        0    28288 2021-10-22 23:48:12.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Hosting.Abstractions.dll
--rw-rw-rw-   0        0        0    57984 2021-10-22 23:52:42.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Hosting.dll
--rw-rw-rw-   0        0        0    64112 2021-10-22 23:51:24.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Logging.Abstractions.dll
--rw-rw-rw-   0        0        0    26736 2021-10-22 23:52:36.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Logging.Configuration.dll
--rw-rw-rw-   0        0        0    54384 2021-10-22 23:52:40.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Logging.Console.dll
--rw-rw-rw-   0        0        0    18032 2021-10-22 23:52:36.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Logging.Debug.dll
--rw-rw-rw-   0        0        0    24176 2021-10-22 23:52:30.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Logging.EventLog.dll
--rw-rw-rw-   0        0        0    34928 2021-10-22 23:52:38.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Logging.EventSource.dll
--rw-rw-rw-   0        0        0    44656 2021-10-22 23:52:28.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Logging.dll
--rw-rw-rw-   0        0        0    22640 2021-10-22 23:48:22.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Options.ConfigurationExtensions.dll
--rw-rw-rw-   0        0        0    58480 2021-10-22 23:48:14.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Options.dll
--rw-rw-rw-   0        0        0    43120 2021-10-22 23:47:28.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Primitives.dll
--rw-rw-rw-   0        0        0    26496 2020-10-19 18:37:20.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Win32.Registry.dll
--rw-rw-rw-   0        0        0    57856 2024-05-06 14:20:50.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/OpcLabs.MqttNet.dll
--rw-rw-rw-   0        0        0    20856 2020-02-19 10:05:18.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Buffers.dll
--rw-rw-rw-   0        0        0    28264 2021-10-22 23:52:04.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.CodeDom.dll
--rw-rw-rw-   0        0        0    43152 2018-05-15 13:29:36.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.ComponentModel.Annotations.dll
--rw-rw-rw-   0        0        0    86120 2021-10-22 23:49:30.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Configuration.ConfigurationManager.dll
--rw-rw-rw-   0        0        0   166512 2021-10-22 23:41:28.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Diagnostics.DiagnosticSource.dll
--rw-rw-rw-   0        0        0    31848 2021-10-22 23:51:28.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Diagnostics.EventLog.dll
--rw-rw-rw-   0        0        0   141184 2020-02-19 10:05:18.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Memory.dll
--rw-rw-rw-   0        0        0   115856 2018-05-15 13:29:44.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Numerics.Vectors.dll
--rw-rw-rw-   0        0        0  1470416 2020-11-10 16:22:52.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Reactive.dll
--rw-rw-rw-   0        0        0    18024 2021-10-22 23:40:18.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Runtime.CompilerServices.Unsafe.dll
--rw-rw-rw-   0        0        0    35952 2021-10-22 23:45:08.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Security.AccessControl.dll
--rw-rw-rw-   0        0        0    27752 2021-10-22 23:48:12.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Security.Permissions.dll
--rw-rw-rw-   0        0        0    18312 2020-10-19 18:46:28.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Security.Principal.Windows.dll
--rw-rw-rw-   0        0        0    21096 2019-11-15 17:31:12.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.ServiceModel.Primitives.dll
--rw-rw-rw-   0        0        0    76904 2021-10-22 23:41:14.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Text.Encodings.Web.dll
--rw-rw-rw-   0        0        0   513128 2021-10-22 23:44:26.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Text.Json.dll
--rw-rw-rw-   0        0        0    25984 2020-02-19 10:05:18.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Threading.Tasks.Extensions.dll
--rw-rw-rw-   0        0        0    25232 2018-05-15 13:29:52.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.ValueTuple.dll
-drwxrwxrwx   0        0        0        0 2024-05-06 14:40:57.151687 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/
--rw-rw-rw-   0        0        0  2875392 2024-02-20 15:44:28.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/BoxedAppSDK.Managed.dll
--rw-rw-rw-   0        0        0    44544 2023-12-08 17:10:44.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/MQTTnet.Extensions.ManagedClient.dll
--rw-rw-rw-   0        0        0   332288 2023-12-08 17:10:16.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/MQTTnet.dll
--rw-rw-rw-   0        0        0    27264 2021-10-22 23:47:46.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Caching.Abstractions.dll
--rw-rw-rw-   0        0        0    38016 2021-10-22 23:50:16.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Caching.Memory.dll
--rw-rw-rw-   0        0        0    25216 2021-10-22 23:47:50.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.Abstractions.dll
--rw-rw-rw-   0        0        0    33920 2021-10-22 23:49:54.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.Binder.dll
--rw-rw-rw-   0        0        0    23152 2021-10-22 23:50:44.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.CommandLine.dll
--rw-rw-rw-   0        0        0    18560 2021-10-22 23:50:12.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.EnvironmentVariables.dll
--rw-rw-rw-   0        0        0    26224 2021-10-22 23:50:06.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.FileExtensions.dll
--rw-rw-rw-   0        0        0    25728 2021-10-22 23:50:12.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.Json.dll
--rw-rw-rw-   0        0        0    24688 2021-10-22 23:50:16.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.UserSecrets.dll
--rw-rw-rw-   0        0        0    36464 2021-10-22 23:49:58.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.dll
--rw-rw-rw-   0        0        0    43632 2021-10-22 23:48:34.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.DependencyInjection.Abstractions.dll
--rw-rw-rw-   0        0        0    81536 2021-10-22 23:49:56.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.DependencyInjection.dll
--rw-rw-rw-   0        0        0    21120 2021-10-22 23:51:18.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.FileProviders.Abstractions.dll
--rw-rw-rw-   0        0        0    42624 2021-10-22 23:51:52.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.FileProviders.Physical.dll
--rw-rw-rw-   0        0        0    44160 2021-10-22 23:47:32.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.FileSystemGlobbing.dll
--rw-rw-rw-   0        0        0    27776 2021-10-22 23:50:04.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Hosting.Abstractions.dll
--rw-rw-rw-   0        0        0    55424 2021-10-22 23:53:18.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Hosting.dll
--rw-rw-rw-   0        0        0    62064 2021-10-22 23:51:20.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Logging.Abstractions.dll
--rw-rw-rw-   0        0        0    26736 2021-10-22 23:50:46.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Logging.Configuration.dll
--rw-rw-rw-   0        0        0    50304 2021-10-22 23:53:16.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Logging.Console.dll
--rw-rw-rw-   0        0        0    18048 2021-10-22 23:50:10.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Logging.Debug.dll
--rw-rw-rw-   0        0        0    24192 2021-10-22 23:50:12.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Logging.EventLog.dll
--rw-rw-rw-   0        0        0    32896 2021-10-22 23:53:08.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Logging.EventSource.dll
--rw-rw-rw-   0        0        0    44656 2021-10-22 23:50:34.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Logging.dll
--rw-rw-rw-   0        0        0    22656 2021-10-22 23:50:42.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Options.ConfigurationExtensions.dll
--rw-rw-rw-   0        0        0    59008 2021-10-22 23:50:00.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Options.dll
--rw-rw-rw-   0        0        0    40048 2021-10-22 23:51:10.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Primitives.dll
--rw-rw-rw-   0        0        0    26224 2021-10-22 23:40:24.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Win32.SystemEvents.dll
--rw-rw-rw-   0        0        0    58880 2024-05-06 14:23:03.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/OpcLabs.MqttNet.dll
--rw-rw-rw-   0        0        0   184944 2021-10-22 23:47:46.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.CodeDom.dll
--rw-rw-rw-   0        0        0   395376 2021-10-22 23:51:46.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Configuration.ConfigurationManager.dll
--rw-rw-rw-   0        0        0    51328 2021-10-22 23:50:48.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Diagnostics.EventLog.dll
--rw-rw-rw-   0        0        0   175216 2021-10-22 23:49:12.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Drawing.Common.dll
--rw-rw-rw-   0        0        0  2318920 2019-11-15 17:31:08.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Private.ServiceModel.dll
--rw-rw-rw-   0        0        0  1455056 2020-11-10 16:22:52.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Reactive.dll
--rw-rw-rw-   0        0        0   186504 2018-05-15 13:29:54.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Security.Cryptography.Pkcs.dll
--rw-rw-rw-   0        0        0    20592 2021-10-22 23:51:04.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Security.Cryptography.ProtectedData.dll
--rw-rw-rw-   0        0        0   167568 2018-05-15 13:29:44.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Security.Cryptography.Xml.dll
--rw-rw-rw-   0        0        0   104048 2021-10-22 23:49:50.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Security.Permissions.dll
--rw-rw-rw-   0        0        0    21576 2019-11-15 17:31:24.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.ServiceModel.Primitives.dll
--rw-rw-rw-   0        0        0    23624 2019-11-15 17:31:16.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.ServiceModel.dll
--rw-rw-rw-   0        0        0    25712 2021-10-22 23:49:44.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Windows.Extensions.dll
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:26.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.IO.Compression_4.1.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:25.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.IO.Compression_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:27.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.Net.Http_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:26.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.Net.Http_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:27.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.Net.Security_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:27.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.Security.Cryptography.Apple_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:27.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.Security.Cryptography.OpenSsl_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:27.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.Security.Cryptography.OpenSsl_4.3.2.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:27.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.Security.Cryptography_4.0.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:25.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System_4.0.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:25.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System_4.3.0.txt
--rw-rw-rw-   0        0        0    11228 2024-05-06 14:34:27.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.win10-arm.Microsoft.Net.UWPCoreRuntimeSdk_2.2.10.txt
--rw-rw-rw-   0        0        0    11228 2024-05-06 14:34:27.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.win10-x64.Microsoft.Net.UWPCoreRuntimeSdk_2.2.10.txt
--rw-rw-rw-   0        0        0    11228 2024-05-06 14:34:27.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.win10-x86.Microsoft.Net.UWPCoreRuntimeSdk_2.2.10.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:27.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.win7.System.Private.Uri_4.3.0.txt
--rw-rw-rw-   0        0        0      932 2024-02-20 15:46:20.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 14:40:57.151687 opclabs_mqttnet-5.80.191/opclabs_mqttnet.egg-info/
--rw-rw-rw-   0        0        0    18761 2024-05-06 14:40:55.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    22252 2024-05-06 14:40:56.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 14:40:55.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-06 14:40:55.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       17 2024-05-06 14:40:55.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-06 14:40:55.000000 opclabs_mqttnet-5.80.191/opclabs_mqttnet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 14:40:57.151687 opclabs_mqttnet-5.80.191/setup.cfg
--rw-rw-rw-   0        0        0     1247 2024-05-06 13:42:15.000000 opclabs_mqttnet-5.80.191/setup.py
+drwxrwxrwx   0        0        0        0 2024-02-16 19:21:03.967215 opclabs_mqttnet-5.80.75/
+-rw-rw-rw-   0        0        0      168 2023-11-14 16:14:16.000000 opclabs_mqttnet-5.80.75/MANIFEST.in
+-rw-rw-rw-   0        0        0    18760 2024-02-16 19:21:03.967215 opclabs_mqttnet-5.80.75/PKG-INFO
+-rw-rw-rw-   0        0        0      726 2023-11-14 16:14:16.000000 opclabs_mqttnet-5.80.75/README.md
+drwxrwxrwx   0        0        0        0 2024-02-16 19:21:03.545434 opclabs_mqttnet-5.80.75/opclabs_mqttnet/
+drwxrwxrwx   0        0        0        0 2024-02-16 19:21:03.826590 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/
+-rw-rw-rw-   0        0        0     2442 2024-02-16 19:17:25.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/MQTTnet.Extensions.ManagedClient_4.3.3.952.html
+-rw-rw-rw-   0        0        0     2442 2024-02-16 19:17:24.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/MQTTnet_4.3.3.952.html
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:22.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Platforms_1.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:22.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Platforms_1.1.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:22.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Platforms_1.1.1.txt
+-rw-rw-rw-   0        0        0     1116 2024-02-16 19:17:23.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Platforms_2.0.0.txt
+-rw-rw-rw-   0        0        0     1116 2024-02-16 19:17:23.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Platforms_2.1.0.txt
+-rw-rw-rw-   0        0        0     1116 2024-02-16 19:17:23.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Platforms_2.1.2.txt
+-rw-rw-rw-   0        0        0     9323 2024-02-16 19:17:23.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Portable.Compatibility_1.0.2.txt
+-rw-rw-rw-   0        0        0     9211 2024-02-16 19:17:23.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Runtime.CoreCLR_1.0.2.txt
+-rw-rw-rw-   0        0        0     9211 2024-02-16 19:17:23.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Runtime.CoreCLR_1.0.3.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:23.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Targets_1.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:23.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Targets_1.1.0.txt
+-rw-rw-rw-   0        0        0    11228 2024-02-16 19:17:23.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.UniversalWindowsPlatform_6.2.10.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:22.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore_5.0.2.txt
+-rw-rw-rw-   0        0        0    11228 2024-02-16 19:17:21.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.Net.Native.Compiler_1.7.6.txt
+-rw-rw-rw-   0        0        0    11228 2024-02-16 19:17:21.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.Net.Native.Compiler_2.2.8-rel-28605-00.txt
+-rw-rw-rw-   0        0        0    11228 2024-02-16 19:17:21.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.Net.UWPCoreRuntimeSdk_2.2.10.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:24.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.Win32.Primitives_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:24.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.Win32.Primitives_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:25.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/NETStandard.Library_1.6.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:28.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.AppContext_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:28.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Buffers_4.3.0.txt
+-rw-rw-rw-   0        0        0     1116 2024-02-16 19:17:28.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Buffers_4.4.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:29.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections.Concurrent_4.0.12.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:28.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections.Concurrent_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:29.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections.Immutable_1.2.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:29.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections.NonGeneric_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:29.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections.NonGeneric_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:29.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections.Specialized_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:29.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections.Specialized_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:28.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections_4.0.11.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:28.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:29.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.ComponentModel.EventBasedAsync_4.0.11.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:29.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.ComponentModel.EventBasedAsync_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:30.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Console_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:30.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Data.Common_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:30.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.Contracts_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:30.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.Debug_4.0.11.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:30.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.Debug_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:30.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.DiagnosticSource_4.0.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:30.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.DiagnosticSource_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:30.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.StackTrace_4.0.2.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:31.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.Tools_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:31.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.Tracing_4.1.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:31.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.Tracing_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:31.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Globalization.Calendars_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:31.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Globalization.Calendars_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:32.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Globalization.Extensions_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:31.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Globalization.Extensions_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:31.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Globalization_4.0.11.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:31.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Globalization_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:32.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.Compression.ZipFile_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:32.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.Compression_4.1.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:32.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.Compression_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:33.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.FileSystem.Primitives_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:33.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.FileSystem.Primitives_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:33.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.FileSystem_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:32.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.FileSystem_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:33.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.IsolatedStorage_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:32.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.IO_4.1.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:32.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.IO_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:33.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Linq.Expressions_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:33.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Linq.Queryable_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:33.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Linq_4.1.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:33.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Linq_4.3.0.txt
+-rw-rw-rw-   0        0        0     1116 2024-02-16 19:17:33.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Memory_4.5.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:34.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Http.Rtc_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:34.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Http_4.1.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:34.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Http_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:34.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Http_4.3.4.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:34.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.NameResolution_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:34.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Primitives_4.0.11.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:34.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Primitives_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:34.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Requests_4.0.11.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:35.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Requests_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:35.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Security_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:35.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Security_4.3.2.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:35.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Sockets_4.1.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:35.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Sockets_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:35.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.WebHeaderCollection_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:35.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.WebSockets.Client_4.3.2.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:35.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.WebSockets_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:36.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Numerics.Vectors.WindowsRuntime_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:36.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Numerics.Vectors_4.3.0.txt
+-rw-rw-rw-   0        0        0     1116 2024-02-16 19:17:36.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Numerics.Vectors_4.4.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:36.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.ObjectModel_4.0.12.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:36.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.ObjectModel_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:36.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Private.DataContractSerialization_4.1.2.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:36.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Private.DataContractSerialization_4.3.0.txt
+-rw-rw-rw-   0        0        0     1116 2024-02-16 19:17:36.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Private.ServiceModel_4.5.3.txt
+-rw-rw-rw-   0        0        0     2442 2024-02-16 19:17:37.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Private.ServiceModel_4.6.0.html
+-rw-rw-rw-   0        0        0     2442 2024-02-16 19:17:37.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Context_7.0.0.html
+-rw-rw-rw-   0        0        0     1116 2024-02-16 19:17:37.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.DispatchProxy_4.5.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:38.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Emit.ILGeneration_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:37.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Emit.ILGeneration_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:38.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Emit.Lightweight_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:38.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Emit.Lightweight_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:37.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Emit_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:37.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Emit_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:38.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Extensions_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:38.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Extensions_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:38.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Metadata_1.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:38.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Primitives_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:38.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Primitives_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:39.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.TypeExtensions_4.1.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:39.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.TypeExtensions_4.3.0.txt
+-rw-rw-rw-   0        0        0     1116 2024-02-16 19:17:39.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.TypeExtensions_4.4.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:37.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection_4.1.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:37.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:39.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Resources.ResourceManager_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:39.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Resources.ResourceManager_4.3.0.txt
+-rw-rw-rw-   0        0        0     1116 2024-02-16 19:17:39.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.CompilerServices.Unsafe_4.5.0.txt
+-rw-rw-rw-   0        0        0     1116 2024-02-16 19:17:39.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.CompilerServices.Unsafe_4.5.2.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:40.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Extensions_4.1.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:39.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Extensions_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:40.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Handles_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:40.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Handles_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:40.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.InteropServices.RuntimeInformation_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:40.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.InteropServices.WindowsRuntime_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:40.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.InteropServices.WindowsRuntime_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:40.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.InteropServices_4.1.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:40.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.InteropServices_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:41.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Numerics_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:41.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Numerics_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:41.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Serialization.Json_4.0.3.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:41.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Serialization.Primitives_4.1.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:41.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Serialization.Primitives_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:41.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Serialization.Xml_4.1.2.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:41.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Serialization.Xml_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:42.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.WindowsRuntime.UI.Xaml_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:42.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.WindowsRuntime_4.0.11.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:41.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.WindowsRuntime_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:39.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime_4.1.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:39.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime_4.3.0.txt
+-rw-rw-rw-   0        0        0     1116 2024-02-16 19:17:42.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.AccessControl_4.5.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:42.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Claims_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:42.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Algorithms_4.2.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:42.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Algorithms_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:42.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Cng_4.2.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:42.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Cng_4.3.0.txt
+-rw-rw-rw-   0        0        0     1116 2024-02-16 19:17:42.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Cng_4.4.0.txt
+-rw-rw-rw-   0        0        0     1116 2024-02-16 19:17:42.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Cng_4.5.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:43.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Csp_4.0.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:42.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Csp_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:43.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Encoding_4.0.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:43.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Encoding_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:43.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.OpenSsl_4.0.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:43.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.OpenSsl_4.3.0.txt
+-rw-rw-rw-   0        0        0     1116 2024-02-16 19:17:43.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Pkcs_4.5.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:43.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Primitives_4.0.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:43.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Primitives_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:44.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.X509Certificates_4.1.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:43.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.X509Certificates_4.3.0.txt
+-rw-rw-rw-   0        0        0     1116 2024-02-16 19:17:44.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Xml_4.5.0.txt
+-rw-rw-rw-   0        0        0     1116 2024-02-16 19:17:44.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Permissions_4.5.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:44.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Principal.Windows_4.3.0.txt
+-rw-rw-rw-   0        0        0     1116 2024-02-16 19:17:44.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Principal.Windows_4.5.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:44.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Principal_4.3.0.txt
+-rw-rw-rw-   0        0        0     2442 2024-02-16 19:17:44.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.ServiceModel.Duplex_4.6.0.html
+-rw-rw-rw-   0        0        0     2442 2024-02-16 19:17:44.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.ServiceModel.Http_4.6.0.html
+-rw-rw-rw-   0        0        0     2442 2024-02-16 19:17:45.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.ServiceModel.NetTcp_4.6.0.html
+-rw-rw-rw-   0        0        0     1116 2024-02-16 19:17:45.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.ServiceModel.Primitives_4.5.3.txt
+-rw-rw-rw-   0        0        0     2442 2024-02-16 19:17:45.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.ServiceModel.Primitives_4.6.0.html
+-rw-rw-rw-   0        0        0     2442 2024-02-16 19:17:45.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.ServiceModel.Security_4.6.0.html
+-rw-rw-rw-   0        0        0     1116 2024-02-16 19:17:46.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Text.Encoding.CodePages_4.5.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:46.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Text.Encoding.Extensions_4.0.11.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:46.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Text.Encoding.Extensions_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:45.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Text.Encoding_4.0.11.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:45.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Text.Encoding_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:46.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Text.RegularExpressions_4.1.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:46.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Text.RegularExpressions_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:46.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.Overlapped_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:47.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.Tasks.Extensions_4.0.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:47.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.Tasks.Extensions_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:47.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.Tasks_4.0.11.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:46.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.Tasks_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:47.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.ThreadPool_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:47.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.Thread_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:47.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.Timer_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:46.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading_4.0.11.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:46.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:47.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Xml.ReaderWriter_4.0.11.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:47.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Xml.ReaderWriter_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:48.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Xml.XDocument_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:48.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Xml.XmlDocument_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:48.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Xml.XmlDocument_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:48.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Xml.XmlSerializer_4.0.11.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:48.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Xml.XmlSerializer_4.3.0.txt
+drwxrwxrwx   0        0        0        0 2024-02-16 19:21:03.904714 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/
+-rw-rw-rw-   0        0        0  2875392 2023-11-14 16:12:36.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/BoxedAppSDK.Managed.dll
+-rw-rw-rw-   0        0        0    44032 2023-12-08 17:10:46.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/MQTTnet.Extensions.ManagedClient.dll
+-rw-rw-rw-   0        0        0   329728 2023-12-08 17:10:22.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/MQTTnet.dll
+-rw-rw-rw-   0        0        0    22144 2021-10-22 23:42:08.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Bcl.AsyncInterfaces.dll
+-rw-rw-rw-   0        0        0    27264 2021-10-22 23:47:34.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Caching.Abstractions.dll
+-rw-rw-rw-   0        0        0    38000 2021-10-22 23:53:04.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Caching.Memory.dll
+-rw-rw-rw-   0        0        0    25200 2021-10-22 23:47:32.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.Abstractions.dll
+-rw-rw-rw-   0        0        0    34432 2021-10-22 23:47:42.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.Binder.dll
+-rw-rw-rw-   0        0        0    23152 2021-10-22 23:51:02.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.CommandLine.dll
+-rw-rw-rw-   0        0        0    18560 2021-10-22 23:51:12.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.EnvironmentVariables.dll
+-rw-rw-rw-   0        0        0    26224 2021-10-22 23:49:04.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.FileExtensions.dll
+-rw-rw-rw-   0        0        0    25728 2021-10-22 23:49:20.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.Json.dll
+-rw-rw-rw-   0        0        0    24688 2021-10-22 23:49:30.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.UserSecrets.dll
+-rw-rw-rw-   0        0        0    36464 2021-10-22 23:47:44.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.dll
+-rw-rw-rw-   0        0        0    47216 2021-10-22 23:48:04.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.DependencyInjection.Abstractions.dll
+-rw-rw-rw-   0        0        0    84608 2021-10-22 23:48:22.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.DependencyInjection.dll
+-rw-rw-rw-   0        0        0    21120 2021-10-22 23:47:34.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.FileProviders.Abstractions.dll
+-rw-rw-rw-   0        0        0    42608 2021-10-22 23:48:22.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.FileProviders.Physical.dll
+-rw-rw-rw-   0        0        0    44160 2021-10-22 23:48:18.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.FileSystemGlobbing.dll
+-rw-rw-rw-   0        0        0    28288 2021-10-22 23:48:12.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Hosting.Abstractions.dll
+-rw-rw-rw-   0        0        0    57984 2021-10-22 23:52:42.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Hosting.dll
+-rw-rw-rw-   0        0        0    64112 2021-10-22 23:51:24.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Logging.Abstractions.dll
+-rw-rw-rw-   0        0        0    26736 2021-10-22 23:52:36.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Logging.Configuration.dll
+-rw-rw-rw-   0        0        0    54384 2021-10-22 23:52:40.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Logging.Console.dll
+-rw-rw-rw-   0        0        0    18032 2021-10-22 23:52:36.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Logging.Debug.dll
+-rw-rw-rw-   0        0        0    24176 2021-10-22 23:52:30.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Logging.EventLog.dll
+-rw-rw-rw-   0        0        0    34928 2021-10-22 23:52:38.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Logging.EventSource.dll
+-rw-rw-rw-   0        0        0    44656 2021-10-22 23:52:28.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Logging.dll
+-rw-rw-rw-   0        0        0    22640 2021-10-22 23:48:22.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Options.ConfigurationExtensions.dll
+-rw-rw-rw-   0        0        0    58480 2021-10-22 23:48:14.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Options.dll
+-rw-rw-rw-   0        0        0    43120 2021-10-22 23:47:28.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Primitives.dll
+-rw-rw-rw-   0        0        0    26496 2020-10-19 18:37:20.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Win32.Registry.dll
+-rw-rw-rw-   0        0        0    57856 2024-02-16 19:06:50.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/OpcLabs.MqttNet.dll
+-rw-rw-rw-   0        0        0    20856 2020-02-19 10:05:18.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Buffers.dll
+-rw-rw-rw-   0        0        0    28264 2021-10-22 23:52:04.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.CodeDom.dll
+-rw-rw-rw-   0        0        0    43152 2018-05-15 13:29:36.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.ComponentModel.Annotations.dll
+-rw-rw-rw-   0        0        0    86120 2021-10-22 23:49:30.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Configuration.ConfigurationManager.dll
+-rw-rw-rw-   0        0        0   166512 2021-10-22 23:41:28.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Diagnostics.DiagnosticSource.dll
+-rw-rw-rw-   0        0        0    31848 2021-10-22 23:51:28.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Diagnostics.EventLog.dll
+-rw-rw-rw-   0        0        0   141184 2020-02-19 10:05:18.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Memory.dll
+-rw-rw-rw-   0        0        0   115856 2018-05-15 13:29:44.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Numerics.Vectors.dll
+-rw-rw-rw-   0        0        0  1470416 2020-11-10 16:22:52.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Reactive.dll
+-rw-rw-rw-   0        0        0    18024 2021-10-22 23:40:18.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Runtime.CompilerServices.Unsafe.dll
+-rw-rw-rw-   0        0        0    35952 2021-10-22 23:45:08.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Security.AccessControl.dll
+-rw-rw-rw-   0        0        0    27752 2021-10-22 23:48:12.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Security.Permissions.dll
+-rw-rw-rw-   0        0        0    18312 2020-10-19 18:46:28.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Security.Principal.Windows.dll
+-rw-rw-rw-   0        0        0    21096 2019-11-15 17:31:12.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.ServiceModel.Primitives.dll
+-rw-rw-rw-   0        0        0    76904 2021-10-22 23:41:14.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Text.Encodings.Web.dll
+-rw-rw-rw-   0        0        0   513128 2021-10-22 23:44:26.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Text.Json.dll
+-rw-rw-rw-   0        0        0    25984 2020-02-19 10:05:18.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Threading.Tasks.Extensions.dll
+-rw-rw-rw-   0        0        0    25232 2018-05-15 13:29:52.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.ValueTuple.dll
+drwxrwxrwx   0        0        0        0 2024-02-16 19:21:03.967215 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/
+-rw-rw-rw-   0        0        0  2875392 2023-11-14 16:12:36.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/BoxedAppSDK.Managed.dll
+-rw-rw-rw-   0        0        0    44544 2023-12-08 17:10:44.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/MQTTnet.Extensions.ManagedClient.dll
+-rw-rw-rw-   0        0        0   332288 2023-12-08 17:10:16.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/MQTTnet.dll
+-rw-rw-rw-   0        0        0    27264 2021-10-22 23:47:46.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Caching.Abstractions.dll
+-rw-rw-rw-   0        0        0    38016 2021-10-22 23:50:16.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Caching.Memory.dll
+-rw-rw-rw-   0        0        0    25216 2021-10-22 23:47:50.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.Abstractions.dll
+-rw-rw-rw-   0        0        0    33920 2021-10-22 23:49:54.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.Binder.dll
+-rw-rw-rw-   0        0        0    23152 2021-10-22 23:50:44.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.CommandLine.dll
+-rw-rw-rw-   0        0        0    18560 2021-10-22 23:50:12.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.EnvironmentVariables.dll
+-rw-rw-rw-   0        0        0    26224 2021-10-22 23:50:06.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.FileExtensions.dll
+-rw-rw-rw-   0        0        0    25728 2021-10-22 23:50:12.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.Json.dll
+-rw-rw-rw-   0        0        0    24688 2021-10-22 23:50:16.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.UserSecrets.dll
+-rw-rw-rw-   0        0        0    36464 2021-10-22 23:49:58.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.dll
+-rw-rw-rw-   0        0        0    43632 2021-10-22 23:48:34.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.DependencyInjection.Abstractions.dll
+-rw-rw-rw-   0        0        0    81536 2021-10-22 23:49:56.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.DependencyInjection.dll
+-rw-rw-rw-   0        0        0    21120 2021-10-22 23:51:18.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.FileProviders.Abstractions.dll
+-rw-rw-rw-   0        0        0    42624 2021-10-22 23:51:52.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.FileProviders.Physical.dll
+-rw-rw-rw-   0        0        0    44160 2021-10-22 23:47:32.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.FileSystemGlobbing.dll
+-rw-rw-rw-   0        0        0    27776 2021-10-22 23:50:04.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Hosting.Abstractions.dll
+-rw-rw-rw-   0        0        0    55424 2021-10-22 23:53:18.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Hosting.dll
+-rw-rw-rw-   0        0        0    62064 2021-10-22 23:51:20.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Logging.Abstractions.dll
+-rw-rw-rw-   0        0        0    26736 2021-10-22 23:50:46.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Logging.Configuration.dll
+-rw-rw-rw-   0        0        0    50304 2021-10-22 23:53:16.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Logging.Console.dll
+-rw-rw-rw-   0        0        0    18048 2021-10-22 23:50:10.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Logging.Debug.dll
+-rw-rw-rw-   0        0        0    24192 2021-10-22 23:50:12.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Logging.EventLog.dll
+-rw-rw-rw-   0        0        0    32896 2021-10-22 23:53:08.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Logging.EventSource.dll
+-rw-rw-rw-   0        0        0    44656 2021-10-22 23:50:34.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Logging.dll
+-rw-rw-rw-   0        0        0    22656 2021-10-22 23:50:42.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Options.ConfigurationExtensions.dll
+-rw-rw-rw-   0        0        0    59008 2021-10-22 23:50:00.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Options.dll
+-rw-rw-rw-   0        0        0    40048 2021-10-22 23:51:10.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Primitives.dll
+-rw-rw-rw-   0        0        0    26224 2021-10-22 23:40:24.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Win32.SystemEvents.dll
+-rw-rw-rw-   0        0        0    58880 2024-02-16 19:08:49.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/OpcLabs.MqttNet.dll
+-rw-rw-rw-   0        0        0   184944 2021-10-22 23:47:46.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.CodeDom.dll
+-rw-rw-rw-   0        0        0   395376 2021-10-22 23:51:46.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Configuration.ConfigurationManager.dll
+-rw-rw-rw-   0        0        0    51328 2021-10-22 23:50:48.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Diagnostics.EventLog.dll
+-rw-rw-rw-   0        0        0   175216 2021-10-22 23:49:12.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Drawing.Common.dll
+-rw-rw-rw-   0        0        0  2318920 2019-11-15 17:31:08.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Private.ServiceModel.dll
+-rw-rw-rw-   0        0        0  1455056 2020-11-10 16:22:52.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Reactive.dll
+-rw-rw-rw-   0        0        0   186504 2018-05-15 13:29:54.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Security.Cryptography.Pkcs.dll
+-rw-rw-rw-   0        0        0    20592 2021-10-22 23:51:04.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Security.Cryptography.ProtectedData.dll
+-rw-rw-rw-   0        0        0   167568 2018-05-15 13:29:44.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Security.Cryptography.Xml.dll
+-rw-rw-rw-   0        0        0   104048 2021-10-22 23:49:50.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Security.Permissions.dll
+-rw-rw-rw-   0        0        0    21576 2019-11-15 17:31:24.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.ServiceModel.Primitives.dll
+-rw-rw-rw-   0        0        0    23624 2019-11-15 17:31:16.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.ServiceModel.dll
+-rw-rw-rw-   0        0        0    25712 2021-10-22 23:49:44.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Windows.Extensions.dll
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:26.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.IO.Compression_4.1.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:26.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.IO.Compression_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:26.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.Net.Http_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:26.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.Net.Http_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:26.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.Net.Security_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:27.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.Security.Cryptography.Apple_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:27.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.Security.Cryptography.OpenSsl_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:27.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.Security.Cryptography.OpenSsl_4.3.2.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:27.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.Security.Cryptography_4.0.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:26.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System_4.0.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:26.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System_4.3.0.txt
+-rw-rw-rw-   0        0        0    11228 2024-02-16 19:17:27.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.win10-arm.Microsoft.Net.UWPCoreRuntimeSdk_2.2.10.txt
+-rw-rw-rw-   0        0        0    11228 2024-02-16 19:17:27.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.win10-x64.Microsoft.Net.UWPCoreRuntimeSdk_2.2.10.txt
+-rw-rw-rw-   0        0        0    11228 2024-02-16 19:17:27.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.win10-x86.Microsoft.Net.UWPCoreRuntimeSdk_2.2.10.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:27.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.win7.System.Private.Uri_4.3.0.txt
+-rw-rw-rw-   0        0        0      932 2023-11-14 16:14:16.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-16 19:21:03.967215 opclabs_mqttnet-5.80.75/opclabs_mqttnet.egg-info/
+-rw-rw-rw-   0        0        0    18760 2024-02-16 19:21:03.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    22252 2024-02-16 19:21:03.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-16 19:21:03.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-02-16 19:21:02.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       17 2024-02-16 19:21:03.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-02-16 19:21:03.000000 opclabs_mqttnet-5.80.75/opclabs_mqttnet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-02-16 19:21:03.967215 opclabs_mqttnet-5.80.75/setup.cfg
+-rw-rw-rw-   0        0        0     1246 2024-02-16 18:57:43.000000 opclabs_mqttnet-5.80.75/setup.py
```

### Comparing `opclabs_mqttnet-5.80.191/PKG-INFO` & `opclabs_mqttnet-5.80.75/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opclabs_mqttnet
-Version: 5.80.191
+Version: 5.80.75
 Summary: MQTT communication package based on MQTTnet and MQTTnet.Extensions.ManagedClient libraries by Christian Kratky.
 Home-page: https://kb.opclabs.com/OpcLabs.MqttNet_communication_package?python
 Author: CODE Consulting and Development, s.r.o.
 Author-email: sales09@opclabs.com
 Keywords: QuickOPC,OPC,UA,PubSub,MQTT
 Description-Content-Type: text/markdown
 License-File: opclabs_mqttnet\OpcLabs.MqttNet\MQTTnet.Extensions.ManagedClient_4.3.3.952.html
```

### Comparing `opclabs_mqttnet-5.80.191/README.md` & `opclabs_mqttnet-5.80.75/README.md`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/MQTTnet.Extensions.ManagedClient_4.3.3.952.html` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/MQTTnet.Extensions.ManagedClient_4.3.3.952.html`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/MQTTnet_4.3.3.952.html` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/MQTTnet_4.3.3.952.html`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Platforms_1.0.1.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Platforms_1.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Platforms_1.1.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Platforms_1.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Platforms_1.1.1.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Platforms_1.1.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Platforms_2.0.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Platforms_2.0.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Platforms_2.1.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Platforms_2.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Platforms_2.1.2.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Platforms_2.1.2.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Portable.Compatibility_1.0.2.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Portable.Compatibility_1.0.2.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Runtime.CoreCLR_1.0.2.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Runtime.CoreCLR_1.0.2.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Runtime.CoreCLR_1.0.3.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Runtime.CoreCLR_1.0.3.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Targets_1.0.1.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Targets_1.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Targets_1.1.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.Targets_1.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.UniversalWindowsPlatform_6.2.10.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore.UniversalWindowsPlatform_6.2.10.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore_5.0.2.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.NETCore_5.0.2.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.Net.Native.Compiler_1.7.6.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.Net.Native.Compiler_1.7.6.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.Net.Native.Compiler_2.2.8-rel-28605-00.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.Net.Native.Compiler_2.2.8-rel-28605-00.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.Net.UWPCoreRuntimeSdk_2.2.10.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.Net.UWPCoreRuntimeSdk_2.2.10.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.Win32.Primitives_4.0.1.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.Win32.Primitives_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.Win32.Primitives_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/Microsoft.Win32.Primitives_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/NETStandard.Library_1.6.1.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/NETStandard.Library_1.6.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.AppContext_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.AppContext_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Buffers_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Buffers_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Buffers_4.4.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Buffers_4.4.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections.Concurrent_4.0.12.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections.Concurrent_4.0.12.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections.Concurrent_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections.Concurrent_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections.Immutable_1.2.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections.Immutable_1.2.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections.NonGeneric_4.0.1.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections.NonGeneric_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections.NonGeneric_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections.NonGeneric_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections.Specialized_4.0.1.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections.Specialized_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections.Specialized_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections.Specialized_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections_4.0.11.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections_4.0.11.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Collections_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.ComponentModel.EventBasedAsync_4.0.11.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.ComponentModel.EventBasedAsync_4.0.11.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.ComponentModel.EventBasedAsync_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.ComponentModel.EventBasedAsync_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Console_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Console_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Data.Common_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Data.Common_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.Contracts_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.Contracts_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.Debug_4.0.11.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.Debug_4.0.11.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.Debug_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.Debug_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.DiagnosticSource_4.0.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.DiagnosticSource_4.0.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.DiagnosticSource_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.DiagnosticSource_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.StackTrace_4.0.2.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.StackTrace_4.0.2.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.Tools_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.Tools_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.Tracing_4.1.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.Tracing_4.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.Tracing_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Diagnostics.Tracing_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Globalization.Calendars_4.0.1.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Globalization.Calendars_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Globalization.Calendars_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Globalization.Calendars_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Globalization.Extensions_4.0.1.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Globalization.Extensions_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Globalization.Extensions_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Globalization.Extensions_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Globalization_4.0.11.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Globalization_4.0.11.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Globalization_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Globalization_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.Compression.ZipFile_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.Compression.ZipFile_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.Compression_4.1.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.Compression_4.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.Compression_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.Compression_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.FileSystem.Primitives_4.0.1.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.FileSystem.Primitives_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.FileSystem.Primitives_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.FileSystem.Primitives_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.FileSystem_4.0.1.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.FileSystem_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.FileSystem_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.FileSystem_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.IsolatedStorage_4.0.1.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.IO.IsolatedStorage_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.IO_4.1.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.IO_4.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.IO_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.IO_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Linq.Expressions_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Linq.Expressions_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Linq.Queryable_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Linq.Queryable_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Linq_4.1.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Linq_4.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Linq_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Linq_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Memory_4.5.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Memory_4.5.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Http.Rtc_4.0.1.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Http.Rtc_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Http_4.1.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Http_4.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Http_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Http_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Http_4.3.4.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Http_4.3.4.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.NameResolution_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.NameResolution_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Primitives_4.0.11.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Primitives_4.0.11.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Primitives_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Primitives_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Requests_4.0.11.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Requests_4.0.11.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Requests_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Requests_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Security_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Security_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Security_4.3.2.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Security_4.3.2.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Sockets_4.1.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Sockets_4.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Sockets_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.Sockets_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.WebHeaderCollection_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.WebHeaderCollection_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.WebSockets.Client_4.3.2.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.WebSockets.Client_4.3.2.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.WebSockets_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Net.WebSockets_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Numerics.Vectors.WindowsRuntime_4.0.1.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Numerics.Vectors.WindowsRuntime_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Numerics.Vectors_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Numerics.Vectors_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Numerics.Vectors_4.4.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Numerics.Vectors_4.4.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.ObjectModel_4.0.12.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.ObjectModel_4.0.12.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.ObjectModel_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.ObjectModel_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Private.DataContractSerialization_4.1.2.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Private.DataContractSerialization_4.1.2.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Private.DataContractSerialization_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Private.DataContractSerialization_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Private.ServiceModel_4.5.3.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Private.ServiceModel_4.5.3.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Private.ServiceModel_4.6.0.html` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Private.ServiceModel_4.6.0.html`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Context_7.0.0.html` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Context_7.0.0.html`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.DispatchProxy_4.5.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.DispatchProxy_4.5.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Emit.ILGeneration_4.0.1.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Emit.ILGeneration_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Emit.ILGeneration_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Emit.ILGeneration_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Emit.Lightweight_4.0.1.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Emit.Lightweight_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Emit.Lightweight_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Emit.Lightweight_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Emit_4.0.1.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Emit_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Emit_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Emit_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Extensions_4.0.1.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Extensions_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Extensions_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Extensions_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Metadata_1.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Metadata_1.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Primitives_4.0.1.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Primitives_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Primitives_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.Primitives_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.TypeExtensions_4.1.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.TypeExtensions_4.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.TypeExtensions_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.TypeExtensions_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.TypeExtensions_4.4.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection.TypeExtensions_4.4.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection_4.1.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection_4.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Reflection_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Resources.ResourceManager_4.0.1.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Resources.ResourceManager_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Resources.ResourceManager_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Resources.ResourceManager_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.CompilerServices.Unsafe_4.5.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.CompilerServices.Unsafe_4.5.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.CompilerServices.Unsafe_4.5.2.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.CompilerServices.Unsafe_4.5.2.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Extensions_4.1.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Extensions_4.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Extensions_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Extensions_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Handles_4.0.1.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Handles_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Handles_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Handles_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.InteropServices.RuntimeInformation_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.InteropServices.RuntimeInformation_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.InteropServices.WindowsRuntime_4.0.1.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.InteropServices.WindowsRuntime_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.InteropServices.WindowsRuntime_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.InteropServices.WindowsRuntime_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.InteropServices_4.1.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.InteropServices_4.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.InteropServices_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.InteropServices_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Numerics_4.0.1.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Numerics_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Numerics_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Numerics_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Serialization.Json_4.0.3.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Serialization.Json_4.0.3.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Serialization.Primitives_4.1.1.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Serialization.Primitives_4.1.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Serialization.Primitives_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Serialization.Primitives_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Serialization.Xml_4.1.2.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Serialization.Xml_4.1.2.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Serialization.Xml_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.Serialization.Xml_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.WindowsRuntime.UI.Xaml_4.0.1.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.WindowsRuntime.UI.Xaml_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.WindowsRuntime_4.0.11.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.WindowsRuntime_4.0.11.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.WindowsRuntime_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime.WindowsRuntime_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime_4.1.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime_4.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Runtime_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.AccessControl_4.5.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.AccessControl_4.5.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Claims_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Claims_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Algorithms_4.2.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Algorithms_4.2.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Algorithms_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Algorithms_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Cng_4.2.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Cng_4.2.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Cng_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Cng_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Cng_4.4.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Cng_4.4.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Cng_4.5.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Cng_4.5.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Csp_4.0.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Csp_4.0.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Csp_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Csp_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Encoding_4.0.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Encoding_4.0.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Encoding_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Encoding_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.OpenSsl_4.0.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.OpenSsl_4.0.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.OpenSsl_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.OpenSsl_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Pkcs_4.5.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Pkcs_4.5.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Primitives_4.0.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Primitives_4.0.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Primitives_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Primitives_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.X509Certificates_4.1.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.X509Certificates_4.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.X509Certificates_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.X509Certificates_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Xml_4.5.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Cryptography.Xml_4.5.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Permissions_4.5.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Permissions_4.5.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Principal.Windows_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Principal.Windows_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Principal.Windows_4.5.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Principal.Windows_4.5.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Principal_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Security.Principal_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.ServiceModel.Duplex_4.6.0.html` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.ServiceModel.Duplex_4.6.0.html`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.ServiceModel.Http_4.6.0.html` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.ServiceModel.Http_4.6.0.html`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.ServiceModel.NetTcp_4.6.0.html` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.ServiceModel.NetTcp_4.6.0.html`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.ServiceModel.Primitives_4.5.3.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.ServiceModel.Primitives_4.5.3.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.ServiceModel.Primitives_4.6.0.html` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.ServiceModel.Primitives_4.6.0.html`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.ServiceModel.Security_4.6.0.html` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.ServiceModel.Security_4.6.0.html`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Text.Encoding.CodePages_4.5.1.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Text.Encoding.CodePages_4.5.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Text.Encoding.Extensions_4.0.11.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Text.Encoding.Extensions_4.0.11.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Text.Encoding.Extensions_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Text.Encoding.Extensions_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Text.Encoding_4.0.11.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Text.Encoding_4.0.11.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Text.Encoding_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Text.Encoding_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Text.RegularExpressions_4.1.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Text.RegularExpressions_4.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Text.RegularExpressions_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Text.RegularExpressions_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.Overlapped_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.Overlapped_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.Tasks.Extensions_4.0.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.Tasks.Extensions_4.0.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.Tasks.Extensions_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.Tasks.Extensions_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.Tasks_4.0.11.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.Tasks_4.0.11.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.Tasks_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.Tasks_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.ThreadPool_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.ThreadPool_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.Thread_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.Thread_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.Timer_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading.Timer_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading_4.0.11.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading_4.0.11.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Threading_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Xml.ReaderWriter_4.0.11.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Xml.ReaderWriter_4.0.11.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Xml.ReaderWriter_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Xml.ReaderWriter_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Xml.XDocument_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Xml.XDocument_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Xml.XmlDocument_4.0.1.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Xml.XmlDocument_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Xml.XmlDocument_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Xml.XmlDocument_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Xml.XmlSerializer_4.0.11.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Xml.XmlSerializer_4.0.11.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/System.Xml.XmlSerializer_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/System.Xml.XmlSerializer_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/BoxedAppSDK.Managed.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/BoxedAppSDK.Managed.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/MQTTnet.Extensions.ManagedClient.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/MQTTnet.Extensions.ManagedClient.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/MQTTnet.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/MQTTnet.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Bcl.AsyncInterfaces.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Bcl.AsyncInterfaces.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Caching.Abstractions.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Caching.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Caching.Memory.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Caching.Memory.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.Abstractions.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.Binder.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.Binder.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.CommandLine.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.CommandLine.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.EnvironmentVariables.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.EnvironmentVariables.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.FileExtensions.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.FileExtensions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.Json.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.Json.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.UserSecrets.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.UserSecrets.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Configuration.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.DependencyInjection.Abstractions.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.DependencyInjection.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.DependencyInjection.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.DependencyInjection.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.FileProviders.Abstractions.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.FileProviders.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.FileProviders.Physical.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.FileProviders.Physical.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.FileSystemGlobbing.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.FileSystemGlobbing.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Hosting.Abstractions.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Hosting.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Hosting.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Hosting.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Logging.Abstractions.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Logging.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Logging.Configuration.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Logging.Configuration.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Logging.Console.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Logging.Console.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Logging.Debug.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Logging.Debug.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Logging.EventLog.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Logging.EventLog.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Logging.EventSource.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Logging.EventSource.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Logging.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Logging.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Options.ConfigurationExtensions.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Options.ConfigurationExtensions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Options.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Options.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Primitives.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Extensions.Primitives.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Win32.Registry.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/Microsoft.Win32.Registry.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/OpcLabs.MqttNet.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/OpcLabs.MqttNet.dll`

 * *Files 5% similar despite different names*

#### pedump {}

```diff
@@ -1,25 +1,25 @@
 
 COFF Header:
 	                Machine: 0x014c
 	               Sections: 0x0003
-	             Time stamp: 0xa0bdcdaf
+	             Time stamp: 0x8367ba46
 	Pointer to Symbol Table: 0x00000000
 	   	   Symbol Count: 0x00000000
 	   Optional Header Size: 0x00e0
 	   	Characteristics: 0x2022
 
 PE Header:
 	         Magic (0x010b): 0x010b
 	             LMajor (6): 0x30
 	             LMinor (0): 0x00
 	              Code Size: 0x0000d800
 	  Initialized Data Size: 0x00000800
 	Uninitialized Data Size: 0x00000000
-	        Entry Point RVA: 0x0000f642
+	        Entry Point RVA: 0x0000f63e
 	 	  Code Base RVA: 0x00002000
 		  Data Base RVA: 0x00010000
 
 
 NT Header:
 	   Image Base (0x400000): 0x10000000
 	Section Alignment (8192): 0x00002000
@@ -29,54 +29,54 @@
 	  	  User Major (0): 0x0000
 	  	  User Minor (0): 0x0000
 	  	Subsys major (4): 0x0006
 	  	Subsys minor (0): 0x0000
 	 	       Reserverd: 0x00000000
 	 	      Image Size: 0x00014000
 	 	     Header Size: 0x00000200
-	            Checksum (0): 0x0001a868
+	            Checksum (0): 0x00012dfa
 	               Subsystem: 0x0003
 	           DLL Flags (0): 0x8560
 	 Stack Reserve Size (1M): 0x00100000
 	Stack commit Size (4096): 0x00001000
 	  Heap Reserve Size (1M): 0x00100000
 	 Heap Commit Size (4096): 0x00001000
 	      Loader flags (0x1): 0x00000000
 	   Data Directories (16): 0x00000010
 
 Data directories:
 	     Export Table: 0x00000000 [0x00000000]
-	     Import Table: 0x0000f5ee [0x0000004f]
-	   Resource Table: 0x00010000 [0x000004e4]
+	     Import Table: 0x0000f5ea [0x0000004f]
+	   Resource Table: 0x00010000 [0x000004d8]
 	  Exception Table: 0x00000000 [0x00000000]
 	Certificate Table: 0x00000000 [0x00000000]
 	      Reloc Table: 0x00012000 [0x0000000c]
-	            Debug: 0x0000f4f0 [0x00000054]
+	            Debug: 0x0000f4ec [0x00000054]
 	        Copyright: 0x00000000 [0x00000000]
 	       Global Ptr: 0x00000000 [0x00000000]
 	        TLS Table: 0x00000000 [0x00000000]
 	Load Config Table: 0x00000000 [0x00000000]
 	     Bound Import: 0x00000000 [0x00000000]
 	              IAT: 0x00002000 [0x00000008]
 	Delay Import Desc: 0x00000000 [0x00000000]
 	       CLI Header: 0x00002008 [0x00000048]
 
 	Name: .text
-	   Virtual Size: 0x0000d648
+	   Virtual Size: 0x0000d644
 	Virtual Address: 0x00002000
 	  Raw Data Size: 0x0000d800
 	   Raw Data Ptr: 0x00000200
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: code, exec, read, 
 
 	Name: .rsrc
-	   Virtual Size: 0x000004e4
+	   Virtual Size: 0x000004d8
 	Virtual Address: 0x00010000
 	  Raw Data Size: 0x00000600
 	   Raw Data Ptr: 0x0000da00
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
@@ -92,31 +92,31 @@
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, discard, read, 
 
           CLI header size: 72
          Runtime required: 2.5
                     Flags: ilonly, 32/64, no-trackdebug, strongnamesigned
-	         Metadata: 0x0000554c [0x00009ac4]
+	         Metadata: 0x0000554c [0x00009ac0]
 	Entry Point Token: 0x00000000
-	     Resources at: 0x0000f010 [0x00000460]
-	   Strong Name at: 0x0000f470 [0x00000080]
+	     Resources at: 0x0000f00c [0x00000460]
+	   Strong Name at: 0x0000f46c [0x00000080]
 	  Code Manager at: 0x00000000 [0x00000000]
 	  VTableFixups at: 0x00000000 [0x00000000]
 	     EAT jumps at: 0x00000000 [0x00000000]
 
 Strong name:
-	 4D 02 52 BC 46 C5 53 43 91 19 44 1F F0 44 7F 03
-	 03 41 AF 7C 43 2F C5 86 51 C8 54 96 58 44 B0 8D
-	 69 DE DB DB F2 7D F1 20 C6 DD 41 31 4A 40 F2 22
-	 4F 74 3C 6E BF 08 E1 9E 8F 05 E9 29 99 58 70 C5
-	 FD 8D FD C9 7E A5 DA 6F B3 05 22 43 B5 9E 7D 64
-	 4A BB 75 17 E0 B4 C7 F5 E7 6C 3B C9 4B CB 32 DE
-	 C0 92 F2 80 B1 F0 1B 14 35 B5 9E 10 D7 51 43 0D
-	 3F 3F DD 9F 88 31 01 0E 5B 7B EF 98 1C 77 0E 9C
+	 9C E2 B5 28 CE 0C 9D 2D B3 5F DF 04 E4 F6 50 D8
+	 A7 70 AD C5 2B 42 9C A5 45 38 35 F6 44 7F 1D 7A
+	 6A 99 2B 97 EF 58 B7 17 0A D0 FF 81 69 BA A4 CD
+	 EF 5D A3 2B 5B BF 4F CC 4F 19 32 99 49 9E DA 79
+	 7B 60 10 63 B5 D6 A6 BE 23 24 FA 19 CA 6C C9 D9
+	 73 3F 1F EB D1 72 DA AD F5 A2 50 B6 39 E8 6B 3F
+	 A6 F6 80 22 0F FB A0 01 4F CA 8B C7 44 8E 1A B9
+	 DC A0 A5 F1 64 CA CC 1C 1C E0 A1 E9 20 26 64 A9
 
 Public key:
 	 00 24 00 00 04 80 00 00 94 00 00 00 06 02 00 00
 	 00 24 00 00 52 53 41 31 00 04 00 00 01 00 01 00
 	 4B 6B 21 84 98 FE 12 E8 25 F6 A1 B4 94 A5 99 C6
 	 3C AD E3 6A 13 D7 9C 98 38 E6 C9 EA DA 3B D6 3E
 	 4E B3 15 85 CB 44 6B 9F 7A A1 FA F8 29 F5 AC 92
@@ -129,15 +129,15 @@
 Metadata header:
            Version: 1.1
     Version string: v4.0.30319
 
 Metadata pointers:
 	Tables (#~): 0x0000006c - 0x00003024 [12216 == 0x00002fb8]
 	    Strings: 0x00003024 - 0x00006bc8 [15268 == 0x00003ba4]
-	       Blob: 0x00008240 - 0x00009ac4 [6276 == 0x00001884]
+	       Blob: 0x00008240 - 0x00009ac0 [6272 == 0x00001880]
 	User string: 0x00006bc8 - 0x00008230 [5736 == 0x00001668]
 	       GUID: 0x00008230 - 0x00008240 [16 == 0x00000010]
 Rows:
 Table Module: 1 records (10 bytes, at 3824)
 Table TypeRef: 188 records (6 bytes, at 382e)
 Table TypeDef: 57 records (14 bytes, at 3c96)
 Table Field: 134 records (6 bytes, at 3fb4)
```

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Buffers.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Buffers.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.CodeDom.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.CodeDom.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.ComponentModel.Annotations.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.ComponentModel.Annotations.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Configuration.ConfigurationManager.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Configuration.ConfigurationManager.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Diagnostics.DiagnosticSource.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Diagnostics.DiagnosticSource.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Diagnostics.EventLog.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Diagnostics.EventLog.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Memory.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Memory.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Numerics.Vectors.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Numerics.Vectors.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Reactive.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Reactive.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Runtime.CompilerServices.Unsafe.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Runtime.CompilerServices.Unsafe.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Security.AccessControl.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Security.AccessControl.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Security.Permissions.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Security.Permissions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Security.Principal.Windows.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Security.Principal.Windows.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.ServiceModel.Primitives.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.ServiceModel.Primitives.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Text.Encodings.Web.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Text.Encodings.Web.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Text.Json.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Text.Json.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Threading.Tasks.Extensions.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.Threading.Tasks.Extensions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.ValueTuple.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net472/System.ValueTuple.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/BoxedAppSDK.Managed.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/BoxedAppSDK.Managed.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/MQTTnet.Extensions.ManagedClient.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/MQTTnet.Extensions.ManagedClient.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/MQTTnet.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/MQTTnet.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Caching.Abstractions.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Caching.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Caching.Memory.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Caching.Memory.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.Abstractions.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.Binder.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.Binder.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.CommandLine.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.CommandLine.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.EnvironmentVariables.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.EnvironmentVariables.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.FileExtensions.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.FileExtensions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.Json.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.Json.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.UserSecrets.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.UserSecrets.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Configuration.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.DependencyInjection.Abstractions.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.DependencyInjection.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.DependencyInjection.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.DependencyInjection.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.FileProviders.Abstractions.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.FileProviders.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.FileProviders.Physical.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.FileProviders.Physical.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.FileSystemGlobbing.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.FileSystemGlobbing.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Hosting.Abstractions.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Hosting.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Hosting.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Hosting.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Logging.Abstractions.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Logging.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Logging.Configuration.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Logging.Configuration.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Logging.Console.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Logging.Console.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Logging.Debug.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Logging.Debug.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Logging.EventLog.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Logging.EventLog.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Logging.EventSource.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Logging.EventSource.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Logging.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Logging.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Options.ConfigurationExtensions.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Options.ConfigurationExtensions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Options.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Options.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Primitives.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Extensions.Primitives.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Win32.SystemEvents.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/Microsoft.Win32.SystemEvents.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/OpcLabs.MqttNet.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/OpcLabs.MqttNet.dll`

 * *Files 5% similar despite different names*

#### pedump {}

```diff
@@ -1,25 +1,25 @@
 
 COFF Header:
 	                Machine: 0x014c
 	               Sections: 0x0003
-	             Time stamp: 0xd89ffbd8
+	             Time stamp: 0x9ee38606
 	Pointer to Symbol Table: 0x00000000
 	   	   Symbol Count: 0x00000000
 	   Optional Header Size: 0x00e0
 	   	Characteristics: 0x2022
 
 PE Header:
 	         Magic (0x010b): 0x010b
 	             LMajor (6): 0x30
 	             LMinor (0): 0x00
 	              Code Size: 0x0000dc00
 	  Initialized Data Size: 0x00000800
 	Uninitialized Data Size: 0x00000000
-	        Entry Point RVA: 0x0000faca
+	        Entry Point RVA: 0x0000fac6
 	 	  Code Base RVA: 0x00002000
 		  Data Base RVA: 0x00010000
 
 
 NT Header:
 	   Image Base (0x400000): 0x10000000
 	Section Alignment (8192): 0x00002000
@@ -29,54 +29,54 @@
 	  	  User Major (0): 0x0000
 	  	  User Minor (0): 0x0000
 	  	Subsys major (4): 0x0004
 	  	Subsys minor (0): 0x0000
 	 	       Reserverd: 0x00000000
 	 	      Image Size: 0x00014000
 	 	     Header Size: 0x00000200
-	            Checksum (0): 0x000173f3
+	            Checksum (0): 0x0001791e
 	               Subsystem: 0x0003
 	           DLL Flags (0): 0x8560
 	 Stack Reserve Size (1M): 0x00100000
 	Stack commit Size (4096): 0x00001000
 	  Heap Reserve Size (1M): 0x00100000
 	 Heap Commit Size (4096): 0x00001000
 	      Loader flags (0x1): 0x00000000
 	   Data Directories (16): 0x00000010
 
 Data directories:
 	     Export Table: 0x00000000 [0x00000000]
-	     Import Table: 0x0000fa76 [0x0000004f]
-	   Resource Table: 0x00010000 [0x000004e4]
+	     Import Table: 0x0000fa72 [0x0000004f]
+	   Resource Table: 0x00010000 [0x000004d8]
 	  Exception Table: 0x00000000 [0x00000000]
 	Certificate Table: 0x00000000 [0x00000000]
 	      Reloc Table: 0x00012000 [0x0000000c]
-	            Debug: 0x0000f978 [0x00000054]
+	            Debug: 0x0000f974 [0x00000054]
 	        Copyright: 0x00000000 [0x00000000]
 	       Global Ptr: 0x00000000 [0x00000000]
 	        TLS Table: 0x00000000 [0x00000000]
 	Load Config Table: 0x00000000 [0x00000000]
 	     Bound Import: 0x00000000 [0x00000000]
 	              IAT: 0x00002000 [0x00000008]
 	Delay Import Desc: 0x00000000 [0x00000000]
 	       CLI Header: 0x00002008 [0x00000048]
 
 	Name: .text
-	   Virtual Size: 0x0000dad0
+	   Virtual Size: 0x0000dacc
 	Virtual Address: 0x00002000
 	  Raw Data Size: 0x0000dc00
 	   Raw Data Ptr: 0x00000200
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: code, exec, read, 
 
 	Name: .rsrc
-	   Virtual Size: 0x000004e4
+	   Virtual Size: 0x000004d8
 	Virtual Address: 0x00010000
 	  Raw Data Size: 0x00000600
 	   Raw Data Ptr: 0x0000de00
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
@@ -92,31 +92,31 @@
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, discard, read, 
 
           CLI header size: 72
          Runtime required: 2.5
                     Flags: ilonly, 32/64, no-trackdebug, strongnamesigned
-	         Metadata: 0x00005678 [0x00009e20]
+	         Metadata: 0x00005678 [0x00009e1c]
 	Entry Point Token: 0x00000000
-	     Resources at: 0x0000f498 [0x00000460]
-	   Strong Name at: 0x0000f8f8 [0x00000080]
+	     Resources at: 0x0000f494 [0x00000460]
+	   Strong Name at: 0x0000f8f4 [0x00000080]
 	  Code Manager at: 0x00000000 [0x00000000]
 	  VTableFixups at: 0x00000000 [0x00000000]
 	     EAT jumps at: 0x00000000 [0x00000000]
 
 Strong name:
-	 6A E0 39 80 EC 4F 07 BD 11 95 42 06 5A B6 4C 95
-	 03 79 50 53 2C 6F 73 92 D6 44 60 6F CC 0C 71 BB
-	 1F 89 D8 91 EC E9 EF A6 08 6E 1A 89 D5 13 D2 2D
-	 37 5F 16 BB 0F 82 37 F2 A7 B6 CD 3C 49 BA B5 85
-	 5B B1 78 01 C0 8D F5 5E E4 9E C1 06 7C F2 25 7F
-	 E2 8D 9F B1 9B A9 55 19 44 35 7A 30 CA F7 C0 76
-	 5A 6A F0 78 8D 82 86 F4 B1 2D AC BB 16 14 BA 27
-	 0F AA 92 D4 E8 F0 A7 B0 66 F6 A0 03 2F A0 DB 3B
+	 9D DB 61 71 DF FF F9 F5 AF F2 DF 46 F1 5C DC A3
+	 54 F3 EC 4D 5B BB C0 1D F0 EC 5B A3 14 4B 8B FF
+	 4B 45 C8 F9 06 5E 91 43 9E 79 02 26 7D 91 31 5B
+	 36 EB 9D 93 90 F1 67 A1 3E 2D E4 D0 9C 66 A1 3D
+	 58 52 7B 9B 70 87 0E 59 B6 D5 91 D7 F7 B8 91 0D
+	 7F 9A 07 9A 74 38 C9 B4 17 A9 24 62 81 EE EF 55
+	 55 02 A4 FF 2C EC CF 9D 35 D7 F5 E2 B7 87 C6 DC
+	 CC BB 3F 82 A2 65 F6 3E 2A 5A EB 3F C9 1E 46 B1
 
 Public key:
 	 00 24 00 00 04 80 00 00 94 00 00 00 06 02 00 00
 	 00 24 00 00 52 53 41 31 00 04 00 00 01 00 01 00
 	 4B 6B 21 84 98 FE 12 E8 25 F6 A1 B4 94 A5 99 C6
 	 3C AD E3 6A 13 D7 9C 98 38 E6 C9 EA DA 3B D6 3E
 	 4E B3 15 85 CB 44 6B 9F 7A A1 FA F8 29 F5 AC 92
@@ -129,15 +129,15 @@
 Metadata header:
            Version: 1.1
     Version string: v4.0.30319
 
 Metadata pointers:
 	Tables (#~): 0x0000006c - 0x0000320c [12704 == 0x000031a0]
 	    Strings: 0x0000320c - 0x00006eb0 [15524 == 0x00003ca4]
-	       Blob: 0x00008504 - 0x00009e20 [6428 == 0x0000191c]
+	       Blob: 0x00008504 - 0x00009e1c [6424 == 0x00001918]
 	User string: 0x00006eb0 - 0x000084f4 [5700 == 0x00001644]
 	       GUID: 0x000084f4 - 0x00008504 [16 == 0x00000010]
 Rows:
 Table Module: 1 records (10 bytes, at 3950)
 Table TypeRef: 192 records (6 bytes, at 395a)
 Table TypeDef: 59 records (14 bytes, at 3dda)
 Table Field: 135 records (6 bytes, at 4114)
```

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.CodeDom.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.CodeDom.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Configuration.ConfigurationManager.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Configuration.ConfigurationManager.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Diagnostics.EventLog.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Diagnostics.EventLog.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Drawing.Common.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Drawing.Common.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Private.ServiceModel.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Private.ServiceModel.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Reactive.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Reactive.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Security.Cryptography.Pkcs.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Security.Cryptography.Pkcs.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Security.Cryptography.ProtectedData.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Security.Cryptography.ProtectedData.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Security.Cryptography.Xml.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Security.Cryptography.Xml.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Security.Permissions.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Security.Permissions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.ServiceModel.Primitives.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.ServiceModel.Primitives.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.ServiceModel.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.ServiceModel.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Windows.Extensions.dll` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/net6.0/System.Windows.Extensions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.IO.Compression_4.1.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.IO.Compression_4.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.IO.Compression_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.IO.Compression_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.Net.Http_4.0.1.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.Net.Http_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.Net.Http_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.Net.Http_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.Net.Security_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.Net.Security_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.Security.Cryptography.Apple_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.Security.Cryptography.Apple_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.Security.Cryptography.OpenSsl_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.Security.Cryptography.OpenSsl_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.Security.Cryptography.OpenSsl_4.3.2.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.Security.Cryptography.OpenSsl_4.3.2.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.Security.Cryptography_4.0.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System.Security.Cryptography_4.0.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System_4.0.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System_4.0.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.native.System_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.win10-arm.Microsoft.Net.UWPCoreRuntimeSdk_2.2.10.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.win10-arm.Microsoft.Net.UWPCoreRuntimeSdk_2.2.10.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.win10-x64.Microsoft.Net.UWPCoreRuntimeSdk_2.2.10.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.win10-x64.Microsoft.Net.UWPCoreRuntimeSdk_2.2.10.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.win10-x86.Microsoft.Net.UWPCoreRuntimeSdk_2.2.10.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.win10-x86.Microsoft.Net.UWPCoreRuntimeSdk_2.2.10.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/OpcLabs.MqttNet/runtime.win7.System.Private.Uri_4.3.0.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/OpcLabs.MqttNet/runtime.win7.System.Private.Uri_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet/__init__.py` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet/__init__.py`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet.egg-info/PKG-INFO` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opclabs_mqttnet
-Version: 5.80.191
+Version: 5.80.75
 Summary: MQTT communication package based on MQTTnet and MQTTnet.Extensions.ManagedClient libraries by Christian Kratky.
 Home-page: https://kb.opclabs.com/OpcLabs.MqttNet_communication_package?python
 Author: CODE Consulting and Development, s.r.o.
 Author-email: sales09@opclabs.com
 Keywords: QuickOPC,OPC,UA,PubSub,MQTT
 Description-Content-Type: text/markdown
 License-File: opclabs_mqttnet\OpcLabs.MqttNet\MQTTnet.Extensions.ManagedClient_4.3.3.952.html
```

### Comparing `opclabs_mqttnet-5.80.191/opclabs_mqttnet.egg-info/SOURCES.txt` & `opclabs_mqttnet-5.80.75/opclabs_mqttnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqttnet-5.80.191/setup.py` & `opclabs_mqttnet-5.80.75/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-version='5.80.191'
+version='5.80.75'
 from setuptools import setup
 
 # Read the contents of the README file.
 from pathlib import Path
 this_directory = Path(__file__).parent
 readme_path = this_directory / "README.md"
 # WindowsPath.read_txt() does not work in IronPython (3.4.1).
```

