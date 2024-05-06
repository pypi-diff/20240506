# Comparing `tmp/opclabs_pcap-5.80.191.tar.gz` & `tmp/opclabs_pcap-5.80.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opclabs_pcap-5.80.191.tar", last modified: Mon May  6 14:41:33 2024, max compression
+gzip compressed data, was "opclabs_pcap-5.80.75.tar", last modified: Fri Feb 16 19:21:24 2024, max compression
```

## Comparing `opclabs_pcap-5.80.191.tar` & `opclabs_pcap-5.80.75.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 14:41:33.183338 opclabs_pcap-5.80.191/
--rw-rw-rw-   0        0        0      150 2024-02-20 15:46:20.000000 opclabs_pcap-5.80.191/MANIFEST.in
--rw-rw-rw-   0        0        0     1268 2024-05-06 14:41:33.183338 opclabs_pcap-5.80.191/PKG-INFO
--rw-rw-rw-   0        0        0      436 2024-02-20 15:46:16.000000 opclabs_pcap-5.80.191/README.md
-drwxrwxrwx   0        0        0        0 2024-05-06 14:41:32.839528 opclabs_pcap-5.80.191/opclabs_pcap/
-drwxrwxrwx   0        0        0        0 2024-05-06 14:41:32.870777 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:56.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/Microsoft.NETCore.Platforms_1.1.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:57.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/Microsoft.NETCore.Targets_1.1.0.txt
--rw-rw-rw-   0        0        0     1116 2024-05-06 14:34:57.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/System.Runtime.CompilerServices.Unsafe_4.6.0.txt
--rw-rw-rw-   0        0        0     9451 2024-05-06 14:34:57.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/System.Runtime_4.3.0.txt
--rw-rw-rw-   0        0        0    35149 2024-02-20 15:46:00.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/gpl-3.0.txt
--rw-rw-rw-   0        0        0     7652 2024-02-20 15:46:00.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/lgpl-3.0.txt
-drwxrwxrwx   0        0        0        0 2024-05-06 14:41:32.980155 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/
--rw-rw-rw-   0        0        0  2875392 2024-02-20 15:44:28.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/BoxedAppSDK.Managed.dll
--rw-rw-rw-   0        0        0    22144 2021-10-22 23:42:08.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Bcl.AsyncInterfaces.dll
--rw-rw-rw-   0        0        0    27264 2021-10-22 23:47:34.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Caching.Abstractions.dll
--rw-rw-rw-   0        0        0    38000 2021-10-22 23:53:04.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Caching.Memory.dll
--rw-rw-rw-   0        0        0    25200 2021-10-22 23:47:32.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.Abstractions.dll
--rw-rw-rw-   0        0        0    34432 2021-10-22 23:47:42.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.Binder.dll
--rw-rw-rw-   0        0        0    23152 2021-10-22 23:51:02.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.CommandLine.dll
--rw-rw-rw-   0        0        0    18560 2021-10-22 23:51:12.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.EnvironmentVariables.dll
--rw-rw-rw-   0        0        0    26224 2021-10-22 23:49:04.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.FileExtensions.dll
--rw-rw-rw-   0        0        0    25728 2021-10-22 23:49:20.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.Json.dll
--rw-rw-rw-   0        0        0    24688 2021-10-22 23:49:30.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.UserSecrets.dll
--rw-rw-rw-   0        0        0    36464 2021-10-22 23:47:44.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.dll
--rw-rw-rw-   0        0        0    47216 2021-10-22 23:48:04.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.DependencyInjection.Abstractions.dll
--rw-rw-rw-   0        0        0    84608 2021-10-22 23:48:22.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.DependencyInjection.dll
--rw-rw-rw-   0        0        0    21120 2021-10-22 23:47:34.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.FileProviders.Abstractions.dll
--rw-rw-rw-   0        0        0    42608 2021-10-22 23:48:22.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.FileProviders.Physical.dll
--rw-rw-rw-   0        0        0    44160 2021-10-22 23:48:18.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.FileSystemGlobbing.dll
--rw-rw-rw-   0        0        0    28288 2021-10-22 23:48:12.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Hosting.Abstractions.dll
--rw-rw-rw-   0        0        0    57984 2021-10-22 23:52:42.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Hosting.dll
--rw-rw-rw-   0        0        0    64112 2021-10-22 23:51:24.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Logging.Abstractions.dll
--rw-rw-rw-   0        0        0    26736 2021-10-22 23:52:36.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Logging.Configuration.dll
--rw-rw-rw-   0        0        0    54384 2021-10-22 23:52:40.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Logging.Console.dll
--rw-rw-rw-   0        0        0    18032 2021-10-22 23:52:36.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Logging.Debug.dll
--rw-rw-rw-   0        0        0    24176 2021-10-22 23:52:30.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Logging.EventLog.dll
--rw-rw-rw-   0        0        0    34928 2021-10-22 23:52:38.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Logging.EventSource.dll
--rw-rw-rw-   0        0        0    44656 2021-10-22 23:52:28.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Logging.dll
--rw-rw-rw-   0        0        0    22640 2021-10-22 23:48:22.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Options.ConfigurationExtensions.dll
--rw-rw-rw-   0        0        0    58480 2021-10-22 23:48:14.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Options.dll
--rw-rw-rw-   0        0        0    43120 2021-10-22 23:47:28.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Primitives.dll
--rw-rw-rw-   0        0        0    26496 2020-10-19 18:37:20.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Win32.Registry.dll
--rw-rw-rw-   0        0        0    30720 2024-05-06 14:20:53.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/OpcLabs.Pcap.dll
--rw-rw-rw-   0        0        0   230400 2019-11-25 14:15:06.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/PacketDotNet.dll
--rw-rw-rw-   0        0        0    59904 2019-12-16 02:35:22.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/SharpPcap.dll
--rw-rw-rw-   0        0        0    20856 2020-02-19 10:05:18.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.Buffers.dll
--rw-rw-rw-   0        0        0    28264 2021-10-22 23:52:04.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.CodeDom.dll
--rw-rw-rw-   0        0        0    43152 2018-05-15 13:29:36.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.ComponentModel.Annotations.dll
--rw-rw-rw-   0        0        0    86120 2021-10-22 23:49:30.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.Configuration.ConfigurationManager.dll
--rw-rw-rw-   0        0        0   166512 2021-10-22 23:41:28.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.Diagnostics.DiagnosticSource.dll
--rw-rw-rw-   0        0        0    31848 2021-10-22 23:51:28.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.Diagnostics.EventLog.dll
--rw-rw-rw-   0        0        0   141184 2020-02-19 10:05:18.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.Memory.dll
--rw-rw-rw-   0        0        0   115856 2018-05-15 13:29:44.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.Numerics.Vectors.dll
--rw-rw-rw-   0        0        0  1470416 2020-11-10 16:22:52.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.Reactive.dll
--rw-rw-rw-   0        0        0    18024 2021-10-22 23:40:18.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.Runtime.CompilerServices.Unsafe.dll
--rw-rw-rw-   0        0        0    35952 2021-10-22 23:45:08.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.Security.AccessControl.dll
--rw-rw-rw-   0        0        0    27752 2021-10-22 23:48:12.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.Security.Permissions.dll
--rw-rw-rw-   0        0        0    18312 2020-10-19 18:46:28.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.Security.Principal.Windows.dll
--rw-rw-rw-   0        0        0    21096 2019-11-15 17:31:12.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.ServiceModel.Primitives.dll
--rw-rw-rw-   0        0        0    76904 2021-10-22 23:41:14.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.Text.Encodings.Web.dll
--rw-rw-rw-   0        0        0   513128 2021-10-22 23:44:26.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.Text.Json.dll
--rw-rw-rw-   0        0        0    25984 2020-02-19 10:05:18.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.Threading.Tasks.Extensions.dll
--rw-rw-rw-   0        0        0    25232 2018-05-15 13:29:52.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.ValueTuple.dll
-drwxrwxrwx   0        0        0        0 2024-05-06 14:41:33.152035 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/
--rw-rw-rw-   0        0        0  2875392 2024-02-20 15:44:28.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/BoxedAppSDK.Managed.dll
--rw-rw-rw-   0        0        0    27264 2021-10-22 23:47:46.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Caching.Abstractions.dll
--rw-rw-rw-   0        0        0    38016 2021-10-22 23:50:16.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Caching.Memory.dll
--rw-rw-rw-   0        0        0    25216 2021-10-22 23:47:50.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.Abstractions.dll
--rw-rw-rw-   0        0        0    33920 2021-10-22 23:49:54.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.Binder.dll
--rw-rw-rw-   0        0        0    23152 2021-10-22 23:50:44.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.CommandLine.dll
--rw-rw-rw-   0        0        0    18560 2021-10-22 23:50:12.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.EnvironmentVariables.dll
--rw-rw-rw-   0        0        0    26224 2021-10-22 23:50:06.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.FileExtensions.dll
--rw-rw-rw-   0        0        0    25728 2021-10-22 23:50:12.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.Json.dll
--rw-rw-rw-   0        0        0    24688 2021-10-22 23:50:16.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.UserSecrets.dll
--rw-rw-rw-   0        0        0    36464 2021-10-22 23:49:58.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.dll
--rw-rw-rw-   0        0        0    43632 2021-10-22 23:48:34.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.DependencyInjection.Abstractions.dll
--rw-rw-rw-   0        0        0    81536 2021-10-22 23:49:56.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.DependencyInjection.dll
--rw-rw-rw-   0        0        0    21120 2021-10-22 23:51:18.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.FileProviders.Abstractions.dll
--rw-rw-rw-   0        0        0    42624 2021-10-22 23:51:52.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.FileProviders.Physical.dll
--rw-rw-rw-   0        0        0    44160 2021-10-22 23:47:32.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.FileSystemGlobbing.dll
--rw-rw-rw-   0        0        0    27776 2021-10-22 23:50:04.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Hosting.Abstractions.dll
--rw-rw-rw-   0        0        0    55424 2021-10-22 23:53:18.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Hosting.dll
--rw-rw-rw-   0        0        0    62064 2021-10-22 23:51:20.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Logging.Abstractions.dll
--rw-rw-rw-   0        0        0    26736 2021-10-22 23:50:46.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Logging.Configuration.dll
--rw-rw-rw-   0        0        0    50304 2021-10-22 23:53:16.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Logging.Console.dll
--rw-rw-rw-   0        0        0    18048 2021-10-22 23:50:10.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Logging.Debug.dll
--rw-rw-rw-   0        0        0    24192 2021-10-22 23:50:12.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Logging.EventLog.dll
--rw-rw-rw-   0        0        0    32896 2021-10-22 23:53:08.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Logging.EventSource.dll
--rw-rw-rw-   0        0        0    44656 2021-10-22 23:50:34.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Logging.dll
--rw-rw-rw-   0        0        0    22656 2021-10-22 23:50:42.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Options.ConfigurationExtensions.dll
--rw-rw-rw-   0        0        0    59008 2021-10-22 23:50:00.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Options.dll
--rw-rw-rw-   0        0        0    40048 2021-10-22 23:51:10.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Primitives.dll
--rw-rw-rw-   0        0        0    26224 2021-10-22 23:40:24.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Win32.SystemEvents.dll
--rw-rw-rw-   0        0        0    31232 2024-05-06 14:23:04.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/OpcLabs.Pcap.dll
--rw-rw-rw-   0        0        0   230400 2019-11-25 14:15:04.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/PacketDotNet.dll
--rw-rw-rw-   0        0        0    59904 2019-12-16 02:35:22.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/SharpPcap.dll
--rw-rw-rw-   0        0        0   184944 2021-10-22 23:47:46.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/System.CodeDom.dll
--rw-rw-rw-   0        0        0   395376 2021-10-22 23:51:46.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Configuration.ConfigurationManager.dll
--rw-rw-rw-   0        0        0    51328 2021-10-22 23:50:48.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Diagnostics.EventLog.dll
--rw-rw-rw-   0        0        0   175216 2021-10-22 23:49:12.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Drawing.Common.dll
--rw-rw-rw-   0        0        0  2318920 2019-11-15 17:31:08.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Private.ServiceModel.dll
--rw-rw-rw-   0        0        0  1455056 2020-11-10 16:22:52.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Reactive.dll
--rw-rw-rw-   0        0        0   186504 2018-05-15 13:29:54.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Security.Cryptography.Pkcs.dll
--rw-rw-rw-   0        0        0    20592 2021-10-22 23:51:04.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Security.Cryptography.ProtectedData.dll
--rw-rw-rw-   0        0        0   167568 2018-05-15 13:29:44.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Security.Cryptography.Xml.dll
--rw-rw-rw-   0        0        0   104048 2021-10-22 23:49:50.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Security.Permissions.dll
--rw-rw-rw-   0        0        0    21576 2019-11-15 17:31:24.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/System.ServiceModel.Primitives.dll
--rw-rw-rw-   0        0        0    23624 2019-11-15 17:31:16.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/System.ServiceModel.dll
--rw-rw-rw-   0        0        0    25712 2021-10-22 23:49:44.000000 opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Windows.Extensions.dll
--rw-rw-rw-   0        0        0      926 2024-02-20 15:46:20.000000 opclabs_pcap-5.80.191/opclabs_pcap/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-06 14:41:33.152035 opclabs_pcap-5.80.191/opclabs_pcap.egg-info/
--rw-rw-rw-   0        0        0     1268 2024-05-06 14:41:32.000000 opclabs_pcap-5.80.191/opclabs_pcap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7433 2024-05-06 14:41:32.000000 opclabs_pcap-5.80.191/opclabs_pcap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 14:41:32.000000 opclabs_pcap-5.80.191/opclabs_pcap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-06 14:41:32.000000 opclabs_pcap-5.80.191/opclabs_pcap.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       17 2024-05-06 14:41:32.000000 opclabs_pcap-5.80.191/opclabs_pcap.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-06 14:41:32.000000 opclabs_pcap-5.80.191/opclabs_pcap.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-06 14:41:33.183338 opclabs_pcap-5.80.191/setup.cfg
--rw-rw-rw-   0        0        0     1175 2024-05-06 13:42:16.000000 opclabs_pcap-5.80.191/setup.py
+drwxrwxrwx   0        0        0        0 2024-02-16 19:21:24.717412 opclabs_pcap-5.80.75/
+-rw-rw-rw-   0        0        0      150 2023-11-14 16:14:16.000000 opclabs_pcap-5.80.75/MANIFEST.in
+-rw-rw-rw-   0        0        0     1267 2024-02-16 19:21:24.717412 opclabs_pcap-5.80.75/PKG-INFO
+-rw-rw-rw-   0        0        0      436 2023-11-14 16:14:16.000000 opclabs_pcap-5.80.75/README.md
+drwxrwxrwx   0        0        0        0 2024-02-16 19:21:24.545546 opclabs_pcap-5.80.75/opclabs_pcap/
+drwxrwxrwx   0        0        0        0 2024-02-16 19:21:24.561163 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:54.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/Microsoft.NETCore.Platforms_1.1.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:55.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/Microsoft.NETCore.Targets_1.1.0.txt
+-rw-rw-rw-   0        0        0     1116 2024-02-16 19:17:55.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/System.Runtime.CompilerServices.Unsafe_4.6.0.txt
+-rw-rw-rw-   0        0        0     9451 2024-02-16 19:17:55.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/System.Runtime_4.3.0.txt
+-rw-rw-rw-   0        0        0    35149 2023-11-14 16:14:01.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/gpl-3.0.txt
+-rw-rw-rw-   0        0        0     7652 2023-11-14 16:14:01.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/lgpl-3.0.txt
+drwxrwxrwx   0        0        0        0 2024-02-16 19:21:24.639285 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/
+-rw-rw-rw-   0        0        0  2875392 2023-11-14 16:12:36.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/BoxedAppSDK.Managed.dll
+-rw-rw-rw-   0        0        0    22144 2021-10-22 23:42:08.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Bcl.AsyncInterfaces.dll
+-rw-rw-rw-   0        0        0    27264 2021-10-22 23:47:34.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Caching.Abstractions.dll
+-rw-rw-rw-   0        0        0    38000 2021-10-22 23:53:04.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Caching.Memory.dll
+-rw-rw-rw-   0        0        0    25200 2021-10-22 23:47:32.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.Abstractions.dll
+-rw-rw-rw-   0        0        0    34432 2021-10-22 23:47:42.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.Binder.dll
+-rw-rw-rw-   0        0        0    23152 2021-10-22 23:51:02.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.CommandLine.dll
+-rw-rw-rw-   0        0        0    18560 2021-10-22 23:51:12.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.EnvironmentVariables.dll
+-rw-rw-rw-   0        0        0    26224 2021-10-22 23:49:04.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.FileExtensions.dll
+-rw-rw-rw-   0        0        0    25728 2021-10-22 23:49:20.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.Json.dll
+-rw-rw-rw-   0        0        0    24688 2021-10-22 23:49:30.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.UserSecrets.dll
+-rw-rw-rw-   0        0        0    36464 2021-10-22 23:47:44.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.dll
+-rw-rw-rw-   0        0        0    47216 2021-10-22 23:48:04.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.DependencyInjection.Abstractions.dll
+-rw-rw-rw-   0        0        0    84608 2021-10-22 23:48:22.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.DependencyInjection.dll
+-rw-rw-rw-   0        0        0    21120 2021-10-22 23:47:34.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.FileProviders.Abstractions.dll
+-rw-rw-rw-   0        0        0    42608 2021-10-22 23:48:22.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.FileProviders.Physical.dll
+-rw-rw-rw-   0        0        0    44160 2021-10-22 23:48:18.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.FileSystemGlobbing.dll
+-rw-rw-rw-   0        0        0    28288 2021-10-22 23:48:12.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Hosting.Abstractions.dll
+-rw-rw-rw-   0        0        0    57984 2021-10-22 23:52:42.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Hosting.dll
+-rw-rw-rw-   0        0        0    64112 2021-10-22 23:51:24.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Logging.Abstractions.dll
+-rw-rw-rw-   0        0        0    26736 2021-10-22 23:52:36.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Logging.Configuration.dll
+-rw-rw-rw-   0        0        0    54384 2021-10-22 23:52:40.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Logging.Console.dll
+-rw-rw-rw-   0        0        0    18032 2021-10-22 23:52:36.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Logging.Debug.dll
+-rw-rw-rw-   0        0        0    24176 2021-10-22 23:52:30.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Logging.EventLog.dll
+-rw-rw-rw-   0        0        0    34928 2021-10-22 23:52:38.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Logging.EventSource.dll
+-rw-rw-rw-   0        0        0    44656 2021-10-22 23:52:28.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Logging.dll
+-rw-rw-rw-   0        0        0    22640 2021-10-22 23:48:22.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Options.ConfigurationExtensions.dll
+-rw-rw-rw-   0        0        0    58480 2021-10-22 23:48:14.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Options.dll
+-rw-rw-rw-   0        0        0    43120 2021-10-22 23:47:28.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Primitives.dll
+-rw-rw-rw-   0        0        0    26496 2020-10-19 18:37:20.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Win32.Registry.dll
+-rw-rw-rw-   0        0        0    30720 2024-02-16 19:06:51.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/OpcLabs.Pcap.dll
+-rw-rw-rw-   0        0        0   230400 2019-11-25 14:15:06.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/PacketDotNet.dll
+-rw-rw-rw-   0        0        0    59904 2019-12-16 02:35:22.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/SharpPcap.dll
+-rw-rw-rw-   0        0        0    20856 2020-02-19 10:05:18.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.Buffers.dll
+-rw-rw-rw-   0        0        0    28264 2021-10-22 23:52:04.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.CodeDom.dll
+-rw-rw-rw-   0        0        0    43152 2018-05-15 13:29:36.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.ComponentModel.Annotations.dll
+-rw-rw-rw-   0        0        0    86120 2021-10-22 23:49:30.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.Configuration.ConfigurationManager.dll
+-rw-rw-rw-   0        0        0   166512 2021-10-22 23:41:28.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.Diagnostics.DiagnosticSource.dll
+-rw-rw-rw-   0        0        0    31848 2021-10-22 23:51:28.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.Diagnostics.EventLog.dll
+-rw-rw-rw-   0        0        0   141184 2020-02-19 10:05:18.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.Memory.dll
+-rw-rw-rw-   0        0        0   115856 2018-05-15 13:29:44.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.Numerics.Vectors.dll
+-rw-rw-rw-   0        0        0  1470416 2020-11-10 16:22:52.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.Reactive.dll
+-rw-rw-rw-   0        0        0    18024 2021-10-22 23:40:18.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.Runtime.CompilerServices.Unsafe.dll
+-rw-rw-rw-   0        0        0    35952 2021-10-22 23:45:08.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.Security.AccessControl.dll
+-rw-rw-rw-   0        0        0    27752 2021-10-22 23:48:12.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.Security.Permissions.dll
+-rw-rw-rw-   0        0        0    18312 2020-10-19 18:46:28.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.Security.Principal.Windows.dll
+-rw-rw-rw-   0        0        0    21096 2019-11-15 17:31:12.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.ServiceModel.Primitives.dll
+-rw-rw-rw-   0        0        0    76904 2021-10-22 23:41:14.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.Text.Encodings.Web.dll
+-rw-rw-rw-   0        0        0   513128 2021-10-22 23:44:26.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.Text.Json.dll
+-rw-rw-rw-   0        0        0    25984 2020-02-19 10:05:18.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.Threading.Tasks.Extensions.dll
+-rw-rw-rw-   0        0        0    25232 2018-05-15 13:29:52.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.ValueTuple.dll
+drwxrwxrwx   0        0        0        0 2024-02-16 19:21:24.717412 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/
+-rw-rw-rw-   0        0        0  2875392 2023-11-14 16:12:36.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/BoxedAppSDK.Managed.dll
+-rw-rw-rw-   0        0        0    27264 2021-10-22 23:47:46.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Caching.Abstractions.dll
+-rw-rw-rw-   0        0        0    38016 2021-10-22 23:50:16.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Caching.Memory.dll
+-rw-rw-rw-   0        0        0    25216 2021-10-22 23:47:50.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.Abstractions.dll
+-rw-rw-rw-   0        0        0    33920 2021-10-22 23:49:54.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.Binder.dll
+-rw-rw-rw-   0        0        0    23152 2021-10-22 23:50:44.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.CommandLine.dll
+-rw-rw-rw-   0        0        0    18560 2021-10-22 23:50:12.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.EnvironmentVariables.dll
+-rw-rw-rw-   0        0        0    26224 2021-10-22 23:50:06.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.FileExtensions.dll
+-rw-rw-rw-   0        0        0    25728 2021-10-22 23:50:12.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.Json.dll
+-rw-rw-rw-   0        0        0    24688 2021-10-22 23:50:16.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.UserSecrets.dll
+-rw-rw-rw-   0        0        0    36464 2021-10-22 23:49:58.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.dll
+-rw-rw-rw-   0        0        0    43632 2021-10-22 23:48:34.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.DependencyInjection.Abstractions.dll
+-rw-rw-rw-   0        0        0    81536 2021-10-22 23:49:56.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.DependencyInjection.dll
+-rw-rw-rw-   0        0        0    21120 2021-10-22 23:51:18.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.FileProviders.Abstractions.dll
+-rw-rw-rw-   0        0        0    42624 2021-10-22 23:51:52.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.FileProviders.Physical.dll
+-rw-rw-rw-   0        0        0    44160 2021-10-22 23:47:32.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.FileSystemGlobbing.dll
+-rw-rw-rw-   0        0        0    27776 2021-10-22 23:50:04.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Hosting.Abstractions.dll
+-rw-rw-rw-   0        0        0    55424 2021-10-22 23:53:18.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Hosting.dll
+-rw-rw-rw-   0        0        0    62064 2021-10-22 23:51:20.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Logging.Abstractions.dll
+-rw-rw-rw-   0        0        0    26736 2021-10-22 23:50:46.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Logging.Configuration.dll
+-rw-rw-rw-   0        0        0    50304 2021-10-22 23:53:16.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Logging.Console.dll
+-rw-rw-rw-   0        0        0    18048 2021-10-22 23:50:10.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Logging.Debug.dll
+-rw-rw-rw-   0        0        0    24192 2021-10-22 23:50:12.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Logging.EventLog.dll
+-rw-rw-rw-   0        0        0    32896 2021-10-22 23:53:08.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Logging.EventSource.dll
+-rw-rw-rw-   0        0        0    44656 2021-10-22 23:50:34.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Logging.dll
+-rw-rw-rw-   0        0        0    22656 2021-10-22 23:50:42.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Options.ConfigurationExtensions.dll
+-rw-rw-rw-   0        0        0    59008 2021-10-22 23:50:00.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Options.dll
+-rw-rw-rw-   0        0        0    40048 2021-10-22 23:51:10.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Primitives.dll
+-rw-rw-rw-   0        0        0    26224 2021-10-22 23:40:24.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Win32.SystemEvents.dll
+-rw-rw-rw-   0        0        0    31232 2024-02-16 19:08:50.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/OpcLabs.Pcap.dll
+-rw-rw-rw-   0        0        0   230400 2019-11-25 14:15:04.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/PacketDotNet.dll
+-rw-rw-rw-   0        0        0    59904 2019-12-16 02:35:22.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/SharpPcap.dll
+-rw-rw-rw-   0        0        0   184944 2021-10-22 23:47:46.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/System.CodeDom.dll
+-rw-rw-rw-   0        0        0   395376 2021-10-22 23:51:46.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Configuration.ConfigurationManager.dll
+-rw-rw-rw-   0        0        0    51328 2021-10-22 23:50:48.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Diagnostics.EventLog.dll
+-rw-rw-rw-   0        0        0   175216 2021-10-22 23:49:12.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Drawing.Common.dll
+-rw-rw-rw-   0        0        0  2318920 2019-11-15 17:31:08.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Private.ServiceModel.dll
+-rw-rw-rw-   0        0        0  1455056 2020-11-10 16:22:52.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Reactive.dll
+-rw-rw-rw-   0        0        0   186504 2018-05-15 13:29:54.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Security.Cryptography.Pkcs.dll
+-rw-rw-rw-   0        0        0    20592 2021-10-22 23:51:04.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Security.Cryptography.ProtectedData.dll
+-rw-rw-rw-   0        0        0   167568 2018-05-15 13:29:44.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Security.Cryptography.Xml.dll
+-rw-rw-rw-   0        0        0   104048 2021-10-22 23:49:50.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Security.Permissions.dll
+-rw-rw-rw-   0        0        0    21576 2019-11-15 17:31:24.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/System.ServiceModel.Primitives.dll
+-rw-rw-rw-   0        0        0    23624 2019-11-15 17:31:16.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/System.ServiceModel.dll
+-rw-rw-rw-   0        0        0    25712 2021-10-22 23:49:44.000000 opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Windows.Extensions.dll
+-rw-rw-rw-   0        0        0      926 2023-11-14 16:14:16.000000 opclabs_pcap-5.80.75/opclabs_pcap/__init__.py
+drwxrwxrwx   0        0        0        0 2024-02-16 19:21:24.717412 opclabs_pcap-5.80.75/opclabs_pcap.egg-info/
+-rw-rw-rw-   0        0        0     1267 2024-02-16 19:21:24.000000 opclabs_pcap-5.80.75/opclabs_pcap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7433 2024-02-16 19:21:24.000000 opclabs_pcap-5.80.75/opclabs_pcap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-16 19:21:24.000000 opclabs_pcap-5.80.75/opclabs_pcap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-02-16 19:21:24.000000 opclabs_pcap-5.80.75/opclabs_pcap.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       17 2024-02-16 19:21:24.000000 opclabs_pcap-5.80.75/opclabs_pcap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-02-16 19:21:24.000000 opclabs_pcap-5.80.75/opclabs_pcap.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-02-16 19:21:24.717412 opclabs_pcap-5.80.75/setup.cfg
+-rw-rw-rw-   0        0        0     1174 2024-02-16 18:57:44.000000 opclabs_pcap-5.80.75/setup.py
```

### Comparing `opclabs_pcap-5.80.191/PKG-INFO` & `opclabs_pcap-5.80.75/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opclabs_pcap
-Version: 5.80.191
+Version: 5.80.75
 Summary: Ethernet and capture file communication package.
 Home-page: https://kb.opclabs.com/OpcLabs.Pcap_communication_package?python
 Author: CODE Consulting and Development, s.r.o.
 Author-email: sales09@opclabs.com
 Keywords: QuickOPC,OPC,UA,PubSub,Ethernet,UDP,capture
 Description-Content-Type: text/markdown
 License-File: opclabs_pcap\OpcLabs.Pcap\Microsoft.NETCore.Platforms_1.1.0.txt
