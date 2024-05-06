# Comparing `tmp/opclabs_mqtt-5.80.191.tar.gz` & `tmp/opclabs_mqtt-5.80.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opclabs_mqtt-5.80.191.tar", last modified: Mon May  6 14:40:10 2024, max compression
+gzip compressed data, was "opclabs_mqtt-5.80.75.tar", last modified: Fri Feb 16 19:20:43 2024, max compression
```

## Comparing `opclabs_mqtt-5.80.191.tar` & `opclabs_mqtt-5.80.75.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 14:40:10.979385 opclabs_mqtt-5.80.191/
--rw-rw-rw-   0        0        0      169 2024-02-20 15:46:20.000000 opclabs_mqtt-5.80.191/MANIFEST.in
--rw-rw-rw-   0        0        0     4851 2024-05-06 14:40:10.979385 opclabs_mqtt-5.80.191/PKG-INFO
--rw-rw-rw-   0        0        0      660 2024-02-20 15:46:16.000000 opclabs_mqtt-5.80.191/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 14:40:10.338742 opclabs_mqtt-5.80.191/opclabs_mqtt/
-drwxrwxrwx   0        0        0        0 2024-05-06 14:40:10.494995 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:33:55.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/Microsoft.NETCore.Platforms_1.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:33:55.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/Microsoft.NETCore.Platforms_1.1.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:33:56.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/Microsoft.NETCore.Targets_1.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:33:56.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/Microsoft.NETCore.Targets_1.1.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:33:56.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Collections.Concurrent_4.0.12.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:33:56.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Collections_4.0.11.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:33:56.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.ComponentModel_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:33:56.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Diagnostics.Contracts_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:33:56.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Diagnostics.Debug_4.0.11.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:33:57.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Diagnostics.Tools_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:33:57.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Diagnostics.TraceSource_4.0.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:33:57.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Diagnostics.Tracing_4.1.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:33:58.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Dynamic.Runtime_4.0.11.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:33:58.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Globalization_4.0.11.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:33:58.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.IO_4.1.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:33:58.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Linq.Expressions_4.1.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:33:58.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Linq_4.1.0.txt
--rw-rw-rw-   0        0        0     1079 2024-05-06 14:33:58.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Net.Mqtt_0.6.0-beta.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:33:59.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.ObjectModel_4.0.12.txt
--rw-rw-rw-   0        0        0     1116 2024-05-06 14:34:00.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Reactive.Core_3.0.0.txt
--rw-rw-rw-   0        0        0     1116 2024-05-06 14:34:01.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Reactive.Interfaces_3.0.0.txt
--rw-rw-rw-   0        0        0     1116 2024-05-06 14:34:01.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Reactive.Linq_3.0.0.txt
--rw-rw-rw-   0        0        0     1116 2024-05-06 14:34:01.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Reactive.PlatformServices_3.0.0.txt
--rw-rw-rw-   0        0        0     1116 2024-05-06 14:34:01.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Reactive.Windows.Threading_3.0.0.txt
--rw-rw-rw-   0        0        0     1116 2024-05-06 14:34:01.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Reactive.WindowsRuntime_3.0.0.txt
--rw-rw-rw-   0        0        0     1116 2024-05-06 14:34:00.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Reactive_3.0.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:01.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Reflection.Emit.ILGeneration_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:01.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Reflection.Emit.Lightweight_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:01.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Reflection.Emit_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:01.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Reflection.Extensions_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:02.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Reflection.Primitives_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:02.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Reflection.TypeExtensions_4.1.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:01.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Reflection_4.1.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:02.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Resources.ResourceManager_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:02.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime.Extensions_4.1.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:02.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime.Handles_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:03.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime.InteropServices.WindowsRuntime_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:02.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime.InteropServices_4.1.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:03.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime.Serialization.Primitives_4.1.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:03.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime.WindowsRuntime_4.0.11.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:02.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime_4.1.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:02.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime_4.3.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:03.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Text.Encoding_4.0.11.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:04.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Threading.Tasks_4.0.11.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:04.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Threading.ThreadPool_4.0.10.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:04.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Threading.Thread_4.0.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:04.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Threading.Timer_4.0.1.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:03.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Threading_4.0.11.txt
-drwxrwxrwx   0        0        0        0 2024-05-06 14:40:10.760623 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/
--rw-rw-rw-   0        0        0  2875392 2024-02-20 15:44:28.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/BoxedAppSDK.Managed.dll
--rw-rw-rw-   0        0        0    22144 2021-10-22 23:42:08.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Bcl.AsyncInterfaces.dll
--rw-rw-rw-   0        0        0    27264 2021-10-22 23:47:34.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Caching.Abstractions.dll
--rw-rw-rw-   0        0        0    38000 2021-10-22 23:53:04.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Caching.Memory.dll
--rw-rw-rw-   0        0        0    25200 2021-10-22 23:47:32.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.Abstractions.dll
--rw-rw-rw-   0        0        0    34432 2021-10-22 23:47:42.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.Binder.dll
--rw-rw-rw-   0        0        0    23152 2021-10-22 23:51:02.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.CommandLine.dll
--rw-rw-rw-   0        0        0    18560 2021-10-22 23:51:12.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.EnvironmentVariables.dll
--rw-rw-rw-   0        0        0    26224 2021-10-22 23:49:04.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.FileExtensions.dll
--rw-rw-rw-   0        0        0    25728 2021-10-22 23:49:20.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.Json.dll
--rw-rw-rw-   0        0        0    24688 2021-10-22 23:49:30.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.UserSecrets.dll
--rw-rw-rw-   0        0        0    36464 2021-10-22 23:47:44.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.dll
--rw-rw-rw-   0        0        0    47216 2021-10-22 23:48:04.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.DependencyInjection.Abstractions.dll
--rw-rw-rw-   0        0        0    84608 2021-10-22 23:48:22.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.DependencyInjection.dll
--rw-rw-rw-   0        0        0    21120 2021-10-22 23:47:34.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.FileProviders.Abstractions.dll
--rw-rw-rw-   0        0        0    42608 2021-10-22 23:48:22.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.FileProviders.Physical.dll
--rw-rw-rw-   0        0        0    44160 2021-10-22 23:48:18.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.FileSystemGlobbing.dll
--rw-rw-rw-   0        0        0    28288 2021-10-22 23:48:12.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Hosting.Abstractions.dll
--rw-rw-rw-   0        0        0    57984 2021-10-22 23:52:42.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Hosting.dll
--rw-rw-rw-   0        0        0    64112 2021-10-22 23:51:24.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Logging.Abstractions.dll
--rw-rw-rw-   0        0        0    26736 2021-10-22 23:52:36.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Logging.Configuration.dll
--rw-rw-rw-   0        0        0    54384 2021-10-22 23:52:40.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Logging.Console.dll
--rw-rw-rw-   0        0        0    18032 2021-10-22 23:52:36.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Logging.Debug.dll
--rw-rw-rw-   0        0        0    24176 2021-10-22 23:52:30.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Logging.EventLog.dll
--rw-rw-rw-   0        0        0    34928 2021-10-22 23:52:38.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Logging.EventSource.dll
--rw-rw-rw-   0        0        0    44656 2021-10-22 23:52:28.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Logging.dll
--rw-rw-rw-   0        0        0    22640 2021-10-22 23:48:22.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Options.ConfigurationExtensions.dll
--rw-rw-rw-   0        0        0    58480 2021-10-22 23:48:14.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Options.dll
--rw-rw-rw-   0        0        0    43120 2021-10-22 23:47:28.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Primitives.dll
--rw-rw-rw-   0        0        0    26496 2020-10-19 18:37:20.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Win32.Registry.dll
--rw-rw-rw-   0        0        0    30720 2024-05-06 14:21:32.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/OpcLabs.Mqtt.dll
--rw-rw-rw-   0        0        0    20856 2020-02-19 10:05:18.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Buffers.dll
--rw-rw-rw-   0        0        0    28264 2021-10-22 23:52:04.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.CodeDom.dll
--rw-rw-rw-   0        0        0    43152 2018-05-15 13:29:36.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.ComponentModel.Annotations.dll
--rw-rw-rw-   0        0        0    86120 2021-10-22 23:49:30.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Configuration.ConfigurationManager.dll
--rw-rw-rw-   0        0        0   166512 2021-10-22 23:41:28.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Diagnostics.DiagnosticSource.dll
--rw-rw-rw-   0        0        0    31848 2021-10-22 23:51:28.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Diagnostics.EventLog.dll
--rw-rw-rw-   0        0        0    19456 2017-03-14 18:20:06.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Diagnostics.Tracer.dll
--rw-rw-rw-   0        0        0   141184 2020-02-19 10:05:18.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Memory.dll
--rw-rw-rw-   0        0        0   142200 2019-07-31 14:15:22.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Net.Mqtt.dll
--rw-rw-rw-   0        0        0   115856 2018-05-15 13:29:44.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Numerics.Vectors.dll
--rw-rw-rw-   0        0        0  1470416 2020-11-10 16:22:52.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Reactive.dll
--rw-rw-rw-   0        0        0    18024 2021-10-22 23:40:18.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Runtime.CompilerServices.Unsafe.dll
--rw-rw-rw-   0        0        0    35952 2021-10-22 23:45:08.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Security.AccessControl.dll
--rw-rw-rw-   0        0        0    27752 2021-10-22 23:48:12.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Security.Permissions.dll
--rw-rw-rw-   0        0        0    18312 2020-10-19 18:46:28.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Security.Principal.Windows.dll
--rw-rw-rw-   0        0        0    21096 2019-11-15 17:31:12.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.ServiceModel.Primitives.dll
--rw-rw-rw-   0        0        0    76904 2021-10-22 23:41:14.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Text.Encodings.Web.dll
--rw-rw-rw-   0        0        0   513128 2021-10-22 23:44:26.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Text.Json.dll
--rw-rw-rw-   0        0        0    25984 2020-02-19 10:05:18.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Threading.Tasks.Extensions.dll
--rw-rw-rw-   0        0        0    25232 2018-05-15 13:29:52.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.ValueTuple.dll
-drwxrwxrwx   0        0        0        0 2024-05-06 14:40:10.948122 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/
--rw-rw-rw-   0        0        0  2875392 2024-02-20 15:44:28.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/BoxedAppSDK.Managed.dll
--rw-rw-rw-   0        0        0    27264 2021-10-22 23:47:46.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Caching.Abstractions.dll
--rw-rw-rw-   0        0        0    38016 2021-10-22 23:50:16.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Caching.Memory.dll
--rw-rw-rw-   0        0        0    25216 2021-10-22 23:47:50.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.Abstractions.dll
--rw-rw-rw-   0        0        0    33920 2021-10-22 23:49:54.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.Binder.dll
--rw-rw-rw-   0        0        0    23152 2021-10-22 23:50:44.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.CommandLine.dll
--rw-rw-rw-   0        0        0    18560 2021-10-22 23:50:12.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.EnvironmentVariables.dll
--rw-rw-rw-   0        0        0    26224 2021-10-22 23:50:06.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.FileExtensions.dll
--rw-rw-rw-   0        0        0    25728 2021-10-22 23:50:12.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.Json.dll
--rw-rw-rw-   0        0        0    24688 2021-10-22 23:50:16.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.UserSecrets.dll
--rw-rw-rw-   0        0        0    36464 2021-10-22 23:49:58.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.dll
--rw-rw-rw-   0        0        0    43632 2021-10-22 23:48:34.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.DependencyInjection.Abstractions.dll
--rw-rw-rw-   0        0        0    81536 2021-10-22 23:49:56.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.DependencyInjection.dll
--rw-rw-rw-   0        0        0    21120 2021-10-22 23:51:18.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.FileProviders.Abstractions.dll
--rw-rw-rw-   0        0        0    42624 2021-10-22 23:51:52.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.FileProviders.Physical.dll
--rw-rw-rw-   0        0        0    44160 2021-10-22 23:47:32.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.FileSystemGlobbing.dll
--rw-rw-rw-   0        0        0    27776 2021-10-22 23:50:04.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Hosting.Abstractions.dll
--rw-rw-rw-   0        0        0    55424 2021-10-22 23:53:18.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Hosting.dll
--rw-rw-rw-   0        0        0    62064 2021-10-22 23:51:20.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Logging.Abstractions.dll
--rw-rw-rw-   0        0        0    26736 2021-10-22 23:50:46.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Logging.Configuration.dll
--rw-rw-rw-   0        0        0    50304 2021-10-22 23:53:16.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Logging.Console.dll
--rw-rw-rw-   0        0        0    18048 2021-10-22 23:50:10.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Logging.Debug.dll
--rw-rw-rw-   0        0        0    24192 2021-10-22 23:50:12.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Logging.EventLog.dll
--rw-rw-rw-   0        0        0    32896 2021-10-22 23:53:08.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Logging.EventSource.dll
--rw-rw-rw-   0        0        0    44656 2021-10-22 23:50:34.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Logging.dll
--rw-rw-rw-   0        0        0    22656 2021-10-22 23:50:42.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Options.ConfigurationExtensions.dll
--rw-rw-rw-   0        0        0    59008 2021-10-22 23:50:00.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Options.dll
--rw-rw-rw-   0        0        0    40048 2021-10-22 23:51:10.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Primitives.dll
--rw-rw-rw-   0        0        0    26224 2021-10-22 23:40:24.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Win32.SystemEvents.dll
--rw-rw-rw-   0        0        0    31232 2024-05-06 14:23:04.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/OpcLabs.Mqtt.dll
--rw-rw-rw-   0        0        0   184944 2021-10-22 23:47:46.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.CodeDom.dll
--rw-rw-rw-   0        0        0   395376 2021-10-22 23:51:46.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Configuration.ConfigurationManager.dll
--rw-rw-rw-   0        0        0    51328 2021-10-22 23:50:48.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Diagnostics.EventLog.dll
--rw-rw-rw-   0        0        0    16896 2017-03-14 18:20:06.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Diagnostics.Tracer.dll
--rw-rw-rw-   0        0        0   175216 2021-10-22 23:49:12.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Drawing.Common.dll
--rw-rw-rw-   0        0        0   142200 2019-07-31 14:15:22.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Net.Mqtt.dll
--rw-rw-rw-   0        0        0  2318920 2019-11-15 17:31:08.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Private.ServiceModel.dll
--rw-rw-rw-   0        0        0  1455056 2020-11-10 16:22:52.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Reactive.dll
--rw-rw-rw-   0        0        0   186504 2018-05-15 13:29:54.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Security.Cryptography.Pkcs.dll
--rw-rw-rw-   0        0        0    20592 2021-10-22 23:51:04.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Security.Cryptography.ProtectedData.dll
--rw-rw-rw-   0        0        0   167568 2018-05-15 13:29:44.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Security.Cryptography.Xml.dll
--rw-rw-rw-   0        0        0   104048 2021-10-22 23:49:50.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Security.Permissions.dll
--rw-rw-rw-   0        0        0    21576 2019-11-15 17:31:24.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.ServiceModel.Primitives.dll
--rw-rw-rw-   0        0        0    23624 2019-11-15 17:31:16.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.ServiceModel.dll
--rw-rw-rw-   0        0        0    25712 2021-10-22 23:49:44.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Windows.Extensions.dll
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:33:56.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/runtime.native.System_4.0.0.txt
--rw-rw-rw-   0        0        0      926 2024-02-20 15:46:20.000000 opclabs_mqtt-5.80.191/opclabs_mqtt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 14:40:10.948122 opclabs_mqtt-5.80.191/opclabs_mqtt.egg-info/
--rw-rw-rw-   0        0        0     4851 2024-05-06 14:40:10.000000 opclabs_mqtt-5.80.191/opclabs_mqtt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10166 2024-05-06 14:40:10.000000 opclabs_mqtt-5.80.191/opclabs_mqtt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 14:40:10.000000 opclabs_mqtt-5.80.191/opclabs_mqtt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-06 14:40:08.000000 opclabs_mqtt-5.80.191/opclabs_mqtt.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       17 2024-05-06 14:40:10.000000 opclabs_mqtt-5.80.191/opclabs_mqtt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-06 14:40:10.000000 opclabs_mqtt-5.80.191/opclabs_mqtt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 14:40:10.979385 opclabs_mqtt-5.80.191/setup.cfg
--rw-rw-rw-   0        0        0     1192 2024-05-06 13:42:14.000000 opclabs_mqtt-5.80.191/setup.py
+drwxrwxrwx   0        0        0        0 2024-02-16 19:20:43.873297 opclabs_mqtt-5.80.75/
+-rw-rw-rw-   0        0        0      169 2023-11-14 16:14:16.000000 opclabs_mqtt-5.80.75/MANIFEST.in
+-rw-rw-rw-   0        0        0     4850 2024-02-16 19:20:43.873297 opclabs_mqtt-5.80.75/PKG-INFO
+-rw-rw-rw-   0        0        0      660 2023-11-14 16:14:16.000000 opclabs_mqtt-5.80.75/README.md
+drwxrwxrwx   0        0        0        0 2024-02-16 19:20:43.670172 opclabs_mqtt-5.80.75/opclabs_mqtt/
+drwxrwxrwx   0        0        0        0 2024-02-16 19:20:43.732669 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:01.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/Microsoft.NETCore.Platforms_1.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:01.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/Microsoft.NETCore.Platforms_1.1.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:01.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/Microsoft.NETCore.Targets_1.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:01.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/Microsoft.NETCore.Targets_1.1.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:02.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Collections.Concurrent_4.0.12.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:02.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Collections_4.0.11.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:02.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.ComponentModel_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:02.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Diagnostics.Contracts_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:02.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Diagnostics.Debug_4.0.11.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:02.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Diagnostics.Tools_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:03.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Diagnostics.TraceSource_4.0.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:03.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Diagnostics.Tracing_4.1.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:03.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Dynamic.Runtime_4.0.11.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:03.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Globalization_4.0.11.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:04.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.IO_4.1.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:04.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Linq.Expressions_4.1.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:04.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Linq_4.1.0.txt
+-rw-rw-rw-   0        0        0     1079 2024-02-16 19:17:04.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Net.Mqtt_0.6.0-beta.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:04.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.ObjectModel_4.0.12.txt
+-rw-rw-rw-   0        0        0     1116 2024-02-16 19:17:05.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Reactive.Core_3.0.0.txt
+-rw-rw-rw-   0        0        0     1116 2024-02-16 19:17:05.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Reactive.Interfaces_3.0.0.txt
+-rw-rw-rw-   0        0        0     1116 2024-02-16 19:17:05.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Reactive.Linq_3.0.0.txt
+-rw-rw-rw-   0        0        0     1116 2024-02-16 19:17:06.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Reactive.PlatformServices_3.0.0.txt
+-rw-rw-rw-   0        0        0     1116 2024-02-16 19:17:06.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Reactive.Windows.Threading_3.0.0.txt
+-rw-rw-rw-   0        0        0     1116 2024-02-16 19:17:06.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Reactive.WindowsRuntime_3.0.0.txt
+-rw-rw-rw-   0        0        0     1116 2024-02-16 19:17:05.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Reactive_3.0.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:06.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Reflection.Emit.ILGeneration_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:06.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Reflection.Emit.Lightweight_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:06.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Reflection.Emit_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:06.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Reflection.Extensions_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:06.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Reflection.Primitives_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:07.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Reflection.TypeExtensions_4.1.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:06.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Reflection_4.1.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:07.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Resources.ResourceManager_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:07.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime.Extensions_4.1.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:07.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime.Handles_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:07.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime.InteropServices.WindowsRuntime_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:07.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime.InteropServices_4.1.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:08.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime.Serialization.Primitives_4.1.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:08.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime.WindowsRuntime_4.0.11.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:07.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime_4.1.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:07.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime_4.3.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:08.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Text.Encoding_4.0.11.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:08.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Threading.Tasks_4.0.11.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:08.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Threading.ThreadPool_4.0.10.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:08.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Threading.Thread_4.0.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:08.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Threading.Timer_4.0.1.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:08.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Threading_4.0.11.txt
+drwxrwxrwx   0        0        0        0 2024-02-16 19:20:43.810795 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/
+-rw-rw-rw-   0        0        0  2875392 2023-11-14 16:12:36.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/BoxedAppSDK.Managed.dll
+-rw-rw-rw-   0        0        0    22144 2021-10-22 23:42:08.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Bcl.AsyncInterfaces.dll
+-rw-rw-rw-   0        0        0    27264 2021-10-22 23:47:34.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Caching.Abstractions.dll
+-rw-rw-rw-   0        0        0    38000 2021-10-22 23:53:04.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Caching.Memory.dll
+-rw-rw-rw-   0        0        0    25200 2021-10-22 23:47:32.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.Abstractions.dll
+-rw-rw-rw-   0        0        0    34432 2021-10-22 23:47:42.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.Binder.dll
+-rw-rw-rw-   0        0        0    23152 2021-10-22 23:51:02.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.CommandLine.dll
+-rw-rw-rw-   0        0        0    18560 2021-10-22 23:51:12.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.EnvironmentVariables.dll
+-rw-rw-rw-   0        0        0    26224 2021-10-22 23:49:04.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.FileExtensions.dll
+-rw-rw-rw-   0        0        0    25728 2021-10-22 23:49:20.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.Json.dll
+-rw-rw-rw-   0        0        0    24688 2021-10-22 23:49:30.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.UserSecrets.dll
+-rw-rw-rw-   0        0        0    36464 2021-10-22 23:47:44.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.dll
+-rw-rw-rw-   0        0        0    47216 2021-10-22 23:48:04.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.DependencyInjection.Abstractions.dll
+-rw-rw-rw-   0        0        0    84608 2021-10-22 23:48:22.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.DependencyInjection.dll
+-rw-rw-rw-   0        0        0    21120 2021-10-22 23:47:34.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.FileProviders.Abstractions.dll
+-rw-rw-rw-   0        0        0    42608 2021-10-22 23:48:22.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.FileProviders.Physical.dll
+-rw-rw-rw-   0        0        0    44160 2021-10-22 23:48:18.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.FileSystemGlobbing.dll
+-rw-rw-rw-   0        0        0    28288 2021-10-22 23:48:12.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Hosting.Abstractions.dll
+-rw-rw-rw-   0        0        0    57984 2021-10-22 23:52:42.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Hosting.dll
+-rw-rw-rw-   0        0        0    64112 2021-10-22 23:51:24.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Logging.Abstractions.dll
+-rw-rw-rw-   0        0        0    26736 2021-10-22 23:52:36.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Logging.Configuration.dll
+-rw-rw-rw-   0        0        0    54384 2021-10-22 23:52:40.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Logging.Console.dll
+-rw-rw-rw-   0        0        0    18032 2021-10-22 23:52:36.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Logging.Debug.dll
+-rw-rw-rw-   0        0        0    24176 2021-10-22 23:52:30.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Logging.EventLog.dll
+-rw-rw-rw-   0        0        0    34928 2021-10-22 23:52:38.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Logging.EventSource.dll
+-rw-rw-rw-   0        0        0    44656 2021-10-22 23:52:28.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Logging.dll
+-rw-rw-rw-   0        0        0    22640 2021-10-22 23:48:22.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Options.ConfigurationExtensions.dll
+-rw-rw-rw-   0        0        0    58480 2021-10-22 23:48:14.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Options.dll
+-rw-rw-rw-   0        0        0    43120 2021-10-22 23:47:28.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Primitives.dll
+-rw-rw-rw-   0        0        0    26496 2020-10-19 18:37:20.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Win32.Registry.dll
+-rw-rw-rw-   0        0        0    30720 2024-02-16 19:07:30.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/OpcLabs.Mqtt.dll
+-rw-rw-rw-   0        0        0    20856 2020-02-19 10:05:18.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Buffers.dll
+-rw-rw-rw-   0        0        0    28264 2021-10-22 23:52:04.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.CodeDom.dll
+-rw-rw-rw-   0        0        0    43152 2018-05-15 13:29:36.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.ComponentModel.Annotations.dll
+-rw-rw-rw-   0        0        0    86120 2021-10-22 23:49:30.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Configuration.ConfigurationManager.dll
+-rw-rw-rw-   0        0        0   166512 2021-10-22 23:41:28.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Diagnostics.DiagnosticSource.dll
+-rw-rw-rw-   0        0        0    31848 2021-10-22 23:51:28.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Diagnostics.EventLog.dll
+-rw-rw-rw-   0        0        0    19456 2017-03-14 18:20:06.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Diagnostics.Tracer.dll
+-rw-rw-rw-   0        0        0   141184 2020-02-19 10:05:18.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Memory.dll
+-rw-rw-rw-   0        0        0   142200 2019-07-31 14:15:22.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Net.Mqtt.dll
+-rw-rw-rw-   0        0        0   115856 2018-05-15 13:29:44.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Numerics.Vectors.dll
+-rw-rw-rw-   0        0        0  1470416 2020-11-10 16:22:52.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Reactive.dll
+-rw-rw-rw-   0        0        0    18024 2021-10-22 23:40:18.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Runtime.CompilerServices.Unsafe.dll
+-rw-rw-rw-   0        0        0    35952 2021-10-22 23:45:08.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Security.AccessControl.dll
+-rw-rw-rw-   0        0        0    27752 2021-10-22 23:48:12.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Security.Permissions.dll
+-rw-rw-rw-   0        0        0    18312 2020-10-19 18:46:28.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Security.Principal.Windows.dll
+-rw-rw-rw-   0        0        0    21096 2019-11-15 17:31:12.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.ServiceModel.Primitives.dll
+-rw-rw-rw-   0        0        0    76904 2021-10-22 23:41:14.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Text.Encodings.Web.dll
+-rw-rw-rw-   0        0        0   513128 2021-10-22 23:44:26.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Text.Json.dll
+-rw-rw-rw-   0        0        0    25984 2020-02-19 10:05:18.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Threading.Tasks.Extensions.dll
+-rw-rw-rw-   0        0        0    25232 2018-05-15 13:29:52.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.ValueTuple.dll
+drwxrwxrwx   0        0        0        0 2024-02-16 19:20:43.873297 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/
+-rw-rw-rw-   0        0        0  2875392 2023-11-14 16:12:36.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/BoxedAppSDK.Managed.dll
+-rw-rw-rw-   0        0        0    27264 2021-10-22 23:47:46.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Caching.Abstractions.dll
+-rw-rw-rw-   0        0        0    38016 2021-10-22 23:50:16.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Caching.Memory.dll
+-rw-rw-rw-   0        0        0    25216 2021-10-22 23:47:50.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.Abstractions.dll
+-rw-rw-rw-   0        0        0    33920 2021-10-22 23:49:54.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.Binder.dll
+-rw-rw-rw-   0        0        0    23152 2021-10-22 23:50:44.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.CommandLine.dll
+-rw-rw-rw-   0        0        0    18560 2021-10-22 23:50:12.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.EnvironmentVariables.dll
+-rw-rw-rw-   0        0        0    26224 2021-10-22 23:50:06.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.FileExtensions.dll
+-rw-rw-rw-   0        0        0    25728 2021-10-22 23:50:12.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.Json.dll
+-rw-rw-rw-   0        0        0    24688 2021-10-22 23:50:16.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.UserSecrets.dll
+-rw-rw-rw-   0        0        0    36464 2021-10-22 23:49:58.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.dll
+-rw-rw-rw-   0        0        0    43632 2021-10-22 23:48:34.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.DependencyInjection.Abstractions.dll
+-rw-rw-rw-   0        0        0    81536 2021-10-22 23:49:56.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.DependencyInjection.dll
+-rw-rw-rw-   0        0        0    21120 2021-10-22 23:51:18.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.FileProviders.Abstractions.dll
+-rw-rw-rw-   0        0        0    42624 2021-10-22 23:51:52.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.FileProviders.Physical.dll
+-rw-rw-rw-   0        0        0    44160 2021-10-22 23:47:32.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.FileSystemGlobbing.dll
+-rw-rw-rw-   0        0        0    27776 2021-10-22 23:50:04.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Hosting.Abstractions.dll
+-rw-rw-rw-   0        0        0    55424 2021-10-22 23:53:18.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Hosting.dll
+-rw-rw-rw-   0        0        0    62064 2021-10-22 23:51:20.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Logging.Abstractions.dll
+-rw-rw-rw-   0        0        0    26736 2021-10-22 23:50:46.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Logging.Configuration.dll
+-rw-rw-rw-   0        0        0    50304 2021-10-22 23:53:16.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Logging.Console.dll
+-rw-rw-rw-   0        0        0    18048 2021-10-22 23:50:10.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Logging.Debug.dll
+-rw-rw-rw-   0        0        0    24192 2021-10-22 23:50:12.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Logging.EventLog.dll
+-rw-rw-rw-   0        0        0    32896 2021-10-22 23:53:08.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Logging.EventSource.dll
+-rw-rw-rw-   0        0        0    44656 2021-10-22 23:50:34.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Logging.dll
+-rw-rw-rw-   0        0        0    22656 2021-10-22 23:50:42.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Options.ConfigurationExtensions.dll
+-rw-rw-rw-   0        0        0    59008 2021-10-22 23:50:00.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Options.dll
+-rw-rw-rw-   0        0        0    40048 2021-10-22 23:51:10.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Primitives.dll
+-rw-rw-rw-   0        0        0    26224 2021-10-22 23:40:24.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Win32.SystemEvents.dll
+-rw-rw-rw-   0        0        0    31232 2024-02-16 19:08:50.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/OpcLabs.Mqtt.dll
+-rw-rw-rw-   0        0        0   184944 2021-10-22 23:47:46.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.CodeDom.dll
+-rw-rw-rw-   0        0        0   395376 2021-10-22 23:51:46.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Configuration.ConfigurationManager.dll
+-rw-rw-rw-   0        0        0    51328 2021-10-22 23:50:48.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Diagnostics.EventLog.dll
+-rw-rw-rw-   0        0        0    16896 2017-03-14 18:20:06.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Diagnostics.Tracer.dll
+-rw-rw-rw-   0        0        0   175216 2021-10-22 23:49:12.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Drawing.Common.dll
+-rw-rw-rw-   0        0        0   142200 2019-07-31 14:15:22.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Net.Mqtt.dll
+-rw-rw-rw-   0        0        0  2318920 2019-11-15 17:31:08.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Private.ServiceModel.dll
+-rw-rw-rw-   0        0        0  1455056 2020-11-10 16:22:52.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Reactive.dll
+-rw-rw-rw-   0        0        0   186504 2018-05-15 13:29:54.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Security.Cryptography.Pkcs.dll
+-rw-rw-rw-   0        0        0    20592 2021-10-22 23:51:04.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Security.Cryptography.ProtectedData.dll
+-rw-rw-rw-   0        0        0   167568 2018-05-15 13:29:44.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Security.Cryptography.Xml.dll
+-rw-rw-rw-   0        0        0   104048 2021-10-22 23:49:50.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Security.Permissions.dll
+-rw-rw-rw-   0        0        0    21576 2019-11-15 17:31:24.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.ServiceModel.Primitives.dll
+-rw-rw-rw-   0        0        0    23624 2019-11-15 17:31:16.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.ServiceModel.dll
+-rw-rw-rw-   0        0        0    25712 2021-10-22 23:49:44.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Windows.Extensions.dll
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:01.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/runtime.native.System_4.0.0.txt
+-rw-rw-rw-   0        0        0      926 2023-11-14 16:14:16.000000 opclabs_mqtt-5.80.75/opclabs_mqtt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-16 19:20:43.873297 opclabs_mqtt-5.80.75/opclabs_mqtt.egg-info/
+-rw-rw-rw-   0        0        0     4850 2024-02-16 19:20:43.000000 opclabs_mqtt-5.80.75/opclabs_mqtt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10166 2024-02-16 19:20:43.000000 opclabs_mqtt-5.80.75/opclabs_mqtt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-16 19:20:43.000000 opclabs_mqtt-5.80.75/opclabs_mqtt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-02-16 19:20:43.000000 opclabs_mqtt-5.80.75/opclabs_mqtt.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       17 2024-02-16 19:20:43.000000 opclabs_mqtt-5.80.75/opclabs_mqtt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-02-16 19:20:43.000000 opclabs_mqtt-5.80.75/opclabs_mqtt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-02-16 19:20:43.873297 opclabs_mqtt-5.80.75/setup.cfg
+-rw-rw-rw-   0        0        0     1191 2024-02-16 18:57:43.000000 opclabs_mqtt-5.80.75/setup.py
```

### Comparing `opclabs_mqtt-5.80.191/PKG-INFO` & `opclabs_mqtt-5.80.75/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opclabs_mqtt
-Version: 5.80.191
+Version: 5.80.75
 Summary: MQTT communication package based on System.Net.Mqtt library by Xamarin (Microsoft).
 Home-page: https://kb.opclabs.com/OpcLabs.Mqtt_communication_package?python
 Author: CODE Consulting and Development, s.r.o.
 Author-email: sales09@opclabs.com
 Keywords: QuickOPC,OPC,UA,PubSub,MQTT
 Description-Content-Type: text/markdown
 License-File: opclabs_mqtt\OpcLabs.Mqtt\Microsoft.NETCore.Platforms_1.0.1.txt