```

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/Microsoft.NETCore.Platforms_1.1.0.txt` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/Microsoft.NETCore.Platforms_1.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/Microsoft.NETCore.Targets_1.1.0.txt` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/Microsoft.NETCore.Targets_1.1.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/System.Runtime.CompilerServices.Unsafe_4.6.0.txt` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/System.Runtime.CompilerServices.Unsafe_4.6.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/System.Runtime_4.3.0.txt` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/System.Runtime_4.3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/gpl-3.0.txt` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/gpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/lgpl-3.0.txt` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/lgpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/BoxedAppSDK.Managed.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/BoxedAppSDK.Managed.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Bcl.AsyncInterfaces.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Bcl.AsyncInterfaces.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Caching.Abstractions.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Caching.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Caching.Memory.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Caching.Memory.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.Abstractions.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.Binder.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.Binder.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.CommandLine.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.CommandLine.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.EnvironmentVariables.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.EnvironmentVariables.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.FileExtensions.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.FileExtensions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.Json.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.Json.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.UserSecrets.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.UserSecrets.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Configuration.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.DependencyInjection.Abstractions.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.DependencyInjection.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.DependencyInjection.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.DependencyInjection.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.FileProviders.Abstractions.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.FileProviders.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.FileProviders.Physical.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.FileProviders.Physical.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.FileSystemGlobbing.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.FileSystemGlobbing.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Hosting.Abstractions.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Hosting.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Hosting.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Hosting.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Logging.Abstractions.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Logging.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Logging.Configuration.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Logging.Configuration.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Logging.Console.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Logging.Console.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Logging.Debug.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Logging.Debug.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Logging.EventLog.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Logging.EventLog.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Logging.EventSource.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Logging.EventSource.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Logging.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Logging.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Options.ConfigurationExtensions.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Options.ConfigurationExtensions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Options.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Options.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Primitives.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Extensions.Primitives.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Win32.Registry.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/Microsoft.Win32.Registry.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/OpcLabs.Pcap.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/OpcLabs.Pcap.dll`

 * *Files 4% similar despite different names*

#### pedump {}

```diff
@@ -1,25 +1,25 @@
 
 COFF Header:
 	                Machine: 0x014c
 	               Sections: 0x0003
-	             Time stamp: 0xe58acd08
+	             Time stamp: 0xcf4455d7
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
-	        Entry Point RVA: 0x00008c6a
+	        Entry Point RVA: 0x00008c66
 	 	  Code Base RVA: 0x00002000
 		  Data Base RVA: 0x0000a000
 
 
 NT Header:
 	   Image Base (0x400000): 0x10000000
 	Section Alignment (8192): 0x00002000
@@ -41,42 +41,42 @@
 	  Heap Reserve Size (1M): 0x00100000
 	 Heap Commit Size (4096): 0x00001000
 	      Loader flags (0x1): 0x00000000
 	   Data Directories (16): 0x00000010
 
 Data directories:
 	     Export Table: 0x00000000 [0x00000000]
-	     Import Table: 0x00008c18 [0x0000004f]
-	   Resource Table: 0x0000a000 [0x000004c8]
+	     Import Table: 0x00008c14 [0x0000004f]
+	   Resource Table: 0x0000a000 [0x000004bc]
 	  Exception Table: 0x00000000 [0x00000000]
 	Certificate Table: 0x00000000 [0x00000000]
 	      Reloc Table: 0x0000c000 [0x0000000c]
-	            Debug: 0x00008b20 [0x00000054]
+	            Debug: 0x00008b1c [0x00000054]
 	        Copyright: 0x00000000 [0x00000000]
 	       Global Ptr: 0x00000000 [0x00000000]
 	        TLS Table: 0x00000000 [0x00000000]
 	Load Config Table: 0x00000000 [0x00000000]
 	     Bound Import: 0x00000000 [0x00000000]
 	              IAT: 0x00002000 [0x00000008]
 	Delay Import Desc: 0x00000000 [0x00000000]
 	       CLI Header: 0x00002008 [0x00000048]
 
 	Name: .text
-	   Virtual Size: 0x00006c70
+	   Virtual Size: 0x00006c6c
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
@@ -92,17 +92,17 @@
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, discard, read, 
 
           CLI header size: 72
          Runtime required: 2.5
                     Flags: ilonly, 32/64, no-trackdebug, notsigned
-	         Metadata: 0x00003410 [0x00005018]
+	         Metadata: 0x00003410 [0x00005014]
 	Entry Point Token: 0x00000000
-	     Resources at: 0x00008428 [0x000006f8]
+	     Resources at: 0x00008424 [0x000006f8]
 	   Strong Name at: 0x00000000 [0x00000000]
 	  Code Manager at: 0x00000000 [0x00000000]
 	  VTableFixups at: 0x00000000 [0x00000000]
 	     EAT jumps at: 0x00000000 [0x00000000]
 
 Strong name: none
 
@@ -111,15 +111,15 @@
 Metadata header:
            Version: 1.1
     Version string: v4.0.30319
 
 Metadata pointers:
 	Tables (#~): 0x0000006c - 0x000018b4 [6216 == 0x00001848]
 	    Strings: 0x000018b4 - 0x00003564 [7344 == 0x00001cb0]
-	       Blob: 0x000044a4 - 0x00005018 [2932 == 0x00000b74]
+	       Blob: 0x000044a4 - 0x00005014 [2928 == 0x00000b70]
 	User string: 0x00003564 - 0x00004494 [3888 == 0x00000f30]
 	       GUID: 0x00004494 - 0x000044a4 [16 == 0x00000010]
 Rows:
 Table Module: 1 records (10 bytes, at 16f0)
 Table TypeRef: 126 records (6 bytes, at 16fa)
 Table TypeDef: 18 records (14 bytes, at 19ee)
 Table Field: 62 records (6 bytes, at 1aea)
```

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/PacketDotNet.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/PacketDotNet.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/SharpPcap.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/SharpPcap.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.Buffers.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.Buffers.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.CodeDom.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.CodeDom.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.ComponentModel.Annotations.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.ComponentModel.Annotations.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.Configuration.ConfigurationManager.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.Configuration.ConfigurationManager.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.Diagnostics.DiagnosticSource.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.Diagnostics.DiagnosticSource.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.Diagnostics.EventLog.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.Diagnostics.EventLog.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.Memory.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.Memory.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.Numerics.Vectors.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.Numerics.Vectors.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.Reactive.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.Reactive.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.Runtime.CompilerServices.Unsafe.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.Runtime.CompilerServices.Unsafe.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.Security.AccessControl.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.Security.AccessControl.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.Security.Permissions.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.Security.Permissions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.Security.Principal.Windows.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.Security.Principal.Windows.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.ServiceModel.Primitives.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.ServiceModel.Primitives.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.Text.Encodings.Web.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.Text.Encodings.Web.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.Text.Json.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.Text.Json.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.Threading.Tasks.Extensions.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.Threading.Tasks.Extensions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net472/System.ValueTuple.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net472/System.ValueTuple.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/BoxedAppSDK.Managed.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/BoxedAppSDK.Managed.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Caching.Abstractions.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Caching.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Caching.Memory.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Caching.Memory.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.Abstractions.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.Binder.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.Binder.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.CommandLine.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.CommandLine.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.EnvironmentVariables.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.EnvironmentVariables.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.FileExtensions.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.FileExtensions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.Json.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.Json.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.UserSecrets.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.UserSecrets.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Configuration.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.DependencyInjection.Abstractions.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.DependencyInjection.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.DependencyInjection.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.DependencyInjection.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.FileProviders.Abstractions.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.FileProviders.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.FileProviders.Physical.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.FileProviders.Physical.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.FileSystemGlobbing.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.FileSystemGlobbing.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Hosting.Abstractions.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Hosting.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Hosting.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Hosting.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Logging.Abstractions.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Logging.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Logging.Configuration.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Logging.Configuration.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Logging.Console.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Logging.Console.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Logging.Debug.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Logging.Debug.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Logging.EventLog.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Logging.EventLog.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Logging.EventSource.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Logging.EventSource.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Logging.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Logging.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Options.ConfigurationExtensions.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Options.ConfigurationExtensions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Options.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Options.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Primitives.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Extensions.Primitives.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Win32.SystemEvents.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/Microsoft.Win32.SystemEvents.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/OpcLabs.Pcap.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/OpcLabs.Pcap.dll`

 * *Files 3% similar despite different names*

#### pedump {}

```diff
@@ -1,25 +1,25 @@
 
 COFF Header:
 	                Machine: 0x014c
 	               Sections: 0x0003