```

### Comparing `opclabs_mqtt-5.80.191/README.md` & `opclabs_mqtt-5.80.75/README.md`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/Microsoft.NETCore.Platforms_1.0.1.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/Microsoft.NETCore.Platforms_1.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/Microsoft.NETCore.Platforms_1.1.0.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/Microsoft.NETCore.Platforms_1.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/Microsoft.NETCore.Targets_1.0.1.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/Microsoft.NETCore.Targets_1.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/Microsoft.NETCore.Targets_1.1.0.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/Microsoft.NETCore.Targets_1.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Collections.Concurrent_4.0.12.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Collections.Concurrent_4.0.12.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Collections_4.0.11.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Collections_4.0.11.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.ComponentModel_4.0.1.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.ComponentModel_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Diagnostics.Contracts_4.3.0.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Diagnostics.Contracts_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Diagnostics.Debug_4.0.11.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Diagnostics.Debug_4.0.11.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Diagnostics.Tools_4.0.1.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Diagnostics.Tools_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Diagnostics.TraceSource_4.0.0.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Diagnostics.TraceSource_4.0.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Diagnostics.Tracing_4.1.0.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Diagnostics.Tracing_4.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Dynamic.Runtime_4.0.11.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Dynamic.Runtime_4.0.11.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Globalization_4.0.11.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Globalization_4.0.11.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.IO_4.1.0.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.IO_4.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Linq.Expressions_4.1.0.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Linq.Expressions_4.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Linq_4.1.0.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Linq_4.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Net.Mqtt_0.6.0-beta.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Net.Mqtt_0.6.0-beta.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.ObjectModel_4.0.12.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.ObjectModel_4.0.12.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Reactive.Core_3.0.0.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Reactive.Core_3.0.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Reactive.Interfaces_3.0.0.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Reactive.Interfaces_3.0.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Reactive.Linq_3.0.0.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Reactive.Linq_3.0.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Reactive.PlatformServices_3.0.0.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Reactive.PlatformServices_3.0.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Reactive.Windows.Threading_3.0.0.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Reactive.Windows.Threading_3.0.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Reactive.WindowsRuntime_3.0.0.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Reactive.WindowsRuntime_3.0.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Reactive_3.0.0.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Reactive_3.0.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Reflection.Emit.ILGeneration_4.0.1.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Reflection.Emit.ILGeneration_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Reflection.Emit.Lightweight_4.0.1.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Reflection.Emit.Lightweight_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Reflection.Emit_4.0.1.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Reflection.Emit_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Reflection.Extensions_4.0.1.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Reflection.Extensions_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Reflection.Primitives_4.0.1.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Reflection.Primitives_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Reflection.TypeExtensions_4.1.0.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Reflection.TypeExtensions_4.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Reflection_4.1.0.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Reflection_4.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Resources.ResourceManager_4.0.1.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Resources.ResourceManager_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime.Extensions_4.1.0.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime.Extensions_4.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime.Handles_4.0.1.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime.Handles_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime.InteropServices.WindowsRuntime_4.0.1.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime.InteropServices.WindowsRuntime_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime.InteropServices_4.1.0.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime.InteropServices_4.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime.Serialization.Primitives_4.1.1.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime.Serialization.Primitives_4.1.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime.WindowsRuntime_4.0.11.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime.WindowsRuntime_4.0.11.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime_4.1.0.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime_4.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime_4.3.0.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Runtime_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Text.Encoding_4.0.11.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Text.Encoding_4.0.11.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Threading.Tasks_4.0.11.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Threading.Tasks_4.0.11.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Threading.ThreadPool_4.0.10.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Threading.ThreadPool_4.0.10.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Threading.Thread_4.0.0.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Threading.Thread_4.0.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Threading.Timer_4.0.1.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Threading.Timer_4.0.1.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/System.Threading_4.0.11.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/System.Threading_4.0.11.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/BoxedAppSDK.Managed.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/BoxedAppSDK.Managed.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Bcl.AsyncInterfaces.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Bcl.AsyncInterfaces.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Caching.Abstractions.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Caching.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Caching.Memory.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Caching.Memory.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.Abstractions.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.Binder.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.Binder.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.CommandLine.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.CommandLine.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.EnvironmentVariables.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.EnvironmentVariables.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.FileExtensions.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.FileExtensions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.Json.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.Json.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.UserSecrets.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.UserSecrets.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Configuration.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.DependencyInjection.Abstractions.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.DependencyInjection.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.DependencyInjection.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.DependencyInjection.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.FileProviders.Abstractions.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.FileProviders.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.FileProviders.Physical.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.FileProviders.Physical.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.FileSystemGlobbing.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.FileSystemGlobbing.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Hosting.Abstractions.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Hosting.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Hosting.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Hosting.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Logging.Abstractions.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Logging.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Logging.Configuration.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Logging.Configuration.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Logging.Console.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Logging.Console.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Logging.Debug.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Logging.Debug.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Logging.EventLog.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Logging.EventLog.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Logging.EventSource.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Logging.EventSource.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Logging.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Logging.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Options.ConfigurationExtensions.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Options.ConfigurationExtensions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Options.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Options.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Primitives.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Extensions.Primitives.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Win32.Registry.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/Microsoft.Win32.Registry.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/OpcLabs.Mqtt.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/OpcLabs.Mqtt.dll`

 * *Files 4% similar despite different names*