-	             Time stamp: 0xb7c79cb1
+	             Time stamp: 0xfb4a91c6
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
-	        Entry Point RVA: 0x00008e8e
+	        Entry Point RVA: 0x00008e8a
 	 	  Code Base RVA: 0x00002000
 		  Data Base RVA: 0x0000a000
 
 
 NT Header:
 	   Image Base (0x400000): 0x10000000
 	Section Alignment (8192): 0x00002000
@@ -41,42 +41,42 @@
 	  Heap Reserve Size (1M): 0x00100000
 	 Heap Commit Size (4096): 0x00001000
 	      Loader flags (0x1): 0x00000000
 	   Data Directories (16): 0x00000010
 
 Data directories:
 	     Export Table: 0x00000000 [0x00000000]
-	     Import Table: 0x00008e3c [0x0000004f]
-	   Resource Table: 0x0000a000 [0x000004c8]
+	     Import Table: 0x00008e38 [0x0000004f]
+	   Resource Table: 0x0000a000 [0x000004bc]
 	  Exception Table: 0x00000000 [0x00000000]
 	Certificate Table: 0x00000000 [0x00000000]
 	      Reloc Table: 0x0000c000 [0x0000000c]
-	            Debug: 0x00008d44 [0x00000054]
+	            Debug: 0x00008d40 [0x00000054]
 	        Copyright: 0x00000000 [0x00000000]
 	       Global Ptr: 0x00000000 [0x00000000]
 	        TLS Table: 0x00000000 [0x00000000]
 	Load Config Table: 0x00000000 [0x00000000]
 	     Bound Import: 0x00000000 [0x00000000]
 	              IAT: 0x00002000 [0x00000008]
 	Delay Import Desc: 0x00000000 [0x00000000]
 	       CLI Header: 0x00002008 [0x00000048]
 
 	Name: .text
-	   Virtual Size: 0x00006e94
+	   Virtual Size: 0x00006e90
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
@@ -92,17 +92,17 @@
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, discard, read, 
 
           CLI header size: 72
          Runtime required: 2.5
                     Flags: ilonly, 32/64, no-trackdebug, notsigned
-	         Metadata: 0x00003540 [0x0000510c]
+	         Metadata: 0x00003540 [0x00005108]
 	Entry Point Token: 0x00000000
-	     Resources at: 0x0000864c [0x000006f8]
+	     Resources at: 0x00008648 [0x000006f8]
 	   Strong Name at: 0x00000000 [0x00000000]
 	  Code Manager at: 0x00000000 [0x00000000]
 	  VTableFixups at: 0x00000000 [0x00000000]
 	     EAT jumps at: 0x00000000 [0x00000000]
 
 Strong name: none
 
@@ -111,15 +111,15 @@
 Metadata header:
            Version: 1.1
     Version string: v4.0.30319
 
 Metadata pointers:
 	Tables (#~): 0x0000006c - 0x00001938 [6348 == 0x000018cc]
 	    Strings: 0x00001938 - 0x00003670 [7480 == 0x00001d38]
-	       Blob: 0x00004584 - 0x0000510c [2952 == 0x00000b88]
+	       Blob: 0x00004584 - 0x00005108 [2948 == 0x00000b84]
 	User string: 0x00003670 - 0x00004574 [3844 == 0x00000f04]
 	       GUID: 0x00004574 - 0x00004584 [16 == 0x00000010]
 Rows:
 Table Module: 1 records (10 bytes, at 1820)
 Table TypeRef: 126 records (6 bytes, at 182a)
 Table TypeDef: 18 records (14 bytes, at 1b1e)
 Table Field: 62 records (6 bytes, at 1c1a)
```

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/PacketDotNet.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/PacketDotNet.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/SharpPcap.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/SharpPcap.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/System.CodeDom.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/System.CodeDom.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Configuration.ConfigurationManager.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Configuration.ConfigurationManager.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Diagnostics.EventLog.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Diagnostics.EventLog.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Drawing.Common.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Drawing.Common.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Private.ServiceModel.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Private.ServiceModel.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Reactive.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Reactive.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Security.Cryptography.Pkcs.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Security.Cryptography.Pkcs.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Security.Cryptography.ProtectedData.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Security.Cryptography.ProtectedData.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Security.Cryptography.Xml.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Security.Cryptography.Xml.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Security.Permissions.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Security.Permissions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/System.ServiceModel.Primitives.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/System.ServiceModel.Primitives.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/System.ServiceModel.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/System.ServiceModel.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Windows.Extensions.dll` & `opclabs_pcap-5.80.75/opclabs_pcap/OpcLabs.Pcap/net6.0/System.Windows.Extensions.dll`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap/__init__.py` & `opclabs_pcap-5.80.75/opclabs_pcap/__init__.py`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap.egg-info/PKG-INFO` & `opclabs_pcap-5.80.75/opclabs_pcap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opclabs_pcap
-Version: 5.80.191
+Version: 5.80.75
 Summary: Ethernet and capture file communication package.
 Home-page: https://kb.opclabs.com/OpcLabs.Pcap_communication_package?python
 Author: CODE Consulting and Development, s.r.o.
 Author-email: sales09@opclabs.com
 Keywords: QuickOPC,OPC,UA,PubSub,Ethernet,UDP,capture
 Description-Content-Type: text/markdown
 License-File: opclabs_pcap\OpcLabs.Pcap\Microsoft.NETCore.Platforms_1.1.0.txt
```

### Comparing `opclabs_pcap-5.80.191/opclabs_pcap.egg-info/SOURCES.txt` & `opclabs_pcap-5.80.75/opclabs_pcap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opclabs_pcap-5.80.191/setup.py` & `opclabs_pcap-5.80.75/setup.py`

 * *Files 1% similar despite different names*

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