#### pedump {}

```diff
@@ -1,25 +1,25 @@
 
 COFF Header:
 	                Machine: 0x014c
 	               Sections: 0x0003
-	             Time stamp: 0xfd906f84
+	             Time stamp: 0xcc5fb339
 	Pointer to Symbol Table: 0x00000000
 	   	   Symbol Count: 0x00000000
 	   Optional Header Size: 0x00e0
 	   	Characteristics: 0x2022
 
 PE Header:
 	         Magic (0x010b): 0x010b
 	             LMajor (6): 0x30
 	             LMinor (0): 0x00
 	              Code Size: 0x00006e00
 	  Initialized Data Size: 0x00000800
 	Uninitialized Data Size: 0x00000000
-	        Entry Point RVA: 0x00008cbe
+	        Entry Point RVA: 0x00008cba
 	 	  Code Base RVA: 0x00002000
 		  Data Base RVA: 0x0000a000
 
 
 NT Header:
 	   Image Base (0x400000): 0x10000000
 	Section Alignment (8192): 0x00002000
@@ -29,54 +29,54 @@
 	  	  User Major (0): 0x0000
 	  	  User Minor (0): 0x0000
 	  	Subsys major (4): 0x0006
 	  	Subsys minor (0): 0x0000
 	 	       Reserverd: 0x00000000
 	 	      Image Size: 0x0000e000
 	 	     Header Size: 0x00000200
-	            Checksum (0): 0x0001751e
+	            Checksum (0): 0x0000a148
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
-	     Import Table: 0x00008c6c [0x0000004f]
-	   Resource Table: 0x0000a000 [0x000004c8]
+	     Import Table: 0x00008c68 [0x0000004f]
+	   Resource Table: 0x0000a000 [0x000004bc]
 	  Exception Table: 0x00000000 [0x00000000]
 	Certificate Table: 0x00000000 [0x00000000]
 	      Reloc Table: 0x0000c000 [0x0000000c]
-	            Debug: 0x00008b74 [0x00000054]
+	            Debug: 0x00008b70 [0x00000054]
 	        Copyright: 0x00000000 [0x00000000]
 	       Global Ptr: 0x00000000 [0x00000000]
 	        TLS Table: 0x00000000 [0x00000000]
 	Load Config Table: 0x00000000 [0x00000000]
 	     Bound Import: 0x00000000 [0x00000000]
 	              IAT: 0x00002000 [0x00000008]
 	Delay Import Desc: 0x00000000 [0x00000000]
 	       CLI Header: 0x00002008 [0x00000048]
 
 	Name: .text
-	   Virtual Size: 0x00006cc4
+	   Virtual Size: 0x00006cc0
 	Virtual Address: 0x00002000
 	  Raw Data Size: 0x00006e00
 	   Raw Data Ptr: 0x00000200
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: code, exec, read, 
 
 	Name: .rsrc
-	   Virtual Size: 0x000004c8
+	   Virtual Size: 0x000004bc
 	Virtual Address: 0x0000a000
 	  Raw Data Size: 0x00000600
 	   Raw Data Ptr: 0x00007000
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
-	         Metadata: 0x000038c0 [0x00004dcc]
+	         Metadata: 0x000038c0 [0x00004dc8]
 	Entry Point Token: 0x00000000
-	     Resources at: 0x0000868c [0x00000468]
-	   Strong Name at: 0x00008af4 [0x00000080]
+	     Resources at: 0x00008688 [0x00000468]
+	   Strong Name at: 0x00008af0 [0x00000080]
 	  Code Manager at: 0x00000000 [0x00000000]
 	  VTableFixups at: 0x00000000 [0x00000000]
 	     EAT jumps at: 0x00000000 [0x00000000]
 
 Strong name:
-	 EA 53 E3 C4 FF 15 84 E9 4E 8F 6C 9F 3E A6 01 72
-	 DD B3 25 D9 53 D3 5E 09 A4 B9 1E 8E 07 18 C6 0D
-	 A2 A1 44 DC 9D 09 6B CF 2B 0E 55 30 76 84 69 53
-	 B7 47 9B 5B 2D 04 87 52 B3 F2 FA CC 2C F0 36 47
-	 6B 4C D7 2B 75 40 CF 7C 62 97 F6 A1 21 61 21 14
-	 9B AA 85 13 72 09 00 76 99 15 9D 9F 54 54 E9 5A
-	 27 A9 AF BA 19 8F C5 9F 77 D2 C4 17 96 7F BC 24
-	 6A 6A 72 E6 D5 CF 3A FB 01 21 CB 85 3E B9 47 0D
+	 90 17 E0 9E 30 81 58 B9 D2 80 86 D2 2D 6A 0C 00
+	 27 A2 4B 6B E1 AC 13 20 B3 7F AA 56 0F 99 49 E3
+	 40 4F 01 BB 3C F7 84 8D E3 25 C5 D7 4F 00 D3 12
+	 F7 B6 6C 2A CD 75 AA B3 CB F6 1B 6E 3A 53 79 C6
+	 0D CA D1 C5 D4 14 A2 F7 3F 54 75 13 FE 35 17 0E
+	 9A 84 3C CD 35 C1 48 9F 52 6B A0 FE 87 67 78 46
+	 CB 87 78 2A 4C 5B D9 38 73 72 59 EA 67 1F 41 1E
+	 7D 0B 7F 4A 60 60 1A 94 EC 12 FC 4C 86 9E EA 8C
 
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
 	Tables (#~): 0x0000006c - 0x00001918 [6316 == 0x000018ac]
 	    Strings: 0x00001918 - 0x0000346c [6996 == 0x00001b54]
-	       Blob: 0x00003c10 - 0x00004dcc [4540 == 0x000011bc]
+	       Blob: 0x00003c10 - 0x00004dc8 [4536 == 0x000011b8]
 	User string: 0x0000346c - 0x00003c00 [1940 == 0x00000794]
 	       GUID: 0x00003c00 - 0x00003c10 [16 == 0x00000010]
 Rows:
 Table Module: 1 records (10 bytes, at 1b98)
 Table TypeRef: 120 records (6 bytes, at 1ba2)
 Table TypeDef: 23 records (14 bytes, at 1e72)
 Table Field: 83 records (6 bytes, at 1fb4)
```

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Buffers.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Buffers.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.CodeDom.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.CodeDom.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.ComponentModel.Annotations.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.ComponentModel.Annotations.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Configuration.ConfigurationManager.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Configuration.ConfigurationManager.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Diagnostics.DiagnosticSource.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Diagnostics.DiagnosticSource.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Diagnostics.EventLog.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Diagnostics.EventLog.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Diagnostics.Tracer.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Diagnostics.Tracer.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Memory.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Memory.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Net.Mqtt.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Net.Mqtt.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Numerics.Vectors.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Numerics.Vectors.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Reactive.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Reactive.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Runtime.CompilerServices.Unsafe.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Runtime.CompilerServices.Unsafe.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Security.AccessControl.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Security.AccessControl.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Security.Permissions.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Security.Permissions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Security.Principal.Windows.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Security.Principal.Windows.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.ServiceModel.Primitives.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.ServiceModel.Primitives.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Text.Encodings.Web.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Text.Encodings.Web.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Text.Json.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Text.Json.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Threading.Tasks.Extensions.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.Threading.Tasks.Extensions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net472/System.ValueTuple.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net472/System.ValueTuple.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/BoxedAppSDK.Managed.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/BoxedAppSDK.Managed.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Caching.Abstractions.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Caching.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Caching.Memory.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Caching.Memory.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.Abstractions.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.Binder.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.Binder.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.CommandLine.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.CommandLine.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.EnvironmentVariables.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.EnvironmentVariables.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.FileExtensions.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.FileExtensions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.Json.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.Json.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.UserSecrets.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.UserSecrets.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Configuration.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.DependencyInjection.Abstractions.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.DependencyInjection.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.DependencyInjection.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.DependencyInjection.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.FileProviders.Abstractions.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.FileProviders.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.FileProviders.Physical.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.FileProviders.Physical.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.FileSystemGlobbing.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.FileSystemGlobbing.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Hosting.Abstractions.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Hosting.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Hosting.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Hosting.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Logging.Abstractions.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Logging.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Logging.Configuration.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Logging.Configuration.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Logging.Console.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Logging.Console.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Logging.Debug.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Logging.Debug.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Logging.EventLog.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Logging.EventLog.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Logging.EventSource.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Logging.EventSource.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Logging.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Logging.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Options.ConfigurationExtensions.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Options.ConfigurationExtensions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Options.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Options.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Primitives.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Extensions.Primitives.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Win32.SystemEvents.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/Microsoft.Win32.SystemEvents.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/OpcLabs.Mqtt.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/OpcLabs.Mqtt.dll`

 * *Files 4% similar despite different names*

#### pedump {}

```diff
@@ -1,25 +1,25 @@
 
 COFF Header:
 	                Machine: 0x014c
 	               Sections: 0x0003
-	             Time stamp: 0xccf2ee47
+	             Time stamp: 0xf2c99c69
 	Pointer to Symbol Table: 0x00000000
 	   	   Symbol Count: 0x00000000
 	   Optional Header Size: 0x00e0
 	   	Characteristics: 0x2022
 
 PE Header:
 	         Magic (0x010b): 0x010b
 	             LMajor (6): 0x30
 	             LMinor (0): 0x00
 	              Code Size: 0x00007000
 	  Initialized Data Size: 0x00000800
 	Uninitialized Data Size: 0x00000000
-	        Entry Point RVA: 0x00008e36
+	        Entry Point RVA: 0x00008e32
 	 	  Code Base RVA: 0x00002000
 		  Data Base RVA: 0x0000a000
 
 
 NT Header:
 	   Image Base (0x400000): 0x10000000
 	Section Alignment (8192): 0x00002000
@@ -29,54 +29,54 @@
 	  	  User Major (0): 0x0000
 	  	  User Minor (0): 0x0000
 	  	Subsys major (4): 0x0004
 	  	Subsys minor (0): 0x0000
 	 	       Reserverd: 0x00000000
 	 	      Image Size: 0x0000e000
 	 	     Header Size: 0x00000200
-	            Checksum (0): 0x000131de
+	            Checksum (0): 0x000094d2
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
-	     Import Table: 0x00008de4 [0x0000004f]
-	   Resource Table: 0x0000a000 [0x000004c8]
+	     Import Table: 0x00008de0 [0x0000004f]
+	   Resource Table: 0x0000a000 [0x000004bc]
 	  Exception Table: 0x00000000 [0x00000000]
 	Certificate Table: 0x00000000 [0x00000000]
 	      Reloc Table: 0x0000c000 [0x0000000c]
-	            Debug: 0x00008cec [0x00000054]
+	            Debug: 0x00008ce8 [0x00000054]
 	        Copyright: 0x00000000 [0x00000000]
 	       Global Ptr: 0x00000000 [0x00000000]
 	        TLS Table: 0x00000000 [0x00000000]
 	Load Config Table: 0x00000000 [0x00000000]
 	     Bound Import: 0x00000000 [0x00000000]
 	              IAT: 0x00002000 [0x00000008]
 	Delay Import Desc: 0x00000000 [0x00000000]
 	       CLI Header: 0x00002008 [0x00000048]
 
 	Name: .text
-	   Virtual Size: 0x00006e3c
+	   Virtual Size: 0x00006e38
 	Virtual Address: 0x00002000
 	  Raw Data Size: 0x00007000
 	   Raw Data Ptr: 0x00000200
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: code, exec, read, 
 
 	Name: .rsrc
-	   Virtual Size: 0x000004c8
+	   Virtual Size: 0x000004bc
 	Virtual Address: 0x0000a000
 	  Raw Data Size: 0x00000600
 	   Raw Data Ptr: 0x00007200
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
-	         Metadata: 0x00003930 [0x00004ed4]
+	         Metadata: 0x00003930 [0x00004ed0]
 	Entry Point Token: 0x00000000
-	     Resources at: 0x00008804 [0x00000468]
-	   Strong Name at: 0x00008c6c [0x00000080]
+	     Resources at: 0x00008800 [0x00000468]
+	   Strong Name at: 0x00008c68 [0x00000080]
 	  Code Manager at: 0x00000000 [0x00000000]
 	  VTableFixups at: 0x00000000 [0x00000000]
 	     EAT jumps at: 0x00000000 [0x00000000]
 
 Strong name:
-	 97 41 DC 32 12 B2 50 39 1D 60 66 AB A9 5C AF 65
-	 2D 67 84 73 06 7A BC 7B 2B C0 0F EA 03 D2 31 A3
-	 5D 77 6D A1 22 45 AD A8 2C 24 C8 29 72 AF E9 FB
-	 82 DB 8E 6A 5B 61 7C 32 1E 8E 76 1F D7 42 06 F5
-	 AF 21 EF A5 D7 B9 F0 9F B1 C2 68 C3 9F 0A CE D4
-	 7B 05 AE 5D CF 45 25 6F 8F F1 89 86 AC 98 34 84
-	 95 01 45 C1 78 1F D5 8F 1C BC 3A 7E AF 57 5D 88
-	 7F 81 FE 66 D0 47 EA 45 8C B4 A3 76 03 6E 9E BE
+	 39 98 C2 17 97 01 89 1B E1 4B 33 86 69 CF 47 C9
+	 57 C6 57 41 D0 67 DA 97 22 F6 05 62 BD C6 BD 3E
+	 6C 03 6B A5 AD 32 69 13 09 78 FC 88 DC 15 F8 A6
+	 AF DB 68 E4 2E 58 DA 00 77 99 5F D4 B9 3F EB CD
+	 B8 8F 5F 2A 72 14 46 CA 04 9C F6 D6 64 6D 25 39
+	 40 F5 86 54 5F 56 8C 60 3E EB DC 77 93 4C 4E EE
+	 A4 06 5C DB AD D7 23 35 7A 4B E5 4B 59 14 89 1E
+	 98 2E 93 45 B7 CA 1A EE CB AF 20 32 39 1A 83 7E
 
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
 	Tables (#~): 0x0000006c - 0x00001990 [6436 == 0x00001924]
 	    Strings: 0x00001990 - 0x00003578 [7144 == 0x00001be8]
-	       Blob: 0x00003d14 - 0x00004ed4 [4544 == 0x000011c0]
+	       Blob: 0x00003d14 - 0x00004ed0 [4540 == 0x000011bc]
 	User string: 0x00003578 - 0x00003d04 [1932 == 0x0000078c]
 	       GUID: 0x00003d04 - 0x00003d14 [16 == 0x00000010]
 Rows:
 Table Module: 1 records (10 bytes, at 1c08)
 Table TypeRef: 121 records (6 bytes, at 1c12)
 Table TypeDef: 23 records (14 bytes, at 1ee8)
 Table Field: 83 records (6 bytes, at 202a)
```

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.CodeDom.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.CodeDom.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Configuration.ConfigurationManager.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Configuration.ConfigurationManager.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Diagnostics.EventLog.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Diagnostics.EventLog.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Diagnostics.Tracer.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Diagnostics.Tracer.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Drawing.Common.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Drawing.Common.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Net.Mqtt.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Net.Mqtt.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Private.ServiceModel.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Private.ServiceModel.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Reactive.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Reactive.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Security.Cryptography.Pkcs.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Security.Cryptography.Pkcs.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Security.Cryptography.ProtectedData.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Security.Cryptography.ProtectedData.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Security.Cryptography.Xml.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Security.Cryptography.Xml.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Security.Permissions.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Security.Permissions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.ServiceModel.Primitives.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.ServiceModel.Primitives.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.ServiceModel.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.ServiceModel.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Windows.Extensions.dll` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/net6.0/System.Windows.Extensions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/OpcLabs.Mqtt/runtime.native.System_4.0.0.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt/OpcLabs.Mqtt/runtime.native.System_4.0.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt/__init__.py` & `opclabs_mqtt-5.80.75/opclabs_mqtt/__init__.py`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt.egg-info/PKG-INFO` & `opclabs_mqtt-5.80.75/opclabs_mqtt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opclabs_mqtt
-Version: 5.80.191
+Version: 5.80.75
 Summary: MQTT communication package based on System.Net.Mqtt library by Xamarin (Microsoft).
 Home-page: https://kb.opclabs.com/OpcLabs.Mqtt_communication_package?python
 Author: CODE Consulting and Development, s.r.o.
 Author-email: sales09@opclabs.com
 Keywords: QuickOPC,OPC,UA,PubSub,MQTT
 Description-Content-Type: text/markdown
 License-File: opclabs_mqtt\OpcLabs.Mqtt\Microsoft.NETCore.Platforms_1.0.1.txt
```

### Comparing `opclabs_mqtt-5.80.191/opclabs_mqtt.egg-info/SOURCES.txt` & `opclabs_mqtt-5.80.75/opclabs_mqtt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opclabs_mqtt-5.80.191/setup.py` & `opclabs_mqtt-5.80.75/setup.py`

 * *Files 8% similar despite different names*

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

