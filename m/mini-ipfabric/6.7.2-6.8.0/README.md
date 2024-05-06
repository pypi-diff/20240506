# Comparing `tmp/mini_ipfabric-6.7.2.tar.gz` & `tmp/mini_ipfabric-6.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mini_ipfabric-6.7.2.tar", max compression
+gzip compressed data, was "mini_ipfabric-6.8.0.tar", max compression
```

## Comparing `mini_ipfabric-6.7.2.tar` & `mini_ipfabric-6.8.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1124 2024-03-13 13:10:27.042976 mini_ipfabric-6.7.2/LICENSE
--rw-r--r--   0        0        0      215 2024-03-15 12:43:49.267552 mini_ipfabric-6.7.2/mini_ipfabric/__init__.py
--rw-r--r--   0        0        0     7422 2024-03-15 12:43:49.268670 mini_ipfabric-6.7.2/mini_ipfabric/client.py
--rw-r--r--   0        0        0        0 2024-03-13 13:11:47.913265 mini_ipfabric-6.7.2/mini_ipfabric/oas/__init__.py
--rw-r--r--   0        0        0   202077 2024-03-13 13:11:47.914575 mini_ipfabric-6.7.2/mini_ipfabric/oas/v6.6.json
--rw-r--r--   0        0        0   202507 2024-03-13 13:11:47.915636 mini_ipfabric-6.7.2/mini_ipfabric/oas/v6.7.json
--rw-r--r--   0        0        0      846 2024-03-15 12:43:49.270760 mini_ipfabric-6.7.2/pyproject.toml
--rw-r--r--   0        0        0     1459 2024-03-13 17:40:01.765447 mini_ipfabric-6.7.2/README.md
--rw-r--r--   0        0        0     2466 1970-01-01 00:00:00.000000 mini_ipfabric-6.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1124 2024-03-13 13:10:27.042976 mini_ipfabric-6.8.0/LICENSE
+-rw-r--r--   0        0        0      215 2024-03-15 12:43:49.267552 mini_ipfabric-6.8.0/mini_ipfabric/__init__.py
+-rw-r--r--   0        0        0     7422 2024-03-15 12:43:49.268670 mini_ipfabric-6.8.0/mini_ipfabric/client.py
+-rw-r--r--   0        0        0        0 2024-03-13 13:11:47.913265 mini_ipfabric-6.8.0/mini_ipfabric/oas/__init__.py
+-rw-r--r--   0        0        0   202507 2024-03-13 13:11:47.915636 mini_ipfabric-6.8.0/mini_ipfabric/oas/v6.7.json
+-rw-r--r--   0        0        0   390704 2024-05-06 15:33:38.445169 mini_ipfabric-6.8.0/mini_ipfabric/oas/v6.8.json
+-rw-r--r--   0        0        0      846 2024-05-06 15:33:38.449169 mini_ipfabric-6.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1459 2024-03-13 17:40:01.765447 mini_ipfabric-6.8.0/README.md
+-rw-r--r--   0        0        0     2466 1970-01-01 00:00:00.000000 mini_ipfabric-6.8.0/PKG-INFO
```

### Comparing `mini_ipfabric-6.7.2/LICENSE` & `mini_ipfabric-6.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mini_ipfabric-6.7.2/mini_ipfabric/client.py` & `mini_ipfabric-6.8.0/mini_ipfabric/client.py`

 * *Files identical despite different names*

### Comparing `mini_ipfabric-6.7.2/mini_ipfabric/oas/v6.6.json` & `mini_ipfabric-6.8.0/mini_ipfabric/oas/v6.7.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9936926821819204%*

 * *Differences: {"'os/feature-flags'": "OrderedDict([('api_endpoint', '/os/feature-flags'), ('get', "*

 * *                       "OrderedDict([('api_endpoint', 'os/feature-flags'), ('web_endpoint', None), "*

 * *                       "('columns', None), ('summary', 'Return enabled feature flags'), "*

 * *                       "('description', 'Returns object of enabled feature flags')])), ('post', "*

 * *                       'None)])',*

 * * "'tables/aci/dtep'": "{'post': {'columns': {insert: [(1, 'type'), (2, 'id'), (3, 'dtepIp'), (7, "*

 * *     […]*

```diff
@@ -600,14 +600,25 @@
             "columns": null,
             "description": "Returns the disk space available in kbytes",
             "summary": "Return available disk space information",
             "web_endpoint": null
         },
         "post": null
     },
+    "os/feature-flags": {
+        "api_endpoint": "/os/feature-flags",
+        "get": {
+            "api_endpoint": "os/feature-flags",
+            "columns": null,
+            "description": "Returns object of enabled feature flags",
+            "summary": "Return enabled feature flags",
+            "web_endpoint": null
+        },
+        "post": null
+    },
     "os/generate-nimpee-cert": {
         "api_endpoint": "/os/generate-nimpee-cert",
         "get": null,
         "post": {
             "api_endpoint": "os/generate-nimpee-cert",
             "columns": null,
             "description": "Generates IP Fabric certificate",
@@ -1506,2837 +1517,2840 @@
     "tables/aci/dtep": {
         "api_endpoint": "/tables/aci/dtep",
         "get": null,
         "post": {
             "api_endpoint": "tables/aci/dtep",
             "columns": [
                 "siteName",
-                "hostname",
+                "type",
+                "id",
+                "dtepIp",
                 "sn",
                 "encap",
                 "role",
-                "dtepIp",
-                "type",
-                "id"
+                "hostname"
             ],
             "description": "IS-IS Dynamic Tunnel End Point inventory",
             "summary": "DTEP Inventory",
             "web_endpoint": "/technology/sdn/aci/dtep"
         }
     },
     "tables/aci/endpoints": {
         "api_endpoint": "/tables/aci/endpoints",
         "get": null,
         "post": {
             "api_endpoint": "tables/aci/endpoints",
             "columns": [
-                "group",
-                "ipFlags",
+                "vrf",
                 "siteName",
+                "vrfVnid",
+                "encapId",
+                "group",
+                "id",
+                "mac",
                 "hostname",
-                "intName",
-                "vlanId",
-                "bdVnid",
                 "sn",
-                "vrf",
+                "ipFlags",
                 "macFlags",
-                "encapId",
+                "vlanId",
+                "vlanVnid",
                 "ip",
+                "bdVnid",
                 "encapType",
-                "vlanVnid",
-                "mac",
-                "id",
-                "vrfVnid"
+                "intName"
             ],
             "description": "Application Centric Infrastructure (ACI) endpoints inventory",
             "summary": "ACI Endpoint",
             "web_endpoint": "/technology/sdn/aci/endpoint"
         }
     },
     "tables/aci/vlan": {
         "api_endpoint": "/tables/aci/vlan",
         "get": null,
         "post": {
             "api_endpoint": "tables/aci/vlan",
             "columns": [
-                "hwId",
-                "encapVlanId",
+                "bdVlanId",
                 "siteName",
-                "hostname",
-                "vlanId",
-                "sn",
+                "encapVlanId",
                 "vlanType",
-                "endpointCount",
+                "id",
                 "encapVlanType",
+                "endpointCount",
                 "fabricVxlanId",
-                "bdVlanId",
-                "id"
+                "sn",
+                "vlanId",
+                "hwId",
+                "hostname"
             ],
             "description": "Application Centric Infrastructure (ACI) VLANs inventory",
             "summary": "ACI VLAN",
             "web_endpoint": "/technology/sdn/aci/vlan"
         }
     },
     "tables/aci/vrf": {
         "api_endpoint": "/tables/aci/vrf",
         "get": null,
         "post": {
             "api_endpoint": "tables/aci/vrf",
             "columns": [
-                "contextId",
-                "vrfType",
-                "siteName",
-                "hostname",
-                "sn",
+                "vrfVxlanId",
                 "vrf",
+                "siteName",
+                "id",
+                "vrfType",
                 "endpointCount",
-                "vrfVxlanId",
-                "status",
-                "id"
+                "sn",
+                "contextId",
+                "hostname",
+                "status"
             ],
             "description": "Application Centric Infrastructure (ACI) virtual routing and forwarding instances inventory",
             "summary": "ACI VRF",
             "web_endpoint": "/technology/sdn/aci/vrf"
         }
     },
     "tables/addressing/arp": {
         "api_endpoint": "/tables/addressing/arp",
         "get": null,
         "post": {
             "api_endpoint": "tables/addressing/arp",
             "columns": [
                 "siteName",
-                "hostname",
-                "intName",
-                "vlanId",
+                "id",
                 "proxy",
+                "vendor",
                 "sn",
+                "vlanId",
+                "intName",
+                "mac",
                 "vrf",
-                "vendor",
-                "ip",
-                "id",
-                "mac"
+                "hostname",
+                "ip"
             ],
             "description": "Address Resolution Protocol (ARP) collected fromt the network",
             "summary": "ARP Table",
             "web_endpoint": "/technology/addressing/arp-table"
         }
     },
     "tables/addressing/duplicate-ip": {
         "api_endpoint": "/tables/addressing/duplicate-ip",
         "get": null,
         "post": {
             "api_endpoint": "tables/addressing/duplicate-ip",
             "columns": [
-                "hostname",
-                "countIntUp",
-                "ip",
                 "id",
-                "count"
+                "countIntUp",
+                "count",
+                "hostname",
+                "ip"
             ],
             "description": "Duplicate IP adresses detected in the network",
             "summary": "Duplicate IP",
             "web_endpoint": "/technology/addressing/managed-duplicate-ip"
         }
     },
     "tables/addressing/hosts": {
         "api_endpoint": "/tables/addressing/hosts",
         "get": null,
         "post": {
             "api_endpoint": "tables/addressing/hosts",
             "columns": [
-                "type",
+                "gateways",
                 "siteName",
-                "edges",
-                "accessPoints",
                 "vlan",
-                "dnsName",
-                "gateways",
-                "vrf",
+                "type",
+                "accessPoints",
+                "id",
                 "vendor",
-                "ip",
-                "uniqId",
                 "mac",
-                "id"
+                "edges",
+                "ip",
+                "vrf",
+                "dnsName",
+                "uniqId"
             ],
             "description": "Detected IPv4 users, hosts, and endpoints from discovered gateways",
             "summary": "IPv4 Network Endpoints",
             "web_endpoint": "/inventory/hosts"
         }
     },
     "tables/addressing/ipv6-hosts": {
         "api_endpoint": "/tables/addressing/ipv6-hosts",
         "get": null,
         "post": {
             "api_endpoint": "tables/addressing/ipv6-hosts",
             "columns": [
-                "siteName",
-                "edges",
-                "uniqId",
                 "gateways",
+                "siteName",
                 "vlan",
+                "type",
+                "id",
+                "ipv6",
+                "edges",
+                "mac",
                 "vrf",
                 "vendor",
-                "ipv6",
-                "id",
-                "type",
-                "mac"
+                "uniqId"
             ],
             "description": "Detected IPv6 users, hosts, and endpoints from discovered gateways",
             "summary": "IPv6 Network endpoints",
             "web_endpoint": "/inventory/hosts/ipv6"
         }
     },
     "tables/addressing/ipv6-managed-devs": {
         "api_endpoint": "/tables/addressing/ipv6-managed-devs",
         "get": null,
         "post": {
             "api_endpoint": "tables/addressing/ipv6-managed-devs",
             "columns": [
                 "siteName",
-                "hostname",
-                "intName",
-                "vlanId",
+                "stateL2",
+                "type",
+                "id",
                 "net",
                 "sn",
-                "vrf",
                 "stateL1",
-                "ip",
-                "stateL2",
-                "id",
-                "type",
-                "mac"
+                "vlanId",
+                "intName",
+                "mac",
+                "vrf",
+                "hostname",
+                "ip"
             ],
             "description": "IPv6 addressess configured on network interfaces",
             "summary": "Managed IPv6 addresses",
             "web_endpoint": "/technology/addressing/managed-ip/ipv6"
         }
     },
     "tables/addressing/ipv6-neighbors": {
         "api_endpoint": "/tables/addressing/ipv6-neighbors",
         "get": null,
         "post": {
             "api_endpoint": "tables/addressing/ipv6-neighbors",
             "columns": [
                 "siteName",
-                "hostname",
-                "intName",
-                "vlanId",
+                "id",
+                "ipv6",
                 "proxy",
+                "vendor",
                 "sn",
+                "vlanId",
+                "mac",
                 "vrf",
-                "vendor",
-                "ipv6",
-                "id",
-                "mac"
+                "hostname",
+                "intName"
             ],
             "description": "Neighbors detected with IPv6 neighbor discovery",
             "summary": "IPv6 Neighbor discovery",
             "web_endpoint": "/technology/addressing/ipv6-neighbor-discovery"
         }
     },
     "tables/addressing/mac": {
         "api_endpoint": "/tables/addressing/mac",
         "get": null,
         "post": {
             "api_endpoint": "tables/addressing/mac",
             "columns": [
-                "fabricPath",
                 "siteName",
-                "hostname",
-                "intName",
-                "vxlans",
                 "vlan",
-                "user",
+                "type",
+                "id",
                 "vni",
-                "sn",
                 "edge",
+                "source",
+                "sn",
+                "user",
                 "vendor",
-                "id",
-                "type",
+                "vxlans",
                 "mac",
-                "source"
+                "hostname",
+                "intName",
+                "fabricPath"
             ],
             "description": "Cumulative MAC address table",
             "summary": "MAC Table",
             "web_endpoint": "/technology/addressing/mac-table"
         }
     },
     "tables/addressing/managed-devs": {
         "api_endpoint": "/tables/addressing/managed-devs",
         "get": null,
         "post": {
             "api_endpoint": "tables/addressing/managed-devs",
             "columns": [
-                "dnsHostnameMatch",
-                "type",
                 "siteName",
-                "hostname",
-                "intName",
-                "vlanId",
-                "dnsReverseMatch",
-                "dnsName",
-                "sn",
-                "vrf",
-                "stateL1",
-                "ip",
                 "stateL2",
+                "type",
+                "dnsHostnameMatch",
+                "id",
                 "net",
                 "mac",
-                "id"
+                "sn",
+                "stateL1",
+                "vlanId",
+                "dnsReverseMatch",
+                "intName",
+                "ip",
+                "vrf",
+                "hostname",
+                "dnsName"
             ],
             "description": "Inventory of IP addresses configured on every managed network device",
             "summary": "Managed IPv4 addresses",
             "web_endpoint": "/technology/addressing/managed-ip"
         }
     },
     "tables/addressing/path-lookup-first-hops": {
         "api_endpoint": "/tables/addressing/path-lookup-first-hops",
         "get": null,
         "post": {
             "api_endpoint": "tables/addressing/path-lookup-first-hops",
             "columns": [
-                "interfaces",
                 "sn",
-                "hostname"
+                "hostname",
+                "interfaces"
             ],
             "description": "",
             "summary": "POST /tables/addressing/path-lookup-first-hops",
             "web_endpoint": null
         }
     },
     "tables/addressing/path-lookup-sources": {
         "api_endpoint": "/tables/addressing/path-lookup-sources",
         "get": null,
         "post": {
             "api_endpoint": "tables/addressing/path-lookup-sources",
             "columns": [
-                "dnsName",
                 "ip",
-                "id"
+                "id",
+                "dnsName"
             ],
             "description": "",
             "summary": "POST /tables/addressing/path-lookup-sources",
             "web_endpoint": null
         }
     },
     "tables/addressing/path-lookup-sources-multicast": {
         "api_endpoint": "/tables/addressing/path-lookup-sources-multicast",
         "get": null,
         "post": {
             "api_endpoint": "tables/addressing/path-lookup-sources-multicast",
             "columns": [
-                "dnsName",
-                "type",
                 "ip",
-                "id"
+                "id",
+                "dnsName",
+                "type"
             ],
-            "description": null,
+            "description": "",
             "summary": "POST /tables/addressing/path-lookup-sources-multicast",
             "web_endpoint": null
         }
     },
     "tables/addressing/path-lookup-sources-unicast": {
         "api_endpoint": "/tables/addressing/path-lookup-sources-unicast",
         "get": null,
         "post": {
             "api_endpoint": "tables/addressing/path-lookup-sources-unicast",
             "columns": [
-                "dnsName",
                 "ip",
-                "id"
+                "id",
+                "dnsName"
             ],
-            "description": null,
+            "description": "",
             "summary": "POST /tables/addressing/path-lookup-sources-unicast",
             "web_endpoint": null
         }
     },
     "tables/apic/applications": {
         "api_endpoint": "/tables/apic/applications",
         "get": null,
         "post": {
             "api_endpoint": "tables/apic/applications",
             "columns": [
-                "apiUrl",
-                "endpointGroupsCount",
-                "name",
                 "slug",
                 "tenant",
                 "id",
-                "priority"
+                "priority",
+                "name",
+                "endpointGroupsCount",
+                "apiUrl"
             ],
             "description": "Cisco Application Centric Infrastructure (ACI) applications inventory",
             "summary": "APIC Applications",
             "web_endpoint": "/technology/sdn/apic/applications"
         }
     },
     "tables/apic/bridge-domains": {
         "api_endpoint": "/tables/apic/bridge-domains",
         "get": null,
         "post": {
             "api_endpoint": "tables/apic/bridge-domains",
             "columns": [
-                "scope",
-                "apiUrl",
-                "pcTag",
-                "name",
+                "slug",
+                "tenant",
                 "vrfName",
                 "subnets",
-                "slug",
                 "type",
-                "tenant",
-                "id"
+                "id",
+                "pcTag",
+                "name",
+                "apiUrl",
+                "scope"
             ],
             "description": "Cisco Application Centric Infrastructure (ACI) bridge-domains inventory",
             "summary": "APIC Bridge Domains",
             "web_endpoint": "/technology/sdn/apic/bridge-domains"
         }
     },
     "tables/apic/contexts": {
         "api_endpoint": "/tables/apic/contexts",
         "get": null,
         "post": {
             "api_endpoint": "tables/apic/contexts",
             "columns": [
-                "isUnenforced",
-                "scope",
-                "apiUrl",
+                "slug",
+                "tenant",
+                "id",
                 "pcTag",
                 "name",
+                "isUnenforced",
                 "bridgeDomainsCount",
-                "slug",
-                "tenant",
-                "id"
+                "apiUrl",
+                "scope"
             ],
             "description": "Cisco Application Centric Infrastructure (ACI) contexts inventory",
             "summary": "APIC Contexts",
             "web_endpoint": "/technology/sdn/apic/contexts"
         }
     },
     "tables/apic/contracts": {
         "api_endpoint": "/tables/apic/contracts",
         "get": null,
         "post": {
             "api_endpoint": "tables/apic/contracts",
             "columns": [
-                "subjectName",
-                "contractName",
-                "consumerMatch",
-                "providerMatch",
                 "apiUrl",
-                "subjectFilters",
-                "serviceGraph",
-                "hasReverseFilterPorts",
                 "slug",
-                "contractScope",
                 "tenant",
-                "id"
+                "contractName",
+                "hasReverseFilterPorts",
+                "id",
+                "subjectFilters",
+                "contractScope",
+                "subjectName",
+                "providerMatch",
+                "consumerMatch",
+                "serviceGraph"
             ],
             "description": "Cisco Application Centric Infrastructure (ACI) contracts inventory'",
             "summary": "APIC Contracts",
             "web_endpoint": "/technology/sdn/apic/contracts"
         }
     },
     "tables/apic/controllers": {
         "api_endpoint": "/tables/apic/controllers",
         "get": null,
         "post": {
             "api_endpoint": "tables/apic/controllers",
             "columns": [
                 "siteName",
-                "hostname",
-                "apiUrl",
-                "health",
-                "sn",
-                "name",
                 "ipv6Addresses",
+                "id",
+                "name",
+                "sn",
                 "ipAddresses",
-                "id"
+                "health",
+                "hostname",
+                "apiUrl"
             ],
             "description": "Cisco Application Centric Infrastructure (ACI) controllers inventory",
             "summary": "Controllers",
             "web_endpoint": "/technology/sdn/apic/controllers"
         }
     },
     "tables/apic/endpoint-groups": {
         "api_endpoint": "/tables/apic/endpoint-groups",
         "get": null,
         "post": {
             "api_endpoint": "tables/apic/endpoint-groups",
             "columns": [
+                "slug",
+                "tenant",
                 "appName",
+                "isPreferredGroupMember",
+                "subnets",
+                "id",
                 "contractsCount",
-                "scope",
-                "apiUrl",
                 "pcTag",
                 "name",
-                "subnets",
-                "isPreferredGroupMember",
-                "slug",
-                "tenant",
-                "id"
+                "apiUrl",
+                "scope"
             ],
             "description": "Cisco Application Centric Infrastructure (ACI) endpoint-groups inventory",
             "summary": "Endpoint Groups",
             "web_endpoint": "/technology/sdn/apic/endpoint-groups"
         }
     },
     "tables/apic/endpoint-groups/contracts": {
         "api_endpoint": "/tables/apic/endpoint-groups/contracts",
         "get": null,
         "post": {
             "api_endpoint": "tables/apic/endpoint-groups/contracts",
             "columns": [
-                "appName",
-                "endpointGroupName",
-                "apiUrl",
-                "name",
                 "slug",
-                "type",
                 "tenant",
-                "id"
+                "appName",
+                "type",
+                "id",
+                "name",
+                "endpointGroupName",
+                "apiUrl"
             ],
             "description": "Cisco Application Centric Infrastructure (ACI) groups and associated contracts inventory",
             "summary": "Endpoint Groups - Contracts",
             "web_endpoint": "/technology/sdn/apic/endpoint-groups-contracts"
         }
     },
     "tables/apic/service-graphs": {
         "api_endpoint": "/tables/apic/service-graphs",
         "get": null,
         "post": {
             "api_endpoint": "tables/apic/service-graphs",
             "columns": [
-                "nodeName",
-                "functionType",
-                "apiUrl",
-                "device",
-                "name",
                 "functionTemplateType",
                 "slug",
-                "state",
                 "tenant",
-                "id"
+                "functionType",
+                "device",
+                "id",
+                "state",
+                "name",
+                "nodeName",
+                "apiUrl"
             ],
             "description": "Cisco Application Centric Infrastructure (ACI) Service Graphs",
             "summary": "APIC Service Graphs",
             "web_endpoint": "/technology/sdn/apic/service-graphs"
         }
     },
     "tables/attributes/filters/keys": {
         "api_endpoint": "/tables/attributes/filters/keys",
         "get": null,
         "post": {
             "api_endpoint": "tables/attributes/filters/keys",
             "columns": [
-                "keyName",
-                "id"
+                "id",
+                "keyName"
             ],
             "description": "",
             "summary": "POST /tables/attributes/filters/keys",
             "web_endpoint": null
         }
     },
     "tables/attributes/filters/values": {
         "api_endpoint": "/tables/attributes/filters/values",
         "get": null,
         "post": {
             "api_endpoint": "tables/attributes/filters/values",
             "columns": [
-                "value",
+                "id",
                 "keyName",
-                "id"
+                "value"
             ],
             "description": "",
             "summary": "POST /tables/attributes/filters/values",
             "web_endpoint": null
         }
     },
     "tables/attributes/graphs": {
         "api_endpoint": "/tables/attributes/graphs",
         "get": null,
         "post": {
             "api_endpoint": "tables/attributes/graphs",
             "columns": [
-                "label",
-                "name",
                 "layout",
+                "id",
+                "name",
                 "path",
-                "id"
+                "label"
             ],
             "description": "",
             "summary": "POST /tables/attributes/graphs",
             "web_endpoint": null
         }
     },
     "tables/attributes/settings/keys": {
         "api_endpoint": "/tables/attributes/settings/keys",
         "get": null,
         "post": {
             "api_endpoint": "tables/attributes/settings/keys",
             "columns": [
-                "keyName",
-                "id"
+                "id",
+                "keyName"
             ],
             "description": "",
             "summary": "POST /tables/attributes/settings/keys",
             "web_endpoint": null
         }
     },
     "tables/attributes/settings/values": {
         "api_endpoint": "/tables/attributes/settings/values",
         "get": null,
         "post": {
             "api_endpoint": "tables/attributes/settings/values",
             "columns": [
-                "value",
+                "id",
                 "keyName",
-                "id"
+                "value"
             ],
             "description": "",
             "summary": "POST /tables/attributes/settings/values",
             "web_endpoint": null
         }
     },
     "tables/attributes/summary": {
         "api_endpoint": "/tables/attributes/summary",
         "get": null,
         "post": {
             "api_endpoint": "tables/attributes/summary",
             "columns": [
-                "label",
-                "name",
                 "layout",
+                "id",
+                "name",
                 "path",
-                "id"
+                "label"
             ],
             "description": "",
             "summary": "POST /tables/attributes/summary",
             "web_endpoint": null
         }
     },
     "tables/cloud/virtual-machines": {
         "api_endpoint": "/tables/cloud/virtual-machines",
         "get": null,
         "post": {
             "api_endpoint": "tables/cloud/virtual-machines",
             "columns": [
-                "os",
+                "slug",
+                "image",
                 "siteName",
-                "hostname",
-                "sn",
-                "name",
                 "numberOfInterfaces",
-                "status",
-                "slug",
                 "id",
-                "image"
+                "name",
+                "os",
+                "sn",
+                "hostname",
+                "status"
             ],
             "description": "Public or private cloud virtual machines",
             "summary": "Virtual Machines",
             "web_endpoint": "/technology/cloud/virtual-machines"
         }
     },
     "tables/cloud/virtual-machines-interfaces": {
         "api_endpoint": "/tables/cloud/virtual-machines-interfaces",
         "get": null,
         "post": {
             "api_endpoint": "tables/cloud/virtual-machines-interfaces",
             "columns": [
+                "slug",
                 "siteName",
-                "hostname",
-                "intName",
-                "vmIntName",
+                "ipv6Addresses",
                 "vmName",
-                "sn",
+                "vmIntId",
+                "vmIntName",
                 "outAcl",
-                "ipv6Addresses",
-                "slug",
+                "id",
+                "sn",
                 "ipAddresses",
-                "inAcl",
-                "vmIntId",
                 "mac",
-                "id"
+                "inAcl",
+                "hostname",
+                "intName"
             ],
             "description": "Public or private cloud virtual machines interfaces",
             "summary": "Virtual Machines Interfaces",
             "web_endpoint": "/technology/cloud/virtual-machines-interfaces"
         }
     },
     "tables/dhcp/relay/global-stats/received": {
         "api_endpoint": "/tables/dhcp/relay/global-stats/received",
         "get": null,
         "post": {
             "api_endpoint": "tables/dhcp/relay/global-stats/received",
             "columns": [
-                "siteName",
-                "sn",
-                "release",
-                "bootReply",
-                "ack",
-                "relayed",
-                "discover",
-                "bootRequest",
                 "total",
-                "hostname",
+                "id",
+                "bootRequest",
                 "dropped",
-                "request",
                 "nak",
+                "discover",
                 "received",
-                "decline",
-                "sent",
+                "hostname",
+                "release",
+                "request",
+                "ack",
+                "sn",
+                "bootReply",
                 "offer",
                 "inform",
-                "id"
+                "siteName",
+                "relayed",
+                "decline",
+                "sent"
             ],
             "description": "DHCP relay global statistics - received messages",
             "summary": "DHCP Relay Global statistics - received",
             "web_endpoint": "/technology/dhcp/relay/global-stats/received"
         }
     },
     "tables/dhcp/relay/global-stats/relayed": {
         "api_endpoint": "/tables/dhcp/relay/global-stats/relayed",
         "get": null,
         "post": {
             "api_endpoint": "tables/dhcp/relay/global-stats/relayed",
             "columns": [
-                "siteName",
-                "sn",
-                "release",
-                "bootReply",
-                "ack",
-                "relayed",
-                "discover",
-                "bootRequest",
                 "total",
-                "hostname",
+                "id",
+                "bootRequest",
                 "dropped",
-                "request",
                 "nak",
+                "discover",
                 "received",
-                "decline",
-                "sent",
+                "hostname",
+                "release",
+                "request",
+                "ack",
+                "sn",
+                "bootReply",
                 "offer",
                 "inform",
-                "id"
+                "siteName",
+                "relayed",
+                "decline",
+                "sent"
             ],
             "description": "DHCP relay global statistics - relayed messages",
             "summary": "DHCP Relay Global statistics - Relayed",
             "web_endpoint": "/technology/dhcp/relay/global-stats/relayed"
         }
     },
     "tables/dhcp/relay/global-stats/sent": {
         "api_endpoint": "/tables/dhcp/relay/global-stats/sent",
         "get": null,
         "post": {
             "api_endpoint": "tables/dhcp/relay/global-stats/sent",
             "columns": [
-                "siteName",
-                "sn",
-                "release",
-                "bootReply",
-                "ack",
-                "relayed",
-                "discover",
-                "bootRequest",
                 "total",
-                "hostname",
+                "id",
+                "bootRequest",
                 "dropped",
-                "request",
                 "nak",
+                "discover",
                 "received",
-                "decline",
-                "sent",
+                "hostname",
+                "release",
+                "request",
+                "ack",
+                "sn",
+                "bootReply",
                 "offer",
                 "inform",
-                "id"
+                "siteName",
+                "relayed",
+                "decline",
+                "sent"
             ],
             "description": "DHCP relay global statistics - sent messages",
             "summary": "DHCP Relay Global statistics - Sent",
             "web_endpoint": "/technology/dhcp/relay/global-stats/sent"
         }
     },
     "tables/dhcp/relay/global-stats/summary": {
         "api_endpoint": "/tables/dhcp/relay/global-stats/summary",
         "get": null,
         "post": {
             "api_endpoint": "tables/dhcp/relay/global-stats/summary",
             "columns": [
                 "siteName",
-                "hostname",
+                "id",
+                "sn",
                 "dropped",
+                "relayed",
                 "received",
-                "sn",
                 "sent",
-                "relayed",
-                "id"
+                "hostname"
             ],
             "description": "DHCP relay global statistics summary",
             "summary": "DHCP Relay Global stats summary",
             "web_endpoint": "/technology/dhcp/relay/global-stats/summary"
         }
     },
     "tables/dhcp/relay/interfaces": {
         "api_endpoint": "/tables/dhcp/relay/interfaces",
         "get": null,
         "post": {
             "api_endpoint": "tables/dhcp/relay/interfaces",
             "columns": [
+                "proxyOptions",
                 "siteName",
-                "hostname",
-                "intName",
-                "dropped",
+                "id",
                 "proxy",
-                "received",
                 "sn",
                 "name",
-                "vrf",
+                "dropped",
+                "received",
+                "options",
+                "relayed",
                 "sent",
                 "ip",
-                "relayed",
-                "proxyOptions",
-                "strategy",
-                "id",
-                "options"
+                "vrf",
+                "hostname",
+                "intName",
+                "strategy"
             ],
             "description": "DHCP relay interfaces inventory",
             "summary": "DHCP Relay Interfaces",
             "web_endpoint": "/technology/dhcp/relay/interfaces"
         }
     },
     "tables/dhcp/relay/interfaces-stats/received": {
         "api_endpoint": "/tables/dhcp/relay/interfaces-stats/received",
         "get": null,
         "post": {
             "api_endpoint": "tables/dhcp/relay/interfaces-stats/received",
             "columns": [
-                "siteName",
-                "hostname",
-                "intName",
                 "total",
+                "siteName",
+                "nak",
+                "id",
+                "bootRequest",
+                "discover",
+                "ack",
+                "request",
                 "sn",
+                "bootReply",
                 "decline",
-                "bootRequest",
-                "release",
                 "offer",
-                "bootReply",
+                "release",
+                "hostname",
                 "inform",
-                "discover",
-                "request",
-                "ack",
-                "id",
-                "nak"
+                "intName"
             ],
             "description": "DHCP relay interfaces statistics - received messages",
             "summary": "DHCP Relay Interfaces stats - Received",
             "web_endpoint": "/technology/dhcp/relay/interfaces-stats/received"
         }
     },
     "tables/dhcp/relay/interfaces-stats/relayed": {
         "api_endpoint": "/tables/dhcp/relay/interfaces-stats/relayed",
         "get": null,
         "post": {
             "api_endpoint": "tables/dhcp/relay/interfaces-stats/relayed",
             "columns": [
-                "siteName",
-                "hostname",
-                "intName",
                 "total",
+                "siteName",
+                "nak",
+                "id",
+                "bootRequest",
+                "discover",
+                "ack",
+                "request",
                 "sn",
+                "bootReply",
                 "decline",
-                "bootRequest",
-                "release",
                 "offer",
-                "bootReply",
+                "release",
+                "hostname",
                 "inform",
-                "discover",
-                "request",
-                "ack",
-                "id",
-                "nak"
+                "intName"
             ],
             "description": "DHCP relay interfaces statistics - relayed messages",
             "summary": "DHCP Relay Interfaces stats - Relayed",
             "web_endpoint": "/technology/dhcp/relay/interfaces-stats/relayed"
         }
     },
     "tables/dhcp/relay/interfaces-stats/sent": {
         "api_endpoint": "/tables/dhcp/relay/interfaces-stats/sent",
         "get": null,
         "post": {
             "api_endpoint": "tables/dhcp/relay/interfaces-stats/sent",
             "columns": [
-                "siteName",
-                "hostname",
-                "intName",
                 "total",
+                "siteName",
+                "nak",
+                "id",
+                "bootRequest",
+                "discover",
+                "ack",
+                "request",
                 "sn",
+                "bootReply",
                 "decline",
-                "bootRequest",
-                "release",
                 "offer",
-                "bootReply",
+                "release",
+                "hostname",
                 "inform",
-                "discover",
-                "request",
-                "ack",
-                "id",
-                "nak"
+                "intName"
             ],
             "description": "DHCP relay interfaces statistics - sent messages",
             "summary": "DHCP Relay Interfaces stats - Sent",
             "web_endpoint": "/technology/dhcp/relay/interfaces-stats/sent"
         }
     },
     "tables/dhcp/server/excluded-ranges": {
         "api_endpoint": "/tables/dhcp/server/excluded-ranges",
         "get": null,
         "post": {
             "api_endpoint": "tables/dhcp/server/excluded-ranges",
             "columns": [
-                "serverId",
                 "siteName",
-                "hostname",
-                "sn",
                 "range",
+                "id",
                 "serverName",
-                "id"
+                "sn",
+                "hostname",
+                "serverId"
             ],
             "description": "DHCP server excluded ranges inventory",
             "summary": "DHCP Server Excluded Ranges",
             "web_endpoint": "/technology/dhcp/server/excluded-ranges"
         }
     },
     "tables/dhcp/server/interfaces": {
         "api_endpoint": "/tables/dhcp/server/interfaces",
         "get": null,
         "post": {
             "api_endpoint": "tables/dhcp/server/interfaces",
             "columns": [
-                "serverId",
                 "siteName",
-                "hostname",
-                "intName",
-                "sn",
+                "id",
                 "serverName",
-                "id"
+                "sn",
+                "hostname",
+                "serverId",
+                "intName"
             ],
             "description": "DHCP server interfaces inventory",
             "summary": "DHCP Server Interfaces",
             "web_endpoint": "/technology/dhcp/server/interfaces"
         }
     },
     "tables/dhcp/server/leases": {
         "api_endpoint": "/tables/dhcp/server/leases",
         "get": null,
         "post": {
             "api_endpoint": "tables/dhcp/server/leases",
             "columns": [
-                "serverId",
                 "siteName",
-                "hostname",
-                "intName",
-                "sn",
-                "vrf",
-                "leaseExpiration",
+                "type",
                 "client",
-                "ip",
+                "id",
                 "state",
+                "leaseExpiration",
                 "serverName",
-                "type",
-                "id"
+                "sn",
+                "intName",
+                "vrf",
+                "hostname",
+                "serverId",
+                "ip"
             ],
             "description": "DHCP Server ",
             "summary": "DHCP Server Leases",
             "web_endpoint": "/technology/dhcp/server/leases"
         }
     },
     "tables/dhcp/server/pools": {
         "api_endpoint": "/tables/dhcp/server/pools",
         "get": null,
         "post": {
             "api_endpoint": "tables/dhcp/server/pools",
             "columns": [
-                "rangeOptions",
-                "serverId",
+                "rangeUsage",
                 "siteName",
-                "hostname",
+                "range",
+                "id",
+                "rangeType",
+                "rangeOptions",
+                "poolOptions",
+                "serverName",
                 "sn",
                 "name",
                 "vrf",
-                "rangeType",
-                "rangeUsage",
-                "range",
-                "serverName",
-                "poolOptions",
-                "id"
+                "hostname",
+                "serverId"
             ],
             "description": "DHCP Server pools inventory",
             "summary": "DHCL Server Pools",
             "web_endpoint": "/technology/dhcp/server/pools"
         }
     },
     "tables/dhcp/server/summary": {
         "api_endpoint": "/tables/dhcp/server/summary",
         "get": null,
         "post": {
             "api_endpoint": "tables/dhcp/server/summary",
             "columns": [
                 "siteName",
-                "excludedRangesCount",
-                "hostname",
+                "leasesCount",
+                "id",
                 "poolsCount",
-                "sn",
-                "intNamesCount",
                 "serverName",
-                "id",
-                "leasesCount"
+                "sn",
+                "excludedRangesCount",
+                "hostname",
+                "intNamesCount"
             ],
             "description": "DHCP server summary information inventory",
             "summary": "DHCP Server Summary",
             "web_endpoint": "/technology/dhcp/server/summary"
         }
     },
     "tables/fhrp/balancing": {
         "api_endpoint": "/tables/fhrp/balancing",
         "get": null,
         "post": {
             "api_endpoint": "tables/fhrp/balancing",
             "columns": [
                 "nei2",
                 "virtIp",
-                "nei1Sn",
-                "pct",
-                "vrf",
                 "nei1",
+                "id",
                 "nei2Sn",
-                "id"
+                "nei1Sn",
+                "vrf",
+                "pct"
             ],
             "description": "Balancing ratios for FHRP gateways",
             "summary": "Active FHRP gateway balancing",
             "web_endpoint": "/technology/fhrp/active-gw-balancing"
         }
     },
     "tables/fhrp/glbp-forwarders": {
         "api_endpoint": "/tables/fhrp/glbp-forwarders",
         "get": null,
         "post": {
             "api_endpoint": "tables/fhrp/glbp-forwarders",
             "columns": [
+                "siteName",
+                "active",
                 "group",
+                "id",
+                "state",
+                "sn",
                 "address",
-                "siteName",
+                "vrf",
                 "hostname",
                 "intName",
-                "sn",
-                "vrf",
-                "forwarder",
-                "active",
-                "state",
-                "id"
+                "forwarder"
             ],
             "description": "GLBP forwarders inventory",
             "summary": "GLBP forwarders",
             "web_endpoint": "/technology/fhrp/glbp-forwarders"
         }
     },
     "tables/fhrp/group-members": {
         "api_endpoint": "/tables/fhrp/group-members",
         "get": null,
         "post": {
             "api_endpoint": "tables/fhrp/group-members",
             "columns": [
-                "virtualIp",
-                "virtualIpv6",
+                "devices",
+                "id",
+                "protocol",
                 "count",
+                "virtualIpv6",
                 "vrf",
-                "protocol",
-                "id",
-                "devices"
+                "virtualIp"
             ],
             "description": "HSRP/VRRP/GLBP Group members - gateway inventory",
             "summary": "HSRP/VRRP/GLBP Group members",
             "web_endpoint": "/technology/fhrp/group-members"
         }
     },
     "tables/fhrp/group-state": {
         "api_endpoint": "/tables/fhrp/group-state",
         "get": null,
         "post": {
             "api_endpoint": "tables/fhrp/group-state",
             "columns": [
-                "group",
-                "virtualIp",
-                "virtualIpv6",
-                "siteName",
-                "hostname",
-                "intName",
-                "secondaryVirtualIpAddresses",
-                "standby",
-                "preempt",
-                "sn",
                 "vrf",
+                "siteName",
                 "active",
+                "group",
+                "id",
+                "priority",
+                "state",
                 "version",
                 "protocol",
-                "state",
-                "id",
+                "sn",
+                "virtualIpv6",
                 "count",
-                "priority"
+                "secondaryVirtualIpAddresses",
+                "preempt",
+                "hostname",
+                "standby",
+                "intName",
+                "virtualIp"
             ],
             "description": "HSRP/VRRP/GLBP Group State - detailed gateway inventory",
             "summary": "HSRP/VRRP/GLBP Group State",
             "web_endpoint": "/technology/fhrp/group-state"
         }
     },
     "tables/fhrp/stproot-alignment": {
         "api_endpoint": "/tables/fhrp/stproot-alignment",
         "get": null,
         "post": {
             "api_endpoint": "tables/fhrp/stproot-alignment",
             "columns": [
                 "siteName",
-                "hostname",
-                "sn",
                 "id",
+                "sn",
                 "count",
+                "hostname",
                 "vlans"
             ],
             "description": "Misaligned FHRP Gateways with STP Root",
             "summary": "FHRP Gateway and STP Root Aligment",
             "web_endpoint": "/technology/fhrp/active-gw-root-alignment"
         }
     },
     "tables/fhrp/virtual-gateways": {
         "api_endpoint": "/tables/fhrp/virtual-gateways",
         "get": null,
         "post": {
             "api_endpoint": "tables/fhrp/virtual-gateways",
             "columns": [
-                "virtualIp",
-                "virtualIpv6",
                 "siteName",
-                "hostname",
-                "intName",
+                "type",
+                "id",
+                "state",
+                "protocol",
                 "sn",
-                "vrf",
                 "virtualMac",
-                "protocol",
-                "state",
-                "type",
-                "id"
+                "virtualIpv6",
+                "vrf",
+                "hostname",
+                "intName",
+                "virtualIp"
             ],
             "description": "Virtual gateways inventory for Arista VARP",
             "summary": "Arista VARP",
             "web_endpoint": "/technology/fhrp/virtual-gateways"
         }
     },
     "tables/global-attributes": {
         "api_endpoint": "/tables/global-attributes",
         "get": null,
         "post": {
             "api_endpoint": "tables/global-attributes",
             "columns": [
-                "hostname",
-                "sn",
-                "name",
                 "id",
-                "value"
+                "name",
+                "sn",
+                "value",
+                "hostname"
             ],
             "description": "Global attributes inventory",
             "summary": "Global Attributes",
             "web_endpoint": null
         }
     },
     "tables/interfaces/connectivity-matrix": {
         "api_endpoint": "/tables/interfaces/connectivity-matrix",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/connectivity-matrix",
             "columns": [
-                "localInt",
+                "localMedia",
                 "siteName",
-                "remoteMedia",
+                "id",
                 "remoteInt",
-                "remoteSn",
-                "localMedia",
+                "localInt",
                 "remoteHost",
                 "localHost",
                 "protocol",
-                "localSn",
-                "id"
+                "remoteSn",
+                "remoteMedia",
+                "localSn"
             ],
             "description": "Logical and physical connectivity matrix for variety of protocols",
             "summary": "Connectivity matrix",
             "web_endpoint": "/technology/interfaces/connectivity-matrix/connectivity-matrix"
         }
     },
     "tables/interfaces/connectivity-matrix/unmanaged-neighbors/detail": {
         "api_endpoint": "/tables/interfaces/connectivity-matrix/unmanaged-neighbors/detail",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/connectivity-matrix/unmanaged-neighbors/detail",
             "columns": [
-                "localAddress",
-                "hostname",
-                "intName",
                 "siteName",
-                "subnet",
-                "sn",
-                "protocol",
+                "neiIpV6",
+                "localAddress",
+                "id",
                 "devType",
+                "localAddressV6",
                 "neiIp",
-                "id",
-                "source"
+                "protocol",
+                "sn",
+                "source",
+                "hostname",
+                "subnet",
+                "intName"
             ],
             "description": "Details for unmanaged neighbors detected via variety of protocols",
             "summary": "Unmanaged Neighbors Detail",
             "web_endpoint": "/technology/interfaces/connectivity-matrix/unmanaged-neighbors-detail"
         }
     },
     "tables/interfaces/connectivity-matrix/unmanaged-neighbors/summary": {
         "api_endpoint": "/tables/interfaces/connectivity-matrix/unmanaged-neighbors/summary",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/connectivity-matrix/unmanaged-neighbors/summary",
             "columns": [
-                "xdpNeiCount",
-                "siteName",
-                "neighbor",
-                "sn",
+                "id",
+                "ipv6",
+                "ospfNeiCount",
                 "capabilities",
-                "ripNeiCount",
-                "eigrpNeiCount",
-                "ldpNeiCount",
-                "ip",
                 "cefPrfx",
-                "isisNeiCount",
-                "bgpNeiCount",
-                "bgpNeiAsn",
+                "ldpNeiCount",
                 "hostname",
                 "bgpReceivedPfx",
+                "isisNeiCount",
+                "bgpNeiAsn",
+                "sn",
                 "cefNeiCount",
-                "ospfNeiCount",
+                "eigrpNeiCount",
+                "xdpNeiCount",
+                "ip",
+                "siteName",
+                "ripNeiCount",
+                "neighbor",
                 "ospfv3NeiCount",
-                "id"
+                "bgpNeiCount"
             ],
             "description": "Summary for unmanaged neighbors detected via variety of protocols",
             "summary": "Unmanaged Neighbors Summary",
             "web_endpoint": "/technology/interfaces/connectivity-matrix/unmanaged-neighbors-summary"
         }
     },
     "tables/interfaces/counters/inbound": {
         "api_endpoint": "/tables/interfaces/counters/inbound",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/counters/inbound",
             "columns": [
-                "inGiants",
-                "inNoBuffer",
-                "hostname",
-                "inBytes",
-                "intName",
                 "inMcast",
+                "inBytes",
+                "inErr",
+                "inNoBuffer",
                 "siteName",
-                "inStompedCrc",
+                "inBcast",
+                "id",
+                "inGiants",
+                "inDrops",
+                "inCrc",
                 "inPkts",
-                "inRunts",
                 "sn",
-                "inCrc",
                 "inOverrun",
-                "inErr",
-                "inDrops",
-                "id",
-                "inBcast"
+                "inRunts",
+                "inStompedCrc",
+                "hostname",
+                "intName"
             ],
             "description": "Interfaces inbound counters - absolute values",
             "summary": "Interfaces Counters - Inbound",
             "web_endpoint": "/technology/interfaces/counters/inbound"
         }
     },
     "tables/interfaces/counters/outbound": {
         "api_endpoint": "/tables/interfaces/counters/outbound",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/counters/outbound",
             "columns": [
-                "outBytes",
                 "siteName",
-                "hostname",
-                "intName",
-                "outBabble",
-                "outDrops",
-                "outErr",
-                "outLateCollisions",
-                "sn",
                 "outCollisions",
-                "outMcast",
-                "outBufferDrop",
-                "outLostCarrier",
                 "outDeferred",
-                "outPkts",
-                "outNoCarrier",
+                "outErr",
                 "id",
-                "outBcast"
+                "outLostCarrier",
+                "outBufferDrop",
+                "sn",
+                "outDrops",
+                "outNoCarrier",
+                "outPkts",
+                "outBytes",
+                "outBcast",
+                "outLateCollisions",
+                "outMcast",
+                "hostname",
+                "intName",
+                "outBabble"
             ],
             "description": "Interfaces outbound counters - absolute values",
             "summary": "Interfaces Counters - Oubound",
             "web_endpoint": "/technology/interfaces/counters/outbound"
         }
     },
     "tables/interfaces/drops/bidirectional": {
         "api_endpoint": "/tables/interfaces/drops/bidirectional",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/drops/bidirectional",
             "columns": [
                 "siteName",
-                "hostname",
-                "dropsRate",
+                "bytesRate",
+                "id",
                 "dropsPktsPct",
-                "intName",
                 "sn",
                 "impactDrops",
-                "bytesRate",
-                "id"
+                "dropsRate",
+                "hostname",
+                "intName"
             ],
             "description": "Input and Output interface drops combined providing a bidirectional view of drops on an interface",
             "summary": "Bidirectional Interface Drops",
             "web_endpoint": "/technology/interfaces/drop-rates/bidirectional"
         }
     },
     "tables/interfaces/drops/bidirectional-device": {
         "api_endpoint": "/tables/interfaces/drops/bidirectional-device",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/drops/bidirectional-device",
             "columns": [
                 "siteName",
-                "hostname",
-                "dropsRate",
+                "bytesRate",
+                "id",
                 "dropsPktsPct",
                 "sn",
                 "impactDrops",
-                "bytesRate",
-                "id"
+                "dropsRate",
+                "hostname"
             ],
             "description": "Input and Output drops of all interfaces on a device combined proviing a per-device view of bidirectional interface drops",
             "summary": "Per-Device Bidirectional Interface Drops",
             "web_endpoint": "/technology/interfaces/drop-rates/device-bidirectional"
         }
     },
     "tables/interfaces/drops/inbound": {
         "api_endpoint": "/tables/interfaces/drops/inbound",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/drops/inbound",
             "columns": [
-                "siteName",
-                "hostname",
-                "intName",
-                "inDropsRate",
-                "sn",
                 "inDropsPktsPct",
+                "inDropsRate",
+                "siteName",
+                "id",
                 "inImpactDrops",
+                "sn",
+                "hostname",
                 "inBytesRate",
-                "id"
+                "intName"
             ],
             "description": "Input interface drops represent packet loss caused by input buffer overflow",
             "summary": "Inbound Interface Drops",
             "web_endpoint": "/technology/interfaces/drop-rates/inbound"
         }
     },
     "tables/interfaces/drops/inbound-device": {
         "api_endpoint": "/tables/interfaces/drops/inbound-device",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/drops/inbound-device",
             "columns": [
-                "siteName",
-                "hostname",
-                "inDropsRate",
-                "sn",
                 "inDropsPktsPct",
+                "inDropsRate",
+                "siteName",
+                "id",
                 "inImpactDrops",
-                "inBytesRate",
-                "id"
+                "sn",
+                "hostname",
+                "inBytesRate"
             ],
             "description": "Input drops of all interfaces on a device combined providing a per-device view of input interface drops",
             "summary": "Per-Device Inbound Interface Drops",
             "web_endpoint": "/technology/interfaces/drop-rates/device-inbound"
         }
     },
     "tables/interfaces/drops/outbound": {
         "api_endpoint": "/tables/interfaces/drops/outbound",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/drops/outbound",
             "columns": [
+                "outDropsPktsPct",
                 "siteName",
-                "hostname",
-                "intName",
-                "outImpactDrops",
+                "id",
                 "outBytesRate",
                 "sn",
                 "outDropsRate",
-                "outDropsPktsPct",
-                "id"
+                "outImpactDrops",
+                "hostname",
+                "intName"
             ],
             "description": "Output interface drops represent outbound packet loss",
             "summary": "Outbound Interface Drops",
             "web_endpoint": "/technology/interfaces/drop-rates/outbound"
         }
     },
     "tables/interfaces/drops/outbound-device": {
         "api_endpoint": "/tables/interfaces/drops/outbound-device",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/drops/outbound-device",
             "columns": [
+                "outDropsPktsPct",
                 "siteName",
-                "hostname",
-                "outImpactDrops",
+                "id",
                 "outBytesRate",
                 "sn",
                 "outDropsRate",
-                "outDropsPktsPct",
-                "id"
+                "outImpactDrops",
+                "hostname"
             ],
             "description": "Output drops of all interfaces on a device combined providing a per-device view of output interface drops",
             "summary": "Per-Device Outbound Interface Drops",
             "web_endpoint": "/technology/interfaces/drop-rates/device-outbound"
         }
     },
     "tables/interfaces/duplex": {
         "api_endpoint": "/tables/interfaces/duplex",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/duplex",
             "columns": [
-                "siteName",
-                "remoteMedia",
+                "localMedia",
                 "remoteIntName",
+                "siteName",
+                "id",
                 "localIntName",
+                "localHostname",
                 "remoteSn",
                 "remoteHostname",
-                "localMedia",
+                "localDuplex",
+                "remoteMedia",
                 "localSn",
                 "status",
-                "localHostname",
-                "localDuplex",
-                "id",
                 "remoteDuplex"
             ],
             "description": "Interface connectivity matrix including duplex information",
             "summary": "Duplex interface matrix",
             "web_endpoint": "/technology/interfaces/duplex"
         }
     },
     "tables/interfaces/errors/bidirectional": {
         "api_endpoint": "/tables/interfaces/errors/bidirectional",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/errors/bidirectional",
             "columns": [
-                "errRate",
-                "siteName",
-                "hostname",
-                "intName",
                 "errPktsPct",
-                "sn",
+                "siteName",
                 "bytesRate",
+                "id",
+                "sn",
                 "impactErr",
-                "id"
+                "errRate",
+                "hostname",
+                "intName"
             ],
             "description": "Sum of inbound and outbound interface error impacts to provide a bidirectional view of overall impact of errors on an interface",
             "summary": "Bidirectional Interface Errors",
             "web_endpoint": "/technology/interfaces/error-rates/bidirectional"
         }
     },
     "tables/interfaces/errors/bidirectional-device": {
         "api_endpoint": "/tables/interfaces/errors/bidirectional-device",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/errors/bidirectional-device",
             "columns": [
-                "errRate",
-                "siteName",
-                "hostname",
                 "errPktsPct",
-                "sn",
+                "siteName",
                 "bytesRate",
+                "id",
+                "sn",
                 "impactErr",
-                "id"
+                "errRate",
+                "hostname"
             ],
             "description": "Bidirectional Input and Output errors of all interfaces on each device combined providing a per-device Impact",
             "summary": "Per-Device Bidirectional Interface Errors",
             "web_endpoint": "/technology/interfaces/error-rates/device-bidirectional"
         }
     },
     "tables/interfaces/errors/disabled": {
         "api_endpoint": "/tables/interfaces/errors/disabled",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/errors/disabled",
             "columns": [
                 "siteName",
-                "hostname",
-                "intName",
-                "sn",
                 "errorReason",
-                "id"
+                "id",
+                "sn",
+                "hostname",
+                "intName"
             ],
             "description": "Interfaces in the network which has been automatically disabled due to an error",
             "summary": "Error-Disabled interfaces",
             "web_endpoint": "/technology/interfaces/errdisabled"
         }
     },
     "tables/interfaces/errors/inbound": {
         "api_endpoint": "/tables/interfaces/errors/inbound",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/errors/inbound",
             "columns": [
+                "inErrPktsPct",
                 "siteName",
-                "hostname",
+                "id",
                 "inErrRate",
-                "intName",
                 "sn",
-                "inErrPktsPct",
                 "inImpactErr",
+                "hostname",
                 "inBytesRate",
-                "id"
+                "intName"
             ],
             "description": "Input interface errors represent packet loss caused by input buffer overflow",
             "summary": "Inbound Interface Errors",
             "web_endpoint": "/technology/interfaces/error-rates/inbound"
         }
     },
     "tables/interfaces/errors/inbound-device": {
         "api_endpoint": "/tables/interfaces/errors/inbound-device",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/errors/inbound-device",
             "columns": [
+                "inErrPktsPct",
                 "siteName",
-                "hostname",
+                "id",
                 "inErrRate",
                 "sn",
-                "inErrPktsPct",
                 "inImpactErr",
-                "inBytesRate",
-                "id"
+                "hostname",
+                "inBytesRate"
             ],
             "description": "Input errors of all interfaces on a device combined providing a per-device view of input interface errors",
             "summary": "Per-Device Inbound Interface Errors",
             "web_endpoint": "/technology/interfaces/error-rates/device-inbound"
         }
     },
     "tables/interfaces/errors/outbound": {
         "api_endpoint": "/tables/interfaces/errors/outbound",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/errors/outbound",
             "columns": [
                 "outErrPktsPct",
                 "siteName",
-                "hostname",
-                "intName",
-                "outErrRate",
+                "id",
                 "outBytesRate",
-                "sn",
                 "outImpactErr",
-                "id"
+                "sn",
+                "outErrRate",
+                "hostname",
+                "intName"
             ],
             "description": "Output interface errors represent outbound packet loss",
             "summary": "Outbound Interface Errors",
             "web_endpoint": "/technology/interfaces/error-rates/outbound"
         }
     },
     "tables/interfaces/errors/outbound-device": {
         "api_endpoint": "/tables/interfaces/errors/outbound-device",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/errors/outbound-device",
             "columns": [
                 "outErrPktsPct",
                 "siteName",
-                "hostname",
-                "outErrRate",
+                "id",
                 "outBytesRate",
-                "sn",
                 "outImpactErr",
-                "id"
+                "sn",
+                "outErrRate",
+                "hostname"
             ],
             "description": "Output errors of all interfaces on a device combined providing a per-device view of output interface errors",
             "summary": "Per-Device Outbound Interface Errors",
             "web_endpoint": "/technology/interfaces/error-rates/device-outbound"
         }
     },
     "tables/interfaces/inconsistencies/details": {
         "api_endpoint": "/tables/interfaces/inconsistencies/details",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/inconsistencies/details",
             "columns": [
                 "siteName",
-                "hostname",
-                "intName",
-                "vlanId",
+                "id",
                 "sn",
-                "id"
+                "vlanId",
+                "hostname",
+                "intName"
             ],
             "description": "VLANs that are not configured in any STP instance - detailed view",
             "summary": "VLANs without STP instance - Detail",
             "web_endpoint": "/technology/spanning-tree/inconsistencies/vlans-no-stp/detail"
         }
     },
     "tables/interfaces/inconsistencies/summary": {
         "api_endpoint": "/tables/interfaces/inconsistencies/summary",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/inconsistencies/summary",
             "columns": [
-                "vlanCount",
-                "hostname",
                 "siteName",
+                "id",
+                "vlanCount",
                 "sn",
-                "id"
+                "hostname"
             ],
             "description": "VLANs that are not configured in any STP instance - summary view",
             "summary": "VLANs without STP instance - Summary",
             "web_endpoint": "/technology/spanning-tree/inconsistencies/vlans-no-stp/summary"
         }
     },
     "tables/interfaces/load/bidirectional": {
         "api_endpoint": "/tables/interfaces/load/bidirectional",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/load/bidirectional",
             "columns": [
                 "siteName",
-                "hostname",
-                "intName",
+                "id",
                 "pkts",
-                "bytes",
                 "sn",
-                "interval",
-                "id"
+                "hostname",
+                "bytes",
+                "intName",
+                "interval"
             ],
             "description": "Interfaces Bidirectional load inventory",
             "summary": "Interfaces Bidirectional load",
             "web_endpoint": "/technology/interfaces/rate/bidirectional"
         }
     },
     "tables/interfaces/load/inbound": {
         "api_endpoint": "/tables/interfaces/load/inbound",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/load/inbound",
             "columns": [
-                "siteName",
-                "hostname",
                 "inBytes",
-                "intName",
+                "siteName",
+                "id",
                 "inPkts",
                 "sn",
-                "interval",
-                "id"
+                "hostname",
+                "intName",
+                "interval"
             ],
             "description": "Interfaces inbound load inventory",
             "summary": "Interfaces Inbound load",
             "web_endpoint": "/technology/interfaces/rate/inbound"
         }
     },
     "tables/interfaces/load/outbound": {
         "api_endpoint": "/tables/interfaces/load/outbound",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/load/outbound",
             "columns": [
-                "outBytes",
                 "siteName",
-                "hostname",
-                "intName",
+                "id",
                 "sn",
-                "interval",
                 "outPkts",
-                "id"
+                "outBytes",
+                "hostname",
+                "intName",
+                "interval"
             ],
             "description": "Interfaces outbound load inventory",
             "summary": "Interfaces Outbound load",
             "web_endpoint": "/technology/interfaces/rate/outbound"
         }
     },
     "tables/interfaces/mtu": {
         "api_endpoint": "/tables/interfaces/mtu",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/mtu",
             "columns": [
-                "dstSn",
                 "srcDev",
                 "siteName",
+                "layer",
+                "dstMtu",
                 "srcMtu",
-                "dstDev",
-                "dstInt",
+                "id",
                 "srcInt",
-                "dstMtu",
-                "layer",
                 "srcSn",
-                "id"
+                "dstInt",
+                "dstSn",
+                "dstDev"
             ],
             "description": "Interface connectivity matrix including Maximum Transmission Unit (MTU) information",
             "summary": "Maximum Transmission Unit Matrix",
             "web_endpoint": "/technology/interfaces/mtu"
         }
     },
     "tables/interfaces/port-channel/balance/inbound": {
         "api_endpoint": "/tables/interfaces/port-channel/balance/inbound",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/port-channel/balance/inbound",
             "columns": [
                 "siteName",
-                "hostname",
-                "intName",
-                "rate",
-                "sn",
-                "members",
+                "variance",
+                "id",
                 "ratios",
                 "protocol",
-                "id",
-                "variance"
+                "sn",
+                "rate",
+                "hostname",
+                "intName",
+                "members"
             ],
             "description": "Link Aggregation (LAG)/PortChannel/EtherChannel inbound balancing ratios",
             "summary": "Port Link-Aggregation inbound",
             "web_endpoint": "/technology/port-channels/inbound-balancing-table"
         }
     },
     "tables/interfaces/port-channel/balance/outbound": {
         "api_endpoint": "/tables/interfaces/port-channel/balance/outbound",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/port-channel/balance/outbound",
             "columns": [
                 "siteName",
-                "hostname",
-                "intName",
-                "rate",
-                "sn",
-                "members",
+                "variance",
+                "id",
                 "ratios",
                 "protocol",
-                "id",
-                "variance"
+                "sn",
+                "rate",
+                "hostname",
+                "intName",
+                "members"
             ],
             "description": "Link Aggregation (LAG)/PortChannel/EtherChannel outbound balancing ratios",
             "summary": "Port Link-Aggregation Outbound",
             "web_endpoint": "/technology/port-channels/outbound-balancing-table"
         }
     },
     "tables/interfaces/port-channel/member-status": {
         "api_endpoint": "/tables/interfaces/port-channel/member-status",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/port-channel/member-status",
             "columns": [
                 "siteName",
-                "hostname",
-                "intName",
-                "sn",
-                "members",
+                "id",
                 "mlagId",
                 "protocol",
-                "id"
+                "sn",
+                "hostname",
+                "intName",
+                "members"
             ],
             "description": "State of each link-aggregation member for all configured Link Aggregation (LAG)/PortChannels/EtherChannels",
             "summary": "Port Link-Aggregation Member Status",
             "web_endpoint": "/technology/port-channels/member-status-table"
         }
     },
     "tables/interfaces/pppoe": {
         "api_endpoint": "/tables/interfaces/pppoe",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/pppoe",
             "columns": [
+                "total",
                 "siteName",
+                "other",
                 "forwarded",
-                "intName",
-                "hostname",
-                "total",
-                "sn",
+                "id",
                 "local",
-                "other",
-                "id"
+                "sn",
+                "hostname",
+                "intName"
             ],
             "description": "Point-to-Point Protocol over Ethernet (PPPoE) interfaces inventory",
             "summary": "PPPoE interfaces",
             "web_endpoint": "/technology/interfaces/pppoe/interfaces"
         }
     },
     "tables/interfaces/pppoe/sessions": {
         "api_endpoint": "/tables/interfaces/pppoe/sessions",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/pppoe/sessions",
             "columns": [
-                "framedIp",
-                "identity",
-                "siteName",
+                "id",
                 "inPktsRate",
-                "sn",
-                "pppMaxPayload",
-                "localIntName",
+                "framedIp",
+                "virtualAccessIntName",
+                "outPktsRate",
+                "outIntName",
+                "outQosPolicy",
+                "hostname",
                 "inBytesRate",
                 "sessionId",
-                "hostname",
                 "isStaticRoute",
-                "virtualAccessIntName",
-                "outPktsRate",
+                "localIntName",
                 "inQosPolicy",
-                "outBytesRate",
                 "state",
-                "outIntName",
-                "outQosPolicy",
-                "id"
+                "sn",
+                "identity",
+                "siteName",
+                "outBytesRate",
+                "pppMaxPayload"
             ],
             "description": "Point-to-Point Protocol over Ethernet (PPPoE) interface sessions inventory",
             "summary": "PPPoE sessions",
             "web_endpoint": "/technology/interfaces/pppoe/sessions"
         }
     },
     "tables/interfaces/storm-control/all": {
         "api_endpoint": "/tables/interfaces/storm-control/all",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/storm-control/all",
             "columns": [
-                "lowerLimit",
+                "unit",
                 "currentTraffic",
-                "action",
-                "hostname",
-                "intName",
                 "siteName",
-                "snmpTrap",
+                "lowerLimit",
                 "upperLimit",
-                "sn",
-                "changes",
+                "id",
                 "state",
-                "unit",
                 "logUpperLimit",
-                "id"
+                "changes",
+                "sn",
+                "action",
+                "snmpTrap",
+                "hostname",
+                "intName"
             ],
             "description": "Details for storm control traffic detection - all traffic",
             "summary": "Storm Control - All Traffic",
             "web_endpoint": "/technology/interfaces/storm-control/all-traffic"
         }
     },
     "tables/interfaces/storm-control/broadcast": {
         "api_endpoint": "/tables/interfaces/storm-control/broadcast",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/storm-control/broadcast",
             "columns": [
-                "lowerLimit",
+                "unit",
                 "currentTraffic",
-                "action",
-                "hostname",
-                "intName",
                 "siteName",
-                "snmpTrap",
+                "lowerLimit",
                 "upperLimit",
-                "sn",
-                "changes",
+                "id",
                 "state",
-                "unit",
                 "logUpperLimit",
-                "id"
+                "changes",
+                "sn",
+                "action",
+                "snmpTrap",
+                "hostname",
+                "intName"
             ],
             "description": "Details for storm control traffic detection - broadcast",
             "summary": "Storm Control - Broadcast",
             "web_endpoint": "/technology/interfaces/storm-control/broadcast"
         }
     },
     "tables/interfaces/storm-control/multicast": {
         "api_endpoint": "/tables/interfaces/storm-control/multicast",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/storm-control/multicast",
             "columns": [
-                "lowerLimit",
+                "unit",
                 "currentTraffic",
-                "action",
-                "hostname",
-                "intName",
                 "siteName",
-                "snmpTrap",
+                "lowerLimit",
                 "upperLimit",
-                "sn",
-                "changes",
+                "id",
                 "state",
-                "unit",
                 "logUpperLimit",
-                "id"
+                "changes",
+                "sn",
+                "action",
+                "snmpTrap",
+                "hostname",
+                "intName"
             ],
             "description": "Details for storm control traffic detection - unicast",
             "summary": "Storm Control - Unicast",
             "web_endpoint": "/technology/interfaces/storm-control/multicast"
         }
     },
     "tables/interfaces/storm-control/unicast": {
         "api_endpoint": "/tables/interfaces/storm-control/unicast",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/storm-control/unicast",
             "columns": [
-                "lowerLimit",
+                "unit",
                 "currentTraffic",
-                "action",
-                "hostname",
-                "intName",
                 "siteName",
-                "snmpTrap",
+                "lowerLimit",
                 "upperLimit",
-                "sn",
-                "changes",
+                "id",
                 "state",
-                "unit",
                 "logUpperLimit",
-                "id"
+                "changes",
+                "sn",
+                "action",
+                "snmpTrap",
+                "hostname",
+                "intName"
             ],
             "description": "Details for storm control traffic detection - multicast",
             "summary": "Storm Control - Multicast",
             "web_endpoint": "/technology/interfaces/storm-control/unicast"
         }
     },
     "tables/interfaces/switchports": {
         "api_endpoint": "/tables/interfaces/switchports",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/switchports",
             "columns": [
-                "mode",
-                "nativeVlan",
+                "macCount",
                 "siteName",
-                "hostname",
-                "intName",
                 "dscr",
-                "sn",
-                "voiceVlan",
+                "id",
+                "trunkVlan",
                 "dynamicMacCount",
+                "mode",
+                "devType",
                 "edge",
+                "sn",
                 "staticMacCount",
-                "trunkVlan",
+                "voiceVlan",
                 "encap",
-                "macCount",
+                "nativeVlan",
                 "accVlan",
-                "devType",
-                "id"
+                "hostname",
+                "intName"
             ],
             "description": "Overview of all L2 Ethernet switchports",
             "summary": "Interfaces Switchport",
             "web_endpoint": "/technology/interfaces/switchport"
         }
     },
     "tables/interfaces/transceivers/errors": {
         "api_endpoint": "/tables/interfaces/transceivers/errors",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/transceivers/errors",
             "columns": [
                 "siteName",
-                "intName",
-                "hostname",
                 "pn",
+                "id",
+                "errorLane",
                 "errorMessage",
                 "sn",
-                "id",
-                "errorLane"
+                "hostname",
+                "intName"
             ],
             "description": "Information oninterfaces transceivers errors messages and thresholds",
             "summary": "Transceivers Errors",
             "web_endpoint": "/technology/interfaces/transceivers/errors"
         }
     },
     "tables/interfaces/transceivers/inventory": {
         "api_endpoint": "/tables/interfaces/transceivers/inventory",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/transceivers/inventory",
             "columns": [
-                "paramsList",
-                "tSn",
+                "tVendor",
                 "siteName",
-                "hostname",
-                "intName",
-                "pn",
                 "dscr",
+                "paramsList",
+                "pn",
+                "id",
+                "type",
                 "sn",
-                "l2",
                 "l1",
-                "tVendor",
-                "type",
-                "id"
+                "l2",
+                "tSn",
+                "hostname",
+                "intName"
             ],
             "description": "Interface transceivers inventory",
             "summary": "Transceivers Inventory",
             "web_endpoint": "/technology/interfaces/transceivers/inventory"
         }
     },
     "tables/interfaces/transceivers/statistics": {
         "api_endpoint": "/tables/interfaces/transceivers/statistics",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/transceivers/statistics",
             "columns": [
-                "deltaValueLow",
-                "siteName",
-                "sn",
+                "unit",
+                "statistic",
+                "pn",
+                "type",
+                "id",
+                "intName",
                 "vendor",
+                "tVendor",
+                "family",
+                "platform",
+                "thresholdLow",
+                "laneOrigIntName",
+                "hostname",
+                "flag",
+                "dscr",
                 "threshold",
+                "sn",
+                "deltaValueLow",
                 "lane",
-                "unit",
                 "model",
+                "siteName",
                 "deltaValueHigh",
-                "thresholdHigh",
-                "thresholdLow",
                 "value",
-                "hostname",
-                "intName",
-                "statistic",
-                "platform",
-                "tVendor",
-                "type",
-                "laneOrigIntName",
-                "pn",
-                "dscr",
-                "flag",
-                "family",
-                "id"
+                "thresholdHigh"
             ],
             "description": "Interface transceivers statistics",
             "summary": "Transceivers Statistics",
             "web_endpoint": "/technology/interfaces/transceivers/statistics"
         }
     },
     "tables/interfaces/transceivers/thresholds": {
         "api_endpoint": "/tables/interfaces/transceivers/thresholds",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/transceivers/thresholds",
             "columns": [
+                "lane",
                 "siteName",
-                "hostname",
-                "intName",
-                "level",
                 "pn",
-                "flag",
-                "sn",
-                "name",
-                "lane",
                 "type",
-                "id"
+                "id",
+                "level",
+                "name",
+                "sn",
+                "hostname",
+                "flag",
+                "intName"
             ],
             "description": "Interface transceivers triggered thresholds",
             "summary": "Transceivers Triggered Thresholds",
             "web_endpoint": "/technology/interfaces/transceivers/triggered-thresholds"
         }
     },
     "tables/interfaces/transfer-rates/bidirectional": {
         "api_endpoint": "/tables/interfaces/transfer-rates/bidirectional",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/transfer-rates/bidirectional",
             "columns": [
+                "pktsRate",
+                "bcastRate",
+                "bytesRate",
                 "mcastRate",
-                "impactLoss",
                 "siteName",
-                "hostname",
-                "intName",
+                "id",
                 "sn",
-                "bcastRate",
-                "pktsRate",
-                "bytesRate",
-                "id"
+                "impactLoss",
+                "hostname",
+                "intName"
             ],
             "description": "Bidirectional interface rates and cumulative loss impact",
             "summary": "Bidirectional Interface Rates",
             "web_endpoint": "/technology/interfaces/transfer-rates/bidirectional"
         }
     },
     "tables/interfaces/transfer-rates/bidirectional-device": {
         "api_endpoint": "/tables/interfaces/transfer-rates/bidirectional-device",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/transfer-rates/bidirectional-device",
             "columns": [
+                "pktsRate",
+                "bcastRate",
+                "bytesRate",
                 "mcastRate",
-                "impactLoss",
                 "siteName",
-                "hostname",
+                "id",
                 "sn",
-                "bcastRate",
-                "pktsRate",
-                "bytesRate",
-                "id"
+                "impactLoss",
+                "hostname"
             ],
             "description": "Per-Device bidirectional transfer rates and cumulative loss impact",
             "summary": "Per-Device Bidirectional Transfer Rates",
             "web_endpoint": "/technology/interfaces/transfer-rates/device-bidirectional"
         }
     },
     "tables/interfaces/transfer-rates/inbound": {
         "api_endpoint": "/tables/interfaces/transfer-rates/inbound",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/transfer-rates/inbound",
             "columns": [
+                "inBcastRate",
                 "siteName",
-                "hostname",
-                "intName",
+                "id",
                 "inImpactLoss",
-                "inPktsRate",
                 "sn",
-                "inBcastRate",
-                "inMcastRate",
+                "inPktsRate",
+                "intName",
+                "hostname",
                 "inBytesRate",
-                "id"
+                "inMcastRate"
             ],
             "description": "Inbound interface rates and cumulative loss impact",
             "summary": "Inbound Interface Transfer Rates",
             "web_endpoint": "/technology/interfaces/transfer-rates/inbound"
         }
     },
     "tables/interfaces/transfer-rates/inbound-device": {
         "api_endpoint": "/tables/interfaces/transfer-rates/inbound-device",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/transfer-rates/inbound-device",
             "columns": [
+                "inBcastRate",
                 "siteName",
-                "hostname",
+                "id",
                 "inImpactLoss",
-                "inPktsRate",
                 "sn",
-                "inBcastRate",
-                "inMcastRate",
+                "inPktsRate",
+                "hostname",
                 "inBytesRate",
-                "id"
+                "inMcastRate"
             ],
             "description": "Per-Device inbound interface transfer rates and cumulative loss impact",
             "summary": "Per-Device Inbound Interface Transfer Rates",
             "web_endpoint": "/technology/interfaces/transfer-rates/device-inbound"
         }
     },
     "tables/interfaces/transfer-rates/outbound": {
         "api_endpoint": "/tables/interfaces/transfer-rates/outbound",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/transfer-rates/outbound",
             "columns": [
-                "outPktsRate",
-                "hostname",
-                "intName",
+                "outMcastRate",
                 "siteName",
+                "outPktsRate",
+                "id",
                 "outBytesRate",
-                "sn",
-                "outImpactLoss",
-                "outMcastRate",
                 "outBcastRate",
-                "id"
+                "outImpactLoss",
+                "sn",
+                "hostname",
+                "intName"
             ],
             "description": "Outbound interface rates and cumulative loss impact",
             "summary": "Outbound Interface Transfer Rates",
             "web_endpoint": "/technology/interfaces/transfer-rates/outbound"
         }
     },
     "tables/interfaces/transfer-rates/outbound-device": {
         "api_endpoint": "/tables/interfaces/transfer-rates/outbound-device",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/transfer-rates/outbound-device",
             "columns": [
-                "outPktsRate",
-                "hostname",
+                "outMcastRate",
                 "siteName",
+                "outPktsRate",
+                "id",
                 "outBytesRate",
-                "sn",
-                "outImpactLoss",
-                "outMcastRate",
                 "outBcastRate",
-                "id"
+                "outImpactLoss",
+                "sn",
+                "hostname"
             ],
             "description": "Per-Device outbound interface transfer rates and cumulative loss impact",
             "summary": "Per-Device Outbound Interface Transfer Rates",
             "web_endpoint": "/technology/interfaces/transfer-rates/device-outbound"
         }
     },
     "tables/interfaces/tunnels/ipv4": {
         "api_endpoint": "/tables/interfaces/tunnels/ipv4",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/tunnels/ipv4",
             "columns": [
-                "tunnelSrcIp",
-                "tunnelProto",
-                "siteName",
-                "hostname",
-                "intName",
-                "tunnelDstIp",
-                "sn",
-                "vrf",
                 "tunnelSrcIntName",
                 "tunnelVrf",
+                "siteName",
+                "id",
+                "tunnelProto",
+                "sn",
                 "ipAddresses",
-                "id"
+                "tunnelDstIp",
+                "vrf",
+                "hostname",
+                "intName",
+                "tunnelSrcIp"
             ],
             "description": "IPv4 Tunnels inventory",
             "summary": "IPv4 Tunnels",
             "web_endpoint": "/technology/interfaces/tunnels/ipv4"
         }
     },
     "tables/interfaces/tunnels/ipv6": {
         "api_endpoint": "/tables/interfaces/tunnels/ipv6",
         "get": null,
         "post": {
             "api_endpoint": "tables/interfaces/tunnels/ipv6",
             "columns": [
-                "tunnelProto",
-                "siteName",
-                "hostname",
-                "intName",
-                "sn",
-                "vrf",
+                "tunnelDstIpv6",
                 "tunnelSrcIntName",
                 "tunnelVrf",
+                "siteName",
                 "ipv6Addresses",
-                "tunnelDstIpv6",
+                "id",
+                "tunnelProto",
                 "tunnelSrcIpv6",
-                "id"
+                "sn",
+                "vrf",
+                "hostname",
+                "intName"
             ],
             "description": "IPv6 Tunnels inventory",
             "summary": "IPv6 Tunnels",
             "web_endpoint": "/technology/interfaces/tunnels/ipv6"
         }
     },
     "tables/inventory/devices": {
         "api_endpoint": "/tables/inventory/devices",
         "get": null,
         "post": {
             "api_endpoint": "tables/inventory/devices",
             "columns": [
-                "loginIp",
-                "siteName",
-                "domain",
-                "sn",
-                "processor",
-                "vendor",
-                "loginType",
-                "loginPort",
-                "hostnameProcessed",
-                "objectId",
                 "slug",
-                "model",
+                "icon",
+                "id",
+                "taskKey",
                 "uptime",
-                "rd",
-                "snHw",
-                "reload",
+                "processor",
                 "version",
-                "mac",
-                "image",
                 "memoryTotalBytes",
-                "taskKey",
-                "hostname",
+                "vendor",
+                "family",
                 "platform",
+                "snHw",
                 "memoryUsedBytes",
+                "loginIp",
                 "fqdn",
-                "icon",
                 "stpDomain",
-                "family",
-                "configReg",
-                "memoryUtilization",
+                "domain",
+                "hostname",
+                "image",
                 "hostnameOriginal",
+                "reload",
+                "sn",
+                "memoryUtilization",
+                "hostnameProcessed",
+                "loginPort",
+                "model",
+                "siteName",
+                "objectId",
+                "rd",
                 "devType",
-                "id"
+                "loginType",
+                "mac",
+                "configReg"
             ],
             "description": "Inventory of all logical or physical managed network infrastructure devices discovered",
             "summary": "Device Inventory",
             "web_endpoint": "/inventory/devices"
         }
     },
     "tables/inventory/discovery-history": {
         "api_endpoint": "/tables/inventory/discovery-history",
         "get": null,
         "post": {
             "api_endpoint": "tables/inventory/discovery-history",
             "columns": [
+                "id",
+                "usernameNotes",
                 "loginIp",
-                "hostname",
                 "sn",
                 "loginType",
-                "username",
-                "usernameNotes",
                 "ts",
-                "id"
+                "hostname",
+                "username"
             ],
             "description": "This view shows all discovered devices in history (no matter which snapshot is selected). IP Fabric will remember used protocol and last successful credential. These informations are preferred in the next discovery run.",
             "summary": "Discovery History",
             "web_endpoint": "/management/discovery-history"
         }
     },
     "tables/inventory/fans": {
         "api_endpoint": "/tables/inventory/fans",
         "get": null,
         "post": {
             "api_endpoint": "tables/inventory/fans",
             "columns": [
-                "siteName",
-                "hostname",
                 "deviceId",
-                "sn",
-                "fanSn",
-                "fanPid",
+                "siteName",
+                "fanId",
                 "fanState",
                 "id",
+                "sn",
                 "fanName",
-                "fanId"
+                "hostname",
+                "fanPid",
+                "fanSn"
             ],
             "description": "Fans detected in all network devices and their current state",
             "summary": "Environment - Fans",
             "web_endpoint": "/technology/platforms/environment/fans"
         }
     },
     "tables/inventory/interfaces": {
         "api_endpoint": "/tables/inventory/interfaces",
         "get": null,
         "post": {
             "api_endpoint": "tables/inventory/interfaces",
             "columns": [
-                "loginIp",
-                "siteName",
-                "sn",
-                "loginType",
-                "transceiverSn",
                 "slug",
-                "l1",
-                "duplex",
-                "reason",
-                "mtu",
-                "mac",
-                "errDisabled",
-                "media",
-                "transceiverPn",
-                "hostname",
-                "intName",
-                "nameOriginal",
-                "primaryIp",
-                "rel",
                 "speedValue",
-                "speed",
                 "id",
-                "hasTransceiver",
-                "speedType",
+                "nameOriginal",
+                "intName",
+                "transceiverPn",
+                "loginIp",
+                "l1",
+                "l2",
+                "rel",
+                "hostname",
                 "transceiverType",
+                "speed",
+                "duplex",
                 "dscr",
+                "primaryIp",
+                "mtu",
+                "transceiverSn",
                 "intNameAlias",
-                "l2"
+                "sn",
+                "hasTransceiver",
+                "siteName",
+                "media",
+                "speedType",
+                "loginType",
+                "reason",
+                "mac",
+                "errDisabled"
             ],
             "description": "Information on every detected physical or logical interface for all discovered devices",
             "summary": "Interface Inventory",
             "web_endpoint": "/inventory/interfaces"
         }
     },
     "tables/inventory/modules": {
         "api_endpoint": "/tables/inventory/modules",
         "get": null,
         "post": {
             "api_endpoint": "tables/inventory/modules",
             "columns": [
-                "siteName",
-                "hostname",
                 "deviceId",
-                "moduleId",
-                "sn",
-                "moduleState",
+                "modulePid",
+                "siteName",
                 "id",
-                "modulePid"
+                "moduleState",
+                "sn",
+                "moduleId",
+                "hostname"
             ],
             "description": "Information about every detected modules and their current the state",
             "summary": "Environment - Modules",
             "web_endpoint": "/technology/platforms/environment/modules"
         }
     },
     "tables/inventory/phones": {
         "api_endpoint": "/tables/inventory/phones",
         "get": null,
         "post": {
             "api_endpoint": "tables/inventory/phones",
             "columns": [
-                "phoneName",
-                "userMac",
+                "phoneInt",
                 "siteName",
-                "userIp",
-                "phoneMac",
+                "switchInt",
+                "switchSn",
+                "id",
                 "voiceVlan",
-                "switchHostname",
-                "vendor",
+                "userMac",
                 "phoneIp",
-                "phoneInt",
-                "switchSn",
-                "switchInt",
-                "id"
+                "phoneMac",
+                "phoneName",
+                "vendor",
+                "switchHostname",
+                "userIp"
             ],
             "description": "Inventory of all detected IP phones and endpoints connected to them",
             "summary": "IP Phones and Connected Devices",
             "web_endpoint": "/technology/ip-telephony/phones"
         }
     },
     "tables/inventory/pn": {
         "api_endpoint": "/tables/inventory/pn",
         "get": null,
         "post": {
             "api_endpoint": "tables/inventory/pn",
             "columns": [
-                "siteName",
-                "hostname",
-                "platform",
+                "deviceSn",
                 "deviceId",
+                "model",
+                "siteName",
                 "dscr",
-                "sn",
+                "platform",
+                "id",
                 "name",
-                "vid",
-                "vendor",
+                "sn",
                 "pid",
-                "model",
-                "deviceSn",
-                "id"
+                "vid",
+                "hostname",
+                "vendor"
             ],
             "description": "Modules and part numbers from inventory of network infrastructure devices",
             "summary": "Modules and Part Numbers Inventory",
             "web_endpoint": "/inventory/part-numbers"
         }
     },
     "tables/inventory/power-supplies": {
         "api_endpoint": "/tables/inventory/power-supplies",
         "get": null,
         "post": {
             "api_endpoint": "tables/inventory/power-supplies",
             "columns": [
-                "pwSupplyType",
-                "pwSupplyState",
-                "hostname",
-                "pwSupplyName",
+                "deviceId",
+                "model",
                 "pwSupplyId",
+                "pwSupplyName",
                 "siteName",
-                "deviceId",
-                "pwSupplySn",
+                "pwSupplyPid",
+                "id",
+                "pwSupplyState",
                 "sn",
+                "pwSupplyType",
                 "pwSupplyCircuit",
-                "pwSupplyPid",
-                "model",
-                "id"
+                "hostname",
+                "pwSupplySn"
             ],
             "description": "Power supplies detected in all network devices and their current state",
             "summary": "Environment - Power Supplies",
             "web_endpoint": "/technology/platforms/environment/power-supplies"
         }
     },
     "tables/inventory/power-supplies-fans": {
         "api_endpoint": "/tables/inventory/power-supplies-fans",
         "get": null,
         "post": {
             "api_endpoint": "tables/inventory/power-supplies-fans",
             "columns": [
-                "fanVendor",
-                "hostname",
-                "siteName",
                 "deviceId",
-                "sn",
-                "fanSn",
+                "siteName",
+                "fanId",
                 "fanState",
                 "id",
+                "sn",
+                "fanVendor",
                 "fanName",
-                "fanId"
+                "hostname",
+                "fanSn"
             ],
             "description": "Power supplies fans detected in all network devices and their current state",
             "summary": "Environment - Power Supplies Fans",
             "web_endpoint": "/technology/platforms/environment/power-supplies-fans"
         }
     },
     "tables/inventory/sites": {
         "api_endpoint": "/tables/inventory/sites",
         "get": null,
         "post": {
             "api_endpoint": "tables/inventory/sites",
             "columns": [
+                "routersCount",
                 "devicesCount",
                 "rDCount",
-                "stpDCount",
                 "siteName",
-                "routersCount",
-                "rDomains",
-                "networksCount",
-                "usersCount",
-                "vlanCount",
                 "switchesCount",
+                "id",
+                "stpDCount",
+                "vlanCount",
                 "stpDomains",
-                "id"
+                "rDomains",
+                "networksCount",
+                "usersCount"
             ],
             "description": "Sites inventory defined by site separation rules or attributes",
             "summary": "Sites Inventory",
             "web_endpoint": "/inventory/sites/overview"
         }
     },
     "tables/inventory/summary/families": {
         "api_endpoint": "/tables/inventory/summary/families",
         "get": null,
         "post": {
             "api_endpoint": "tables/inventory/summary/families",
             "columns": [
-                "devicesCount",
                 "modelsCount",
                 "platformsCount",
-                "vendor",
+                "devicesCount",
                 "family",
-                "id"
+                "id",
+                "vendor"
             ],
             "description": "Inventory covering vendor - families distribution",
             "summary": "Vendor Families Overview",
             "web_endpoint": "/inventory/devices/families"
         }
     },
     "tables/inventory/summary/models": {
         "api_endpoint": "/tables/inventory/summary/models",
         "get": null,
         "post": {
             "api_endpoint": "tables/inventory/summary/models",
             "columns": [
                 "devicesCount",
-                "platform",
-                "vendor",
-                "model",
                 "family",
-                "id"
+                "model",
+                "platform",
+                "id",
+                "vendor"
             ],
             "description": "Inventory covering vendor - families - platforms - models distribution",
             "summary": "Vendor Models Overview",
             "web_endpoint": "/inventory/devices/models"
         }
     },
     "tables/inventory/summary/platforms": {
         "api_endpoint": "/tables/inventory/summary/platforms",
         "get": null,
         "post": {
             "api_endpoint": "tables/inventory/summary/platforms",
             "columns": [
-                "devicesCount",
                 "modelsCount",
-                "platform",
-                "vendor",
+                "devicesCount",
                 "family",
-                "id"
+                "platform",
+                "id",
+                "vendor"
             ],
             "description": "Inventory covering vendor - families - platforms distribution",
             "summary": "Vendor Platforms Overview",
             "web_endpoint": "/inventory/devices/platforms"
         }
     },
     "tables/inventory/summary/vendors": {
         "api_endpoint": "/tables/inventory/summary/vendors",
         "get": null,
         "post": {
             "api_endpoint": "tables/inventory/summary/vendors",
             "columns": [
-                "devicesCount",
                 "modelsCount",
                 "platformsCount",
+                "devicesCount",
+                "id",
                 "vendor",
-                "familiesCount",
-                "id"
+                "familiesCount"
             ],
             "description": "Inventory covering vendor distribution",
             "summary": "Vendors Overview",
             "web_endpoint": "/inventory/devices/vendors"
         }
     },
     "tables/inventory/temperature-sensors": {
         "api_endpoint": "/tables/inventory/temperature-sensors",
         "get": null,
         "post": {
             "api_endpoint": "tables/inventory/temperature-sensors",
             "columns": [
-                "thermalState",
-                "siteName",
-                "hostname",
                 "deviceId",
-                "sn",
-                "thermalId",
                 "model",
+                "siteName",
+                "thermalId",
                 "id",
+                "sn",
+                "thermalState",
+                "hostname",
                 "thermalDescription"
             ],
             "description": "Status of temperature sensors",
             "summary": "Environment - Temperature sensors",
             "web_endpoint": "/technology/platforms/environment/temperature-sensors"
         }
     },
     "tables/jobs": {
         "api_endpoint": "/tables/jobs",
         "get": null,
         "post": {
             "api_endpoint": "tables/jobs",
             "columns": [
+                "status",
                 "finishedAt",
+                "isDone",
+                "id",
                 "startedAt",
-                "downloadFile",
                 "name",
                 "scheduledAt",
-                "status",
                 "username",
                 "snapshot",
-                "id",
-                "isDone"
+                "downloadFile"
             ],
             "description": "IP Fabric scheduled or running jobs",
             "summary": "Platform Jobs",
             "web_endpoint": null
         }
     },
     "tables/load-balancing/f5-partitions": {
         "api_endpoint": "/tables/load-balancing/f5-partitions",
         "get": null,
         "post": {
             "api_endpoint": "tables/load-balancing/f5-partitions",
             "columns": [
                 "siteName",
-                "hostname",
+                "id",
+                "partitionName",
                 "partitionDescription",
                 "sn",
-                "partitionName",
-                "id"
+                "hostname"
             ],
             "description": "F5 Partitions inventory",
             "summary": "F5 Partitions",
             "web_endpoint": "/technology/load-balancing/f5-partitions"
         }
     },
     "tables/load-balancing/virtual-servers": {
         "api_endpoint": "/tables/load-balancing/virtual-servers",
         "get": null,
         "post": {
             "api_endpoint": "tables/load-balancing/virtual-servers",
             "columns": [
-                "portName",
-                "siteName",
-                "poolsCount",
-                "sn",
+                "id",
                 "clientProfile",
+                "pools",
+                "protocolNumber",
                 "protocolName",
-                "virtualServerName",
-                "vrf",
-                "reason",
-                "portNumber",
+                "portName",
+                "poolsCount",
                 "availability",
-                "partition",
                 "hostname",
-                "protocolNumber",
-                "sourceNat",
-                "pools",
                 "vip",
-                "vip6",
+                "vrf",
+                "partition",
                 "state",
-                "id"
+                "sn",
+                "sourceNat",
+                "portNumber",
+                "siteName",
+                "reason",
+                "vip6",
+                "virtualServerName"
             ],
             "description": "Load balancing - virtual servers inventory",
             "summary": "Virtual Servers",
             "web_endpoint": "/technology/load-balancing/virtual-servers"
         }
     },
     "tables/load-balancing/virtual-servers/pool-members": {
         "api_endpoint": "/tables/load-balancing/virtual-servers/pool-members",
         "get": null,
         "post": {
             "api_endpoint": "tables/load-balancing/virtual-servers/pool-members",
             "columns": [
-                "port",
-                "hostname",
+                "memberIpV6",
                 "siteName",
+                "port",
+                "id",
+                "state",
+                "poolName",
                 "memberIp",
                 "sn",
-                "vrf",
-                "memberIpV6",
-                "poolName",
-                "state",
-                "poolMemberName",
                 "availability",
-                "id"
+                "vrf",
+                "hostname",
+                "poolMemberName"
             ],
             "description": "Load balancing - virtual servers and pool members inventory",
             "summary": "Virtual Servers - Pool members",
             "web_endpoint": "/technology/load-balancing/virtual-servers-pool-members"
         }
     },
     "tables/load-balancing/virtual-servers/pools": {
         "api_endpoint": "/tables/load-balancing/virtual-servers/pools",
         "get": null,
         "post": {
             "api_endpoint": "tables/load-balancing/virtual-servers/pools",
             "columns": [
                 "siteName",
-                "hostname",
+                "id",
+                "membersCount",
                 "sn",
-                "members",
+                "hostname",
                 "poolName",
-                "membersCount",
-                "id"
+                "members"
             ],
             "description": "Load balancing - virtual servers and pools inventory",
             "summary": "Virtual Servers - Pools",
             "web_endpoint": "/technology/load-balancing/virtual-servers-pools"
         }
     },
     "tables/management/banners/banners": {
         "api_endpoint": "/tables/management/banners/banners",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/banners/banners",
             "columns": [
                 "siteName",
-                "hostname",
-                "text",
-                "sn",
                 "type",
-                "id"
+                "id",
+                "sn",
+                "hostname",
+                "text"
             ],
             "description": "Types and texts of the device banners",
             "summary": "Device Banners",
             "web_endpoint": "/technology/management/banners/banners"
         }
     },
     "tables/management/banners/summary": {
         "api_endpoint": "/tables/management/banners/summary",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/banners/summary",
             "columns": [
-                "motdBanner",
                 "siteName",
-                "hostname",
-                "sn",
                 "loginBanner",
-                "id"
+                "id",
+                "sn",
+                "motdBanner",
+                "hostname"
             ],
             "description": "Summary view for device banners",
             "summary": "Banners Summary",
             "web_endpoint": "/technology/management/banners/summary"
         }
     },
     "tables/management/changes/connectivity": {
         "api_endpoint": "/tables/management/changes/connectivity",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/changes/connectivity",
             "columns": [
-                "localInt",
-                "remoteMedia",
-                "remoteInt",
-                "remoteSn",
                 "localMedia",
+                "id",
+                "remoteInt",
+                "localInt",
                 "remoteHost",
                 "localHost",
-                "status",
                 "protocol",
+                "remoteSn",
+                "remoteMedia",
                 "localSn",
-                "id"
+                "status"
             ],
             "description": "Changes in connectivity matrix between selected snapshots",
             "summary": "Changes in connectivity matrix",
             "web_endpoint": null
         }
     },
     "tables/management/changes/devices": {
         "api_endpoint": "/tables/management/changes/devices",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/changes/devices",
             "columns": [
+                "image",
+                "id",
                 "uptime",
                 "loginIp",
-                "hostname",
-                "sn",
                 "processor",
-                "configReg",
-                "status",
                 "reload",
                 "version",
-                "id",
-                "image"
+                "sn",
+                "configReg",
+                "hostname",
+                "status"
             ],
             "description": "Changes in discovered devices between selected snapshots",
             "summary": "Changes in devices",
             "web_endpoint": null
         }
     },
     "tables/management/changes/managed-devs": {
         "api_endpoint": "/tables/management/changes/managed-devs",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/changes/managed-devs",
             "columns": [
-                "hostname",
-                "intName",
+                "type",
+                "id",
+                "net",
                 "sn",
-                "status",
+                "intName",
+                "hostname",
                 "ip",
-                "net",
-                "type",
-                "id"
+                "status"
             ],
             "description": "Changes in managed interface IP addresses between selected snapshots",
             "summary": "Changes in Managed IP",
             "web_endpoint": null
         }
     },
     "tables/management/changes/pn": {
         "api_endpoint": "/tables/management/changes/pn",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/changes/pn",
             "columns": [
-                "hostname",
                 "deviceId",
                 "dscr",
-                "sn",
+                "id",
                 "name",
-                "vid",
-                "status",
+                "sn",
                 "pid",
-                "id"
+                "vid",
+                "hostname",
+                "status"
             ],
             "description": "Changes in part numbers between selected snapshots",
             "summary": "Changes in Part Numbers",
             "web_endpoint": null
         }
     },
     "tables/management/configuration": {
         "api_endpoint": "/tables/management/configuration",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/configuration",
             "columns": [
-                "lastCheckAt",
-                "hostname",
-                "sn",
-                "lastChangeAt",
-                "status",
                 "hash",
+                "id",
+                "lastChangeAt",
+                "sn",
+                "lastCheckAt",
                 "reason",
-                "id"
+                "hostname",
+                "status"
             ],
             "description": "Inventory of all captured configuration files",
             "summary": "Configuration Files",
             "web_endpoint": null
         }
     },
     "tables/management/configuration/download": {
@@ -4374,4268 +4388,4274 @@
     },
     "tables/management/configuration/saved": {
         "api_endpoint": "/tables/management/configuration/saved",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/configuration/saved",
             "columns": [
-                "uptime",
+                "siteName",
+                "startupConfigExists",
                 "blobKey",
+                "id",
+                "uptime",
                 "loginIp",
-                "siteName",
+                "sn",
                 "hostname",
                 "currentConfigExists",
-                "sn",
-                "status",
-                "startupConfigExists",
-                "id"
+                "status"
             ],
             "description": "Compare the current and startup configuration files",
             "summary": "Saved Config Consistency",
             "web_endpoint": "/management/saved-config-consistency"
         }
     },
     "tables/management/connectivity-errors": {
         "api_endpoint": "/tables/management/connectivity-errors",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/connectivity-errors",
             "columns": [
-                "sshType",
                 "telnetType",
+                "sshType",
+                "id",
                 "date",
-                "ip",
-                "sshMsg",
                 "telnetMsg",
-                "id"
+                "ip",
+                "sshMsg"
             ],
             "description": "Observe connectivity errors for failed configuration file downloads",
             "summary": "Configuration Management Connectivity Errors",
             "web_endpoint": "/management/configuration/connectivity-errors"
         }
     },
     "tables/management/discovery-runs": {
         "api_endpoint": "/tables/management/discovery-runs",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/discovery-runs",
             "columns": [
-                "deviceCount",
-                "interfaceActiveCount",
-                "tsStart",
-                "partNumbersCount",
-                "connectionCount",
-                "tsEnd",
-                "interfaceCount",
-                "userCount",
-                "managedIpCount",
                 "status",
+                "interfaceActiveCount",
                 "tsChange",
+                "tsEnd",
+                "id",
                 "isLastSnapshot",
                 "interfaceEdgeCount",
-                "id"
+                "userCount",
+                "tsStart",
+                "connectionCount",
+                "interfaceCount",
+                "partNumbersCount",
+                "deviceCount",
+                "managedIpCount"
             ],
             "description": "",
             "summary": "Changes",
             "web_endpoint": "/reports/network-analysis-report"
         }
     },
     "tables/management/dns/servers": {
         "api_endpoint": "/tables/management/dns/servers",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/dns/servers",
             "columns": [
-                "type",
-                "searchDomains",
-                "hostname",
                 "siteName",
-                "sn",
-                "vrf",
+                "type",
+                "id",
                 "ipv6",
+                "sn",
                 "srcIntName",
+                "searchDomains",
+                "vrf",
+                "hostname",
                 "ip",
-                "parentId",
-                "id"
+                "parentId"
             ],
             "description": "Inventory of configured DNS servers on managed network devices",
             "summary": "DNS Servers",
             "web_endpoint": "/technology/management/dns/servers"
         }
     },
     "tables/management/dns/settings": {
         "api_endpoint": "/tables/management/dns/settings",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/dns/settings",
             "columns": [
-                "retry",
-                "hostname",
                 "siteName",
-                "sn",
-                "protocols",
+                "id",
                 "timeout",
+                "retry",
                 "dnsServersCount",
-                "id"
+                "sn",
+                "protocols",
+                "hostname"
             ],
             "description": "Inventory of additional DNS settings on managed network devices",
             "summary": "DNS Settings",
             "web_endpoint": "/technology/management/dns/settings"
         }
     },
     "tables/management/flow/netflow/collectors": {
         "api_endpoint": "/tables/management/flow/netflow/collectors",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/flow/netflow/collectors",
             "columns": [
-                "port",
-                "hostname",
                 "siteName",
+                "port",
+                "collector",
                 "srcInterface",
+                "id",
+                "version",
+                "protocol",
                 "sn",
                 "vrf",
-                "srcAddress",
-                "protocol",
-                "version",
-                "collector",
-                "id"
+                "hostname",
+                "srcAddress"
             ],
             "description": "Inventory of NetFlow collectors configured on managed network devices",
             "summary": "NetFlow Collectors",
             "web_endpoint": "/technology/management/flow/netflow-collectors"
         }
     },
     "tables/management/flow/netflow/devices": {
         "api_endpoint": "/tables/management/flow/netflow/devices",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/flow/netflow/devices",
             "columns": [
                 "inactiveTimeout",
                 "siteName",
-                "hostname",
-                "activeTimeout",
-                "sn",
                 "countNetflowCollectors",
+                "id",
+                "sn",
+                "activeTimeout",
                 "countNetflowInterfaces",
-                "id"
+                "hostname"
             ],
             "description": "Managed network devices with configured NetFlow collectors",
             "summary": "NetFlow Devices",
             "web_endpoint": "/technology/management/flow/netflow-devices"
         }
     },
     "tables/management/flow/netflow/interfaces": {
         "api_endpoint": "/tables/management/flow/netflow/interfaces",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/flow/netflow/interfaces",
             "columns": [
                 "siteName",
-                "hostname",
-                "interface",
-                "sn",
                 "directions",
-                "id"
+                "id",
+                "sn",
+                "interface",
+                "hostname"
             ],
             "description": "Inventory of interfaces participating in NetFlow collection",
             "summary": "NetFlow Interfaces",
             "web_endpoint": "/technology/management/flow/netflow-interfaces"
         }
     },
     "tables/management/flow/overview": {
         "api_endpoint": "/tables/management/flow/overview",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/flow/overview",
             "columns": [
-                "countSflowSources",
-                "hostname",
                 "siteName",
-                "sn",
+                "countSflowCollectors",
                 "countNetflowCollectors",
+                "id",
+                "sn",
                 "countNetflowInterfaces",
-                "countSflowCollectors",
-                "id"
+                "hostname",
+                "countSflowSources"
             ],
             "description": "Summary inventory of devices participating in either NetFlow or sFlow collection",
             "summary": "Flow Overview",
             "web_endpoint": "/technology/management/flow/overview"
         }
     },
     "tables/management/flow/sflow/collectors": {
         "api_endpoint": "/tables/management/flow/sflow/collectors",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/flow/sflow/collectors",
             "columns": [
-                "port",
-                "hostname",
                 "siteName",
+                "port",
+                "collector",
+                "id",
                 "sn",
                 "vrf",
-                "collector",
-                "id"
+                "hostname"
             ],
             "description": "Inventory of sFlow collectors configured on managed network devices",
             "summary": "sFlow Collectors",
             "web_endpoint": "/technology/management/flow/sflow-collectors"
         }
     },
     "tables/management/flow/sflow/devices": {
         "api_endpoint": "/tables/management/flow/sflow/devices",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/flow/sflow/devices",
             "columns": [
+                "ingressSampleRate",
                 "siteName",
-                "hostname",
+                "countSflowCollectors",
+                "id",
                 "agent",
-                "srcAddress6",
-                "egressSampleRate",
                 "sn",
+                "egressSampleRate",
                 "pollingInterval",
-                "srcAddress",
+                "srcAddress6",
+                "hostname",
                 "countSflowSources",
-                "countSflowCollectors",
-                "id",
-                "ingressSampleRate"
+                "srcAddress"
             ],
             "description": "Managed network devices with configured sFlow collectors",
             "summary": "sFlow Devices",
             "web_endpoint": "/technology/management/flow/sflow-devices"
         }
     },
     "tables/management/flow/sflow/sources": {
         "api_endpoint": "/tables/management/flow/sflow/sources",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/flow/sflow/sources",
             "columns": [
+                "ingressSampleRate",
                 "siteName",
-                "hostname",
-                "egressSampleRate",
-                "sn",
-                "name",
-                "directions",
-                "pollingInterval",
                 "type",
+                "directions",
                 "id",
-                "ingressSampleRate"
+                "name",
+                "sn",
+                "egressSampleRate",
+                "pollingInterval",
+                "hostname"
             ],
             "description": "Inventory of sources participating in sFlow collection",
             "summary": "sFlow Data Sources",
             "web_endpoint": "/technology/management/flow/sflow-data-sources"
         }
     },
     "tables/management/licenses": {
         "api_endpoint": "/tables/management/licenses",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/licenses",
             "columns": [
-                "description",
+                "licenseName",
+                "index",
+                "licenseType",
+                "reservationStatus",
+                "siteName",
                 "licenseEvalPeriodTotal",
-                "hostname",
-                "numberOfDetails",
+                "id",
+                "licenseInUse",
                 "licenseActive",
-                "siteName",
+                "numberOfDetails",
                 "sn",
-                "reservationStatus",
-                "status",
-                "index",
-                "licenseName",
                 "licensePeriodLeft",
                 "licenseCount",
-                "id",
-                "licenseType",
-                "licenseInUse"
+                "hostname",
+                "description",
+                "status"
             ],
             "description": "Licenses inventory for managed network devices",
             "summary": "Managed Licenses",
             "web_endpoint": "/technology/management/licenses/license/licenses"
         }
     },
     "tables/management/licenses/cisco-smart-licenses/authorization": {
         "api_endpoint": "/tables/management/licenses/cisco-smart-licenses/authorization",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/licenses/cisco-smart-licenses/authorization",
             "columns": [
+                "lastCommunicationTime",
                 "siteName",
-                "hostname",
+                "id",
+                "authorizationTime",
                 "communicationDeadlineTime",
-                "lastCommunicationStatus",
                 "sn",
-                "status",
-                "lastCommunicationTime",
-                "authorizationTime",
-                "id"
+                "hostname",
+                "lastCommunicationStatus",
+                "status"
             ],
             "description": "Cisco smart license authorization inventory",
             "summary": "Cisco Smart License Authorization",
             "web_endpoint": "/technology/management/licenses/cisco-smart-license/authorization"
         }
     },
     "tables/management/licenses/cisco-smart-licenses/registration": {
         "api_endpoint": "/tables/management/licenses/cisco-smart-licenses/registration",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/licenses/cisco-smart-licenses/registration",
             "columns": [
-                "smartAccount",
+                "initialRegistrationTime",
                 "siteName",
-                "hostname",
                 "initialRegistrationStatus",
+                "registrationExpires",
+                "id",
                 "virtualAccount",
                 "sn",
-                "initialRegistrationTime",
-                "status",
-                "id",
-                "registrationExpires"
+                "smartAccount",
+                "hostname",
+                "status"
             ],
             "description": "Cisco smart license registration inventory",
             "summary": "Cisco Smart License Registration",
             "web_endpoint": "/technology/management/licenses/cisco-smart-license/registration"
         }
     },
     "tables/management/licenses/cisco-smart-licenses/reservations": {
         "api_endpoint": "/tables/management/licenses/cisco-smart-licenses/reservations",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/licenses/cisco-smart-licenses/reservations",
             "columns": [
-                "siteName",
-                "hostname",
-                "sn",
-                "name",
                 "totalReservedCount",
+                "siteName",
                 "type",
-                "id"
+                "id",
+                "name",
+                "sn",
+                "hostname"
             ],
             "description": "Cisco smart license reservations inventory",
             "summary": "Cisco Smart License Reservations",
             "web_endpoint": "/technology/management/licenses/cisco-smart-license/reservations"
         }
     },
     "tables/management/licenses/detail": {
         "api_endpoint": "/tables/management/licenses/detail",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/licenses/detail",
             "columns": [
                 "siteName",
-                "hostname",
-                "sn",
-                "name",
-                "license",
                 "id",
-                "detail"
+                "name",
+                "detail",
+                "sn",
+                "hostname",
+                "license"
             ],
             "description": "Licenses detailed inventory for managed network devices",
             "summary": "Managed License detail",
             "web_endpoint": "/technology/management/licenses/license/detail"
         }
     },
     "tables/management/licenses/summary": {
         "api_endpoint": "/tables/management/licenses/summary",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/licenses/summary",
             "columns": [
                 "siteName",
-                "hostname",
-                "numberOfLicenses",
-                "sn",
                 "type",
-                "id"
+                "id",
+                "sn",
+                "hostname",
+                "numberOfLicenses"
             ],
             "description": "Licenses summary inventory including license type and number of licenses",
             "summary": "Managed License Summary",
             "web_endpoint": "/technology/management/licenses/license/summary"
         }
     },
     "tables/management/logging/local": {
         "api_endpoint": "/tables/management/logging/local",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/logging/local",
             "columns": [
                 "siteName",
-                "hostname",
-                "sn",
-                "fileName",
                 "type",
+                "id",
+                "fileName",
+                "sn",
                 "filters",
-                "id"
+                "hostname"
             ],
             "description": "Local system message logging targets and associated parameters",
             "summary": "Local Logging Services",
             "web_endpoint": "/technology/management/logging/local-services"
         }
     },
     "tables/management/logging/remote": {
         "api_endpoint": "/tables/management/logging/remote",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/logging/remote",
             "columns": [
-                "facility",
-                "port",
-                "hostname",
+                "host",
                 "siteName",
+                "port",
                 "srcInterface",
-                "host",
-                "sn",
-                "vrf",
-                "srcAddress",
-                "protocol",
                 "type",
+                "id",
+                "facility",
+                "protocol",
+                "sn",
                 "filters",
-                "id"
+                "vrf",
+                "hostname",
+                "srcAddress"
             ],
             "description": "Remote system message logging targets and associated parameters",
             "summary": "Remote Logging Services",
             "web_endpoint": "/technology/management/logging/remote-services"
         }
     },
     "tables/management/logging/summary": {
         "api_endpoint": "/tables/management/logging/summary",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/logging/summary",
             "columns": [
+                "countRemoteServices",
                 "siteName",
-                "hostname",
+                "id",
                 "sn",
-                "countRemoteServices",
                 "countLocalServices",
-                "id"
+                "hostname"
             ],
             "description": "Summary of the system message logging configuration for remote and local targets configured on managed network devices",
             "summary": "Logging Summary",
             "web_endpoint": "/technology/management/logging/summary"
         }
     },
     "tables/management/ntp/sources": {
         "api_endpoint": "/tables/management/ntp/sources",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/ntp/sources",
             "columns": [
-                "jitter",
-                "when",
                 "siteName",
-                "hostname",
-                "poll",
-                "offset",
-                "sn",
-                "reachable",
-                "reference",
-                "stratum",
                 "flags",
-                "reach",
                 "delay",
+                "reach",
                 "id",
-                "source"
+                "stratum",
+                "source",
+                "sn",
+                "offset",
+                "jitter",
+                "poll",
+                "reference",
+                "hostname",
+                "reachable",
+                "when"
             ],
             "description": "Detailed status of all NTP peerings configured on managed network devices",
             "summary": "NTP Sources",
             "web_endpoint": "/technology/management/ntp/sources"
         }
     },
     "tables/management/ntp/summary": {
         "api_endpoint": "/tables/management/ntp/summary",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/ntp/summary",
             "columns": [
-                "siteName",
-                "hostname",
-                "reachableSources",
-                "sn",
                 "confSources",
                 "sources",
-                "id"
+                "siteName",
+                "id",
+                "sn",
+                "reachableSources",
+                "hostname"
             ],
             "description": "Summary view for managed network devices and their configured NTP peerings",
             "summary": "NTP Summary",
             "web_endpoint": "/technology/management/ntp/summary"
         }
     },
     "tables/management/oam/unidirectional-link-detection/interfaces": {
         "api_endpoint": "/tables/management/oam/unidirectional-link-detection/interfaces",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/oam/unidirectional-link-detection/interfaces",
             "columns": [
+                "operState",
                 "siteName",
-                "hostname",
-                "intName",
-                "portAdminState",
+                "id",
+                "neighborsCount",
+                "protocol",
                 "sn",
                 "bidState",
-                "portOperState",
-                "protocol",
-                "operState",
-                "neighborsCount",
-                "id"
+                "portAdminState",
+                "hostname",
+                "intName",
+                "portOperState"
             ],
             "description": "Unidirectional Link Detection (UDLD) interfaces inventory",
             "summary": "UDLD Interfaces",
             "web_endpoint": "/technology/oam/udld/interfaces"
         }
     },
     "tables/management/oam/unidirectional-link-detection/neighbors": {
         "api_endpoint": "/tables/management/oam/unidirectional-link-detection/neighbors",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/oam/unidirectional-link-detection/neighbors",
             "columns": [
-                "siteName",
-                "hostname",
-                "intName",
                 "deviceId",
+                "siteName",
+                "id",
+                "state",
                 "neighborHostname",
-                "portId",
                 "sn",
-                "state",
-                "id"
+                "portId",
+                "hostname",
+                "intName"
             ],
             "description": "Unidirectional Link Detection (UDLD) neighbors inventory",
             "summary": "UDLD Neighbors",
             "web_endpoint": "/technology/oam/udld/neighbors"
         }
     },
     "tables/management/osver-consistency": {
         "api_endpoint": "/tables/management/osver-consistency",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/osver-consistency",
             "columns": [
-                "maintenance",
-                "minor",
-                "pctModel",
+                "family",
+                "model",
+                "train",
                 "platform",
-                "pct",
-                "vendor",
                 "major",
-                "version",
-                "train",
-                "rebuild",
-                "model",
-                "family",
                 "id",
-                "count"
+                "pctModel",
+                "rebuild",
+                "version",
+                "minor",
+                "count",
+                "pct",
+                "vendor",
+                "maintenance"
             ],
             "description": "Operating system consistency table presents the variation of OS versions within each platform and family.",
             "summary": "OS Version Consistency",
             "web_endpoint": "/inventory/os-versions"
         }
     },
     "tables/management/port-mirroring": {
         "api_endpoint": "/tables/management/port-mirroring",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/port-mirroring",
             "columns": [
+                "src",
                 "siteName",
-                "hostname",
+                "sessionId",
                 "dscr",
-                "sn",
-                "src",
-                "dst",
-                "status",
                 "type",
                 "id",
+                "dst",
                 "params",
-                "sessionId"
+                "sn",
+                "hostname",
+                "status"
             ],
             "description": "Port Mirroring table lists all SPAN, RSPAN and ERSPAN sessions configured in the network with their parameters",
             "summary": "Port Mirroring",
             "web_endpoint": "/technology/management/port-mirroring"
         }
     },
     "tables/management/ptp/interfaces": {
         "api_endpoint": "/tables/management/ptp/interfaces",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/ptp/interfaces",
             "columns": [
                 "siteName",
-                "hostname",
-                "intName",
-                "sn",
+                "id",
                 "state",
-                "id"
+                "sn",
+                "hostname",
+                "intName"
             ],
             "description": "Precision Time Protocol (PTP) interfaces inventory",
             "summary": "PTP Interfaces",
             "web_endpoint": "/technology/management/ptp/interfaces"
         }
     },
     "tables/management/ptp/local-clock": {
         "api_endpoint": "/tables/management/ptp/local-clock",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/ptp/local-clock",
             "columns": [
-                "mode",
-                "priority2",
-                "siteName",
-                "hostname",
+                "priority1",
                 "meanPathDelay",
-                "offsetFromMaster",
+                "siteName",
                 "numberOfIfaces",
-                "domain",
+                "id",
+                "mode",
+                "source",
                 "sn",
-                "localClockIdentity",
-                "stepsRemoved",
+                "offsetFromMaster",
                 "deviceStatus",
-                "priority1",
-                "id",
-                "source"
+                "domain",
+                "priority2",
+                "localClockIdentity",
+                "hostname",
+                "stepsRemoved"
             ],
             "description": "Precision Time Protocol (PTP) local clock inventory",
             "summary": "PTP Local clock",
             "web_endpoint": "/technology/management/ptp/local-clock"
         }
     },
     "tables/management/ptp/masters": {
         "api_endpoint": "/tables/management/ptp/masters",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/ptp/masters",
             "columns": [
-                "parentIPAddress",
-                "siteName",
-                "hostname",
                 "parentClockIdentity",
-                "priority2",
-                "sn",
                 "grandmasterClockIdentity",
                 "priority1",
-                "id"
+                "siteName",
+                "id",
+                "sn",
+                "parentIPAddress",
+                "priority2",
+                "hostname"
             ],
             "description": "Precision Time Protocol (PTP) masters inventory",
             "summary": "PTP Masters",
             "web_endpoint": "/technology/management/ptp/masters"
         }
     },
     "tables/management/snapshots": {
         "api_endpoint": "/tables/management/snapshots",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/snapshots",
             "columns": [
-                "locked",
-                "finishStatus",
-                "creatorUsername",
-                "deviceRemovedCount",
+                "id",
                 "unloadedSize",
-                "tsStart",
-                "tsChange",
                 "isLastSnapshot",
+                "interfaceCount",
+                "loadedSize",
+                "deviceRemovedCount",
+                "totalDevCount",
+                "sites",
+                "deviceAddedCount",
+                "tsChange",
                 "tsEnd",
+                "locked",
                 "note",
+                "status",
                 "interfaceActiveCount",
-                "name",
-                "loadedSize",
+                "creatorUsername",
+                "finishStatus",
                 "loading",
-                "status",
-                "totalDevCount",
-                "id",
                 "interfaceEdgeCount",
-                "interfaceCount",
                 "userCount",
+                "name",
                 "fromArchive",
-                "deviceAddedCount",
-                "sites"
+                "tsStart"
             ],
             "description": "",
             "summary": "POST /tables/management/snapshots",
             "web_endpoint": null
         }
     },
     "tables/management/snmp/communities": {
         "api_endpoint": "/tables/management/snmp/communities",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/snmp/communities",
             "columns": [
-                "group",
                 "siteName",
-                "hostname",
-                "view",
+                "group",
+                "id",
                 "acl",
-                "sn",
-                "name",
                 "authorization",
+                "name",
+                "sn",
                 "prefixes",
-                "id"
+                "hostname",
+                "view"
             ],
             "description": "SNMP communities and the associated scope restrictions configured on managed network devices",
             "summary": "SNMP Communities",
             "web_endpoint": "/technology/management/snmp/communities"
         }
     },
     "tables/management/snmp/summary": {
         "api_endpoint": "/tables/management/snmp/summary",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/snmp/summary",
             "columns": [
-                "communitiesCount",
+                "model",
                 "siteName",
-                "hostname",
-                "usersCount",
-                "sn",
-                "name",
-                "contact",
-                "vendor",
+                "id",
                 "localEngineId",
-                "trapHostsCount",
+                "vendor",
+                "contact",
+                "name",
+                "sn",
                 "location",
-                "model",
-                "id"
+                "usersCount",
+                "trapHostsCount",
+                "hostname",
+                "communitiesCount"
             ],
             "description": "Summary of SNMP protocol configuration on managed network devices",
             "summary": "SNMP Summary",
             "web_endpoint": "/technology/management/snmp/summary"
         }
     },
     "tables/management/snmp/trap-hosts": {
         "api_endpoint": "/tables/management/snmp/trap-hosts",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/snmp/trap-hosts",
             "columns": [
-                "dstHost",
+                "vrf",
                 "siteName",
-                "hostname",
+                "type",
                 "srcInterface",
+                "id",
+                "version",
                 "user",
                 "sn",
-                "vrf",
                 "community",
-                "srcIp",
                 "dstPort",
-                "version",
-                "type",
-                "id"
+                "srcIp",
+                "hostname",
+                "dstHost"
             ],
             "description": "Configured destination hosts for SNMP traps and SNMP inform requests",
             "summary": "SNMP Hosts",
             "web_endpoint": "/technology/management/snmp/trap-hosts"
         }
     },
     "tables/management/snmp/users": {
         "api_endpoint": "/tables/management/snmp/users",
         "get": null,
         "post": {
             "api_endpoint": "tables/management/snmp/users",
             "columns": [
-                "group",
                 "siteName",
-                "hostname",
-                "privacy",
+                "group",
+                "id",
                 "acl",
-                "sn",
                 "name",
-                "id",
-                "authentication"
+                "sn",
+                "authentication",
+                "hostname",
+                "privacy"
             ],
             "description": "SNMP users and the associated scope restrictions configured on managed network devices",
             "summary": "SNMP Users",
             "web_endpoint": "/technology/management/snmp/users"
         }
     },
     "tables/mpls/forwarding": {
         "api_endpoint": "/tables/mpls/forwarding",
         "get": null,
         "post": {
             "api_endpoint": "tables/mpls/forwarding",
             "columns": [
+                "labelIn",
+                "nexthop",
                 "siteName",
-                "hostname",
+                "id",
                 "network",
-                "sn",
-                "nexthop",
-                "labelIn",
                 "prefix",
-                "id"
+                "sn",
+                "hostname"
             ],
             "description": "MPLS forwarding table maps labels to their associated next hops",
             "summary": "MPLS Forwarding",
             "web_endpoint": "/technology/mpls/forwarding"
         }
     },
     "tables/mpls/l2-vpn/circuit-cross-connect": {
         "api_endpoint": "/tables/mpls/l2-vpn/circuit-cross-connect",
         "get": null,
         "post": {
             "api_endpoint": "tables/mpls/l2-vpn/circuit-cross-connect",
             "columns": [
-                "ac",
-                "hostname",
+                "neiHostname",
                 "localLabel",
+                "upTrans",
                 "siteName",
+                "stateOrig",
                 "timeLastUp",
-                "neiSn",
-                "sn",
-                "name",
-                "receiveLsp",
-                "remoteLabel",
-                "upTrans",
-                "transmitLsp",
+                "id",
+                "ac",
                 "neiSiteName",
-                "stateOrig",
                 "state",
-                "neiHostname",
                 "neiIp",
-                "id"
+                "name",
+                "sn",
+                "neiSn",
+                "receiveLsp",
+                "transmitLsp",
+                "hostname",
+                "remoteLabel"
             ],
             "description": "L2 VPN circuit cross-connect inventory with associated parameters",
             "summary": "Circuit Cross-Connect",
             "web_endpoint": "/technology/mpls/l2vpn/circuit-cross-connect"
         }
     },
     "tables/mpls/l2-vpn/curcit-cross-connect": {
         "api_endpoint": "/tables/mpls/l2-vpn/curcit-cross-connect",
         "get": null,
         "post": {
             "api_endpoint": "tables/mpls/l2-vpn/curcit-cross-connect",
             "columns": [
-                "ac",
-                "hostname",
+                "neiHostname",
                 "localLabel",
+                "upTrans",
                 "siteName",
+                "stateOrig",
                 "timeLastUp",
-                "neiSn",
-                "sn",
-                "name",
-                "receiveLsp",
-                "remoteLabel",
-                "upTrans",
-                "transmitLsp",
+                "id",
+                "ac",
                 "neiSiteName",
-                "stateOrig",
                 "state",
-                "neiHostname",
                 "neiIp",
-                "id"
+                "name",
+                "sn",
+                "neiSn",
+                "receiveLsp",
+                "transmitLsp",
+                "hostname",
+                "remoteLabel"
             ],
             "description": "L2 VPN circuit cross-connect inventory with associated parameters",
             "summary": "Circuit Cross-Connect",
             "web_endpoint": "/technology/mpls/l2vpn/curcit-cross-connect"
         }
     },
     "tables/mpls/l2-vpn/point-to-multipoint": {
         "api_endpoint": "/tables/mpls/l2-vpn/point-to-multipoint",
         "get": null,
         "post": {
             "api_endpoint": "tables/mpls/l2-vpn/point-to-multipoint",
             "columns": [
-                "ac",
-                "hostname",
+                "neiHostname",
                 "siteName",
+                "id",
+                "bridgeDomain",
                 "localIntName",
-                "neiSn",
+                "ac",
+                "neiSiteName",
+                "neiIp",
                 "name",
-                "bridgeDomain",
                 "sn",
-                "neiSiteName",
                 "state",
-                "neiHostname",
-                "neiIp",
-                "id"
+                "neiSn",
+                "hostname"
             ],
             "description": "L2 VPN Virtual Private LAN Service (VPLS) circuits inventory with associated parameters",
             "summary": "Point to multipoint - VPLS",
             "web_endpoint": "/technology/mpls/l2vpn/point-to-multipoint-vpls"
         }
     },
     "tables/mpls/l2-vpn/point-to-point-vpws": {
         "api_endpoint": "/tables/mpls/l2-vpn/point-to-point-vpws",
         "get": null,
         "post": {
             "api_endpoint": "tables/mpls/l2-vpn/point-to-point-vpws",
             "columns": [
-                "ac",
-                "siteName",
-                "routeTargetImport",
-                "sn",
+                "neiHostname",
                 "remoteId",
+                "stateOrig",
+                "id",
+                "neiSiteName",
+                "neiSn",
                 "localLabel",
-                "rd",
-                "routeTargetExport",
-                "neiHostname",
-                "signallingProtocol",
-                "group",
+                "routeTargetImport",
                 "hostname",
-                "neiSn",
-                "vcId",
-                "name",
-                "neiSiteName",
-                "stateOrig",
-                "neiIp",
-                "localId",
                 "remoteLabel",
+                "signallingProtocol",
                 "state",
-                "id"
+                "routeTargetExport",
+                "neiIp",
+                "sn",
+                "siteName",
+                "rd",
+                "group",
+                "ac",
+                "localId",
+                "name",
+                "vcId"
             ],
             "description": "Virtual private wire service (VPWS) Layer 2 VPNs inventory with associated parameters",
             "summary": "Point to point - VPWS",
             "web_endpoint": "/technology/mpls/l2vpn/point-to-point-vpws"
         }
     },
     "tables/mpls/l2-vpn/pseudowires": {
         "api_endpoint": "/tables/mpls/l2-vpn/pseudowires",
         "get": null,
         "post": {
             "api_endpoint": "tables/mpls/l2-vpn/pseudowires",
             "columns": [
+                "neiHostname",
                 "localLabel",
-                "hostname",
-                "intName",
                 "siteName",
-                "neiSn",
-                "sn",
-                "remoteLabel",
-                "neiSiteName",
-                "state",
-                "neiHostname",
                 "type",
+                "id",
+                "state",
+                "neiSiteName",
                 "neiIp",
-                "id"
+                "sn",
+                "neiSn",
+                "hostname",
+                "intName",
+                "remoteLabel"
             ],
             "description": "L2 VPN pseudowires inventory",
             "summary": "All Pseudowires",
             "web_endpoint": "/technology/mpls/l2vpn/all-pseudowires"
         }
     },
     "tables/mpls/l3-vpn/pe-routers": {
         "api_endpoint": "/tables/mpls/l3-vpn/pe-routers",
         "get": null,
         "post": {
             "api_endpoint": "tables/mpls/l3-vpn/pe-routers",
             "columns": [
                 "siteName",
-                "hostname",
-                "ldpIntCount",
+                "id",
                 "sn",
                 "vrfCount",
-                "id"
+                "ldpIntCount",
+                "hostname"
             ],
             "description": "Provider Edge routers inventory participating in L3VPNs",
             "summary": "PE Routers",
             "web_endpoint": "/technology/mpls/l3vpn/pe-routers"
         }
     },
     "tables/mpls/l3-vpn/pe-routes": {
         "api_endpoint": "/tables/mpls/l3-vpn/pe-routes",
         "get": null,
         "post": {
             "api_endpoint": "tables/mpls/l3-vpn/pe-routes",
             "columns": [
-                "dstSn",
-                "srcHostname",
-                "prefix",
-                "dstSiteName",
-                "rt",
-                "dstVrf",
                 "dstHostname",
-                "srcSn",
                 "id",
                 "srcVrf",
-                "srcSiteName"
+                "dstSiteName",
+                "srcSiteName",
+                "prefix",
+                "dstVrf",
+                "rt",
+                "srcHostname",
+                "srcSn",
+                "dstSn"
             ],
             "description": "Routes on PE in VRF including originating source PE",
             "summary": "PE Routes",
             "web_endpoint": "/technology/mpls/l3vpn/pe-routes"
         }
     },
     "tables/mpls/l3-vpn/pe-vrfs": {
         "api_endpoint": "/tables/mpls/l3-vpn/pe-vrfs",
         "get": null,
         "post": {
             "api_endpoint": "tables/mpls/l3-vpn/pe-vrfs",
             "columns": [
-                "af",
-                "siteName",
-                "hostname",
                 "routeCount",
+                "siteName",
                 "rd",
+                "id",
                 "sn",
+                "af",
                 "vrf",
-                "id"
+                "hostname"
             ],
             "description": "VRF configured on PE routers with summary of routes in VRF",
             "summary": "VRFs on PE Routers",
             "web_endpoint": "/technology/mpls/l3vpn/vrf-on-pe"
         }
     },
     "tables/mpls/l3-vpn/vrf-targets": {
         "api_endpoint": "/tables/mpls/l3-vpn/vrf-targets",
         "get": null,
         "post": {
             "api_endpoint": "tables/mpls/l3-vpn/vrf-targets",
             "columns": [
-                "af",
                 "siteName",
-                "hostname",
-                "exportRT",
+                "importRT",
                 "rd",
+                "id",
                 "sn",
-                "importRT",
+                "af",
+                "exportRT",
                 "vrf",
-                "id"
+                "hostname"
             ],
             "description": "Route targets import and export configured in VRF",
             "summary": "VRF Route Targets",
             "web_endpoint": "/technology/mpls/l3vpn/vrf-route-targets"
         }
     },
     "tables/mpls/ldp/interfaces": {
         "api_endpoint": "/tables/mpls/ldp/interfaces",
         "get": null,
         "post": {
             "api_endpoint": "tables/mpls/ldp/interfaces",
             "columns": [
-                "neiCount",
+                "siteName",
                 "localAddress",
-                "hostname",
-                "intName",
+                "id",
                 "localId",
-                "siteName",
                 "sn",
-                "timerHoldtime",
+                "neiCount",
                 "timerHello",
-                "id"
+                "hostname",
+                "intName",
+                "timerHoldtime"
             ],
             "description": "Label Distribution Protocol (LDP) interfaces inventory",
             "summary": "LDP Interfaces",
             "web_endpoint": "/technology/mpls/ldp/interfaces"
         }
     },
     "tables/mpls/ldp/neighbors": {
         "api_endpoint": "/tables/mpls/ldp/neighbors",
         "get": null,
         "post": {
             "api_endpoint": "tables/mpls/ldp/neighbors",
             "columns": [
-                "localAddress",
-                "siteName",
-                "sn",
+                "neiHostname",
+                "id",
+                "neiSiteName",
+                "neiSn",
+                "neiId",
                 "neiDevType",
-                "target",
+                "intName",
                 "neiAddress",
-                "neiId",
-                "vrf",
-                "neiHostname",
-                "subnet",
+                "neiIntName",
+                "localAddress",
                 "hostname",
-                "intName",
+                "subnet",
+                "source",
+                "sn",
+                "siteName",
                 "currStateTime",
-                "neiSn",
-                "neiIntName",
-                "neiSiteName",
                 "devType",
-                "id",
-                "source"
+                "vrf",
+                "target"
             ],
             "description": "Label Distribution Protocol (LDP) neighbors inventory",
             "summary": "LDP Neighbors",
             "web_endpoint": "/technology/mpls/ldp/neighbors"
         }
     },
     "tables/mpls/rsvp/interfaces": {
         "api_endpoint": "/tables/mpls/rsvp/interfaces",
         "get": null,
         "post": {
             "api_endpoint": "tables/mpls/rsvp/interfaces",
             "columns": [
-                "neiCount",
-                "allocatedBw",
-                "localAddress",
-                "hostname",
-                "intName",
-                "siteName",
+                "linkProtectionUnprotectedLsp",
                 "linkProtectionBypass",
+                "siteName",
+                "localAddress",
+                "linkProtectionLsp",
+                "id",
+                "allocatedBw",
+                "linkProtectionProtectedLsp",
+                "sn",
+                "neiCount",
                 "linkProtectionStatus",
                 "maxBw",
-                "sn",
-                "linkProtectionProtectedLsp",
-                "linkProtectionUnprotectedLsp",
-                "id",
-                "linkProtectionLsp"
+                "hostname",
+                "intName"
             ],
             "description": "Resource Reservation Protocol (RSVP) interfaces inventory",
             "summary": "RSVP Interfaces",
             "web_endpoint": "/technology/mpls/rsvp/interfaces"
         }
     },
     "tables/mpls/rsvp/neighbors": {
         "api_endpoint": "/tables/mpls/rsvp/neighbors",
         "get": null,
         "post": {
             "api_endpoint": "tables/mpls/rsvp/neighbors",
             "columns": [
+                "neiHostname",
+                "id",
+                "neiSiteName",
+                "neiSn",
+                "linkProtectionBackupLspsCount",
+                "intName",
+                "neiAddress",
+                "frrLspsCount",
                 "localAddress",
+                "linkProtectionLspName",
                 "frrStatus",
-                "siteName",
-                "sn",
+                "linkProtectionStatus",
+                "hostname",
                 "linkProtectionBypassLsp",
-                "linkProtectionBackupRoutesCount",
-                "linkProtectionBackupLspsCount",
-                "neiAddress",
-                "neiId",
-                "vrf",
-                "neiHostname",
+                "sn",
+                "linkProtectionBypassExplicitRoute",
+                "status",
                 "via",
-                "hostname",
-                "intName",
+                "siteName",
                 "currStateTime",
-                "neiSn",
-                "linkProtectionLspName",
-                "status",
-                "neiSiteName",
-                "linkProtectionBypassExplicitRoute",
                 "localId",
-                "linkProtectionStatus",
-                "frrLspsCount",
-                "id"
+                "linkProtectionBackupRoutesCount",
+                "vrf",
+                "neiId"
             ],
             "description": "Resource Reservation Protocol (RSVP) neighbors inventory",
             "summary": "RSVP Neighbors",
             "web_endpoint": "/technology/mpls/rsvp/neighbors"
         }
     },
     "tables/multicast/igmp/groups": {
         "api_endpoint": "/tables/multicast/igmp/groups",
         "get": null,
         "post": {
             "api_endpoint": "tables/multicast/igmp/groups",
             "columns": [
-                "uptime",
-                "lastReporter",
+                "groupIp",
                 "siteName",
-                "hostname",
-                "intName",
-                "expires",
+                "lastReporter",
+                "type",
+                "id",
+                "uptime",
                 "sn",
+                "expires",
                 "sourceIp",
                 "vrf",
-                "groupIp",
-                "type",
-                "id"
+                "hostname",
+                "intName"
             ],
             "description": "Internet Group Management Protocol (IGMP) groups inventory and their associated hosts",
             "summary": "IGMP Groups",
             "web_endpoint": "/technology/multicast/igmp/groups"
         }
     },
     "tables/multicast/igmp/interfaces": {
         "api_endpoint": "/tables/multicast/igmp/interfaces",
         "get": null,
         "post": {
             "api_endpoint": "tables/multicast/igmp/interfaces",
             "columns": [
+                "lastMemberQueryCount",
                 "siteName",
-                "hostname",
-                "intName",
+                "id",
                 "queryInterval",
-                "sn",
-                "vrf",
-                "lastMemberQueryCount",
-                "lastMemberQueryInterval",
-                "querierIp",
                 "queryResponseTime",
                 "version",
-                "id"
+                "sn",
+                "lastMemberQueryInterval",
+                "vrf",
+                "hostname",
+                "intName",
+                "querierIp"
             ],
             "description": "Internet Group Management Protocol (IGMP) interfaces inventory",
             "summary": "IGMP Interfaces",
             "web_endpoint": "/technology/multicast/igmp/interfaces"
         }
     },
     "tables/multicast/igmp/snooping/global": {
         "api_endpoint": "/tables/multicast/igmp/snooping/global",
         "get": null,
         "post": {
             "api_endpoint": "tables/multicast/igmp/snooping/global",
             "columns": [
-                "siteName",
-                "hostname",
                 "v3enabled",
+                "siteName",
+                "id",
+                "enabled",
                 "v3reportSuppression",
-                "omf",
                 "sn",
-                "reportSuppression",
-                "enabled",
-                "id",
-                "v2fastLeave"
+                "omf",
+                "v2fastLeave",
+                "hostname",
+                "reportSuppression"
             ],
             "description": "Internet Group Management Protocol (IGMP) snooping global inventory",
             "summary": "IGMP Snooping",
             "web_endpoint": "/technology/multicast/igmp/snooping/global"
         }
     },
     "tables/multicast/igmp/snooping/groups": {
         "api_endpoint": "/tables/multicast/igmp/snooping/groups",
         "get": null,
         "post": {
             "api_endpoint": "tables/multicast/igmp/snooping/groups",
             "columns": [
+                "groupIp",
                 "siteName",
-                "hostname",
-                "flood",
                 "vlan",
-                "intNameList",
+                "type",
+                "id",
+                "version",
                 "sn",
                 "sourceIp",
-                "groupIp",
-                "version",
-                "type",
-                "id"
+                "intNameList",
+                "hostname",
+                "flood"
             ],
             "description": "Internet Group Management Protocol (IGMP) snooping groups inventory",
             "summary": "IGMP Snooping Groups",
             "web_endpoint": "/technology/multicast/igmp/snooping/groups"
         }
     },
     "tables/multicast/igmp/snooping/vlans": {
         "api_endpoint": "/tables/multicast/igmp/snooping/vlans",
         "get": null,
         "post": {
             "api_endpoint": "tables/multicast/igmp/snooping/vlans",
             "columns": [
                 "siteName",
-                "hostname",
-                "v3reportSuppression",
-                "v2fastLeave",
                 "vlan",
-                "omf",
+                "floodingToVlan",
+                "id",
+                "enabled",
+                "v3reportSuppression",
+                "lookupMode",
                 "sn",
+                "omf",
                 "explicitTracking",
-                "querierIp",
-                "vlanVpc",
                 "reportSuppression",
-                "enabled",
-                "id",
-                "lookupMode",
-                "floodingToVlan"
+                "v2fastLeave",
+                "hostname",
+                "querierIp",
+                "vlanVpc"
             ],
             "description": "Internet Group Management Protocol (IGMP) snooping VLANs inventory",
             "summary": "IGMP Snooping Vlans",
             "web_endpoint": "/technology/multicast/igmp/snooping/vlans"
         }
     },
     "tables/multicast/mac": {
         "api_endpoint": "/tables/multicast/mac",
         "get": null,
         "post": {
             "api_endpoint": "tables/multicast/mac",
             "columns": [
                 "siteName",
-                "hostname",
                 "vlan",
-                "intNameList",
-                "sn",
-                "id",
                 "type",
-                "mac"
+                "id",
+                "mac",
+                "sn",
+                "intNameList",
+                "hostname"
             ],
             "description": "Multicast MAC Table inventory",
             "summary": "Multicast MAC Table",
             "web_endpoint": "/technology/multicast/mac"
         }
     },
     "tables/multicast/pim/interfaces": {
         "api_endpoint": "/tables/multicast/pim/interfaces",
         "get": null,
         "post": {
             "api_endpoint": "tables/multicast/pim/interfaces",
             "columns": [
-                "neiCount",
-                "queryTimer",
-                "hostname",
                 "drIp",
-                "intName",
-                "dr",
                 "siteName",
+                "id",
+                "priority",
+                "version",
                 "sn",
-                "vrf",
+                "neiCount",
+                "queryTimer",
                 "ip",
-                "version",
-                "id",
-                "priority"
+                "vrf",
+                "hostname",
+                "intName",
+                "isDr"
             ],
             "description": "Protocol-Independent Multicast (PIM) interfaces inventory",
             "summary": "PIM Interfaces",
             "web_endpoint": "/technology/multicast/pim/interfaces"
         }
     },
     "tables/multicast/pim/neighbors": {
         "api_endpoint": "/tables/multicast/pim/neighbors",
         "get": null,
         "post": {
             "api_endpoint": "tables/multicast/pim/neighbors",
             "columns": [
-                "localAddress",
-                "siteName",
-                "expires",
-                "sn",
-                "neiDevType",
+                "neiHostname",
+                "id",
+                "priority",
+                "neiSiteName",
                 "uptime",
-                "target",
-                "dr",
-                "neiAddress",
-                "vrf",
                 "version",
-                "neiHostname",
-                "subnet",
-                "hostname",
-                "intName",
                 "neiSn",
+                "neiDevType",
+                "intName",
+                "neiAddress",
                 "neiIntName",
-                "neiSiteName",
                 "flags",
-                "priority",
+                "localAddress",
+                "hostname",
+                "subnet",
+                "source",
+                "sn",
+                "siteName",
                 "mode",
                 "devType",
-                "id",
-                "source"
+                "expires",
+                "vrf",
+                "target",
+                "isDr"
             ],
             "description": "Protocol-Independent Multicast (PIM) neighbors inventory",
             "summary": "PIM Neighbors",
             "web_endpoint": "/technology/multicast/pim/neighbors"
         }
     },
     "tables/multicast/pim/rp/bsr": {
         "api_endpoint": "/tables/multicast/pim/rp/bsr",
         "get": null,
         "post": {
             "api_endpoint": "tables/multicast/pim/rp/bsr",
             "columns": [
-                "bsrRouters",
                 "siteName",
-                "hostname",
-                "sn",
-                "vrf",
                 "bsrIp",
+                "id",
                 "bsrRoutersCount",
-                "id"
+                "sn",
+                "bsrRouters",
+                "vrf",
+                "hostname"
             ],
             "description": "Protocol-Independent Multicast (PIM) rendezvous points (RP) inventory",
             "summary": "PIM Bootstrap RP",
             "web_endpoint": "/technology/multicast/rp/bsr"
         }
     },
     "tables/multicast/pim/rp/mappings": {
         "api_endpoint": "/tables/multicast/pim/rp/mappings",
         "get": null,
         "post": {
             "api_endpoint": "tables/multicast/pim/rp/mappings",
             "columns": [
-                "rpRouters",
-                "uptime",
                 "siteName",
-                "hostname",
-                "rpIp",
+                "id",
+                "uptime",
                 "sn",
+                "rpRouters",
+                "rpIp",
                 "vrf",
-                "groupsCount",
-                "id"
+                "hostname",
+                "groupsCount"
             ],
             "description": "Protocol-Independent Multicast (PIM) and rendezvous points (RP) mappings",
             "summary": "PIM Boostrap RP mappings",
             "web_endpoint": "/technology/multicast/rp/mappings"
         }
     },
     "tables/multicast/pim/rp/mappings-groups": {
         "api_endpoint": "/tables/multicast/pim/rp/mappings-groups",
         "get": null,
         "post": {
             "api_endpoint": "tables/multicast/pim/rp/mappings-groups",
             "columns": [
-                "rpRouters",
-                "uptime",
                 "siteName",
-                "hostname",
-                "rpIp",
+                "id",
+                "uptime",
+                "groupNet",
+                "learnedFrom",
                 "sn",
-                "vrf",
+                "rpRouters",
                 "groupUptime",
-                "learnedFrom",
-                "id",
-                "groupNet"
+                "rpIp",
+                "vrf",
+                "hostname"
             ],
             "description": "Protocol-Independent Multicast (PIM) and rendezvous points (RP) mapping groups",
             "summary": "PIM Bootstrap RP mappings groups",
             "web_endpoint": "/technology/multicast/rp/mappings-groups"
         }
     },
     "tables/multicast/pim/rp/overview": {
         "api_endpoint": "/tables/multicast/pim/rp/overview",
         "get": null,
         "post": {
             "api_endpoint": "tables/multicast/pim/rp/overview",
             "columns": [
-                "rpHostname",
-                "vrfList",
-                "siteName",
                 "routersCount",
-                "rpIp",
+                "siteName",
+                "vrfList",
+                "id",
+                "rpHostname",
                 "rpSn",
-                "id"
+                "rpIp"
             ],
             "description": "Rendezvous points (RP) routers inventory",
             "summary": "RP Routers",
             "web_endpoint": "/technology/multicast/rp/overview"
         }
     },
     "tables/multicast/routes/counters": {
         "api_endpoint": "/tables/multicast/routes/counters",
         "get": null,
         "post": {
             "api_endpoint": "tables/multicast/routes/counters",
             "columns": [
-                "siteName",
+                "id",
                 "inPktsRate",
-                "inPkts",
-                "sn",
+                "avgPkt",
+                "outPktsRate",
                 "rpfNeiIp",
-                "sourceNet",
-                "vrf",
-                "otherErrRate",
+                "rpfErr",
+                "outPkts",
                 "rpfErrRate",
-                "avgPkt",
+                "otherErr",
+                "hostname",
+                "sourceNet",
                 "inIntName",
                 "groupNet",
-                "otherErr",
+                "inPkts",
+                "sn",
+                "otherErrRate",
+                "siteName",
                 "group",
-                "hostname",
-                "outPkts",
-                "rpfErr",
-                "outPktsRate",
-                "id"
+                "vrf"
             ],
             "description": "Multicast routing table counters with RPF and other errors",
             "summary": "MRoute Counters",
             "web_endpoint": "/technology/multicast/mroute/counters"
         }
     },
     "tables/multicast/routes/first-hop-router": {
         "api_endpoint": "/tables/multicast/routes/first-hop-router",
         "get": null,
         "post": {
             "api_endpoint": "tables/multicast/routes/first-hop-router",
             "columns": [
                 "siteName",
-                "fwdCount",
-                "hostname",
                 "sourceCount",
+                "id",
                 "sn",
-                "id"
+                "fwdCount",
+                "hostname"
             ],
             "description": "Multicast first hop routers inventory",
             "summary": "Multicast First Hop Routers",
             "web_endpoint": "/technology/multicast/mroute/first-hop-router"
         }
     },
     "tables/multicast/routes/outgoing-interfaces": {
         "api_endpoint": "/tables/multicast/routes/outgoing-interfaces",
         "get": null,
         "post": {
             "api_endpoint": "tables/multicast/routes/outgoing-interfaces",
             "columns": [
+                "family",
+                "flags",
+                "siteName",
                 "group",
+                "id",
+                "age",
                 "mode",
-                "siteName",
-                "hostname",
-                "intName",
-                "sn",
                 "sourceNet",
-                "vrf",
                 "vendor",
-                "flags",
-                "age",
-                "family",
-                "id",
-                "groupNet"
+                "groupNet",
+                "sn",
+                "vrf",
+                "hostname",
+                "intName"
             ],
             "description": "Multicast routing table outgoing interface list detail",
             "summary": "Multicast OIL",
             "web_endpoint": "/technology/multicast/mroute/oil-detail"
         }
     },
     "tables/multicast/routes/overview": {
         "api_endpoint": "/tables/multicast/routes/overview",
         "get": null,
         "post": {
             "api_endpoint": "tables/multicast/routes/overview",
             "columns": [
                 "siteName",
-                "hostname",
                 "activeRoutesCount",
+                "id",
                 "routesCount",
                 "sn",
                 "vrf",
-                "id"
+                "hostname"
             ],
             "description": "Overview of devices with multicast routes in mroute table",
             "summary": "MRoute Overview",
             "web_endpoint": "/technology/multicast/mroute/overview"
         }
     },
     "tables/multicast/routes/sources": {
         "api_endpoint": "/tables/multicast/routes/sources",
         "get": null,
         "post": {
             "api_endpoint": "tables/multicast/routes/sources",
             "columns": [
-                "group",
-                "mac",
-                "siteName",
-                "hostname",
-                "sn",
-                "vrf",
-                "sourceNet",
                 "incomingInt",
+                "oilCount",
+                "siteName",
                 "isLocal",
+                "group",
                 "id",
+                "sourceNet",
                 "groupNet",
-                "oilCount"
+                "sn",
+                "mac",
+                "vrf",
+                "hostname"
             ],
             "description": "Routers with multicast sources inventory",
             "summary": "Routers with Multicast Sources",
             "web_endpoint": "/technology/multicast/mroute/sources"
         }
     },
     "tables/multicast/routes/table": {
         "api_endpoint": "/tables/multicast/routes/table",
         "get": null,
         "post": {
             "api_endpoint": "tables/multicast/routes/table",
             "columns": [
-                "group",
+                "family",
+                "flags",
                 "siteName",
-                "hostname",
+                "group",
+                "id",
+                "age",
                 "rpfNeiIp",
-                "outIntNames",
-                "rpIp",
+                "sourceNet",
                 "inIntName",
+                "groupNet",
                 "sn",
-                "sourceNet",
+                "rpIp",
+                "outIntNames",
                 "vrf",
-                "vendor",
-                "flags",
-                "age",
-                "family",
-                "id",
-                "groupNet"
+                "hostname",
+                "vendor"
             ],
             "description": "Global multicast routing table",
             "summary": "Multicast Routing Table",
             "web_endpoint": "/technology/multicast/mroute/table"
         }
     },
     "tables/neighbors/all": {
         "api_endpoint": "/tables/neighbors/all",
         "get": null,
         "post": {
             "api_endpoint": "tables/neighbors/all",
             "columns": [
-                "localInt",
-                "netDev",
-                "remoteIpv6List",
+                "remoteIp",
                 "siteName",
-                "remoteInt",
-                "remoteSn",
-                "protocols",
                 "capabilities",
+                "id",
+                "managedDev",
+                "remoteDevType",
+                "localInt",
+                "remoteInt",
                 "remoteHost",
                 "localHost",
-                "remoteDevType",
-                "managedDev",
+                "remoteSn",
+                "protocols",
+                "remoteIpv6List",
                 "localSn",
-                "id",
-                "remoteIp"
+                "netDev"
             ],
             "description": "Discovery protocol neighbors inventory (CDP, LLDP, mDP)",
             "summary": "Discovery Protocol Neighbors",
             "web_endpoint": "/technology/cdp-lldp/all-neighbors"
         }
     },
     "tables/neighbors/endpoints": {
         "api_endpoint": "/tables/neighbors/endpoints",
         "get": null,
         "post": {
             "api_endpoint": "tables/neighbors/endpoints",
             "columns": [
-                "localInt",
-                "netDev",
-                "remoteIpv6List",
+                "remoteIp",
                 "siteName",
-                "remoteInt",
-                "remoteSn",
-                "protocols",
                 "capabilities",
+                "id",
+                "managedDev",
+                "remoteDevType",
+                "localInt",
+                "remoteInt",
                 "remoteHost",
                 "localHost",
-                "remoteDevType",
-                "managedDev",
+                "remoteSn",
+                "protocols",
+                "remoteIpv6List",
                 "localSn",
-                "id",
-                "remoteIp"
+                "netDev"
             ],
             "description": "Endpoints viewed by discover protocols",
             "summary": "Discovery Protocols - Endpoints",
             "web_endpoint": "/technology/cdp-lldp/endpoints"
         }
     },
     "tables/neighbors/unidirectional": {
         "api_endpoint": "/tables/neighbors/unidirectional",
         "get": null,
         "post": {
             "api_endpoint": "tables/neighbors/unidirectional",
             "columns": [
-                "localInt",
-                "remoteIpv6List",
+                "remoteIp",
                 "siteName",
-                "remoteInt",
-                "remoteSn",
-                "protocols",
                 "capabilities",
+                "id",
+                "remoteInt",
+                "localInt",
                 "remoteHost",
                 "localHost",
-                "localSn",
-                "id",
-                "remoteIp"
+                "remoteSn",
+                "protocols",
+                "remoteIpv6List",
+                "localSn"
             ],
             "description": "Unidirectional discovery protocol relationship between managed network devices",
             "summary": "Discovery Protocols - Unidirectional Neighbors",
             "web_endpoint": "/technology/cdp-lldp/unidirectional-neighbors"
         }
     },
     "tables/neighbors/unmanaged": {
         "api_endpoint": "/tables/neighbors/unmanaged",
         "get": null,
         "post": {
             "api_endpoint": "tables/neighbors/unmanaged",
             "columns": [
-                "localInt",
-                "remoteIpv6List",
+                "remoteIp",
                 "siteName",
-                "remoteInt",
-                "protocols",
                 "capabilities",
+                "id",
+                "remoteInt",
+                "localInt",
                 "remoteHost",
                 "localHost",
-                "localSn",
-                "id",
-                "remoteIp"
+                "protocols",
+                "remoteIpv6List",
+                "localSn"
             ],
             "description": "Unmanaged neighbors detected by discovery protocols of managed network devices",
             "summary": "Discovery protocols - Unmanaged Neighbors",
             "web_endpoint": "/technology/cdp-lldp/unmanaged-neighbors"
         }
     },
     "tables/networks": {
         "api_endpoint": "/tables/networks",
         "get": null,
         "post": {
             "api_endpoint": "tables/networks",
             "columns": [
-                "siteName",
-                "vlanId",
-                "gwcount",
                 "gwV",
-                "hosts",
-                "vrf",
+                "siteName",
                 "gwcountV",
-                "mask",
-                "gw",
+                "hosts",
+                "id",
                 "net",
-                "id"
+                "vlanId",
+                "gw",
+                "mask",
+                "vrf",
+                "gwcount"
             ],
             "description": "Detected Layer 3 network (connected/direct/local) inventory",
             "summary": "Managed Networks",
             "web_endpoint": "/technology/networks/managed-networks"
         }
     },
     "tables/networks/domain": {
         "api_endpoint": "/tables/networks/domain",
         "get": null,
         "post": {
             "api_endpoint": "tables/networks/domain",
             "columns": [
                 "siteName",
-                "routers",
                 "rd",
-                "users",
+                "routers",
                 "id",
+                "users",
                 "networks"
             ],
             "description": "",
             "summary": "POST /tables/networks/domain",
             "web_endpoint": null
         }
     },
     "tables/networks/gateway-redundancy": {
         "api_endpoint": "/tables/networks/gateway-redundancy",
         "get": null,
         "post": {
             "api_endpoint": "tables/networks/gateway-redundancy",
             "columns": [
-                "siteName",
-                "vlanId",
-                "gwcount",
                 "gwV",
-                "hosts",
-                "vrf",
+                "siteName",
                 "gwcountV",
-                "mask",
-                "gw",
+                "hosts",
+                "id",
                 "net",
-                "id"
+                "vlanId",
+                "gw",
+                "mask",
+                "vrf",
+                "gwcount"
             ],
             "description": "Inventory of available gateways for each discovered network",
             "summary": "Gateway Redundancy",
             "web_endpoint": "/technology/networks/gateway-redundancy"
         }
     },
     "tables/networks/ipv6-routes": {
         "api_endpoint": "/tables/networks/ipv6-routes",
         "get": null,
         "post": {
             "api_endpoint": "tables/networks/ipv6-routes",
             "columns": [
+                "nexthop",
                 "siteName",
-                "hostname",
-                "nhCount",
+                "nhLowestMetric",
+                "id",
                 "network",
+                "prefix",
+                "protocol",
+                "nhLowestAge",
                 "sn",
+                "nhCount",
                 "vrf",
-                "nexthop",
-                "nhLowestMetric",
-                "protocol",
-                "prefix",
-                "id",
-                "nhLowestAge"
+                "hostname"
             ],
             "description": "Global IPv6 routing table",
             "summary": "IPv6 Routing Table",
             "web_endpoint": "/technology/routing/routes/ipv6"
         }
     },
     "tables/networks/path-lookup-checks": {
         "api_endpoint": "/tables/networks/path-lookup-checks",
         "get": null,
         "post": {
             "api_endpoint": "tables/networks/path-lookup-checks",
             "columns": [
-                "parameters",
-                "srcPorts",
-                "dstPorts",
                 "networkMode",
-                "receiver",
+                "passingTraffic",
                 "result",
-                "src",
                 "securedPath",
-                "vrf",
-                "dst",
-                "expectedPassingTraffic",
                 "settings",
                 "flags",
-                "protocol",
+                "dstPorts",
+                "src",
+                "srcPorts",
                 "type",
                 "id",
-                "passingTraffic"
+                "receiver",
+                "dst",
+                "protocol",
+                "expectedPassingTraffic",
+                "vrf",
+                "parameters"
             ],
             "description": "Saved path simulations inventory, including End-to-End settings intended and simulated result.",
             "summary": "Saved Path Simulations",
             "web_endpoint": "/technology/routing/path-verifications"
         }
     },
     "tables/networks/policies/prefix-lists/ipv4": {
         "api_endpoint": "/tables/networks/policies/prefix-lists/ipv4",
         "get": null,
         "post": {
             "api_endpoint": "tables/networks/policies/prefix-lists/ipv4",
             "columns": [
-                "action",
-                "hostname",
                 "siteName",
+                "maskEqual",
+                "id",
                 "maskMax",
-                "sn",
+                "sequence",
+                "prefix",
                 "name",
+                "sn",
+                "action",
                 "mask",
-                "maskEqual",
                 "maskMin",
-                "prefix",
-                "id",
-                "sequence"
+                "hostname"
             ],
             "description": "",
             "summary": "POST /tables/networks/policies/prefix-lists/ipv4",
             "web_endpoint": "/technology/routing/prefix-lists/ipv4"
         }
     },
     "tables/networks/policies/prefix-lists/ipv6": {
         "api_endpoint": "/tables/networks/policies/prefix-lists/ipv6",
         "get": null,
         "post": {
             "api_endpoint": "tables/networks/policies/prefix-lists/ipv6",
             "columns": [
-                "action",
-                "hostname",
                 "siteName",
+                "maskEqual",
+                "id",
                 "maskMax",
-                "sn",
+                "sequence",
+                "prefix",
                 "name",
-                "maskEqual",
+                "sn",
+                "action",
                 "maskMin",
-                "prefix",
-                "id",
-                "sequence"
+                "hostname"
             ],
             "description": "",
             "summary": "POST /tables/networks/policies/prefix-lists/ipv6",
             "web_endpoint": "/technology/routing/prefix-lists/ipv6"
         }
     },
     "tables/networks/policies/routing": {
         "api_endpoint": "/tables/networks/policies/routing",
         "get": null,
         "post": {
             "api_endpoint": "tables/networks/policies/routing",
             "columns": [
-                "action",
-                "hostname",
                 "matchedBytes",
                 "siteName",
-                "continue",
-                "matchedPackets",
-                "sn",
-                "name",
                 "matchList",
-                "setList",
                 "type",
                 "id",
-                "sequence"
+                "sequence",
+                "name",
+                "sn",
+                "action",
+                "matchedPackets",
+                "setList",
+                "continue",
+                "hostname"
             ],
             "description": "",
             "summary": "POST /tables/networks/policies/routing",
             "web_endpoint": "/technology/routing/policy/policies"
         }
     },
     "tables/networks/policies/routing/interfaces": {
         "api_endpoint": "/tables/networks/policies/routing/interfaces",
         "get": null,
         "post": {
             "api_endpoint": "tables/networks/policies/routing/interfaces",
             "columns": [
+                "addressFamily",
                 "siteName",
+                "id",
+                "name",
+                "sn",
                 "hostname",
                 "intName",
-                "addressFamily",
-                "sn",
-                "name",
-                "status",
-                "id"
+                "status"
             ],
             "description": "",
             "summary": "POST /tables/networks/policies/routing/interfaces",
             "web_endpoint": "/technology/routing/policy/pbr-interfaces"
         }
     },
     "tables/networks/route-stability": {
         "api_endpoint": "/tables/networks/route-stability",
         "get": null,
         "post": {
             "api_endpoint": "tables/networks/route-stability",
             "columns": [
-                "ribCount",
                 "presence",
-                "ratioInfo",
+                "ribCount",
                 "ratioCrit",
+                "id",
                 "prefix",
                 "ratioWarn",
-                "id"
+                "ratioInfo"
             ],
             "description": "Unique routed networks, the number of times route is observed, expressed in absolute and percentage values",
             "summary": "Routing Stability",
             "web_endpoint": "/technology/routing/route-stability"
         }
     },
     "tables/networks/routes": {
         "api_endpoint": "/tables/networks/routes",
         "get": null,
         "post": {
             "api_endpoint": "tables/networks/routes",
             "columns": [
+                "nexthop",
                 "siteName",
-                "hostname",
-                "nhCount",
+                "nhLowestMetric",
+                "id",
                 "network",
+                "prefix",
+                "protocol",
+                "nhLowestAge",
                 "sn",
+                "nhCount",
                 "vrf",
-                "nexthop",
-                "nhLowestMetric",
-                "protocol",
-                "prefix",
-                "id",
-                "nhLowestAge"
+                "hostname"
             ],
             "description": "Global IPv4 routing table",
             "summary": "IPv4 Routing Table",
             "web_endpoint": "/technology/routing/routes"
         }
     },
     "tables/networks/summary/protocols": {
         "api_endpoint": "/tables/networks/summary/protocols",
         "get": null,
         "post": {
             "api_endpoint": "tables/networks/summary/protocols",
             "columns": [
                 "siteName",
-                "hostname",
-                "replicates",
-                "sn",
-                "vrf",
                 "subnets",
+                "id",
                 "memory",
                 "overhead",
+                "sn",
+                "networks",
                 "protocol",
-                "id",
-                "networks"
+                "vrf",
+                "hostname",
+                "replicates"
             ],
             "description": "Summary routing table information about routing protocols for all managed devices",
             "summary": "Network Routing Protocols Summary",
             "web_endpoint": "/technology/routing/summary/protocols"
         }
     },
     "tables/networks/summary/protocols/bgp": {
         "api_endpoint": "/tables/networks/summary/protocols/bgp",
         "get": null,
         "post": {
             "api_endpoint": "tables/networks/summary/protocols/bgp",
             "columns": [
-                "internal",
-                "hostname",
-                "siteName",
+                "external",
                 "as",
+                "siteName",
+                "id",
+                "local",
                 "sn",
+                "internal",
                 "vrf",
-                "local",
-                "external",
-                "id"
+                "hostname"
             ],
             "description": "Border Gateway Protocol (BGP) routes summary",
             "summary": "BGP Protocol Routes Summary",
             "web_endpoint": "/technology/routing/summary/bgp"
         }
     },
     "tables/networks/summary/protocols/eigrp": {
         "api_endpoint": "/tables/networks/summary/protocols/eigrp",
         "get": null,
         "post": {
             "api_endpoint": "tables/networks/summary/protocols/eigrp",
             "columns": [
                 "siteName",
-                "hostname",
-                "replicates",
-                "sn",
-                "vrf",
                 "subnets",
+                "id",
                 "memory",
                 "overhead",
+                "sn",
+                "networks",
                 "protocol",
-                "id",
-                "networks"
+                "vrf",
+                "hostname",
+                "replicates"
             ],
             "description": "Enhanced Interior Gateway Routing Protocol (EIGRP) routes summary",
             "summary": "EIGRP Protocol Routes Summary",
             "web_endpoint": "/technology/routing/summary/eigrp"
         }
     },
     "tables/networks/summary/protocols/isis": {
         "api_endpoint": "/tables/networks/summary/protocols/isis",
         "get": null,
         "post": {
             "api_endpoint": "tables/networks/summary/protocols/isis",
             "columns": [
-                "level2",
+                "level1",
                 "siteName",
-                "hostname",
                 "interArea",
+                "id",
+                "level2",
                 "sn",
                 "vrf",
-                "level1",
-                "id"
+                "hostname"
             ],
             "description": "Intermediate System to Intermediate System (IS-IS) routes summary",
             "summary": "IS-IS Protocol Routes Summary",
             "web_endpoint": "/technology/routing/summary/isis"
         }
     },
     "tables/networks/summary/protocols/ospf": {
         "api_endpoint": "/tables/networks/summary/protocols/ospf",
         "get": null,
         "post": {
             "api_endpoint": "tables/networks/summary/protocols/ospf",
             "columns": [
-                "nssaEx2",
+                "vrf",
                 "external1",
-                "intraArea",
+                "interArea",
                 "process",
-                "hostname",
-                "nssaEx1",
                 "siteName",
-                "interArea",
+                "id",
+                "nssaEx1",
                 "sn",
-                "vrf",
-                "external2",
-                "id"
+                "nssaEx2",
+                "intraArea",
+                "hostname",
+                "external2"
             ],
             "description": "Open Shortest Path First routes summary",
             "summary": "OSPF Protocol Routes Summary",
             "web_endpoint": "/technology/routing/summary/ospf"
         }
     },
     "tables/networks/summary/protocols/ospfv3": {
         "api_endpoint": "/tables/networks/summary/protocols/ospfv3",
         "get": null,
         "post": {
             "api_endpoint": "tables/networks/summary/protocols/ospfv3",
             "columns": [
-                "nssaEx2",
+                "vrf",
                 "external1",
-                "intraArea",
+                "interArea",
                 "siteName",
-                "hostname",
+                "id",
                 "nssaEx1",
-                "interArea",
                 "sn",
-                "vrf",
-                "external2",
-                "id"
+                "nssaEx2",
+                "intraArea",
+                "hostname",
+                "external2"
             ],
             "description": "Open Shortest Path First v3 (OSPFv3) routes summary",
             "summary": "OSPFv3 Protocol Routes Summary",
             "web_endpoint": "/technology/routing/summary/ospfv3"
         }
     },
     "tables/networks/summary/protocols/rip": {
         "api_endpoint": "/tables/networks/summary/protocols/rip",
         "get": null,
         "post": {
             "api_endpoint": "tables/networks/summary/protocols/rip",
             "columns": [
                 "siteName",
-                "hostname",
-                "replicates",
-                "sn",
-                "vrf",
                 "subnets",
+                "id",
                 "memory",
                 "overhead",
+                "sn",
+                "networks",
                 "protocol",
-                "id",
-                "networks"
+                "vrf",
+                "hostname",
+                "replicates"
             ],
             "description": "Routing Information Protocol (RIP) routes summary",
             "summary": "RIP Protocol Routes Summary",
             "web_endpoint": "/technology/routing/summary/rip"
         }
     },
     "tables/platforms/cluster/srx": {
         "api_endpoint": "/tables/platforms/cluster/srx",
         "get": null,
         "post": {
             "api_endpoint": "tables/platforms/cluster/srx",
             "columns": [
-                "group",
                 "siteName",
-                "hostname",
-                "sn",
-                "name",
                 "clusterId",
-                "state",
                 "type",
+                "group",
                 "id",
-                "priority"
+                "priority",
+                "state",
+                "name",
+                "sn",
+                "hostname"
             ],
             "description": "Juniper SRX Clusters inventory",
             "summary": "Juniper SRX Cluster",
             "web_endpoint": "/technology/platforms/cluster/srx"
         }
     },
     "tables/platforms/devices": {
         "api_endpoint": "/tables/platforms/devices",
         "get": null,
         "post": {
             "api_endpoint": "tables/platforms/devices",
             "columns": [
-                "contextId",
                 "siteName",
-                "hostname",
+                "id",
                 "sn",
                 "contextType",
                 "contextName",
-                "id"
+                "contextId",
+                "hostname"
             ],
             "description": "",
             "summary": "POST /tables/platforms/devices",
             "web_endpoint": "/technology/platforms/logical-devices"
         }
     },
     "tables/platforms/fabric-path/neighbors": {
         "api_endpoint": "/tables/platforms/fabric-path/neighbors",
         "get": null,
         "post": {
             "api_endpoint": "tables/platforms/fabric-path/neighbors",
             "columns": [
                 "siteName",
-                "hostname",
-                "level",
-                "holdTime",
-                "interfaces",
-                "sn",
                 "systemId",
+                "holdTime",
+                "id",
                 "state",
-                "id"
+                "level",
+                "sn",
+                "hostname",
+                "interfaces"
             ],
             "description": "",
             "summary": "POST /tables/platforms/fabric-path/neighbors",
             "web_endpoint": "/technology/platforms/cisco-fabric-path/isis-neighbors"
         }
     },
     "tables/platforms/fabric-path/routes": {
         "api_endpoint": "/tables/platforms/fabric-path/routes",
         "get": null,
         "post": {
             "api_endpoint": "tables/platforms/fabric-path/routes",
             "columns": [
-                "switchId",
                 "siteName",
-                "hostname",
+                "id",
+                "switchId",
+                "physicalInterfaces",
                 "localId",
                 "sn",
                 "subswitchId",
-                "physicalInterfaces",
-                "id"
+                "hostname"
             ],
             "description": "",
             "summary": "POST /tables/platforms/fabric-path/routes",
             "web_endpoint": "/technology/platforms/cisco-fabric-path/routes"
         }
     },
     "tables/platforms/fabric-path/summary": {
         "api_endpoint": "/tables/platforms/fabric-path/summary",
         "get": null,
         "post": {
             "api_endpoint": "tables/platforms/fabric-path/summary",
             "columns": [
                 "siteName",
-                "hostname",
-                "routesCount",
-                "sn",
                 "switchesCount",
+                "id",
                 "neighborsCount",
-                "id"
+                "routesCount",
+                "sn",
+                "hostname"
             ],
             "description": "",
             "summary": "POST /tables/platforms/fabric-path/summary",
             "web_endpoint": "/technology/platforms/cisco-fabric-path/summary"
         }
     },
     "tables/platforms/fabric-path/switches": {
         "api_endpoint": "/tables/platforms/fabric-path/switches",
         "get": null,
         "post": {
             "api_endpoint": "tables/platforms/fabric-path/switches",
             "columns": [
-                "switchId",
                 "siteName",
-                "hostname",
-                "emulatedAnycast",
-                "sn",
-                "local",
-                "systemId",
-                "static",
                 "flags",
+                "systemId",
+                "id",
                 "state",
-                "id"
+                "local",
+                "switchId",
+                "sn",
+                "emulatedAnycast",
+                "static",
+                "hostname"
             ],
             "description": "",
             "summary": "POST /tables/platforms/fabric-path/switches",
             "web_endpoint": "/technology/platforms/cisco-fabric-path/switch-ids"
         }
     },
     "tables/platforms/fex/interfaces": {
         "api_endpoint": "/tables/platforms/fex/interfaces",
         "get": null,
         "post": {
             "api_endpoint": "tables/platforms/fex/interfaces",
             "columns": [
-                "fex",
+                "fexIntName",
+                "fexSn",
                 "siteName",
-                "hostname",
-                "intName",
+                "id",
                 "sn",
-                "fexSn",
-                "fexIntName",
-                "id"
+                "hostname",
+                "fex",
+                "intName"
             ],
             "description": "Cisco Fabric EXtender (FEX) interfaces inventory",
             "summary": "Cisco FEX Interfaces",
             "web_endpoint": "/technology/platforms/fex/fex-ints"
         }
     },
     "tables/platforms/fex/modules": {
         "api_endpoint": "/tables/platforms/fex/modules",
         "get": null,
         "post": {
             "api_endpoint": "tables/platforms/fex/modules",
             "columns": [
-                "fex",
-                "sn",
-                "ver",
+                "model",
                 "parents",
                 "fexId",
-                "model",
-                "id"
+                "id",
+                "sn",
+                "ver",
+                "fex"
             ],
             "description": "Cisco Fabric EXtender (FEX) modules inventory",
             "summary": "Cisco FEX Modules",
             "web_endpoint": "/technology/platforms/fex/fex-modules"
         }
     },
     "tables/platforms/mlag/pairs": {
         "api_endpoint": "/tables/platforms/mlag/pairs",
         "get": null,
         "post": {
             "api_endpoint": "tables/platforms/mlag/pairs",
             "columns": [
-                "primaryStatus",
-                "primaryLinkIntName",
+                "secondaryHostname",
+                "primarySn",
                 "siteName",
-                "secondaryLinkIntName",
-                "primaryHostname",
+                "primaryLinkIntName",
+                "systemId",
+                "id",
+                "secondaryStatus",
                 "domain",
-                "secondaryHostname",
+                "secondaryLinkIntName",
+                "primaryStatus",
                 "secondarySn",
-                "secondaryStatus",
-                "systemId",
-                "primarySn",
-                "id"
+                "primaryHostname"
             ],
             "description": "Multi-chassis link aggregation group (MLAG) pairs inventory",
             "summary": "MLAG Pairs",
             "web_endpoint": "/technology/port-channels/mlag/pairs"
         }
     },
     "tables/platforms/mlag/peers": {
         "api_endpoint": "/tables/platforms/mlag/peers",
         "get": null,
         "post": {
             "api_endpoint": "tables/platforms/mlag/peers",
             "columns": [
+                "remoteIp",
                 "siteName",
-                "hostname",
-                "domain",
-                "localIp",
-                "sn",
                 "systemId",
-                "status",
-                "linkIntName",
-                "role",
                 "type",
                 "id",
-                "remoteIp"
+                "linkIntName",
+                "sn",
+                "domain",
+                "localIp",
+                "role",
+                "hostname",
+                "status"
             ],
             "description": "Multi-chassis link aggregation group (MLAG) peer-links inventory",
             "summary": "MLAG Peer Links",
             "web_endpoint": "/technology/port-channels/mlag/peer-links"
         }
     },
     "tables/platforms/mlag/switches": {
         "api_endpoint": "/tables/platforms/mlag/switches",
         "get": null,
         "post": {
             "api_endpoint": "tables/platforms/mlag/switches",
             "columns": [
                 "siteName",
-                "hostname",
-                "domain",
-                "sn",
                 "systemId",
                 "type",
-                "id"
+                "id",
+                "sn",
+                "domain",
+                "hostname"
             ],
             "description": "Multi-chassis link aggregation group (MLAG) switches inventory",
             "summary": "MLAG Switches",
             "web_endpoint": "/technology/port-channels/mlag/switches"
         }
     },
     "tables/platforms/mlag/vpc": {
         "api_endpoint": "/tables/platforms/mlag/vpc",
         "get": null,
         "post": {
             "api_endpoint": "tables/platforms/mlag/vpc",
             "columns": [
                 "siteName",
-                "hostname",
-                "intName",
+                "id",
+                "sn",
                 "keepaliveStatus",
                 "domain",
-                "sn",
-                "status",
                 "role",
-                "id",
-                "configConsistStatus"
+                "configConsistStatus",
+                "hostname",
+                "intName",
+                "status"
             ],
             "description": "Cisco vPC (Virtual Port-Channel) domains and interfaces inventory",
             "summary": "Cisco vPC",
             "web_endpoint": "/technology/port-channels/mlag/vpc"
         }
     },
     "tables/platforms/poe/devices": {
         "api_endpoint": "/tables/platforms/poe/devices",
         "get": null,
         "post": {
             "api_endpoint": "tables/platforms/poe/devices",
             "columns": [
-                "operOnCount",
                 "siteName",
-                "hostname",
-                "sn",
                 "powerUsedSum",
-                "poeDeviceClassMax",
-                "powerFromPsSum",
+                "operOnCount",
                 "id",
-                "interfacesCount"
+                "poeDeviceClassMax",
+                "sn",
+                "interfacesCount",
+                "hostname",
+                "powerFromPsSum"
             ],
             "description": "Power over Ethernet (PoE) devices inventory",
             "summary": "PoE devices",
             "web_endpoint": "/technology/platforms/poe/devices"
         }
     },
     "tables/platforms/poe/interfaces": {
         "api_endpoint": "/tables/platforms/poe/interfaces",
         "get": null,
         "post": {
             "api_endpoint": "tables/platforms/poe/interfaces",
             "columns": [
-                "admin",
-                "poeDeviceName",
+                "powerUsed",
                 "siteName",
-                "intName",
-                "hostname",
+                "powerFromPs",
+                "id",
+                "powerMax",
                 "powerGranted",
                 "sn",
+                "admin",
+                "poeDeviceName",
+                "poeDeviceClass",
                 "oper",
-                "powerUsed",
-                "powerMax",
-                "powerFromPs",
-                "id",
-                "poeDeviceClass"
+                "hostname",
+                "intName"
             ],
             "description": "Power over Ethernet (PoE) interfaces inventory",
             "summary": "PoE Interfaces",
             "web_endpoint": "/technology/platforms/poe/interfaces"
         }
     },
     "tables/platforms/poe/modules": {
         "api_endpoint": "/tables/platforms/poe/modules",
         "get": null,
         "post": {
             "api_endpoint": "tables/platforms/poe/modules",
             "columns": [
+                "wattsRemaining",
+                "siteName",
                 "wattsAvailable",
+                "id",
                 "wattsUsed",
-                "siteName",
-                "hostname",
+                "sn",
                 "wattsUsedPct",
                 "moduleId",
-                "sn",
-                "wattsRemaining",
-                "id",
-                "isPoE"
+                "isPoE",
+                "hostname"
             ],
             "description": "Power over Ethernet (PoE) and associated device modules inventory",
             "summary": "PoE - Device Modules",
             "web_endpoint": "/technology/platforms/poe/modules"
         }
     },
     "tables/platforms/stack": {
         "api_endpoint": "/tables/platforms/stack",
         "get": null,
         "post": {
             "api_endpoint": "tables/platforms/stack",
             "columns": [
+                "master",
                 "siteName",
                 "connectionsCount",
-                "sn",
-                "master",
-                "uptimeLow",
-                "membersCount",
+                "id",
                 "uptimeDiff",
-                "id"
+                "membersCount",
+                "sn",
+                "uptimeLow"
             ],
             "description": "Discovered switch stacks, number of members in each stack, and the total number of stack ports",
             "summary": "Switch stacks",
             "web_endpoint": "/technology/platforms/stack/stacks"
         }
     },
     "tables/platforms/stack/connections": {
         "api_endpoint": "/tables/platforms/stack/connections",
         "get": null,
         "post": {
             "api_endpoint": "tables/platforms/stack/connections",
             "columns": [
-                "siteName",
-                "member",
-                "interfaces",
-                "sn",
-                "status",
+                "membersKnownCount",
                 "master",
+                "siteName",
+                "stackPort",
+                "id",
                 "membersCount",
+                "sn",
+                "member",
                 "neiSwitchId",
-                "membersKnownCount",
-                "stackPort",
-                "id"
+                "interfaces",
+                "status"
             ],
             "description": "Switch stack interfaces and their current state",
             "summary": "Stack Ports",
             "web_endpoint": "/technology/platforms/stack/connections"
         }
     },
     "tables/platforms/stack/members": {
         "api_endpoint": "/tables/platforms/stack/members",
         "get": null,
         "post": {
             "api_endpoint": "tables/platforms/stack/members",
             "columns": [
-                "uptime",
-                "hwVer",
+                "master",
+                "image",
                 "siteName",
-                "member",
                 "pn",
-                "sn",
                 "connectionsCount",
-                "ver",
-                "master",
-                "role",
-                "state",
                 "id",
                 "memberSn",
-                "mac",
-                "image"
+                "state",
+                "uptime",
+                "sn",
+                "member",
+                "hwVer",
+                "ver",
+                "role",
+                "mac"
             ],
             "description": "Stack members and their current state",
             "summary": "Stack Members",
             "web_endpoint": "/technology/platforms/stack/members"
         }
     },
     "tables/platforms/vdc/devices": {
         "api_endpoint": "/tables/platforms/vdc/devices",
         "get": null,
         "post": {
             "api_endpoint": "tables/platforms/vdc/devices",
             "columns": [
-                "vdcId",
                 "siteName",
-                "hostname",
-                "stpDomain",
                 "rd",
-                "sn",
+                "id",
                 "snHw",
-                "id"
+                "sn",
+                "stpDomain",
+                "vdcId",
+                "hostname"
             ],
             "description": "Cisco Virtual Device Context (VDC) devices inventory",
             "summary": "Cisco VDC Devices",
             "web_endpoint": "/technology/platforms/vdc/vdc-devices"
         }
     },
     "tables/platforms/vss/chassis": {
         "api_endpoint": "/tables/platforms/vss/chassis",
         "get": null,
         "post": {
             "api_endpoint": "tables/platforms/vss/chassis",
             "columns": [
+                "chassisId",
                 "siteName",
-                "currentStateTime",
-                "hostname",
+                "controlState",
+                "id",
+                "state",
+                "version",
                 "sn",
-                "chassisId",
                 "slot",
-                "version",
-                "state",
                 "fabricState",
-                "controlState",
-                "id",
-                "chassisSn"
+                "hostname",
+                "chassisSn",
+                "currentStateTime"
             ],
             "description": "Cisco Virtual Switching System (VSS) chassis information overview",
             "summary": "Cisco VSS Chassis",
             "web_endpoint": "/technology/platforms/vss/chassis"
         }
     },
     "tables/platforms/vss/overview": {
         "api_endpoint": "/tables/platforms/vss/overview",
         "get": null,
         "post": {
             "api_endpoint": "tables/platforms/vss/overview",
             "columns": [
-                "operatingRedundancyMode",
-                "peerSwitchId",
-                "configuredRedundancyMode",
-                "hostname",
-                "domainNumber",
                 "siteName",
+                "configuredRedundancyMode",
+                "id",
                 "switchId",
+                "peerSwitchId",
+                "operatingRedundancyMode",
                 "sn",
+                "domainNumber",
                 "switchoverReason",
-                "id"
+                "hostname"
             ],
             "description": "Cisco Virtual Switching System (VSS) protocol overview",
             "summary": "Cisco VSS Overview",
             "web_endpoint": "/technology/platforms/vss/overview"
         }
     },
     "tables/platforms/vss/vsl": {
         "api_endpoint": "/tables/platforms/vss/vsl",
         "get": null,
         "post": {
             "api_endpoint": "tables/platforms/vss/vsl",
             "columns": [
-                "portList",
                 "siteName",
-                "hostname",
-                "sn",
                 "flags",
                 "portChannel",
-                "id"
+                "id",
+                "sn",
+                "portList",
+                "hostname"
             ],
             "description": "Cisco virtual switch link (VSL) overview",
             "summary": "Cisco VSL",
             "web_endpoint": "/technology/platforms/vss/vsl"
         }
     },
     "tables/policies": {
         "api_endpoint": "/tables/policies",
         "get": null,
         "post": {
             "api_endpoint": "tables/policies",
             "columns": [
-                "description",
-                "isSystem",
                 "apiScopeIds",
+                "scopeType",
+                "id",
+                "name",
                 "attributeFilters",
                 "attributeScopeIds",
-                "name",
-                "scopeType",
-                "id"
+                "description",
+                "isSystem"
             ],
             "description": "",
             "summary": "POST /tables/policies",
             "web_endpoint": "/settings/administration/policies"
         }
     },
     "tables/qos/marking": {
         "api_endpoint": "/tables/qos/marking",
         "get": null,
         "post": {
             "api_endpoint": "tables/qos/marking",
             "columns": [
-                "value",
                 "siteName",
-                "intName",
-                "hostname",
-                "policy",
                 "parentPolicy",
+                "type",
+                "id",
+                "childPolicy",
                 "sn",
-                "match",
                 "packets",
-                "childPolicy",
+                "set",
                 "class",
-                "type",
-                "id",
-                "set"
+                "match",
+                "value",
+                "hostname",
+                "policy",
+                "intName"
             ],
             "description": "Quality of Service (QoS) marking policies",
             "summary": "QoS Marking",
             "web_endpoint": "/technology/qos/marking"
         }
     },
     "tables/qos/policing": {
         "api_endpoint": "/tables/qos/policing",
         "get": null,
         "post": {
             "api_endpoint": "tables/qos/policing",
             "columns": [
-                "siteName",
-                "exceededBps",
-                "sn",
-                "conformedBytes",
-                "bc",
-                "match",
-                "childPolicy",
-                "cir",
-                "intName",
-                "hostname",
-                "conformedPkts",
-                "exceededBytes",
                 "type",
-                "action",
-                "exceededPkts",
-                "policy",
-                "parentPolicy",
+                "id",
                 "policeType",
+                "exceededBytes",
+                "policy",
+                "intName",
+                "cir",
+                "match",
                 "class",
+                "conformedPkts",
+                "hostname",
+                "bc",
+                "sn",
+                "childPolicy",
+                "exceededPkts",
                 "conformedBps",
-                "id"
+                "siteName",
+                "parentPolicy",
+                "conformedBytes",
+                "action",
+                "exceededBps"
             ],
             "description": "Quality of Service (QoS) policing rules'",
             "summary": "QoS Policing",
             "web_endpoint": "/technology/qos/policing"
         }
     },
     "tables/qos/policy-maps": {
         "api_endpoint": "/tables/qos/policy-maps",
         "get": null,
         "post": {
             "api_endpoint": "tables/qos/policy-maps",
             "columns": [
-                "rateDrop",
                 "siteName",
-                "hostname",
-                "intName",
-                "rateOffered",
-                "policy",
                 "parentPolicy",
-                "bytes",
+                "rateDrop",
+                "type",
+                "id",
+                "rateInterval",
+                "childPolicy",
+                "rateOffered",
                 "sn",
-                "match",
                 "packets",
-                "childPolicy",
-                "rateInterval",
                 "class",
-                "type",
-                "id"
+                "match",
+                "policy",
+                "hostname",
+                "bytes",
+                "intName"
             ],
             "description": "Quality of Service (QoS) applied service policies to interfaces",
             "summary": "QoS Applied Service-Policies",
             "web_endpoint": "/technology/qos/policy-class-map"
         }
     },
     "tables/qos/priority-queuing": {
         "api_endpoint": "/tables/qos/priority-queuing",
         "get": null,
         "post": {
             "api_endpoint": "tables/qos/priority-queuing",
             "columns": [
                 "siteName",
-                "intName",
-                "hostname",
-                "exDrops",
-                "policy",
                 "parentPolicy",
-                "sn",
-                "match",
+                "type",
+                "id",
                 "childPolicy",
+                "sn",
                 "strictPriority",
                 "class",
-                "type",
-                "id"
+                "match",
+                "exDrops",
+                "hostname",
+                "policy",
+                "intName"
             ],
             "description": "Quality of Service (QoS) policies and classes and associated parameters",
             "summary": "QoS Priority Policies and Classes",
             "web_endpoint": "/technology/qos/priority-queueing"
         }
     },
     "tables/qos/queuing": {
         "api_endpoint": "/tables/qos/queuing",
         "get": null,
         "post": {
             "api_endpoint": "tables/qos/queuing",
             "columns": [
-                "pktsOutput",
                 "queueDepth",
                 "siteName",
-                "intName",
-                "hostname",
-                "totalDrops",
-                "policy",
                 "parentPolicy",
-                "noBufferDrops",
-                "sn",
-                "match",
+                "type",
+                "totalDrops",
+                "pktsOutput",
+                "id",
+                "queueLimit",
                 "bandwidth",
                 "childPolicy",
-                "queueLimit",
-                "class",
+                "sn",
                 "bytesOutput",
-                "type",
-                "id"
+                "noBufferDrops",
+                "class",
+                "match",
+                "hostname",
+                "policy",
+                "intName"
             ],
             "description": "Quality of Service (QoS) policy and classes queing parameters",
             "summary": "QoS Queuing",
             "web_endpoint": "/technology/qos/queueing"
         }
     },
     "tables/qos/random-drops": {
         "api_endpoint": "/tables/qos/random-drops",
         "get": null,
         "post": {
             "api_endpoint": "tables/qos/random-drops",
             "columns": [
-                "siteName",
-                "classRandom",
-                "sn",
-                "tailDropPkts",
+                "type",
+                "id",
                 "ranDropPkts",
-                "transBytes",
-                "maxThresh",
-                "match",
-                "tailDropBytes",
-                "childPolicy",
+                "policy",
                 "intName",
+                "minThresh",
+                "transBytes",
+                "class",
                 "hostname",
-                "markProb",
-                "type",
+                "sn",
+                "classRandom",
+                "tailDropPkts",
+                "childPolicy",
                 "transPkts",
-                "minThresh",
-                "policy",
-                "parentPolicy",
+                "tailDropBytes",
+                "maxThresh",
+                "markProb",
                 "ranDropBytes",
-                "class",
-                "id"
+                "siteName",
+                "parentPolicy",
+                "match"
             ],
             "description": "Inventory of classes with a random early drop detection action and associated parameters",
             "summary": "QoS Classes with Random Drops",
             "web_endpoint": "/technology/qos/random-drops"
         }
     },
     "tables/qos/shaping": {
         "api_endpoint": "/tables/qos/shaping",
         "get": null,
         "post": {
             "api_endpoint": "tables/qos/shaping",
             "columns": [
                 "be",
                 "siteName",
-                "intName",
-                "hostname",
-                "shapeType",
-                "policy",
-                "parentPolicy",
-                "sn",
-                "match",
-                "childPolicy",
                 "cir",
-                "targetRate",
-                "class",
+                "parentPolicy",
                 "type",
+                "targetRate",
                 "id",
-                "bc"
+                "childPolicy",
+                "bc",
+                "sn",
+                "class",
+                "match",
+                "shapeType",
+                "hostname",
+                "policy",
+                "intName"
             ],
             "description": "Quality of Service (QoS) classes and shaping information",
             "summary": "QoS Shaping",
             "web_endpoint": "/technology/qos/shaping"
         }
     },
     "tables/reports/discovery-errors": {
         "api_endpoint": "/tables/reports/discovery-errors",
         "get": null,
         "post": {
             "api_endpoint": "tables/reports/discovery-errors",
             "columns": [
+                "slug",
+                "objectId",
                 "hasLogFile",
+                "id",
+                "errorType",
+                "errorText",
                 "loginIp",
-                "dnsName",
+                "version",
                 "taskId",
                 "loginType",
-                "objectId",
-                "slug",
-                "errorText",
-                "version",
-                "errorType",
-                "id"
+                "dnsName"
             ],
             "description": "",
             "summary": "POST /tables/reports/discovery-errors",
             "web_endpoint": "/snapshot-management/errors"
         }
     },
     "tables/reports/discovery-tasks": {
         "api_endpoint": "/tables/reports/discovery-tasks",
         "get": null,
         "post": {
             "api_endpoint": "tables/reports/discovery-tasks",
             "columns": [
+                "slug",
+                "objectId",
                 "hasLogFile",
-                "attemptCount",
-                "context",
-                "dnsName",
+                "id",
+                "errorType",
+                "vendor",
                 "errorMessage",
+                "context",
                 "errorReasons",
-                "vendor",
-                "status",
-                "ip",
-                "objectId",
-                "slug",
-                "errorType",
                 "mac",
-                "id",
-                "source"
+                "source",
+                "ip",
+                "attemptCount",
+                "dnsName",
+                "status"
             ],
             "description": "",
             "summary": "POST /tables/reports/discovery-tasks",
             "web_endpoint": "/snapshot-management/tasks"
         }
     },
     "tables/reports/eof/detail": {
         "api_endpoint": "/tables/reports/eof/detail",
         "get": null,
         "post": {
             "api_endpoint": "tables/reports/eof/detail",
             "columns": [
-                "url",
-                "endMaintenance",
+                "deviceSn",
+                "family",
+                "model",
                 "siteName",
-                "endSupport",
-                "hostname",
-                "platform",
                 "dscr",
+                "platform",
+                "id",
+                "replacement",
                 "sn",
+                "endSupport",
+                "pid",
+                "url",
                 "endSale",
+                "hostname",
                 "vendor",
-                "pid",
-                "model",
-                "replacement",
-                "deviceSn",
-                "family",
-                "id"
+                "endMaintenance"
             ],
             "description": "End of Life (EoL) detailed information on all detected part number for managed network devices",
             "summary": "Hardware EoL - Detail",
             "web_endpoint": "/inventory/end-of-life-milestones/detail"
         }
     },
     "tables/reports/eof/summary": {
         "api_endpoint": "/tables/reports/eof/summary",
         "get": null,
         "post": {
             "api_endpoint": "tables/reports/eof/summary",
             "columns": [
-                "url",
-                "endMaintenance",
-                "endSupport",
                 "dscr",
+                "id",
                 "pidCount",
+                "replacement",
+                "endSupport",
+                "pid",
+                "url",
                 "endSale",
                 "vendor",
-                "pid",
-                "replacement",
-                "id"
+                "endMaintenance"
             ],
             "description": "End of Life (EoL) summary information on all detected part number for managed network devices",
             "summary": "Hardware EoL - Summary",
             "web_endpoint": "/inventory/end-of-life-milestones/summary"
         }
     },
     "tables/reports/settings-oui": {
         "api_endpoint": "/tables/reports/settings-oui",
         "get": null,
         "post": {
             "api_endpoint": "tables/reports/settings-oui",
             "columns": [
+                "id",
                 "enabled",
-                "vendor",
                 "oui",
-                "id"
+                "vendor"
             ],
             "description": "Internal database for Organizational Unique Identifier (OUI) to either allow ARP discovery or not",
             "summary": "Settings for OUI Discovery",
             "web_endpoint": "/settings/discovery-snapshots/global-discovery-configuration/oui"
         }
     },
     "tables/roles": {
         "api_endpoint": "/tables/roles",
         "get": null,
         "post": {
             "api_endpoint": "tables/roles",
             "columns": [
-                "isAdmin",
-                "description",
-                "isSystem",
-                "name",
                 "policyIds",
                 "type",
-                "id"
+                "id",
+                "name",
+                "isAdmin",
+                "description",
+                "isSystem"
             ],
             "description": "User management roles database used for user management policies",
             "summary": "RBAC - User Management Roles",
             "web_endpoint": "/settings/administration/roles"
         }
     },
     "tables/routing/protocols/bgp/address-families": {
         "api_endpoint": "/tables/routing/protocols/bgp/address-families",
         "get": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/bgp/address-families",
             "columns": [
-                "totalReceivedPrefixes",
-                "localAddress",
-                "siteName",
-                "devType",
-                "sn",
-                "neiDevType",
+                "neiHostname",
+                "type",
+                "id",
+                "keepalive",
+                "neiSiteName",
                 "localAs",
+                "neiSn",
+                "neiDevType",
+                "neiAddress",
+                "family",
+                "localAddress",
+                "localAddressV6",
+                "dstInt",
+                "hostname",
+                "holdTime",
+                "state",
                 "source",
+                "sn",
+                "totalReceivedPrefixes",
+                "receivedPrefix",
                 "target",
-                "neiAddress",
-                "neiId",
-                "vrf",
-                "neiAs",
-                "neiHostname",
                 "neiAddressV6",
-                "hostname",
+                "siteName",
                 "currStateTime",
-                "holdTime",
-                "neiSn",
-                "neiSiteName",
-                "type",
+                "neiAs",
+                "devType",
                 "localId",
-                "receivedPrefix",
-                "dstInt",
-                "localAddressV6",
-                "state",
-                "family",
-                "id",
-                "keepalive"
+                "vrf",
+                "neiId"
             ],
             "description": "Border Gateway Protocol (BGP) and its address-families inventory",
             "summary": "BGP Address Families",
             "web_endpoint": "/technology/routing/bgp/address-families"
         }
     },
     "tables/routing/protocols/bgp/neighbors": {
         "api_endpoint": "/tables/routing/protocols/bgp/neighbors",
         "get": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/bgp/neighbors",
             "columns": [
-                "totalReceivedPrefixes",
-                "localAddress",
-                "siteName",
-                "sn",
-                "neiDevType",
+                "neiHostname",
+                "type",
+                "id",
+                "keepalive",
+                "neiSiteName",
                 "localAs",
-                "source",
-                "routingPoliciesOut",
-                "target",
+                "neiSn",
+                "neiDevType",
                 "neiAddress",
-                "neiId",
-                "vrf",
-                "neiAs",
+                "localAddress",
                 "srcInt",
-                "neiHostname",
-                "routingPoliciesIn",
-                "neiAddressV6",
+                "localAddressV6",
+                "routingPoliciesOut",
+                "dstInt",
                 "hostname",
-                "currStateTime",
                 "holdTime",
-                "neiSn",
-                "neiSiteName",
-                "type",
-                "localId",
-                "dstInt",
-                "localAddressV6",
                 "state",
+                "routingPoliciesIn",
+                "source",
+                "sn",
+                "totalReceivedPrefixes",
+                "target",
+                "neiAddressV6",
+                "siteName",
+                "currStateTime",
+                "neiAs",
                 "devType",
-                "id",
-                "keepalive"
+                "localId",
+                "vrf",
+                "neiId"
             ],
             "description": "Border Gateway Protocol (BGP) neighbors inventory",
             "summary": "BGP Neighbors",
             "web_endpoint": "/technology/routing/bgp/neighbors"
         }
     },
     "tables/routing/protocols/eigrp/interfaces": {
         "api_endpoint": "/tables/routing/protocols/eigrp/interfaces",
         "get": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/eigrp/interfaces",
             "columns": [
-                "neiCount",
                 "siteName",
-                "hostname",
-                "intName",
-                "timerHold",
+                "id",
                 "sn",
-                "vrf",
-                "localAsn",
+                "timerHold",
+                "neiCount",
                 "timerHello",
-                "id"
+                "vrf",
+                "hostname",
+                "intName",
+                "localAsn"
             ],
             "description": "Enhanced Interior Gateway Routing Protocol (EIGRP) interfaces inventory",
             "summary": "EIGRP Interfaces",
             "web_endpoint": "/technology/routing/eigrp/interfaces"
         }
     },
     "tables/routing/protocols/eigrp/neighbors": {
         "api_endpoint": "/tables/routing/protocols/eigrp/neighbors",
         "get": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/eigrp/neighbors",
             "columns": [
-                "localAddress",
-                "siteName",
-                "sn",
-                "neiAsn",
-                "neiDevType",
-                "target",
-                "neiAddress",
-                "vrf",
                 "neiHostname",
+                "id",
+                "neiSiteName",
+                "neiSn",
+                "neiDevType",
+                "intName",
                 "localAsn",
-                "subnet",
+                "neiAddress",
+                "neiIntName",
+                "localAddress",
                 "hostname",
-                "intName",
+                "subnet",
+                "source",
+                "sn",
+                "siteName",
                 "currStateTime",
-                "neiSn",
-                "neiIntName",
-                "neiSiteName",
                 "devType",
-                "id",
-                "source"
+                "neiAsn",
+                "vrf",
+                "target"
             ],
             "description": "Enhanced Interior Gateway Routing Protocol (EIGRP) neighbors inventory",
             "summary": "EIGRP Neighbors",
             "web_endpoint": "/technology/routing/eigrp/neighbors"
         }
     },
     "tables/routing/protocols/is-is/interfaces": {
         "api_endpoint": "/tables/routing/protocols/is-is/interfaces",
         "get": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/is-is/interfaces",
             "columns": [
-                "levelConfig",
-                "neiCount",
+                "snpa",
                 "siteName",
-                "hostname",
                 "circuitType",
-                "intName",
+                "circuitLevel",
+                "id",
                 "sn",
+                "levelConfig",
+                "neiCount",
                 "vrf",
-                "snpa",
-                "circuitLevel",
-                "id"
+                "hostname",
+                "intName"
             ],
             "description": "Intermediate System to Intermediate System (IS-IS) interfaces inventory",
             "summary": "IS-IS Interfaces",
             "web_endpoint": "/technology/routing/is-is/interfaces"
         }
     },
     "tables/routing/protocols/is-is/levels": {
         "api_endpoint": "/tables/routing/protocols/is-is/levels",
         "get": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/is-is/levels",
             "columns": [
+                "localPassive",
+                "localHoldTime",
                 "siteName",
-                "hostname",
-                "intName",
                 "localHello",
-                "remoteIntName",
                 "localPriority",
+                "id",
+                "state",
+                "localMetric",
                 "remoteSiteName",
-                "remoteSn",
                 "remoteHostname",
+                "remoteSn",
                 "sn",
-                "localPassive",
-                "localMetric",
-                "state",
-                "remoteMetric",
                 "localLevel",
-                "id",
-                "localHoldTime"
+                "hostname",
+                "intName",
+                "remoteMetric",
+                "remoteIntName"
             ],
             "description": "Intermediate System to Intermediate System (IS-IS) interface level config",
             "summary": "IS-IS Levels",
             "web_endpoint": "/technology/routing/is-is/levels"
         }
     },
     "tables/routing/protocols/is-is/neighbors": {
         "api_endpoint": "/tables/routing/protocols/is-is/neighbors",
         "get": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/is-is/neighbors",
             "columns": [
+                "neiHostname",
+                "id",
+                "neiSiteName",
+                "neiSn",
+                "neiSystemName",
+                "neiDevType",
+                "intName",
+                "neiAddress",
+                "neiIntName",
                 "localAddress",
-                "siteName",
+                "localAddressV6",
+                "hostname",
+                "subnet",
+                "state",
+                "source",
                 "sn",
-                "neiDevType",
+                "neiSnpa",
+                "neiAreas",
                 "localIsType",
-                "neiSystemName",
                 "target",
-                "neiAddress",
-                "neiId",
-                "vrf",
-                "neiHostname",
                 "neiAddressV6",
-                "neiSnpa",
-                "subnet",
-                "hostname",
-                "intName",
-                "currStateTime",
-                "neiSn",
-                "neiIntName",
-                "neiSiteName",
-                "neiIsType",
-                "localId",
-                "neiAreas",
                 "localAreas",
-                "localAddressV6",
-                "state",
+                "siteName",
+                "currStateTime",
                 "devType",
-                "id",
-                "source"
+                "localId",
+                "neiIsType",
+                "vrf",
+                "neiId"
             ],
             "description": "Intermediate System to Intermediate System (IS-IS) neighbors inventory",
             "summary": "IS-IS Neighbors",
             "web_endpoint": "/technology/routing/is-is/neighbors"
         }
     },
     "tables/routing/protocols/lisp/ipv4-databases": {
         "api_endpoint": "/tables/routing/protocols/lisp/ipv4-databases",
         "get": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/lisp/ipv4-databases",
             "columns": [
                 "siteName",
-                "hostname",
-                "ipv6DatabaseServer",
-                "instanceId",
-                "sn",
                 "ipv4DatabaseServer",
+                "id",
                 "state",
-                "id"
+                "instanceId",
+                "sn",
+                "hostname",
+                "ipv6DatabaseServer"
             ],
             "description": "IPv4 LISP Mapping and Location Repository",
             "summary": "LISP IPv4 Map Resolvers",
             "web_endpoint": "/technology/routing/lisp/map-resolvers/ipv4"
         }
     },
     "tables/routing/protocols/lisp/ipv4-routes": {
         "api_endpoint": "/tables/routing/protocols/lisp/ipv4-routes",
         "get": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/lisp/ipv4-routes",
             "columns": [
                 "siteName",
-                "hostname",
+                "id",
                 "instanceId",
-                "registeredIp",
                 "sn",
-                "id",
+                "registeredIp",
+                "hostname",
                 "eidPrefix"
             ],
             "description": "IPv4 LISP table, Address mapping and routing",
             "summary": "LISP IPv4 Routes",
             "web_endpoint": "/technology/routing/lisp/routes/ipv4"
         }
     },
     "tables/routing/protocols/lisp/ipv6-databases": {
         "api_endpoint": "/tables/routing/protocols/lisp/ipv6-databases",
         "get": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/lisp/ipv6-databases",
             "columns": [
                 "siteName",
-                "hostname",
-                "ipv6DatabaseServer",
-                "instanceId",
-                "sn",
                 "ipv4DatabaseServer",
+                "id",
                 "state",
-                "id"
+                "instanceId",
+                "sn",
+                "hostname",
+                "ipv6DatabaseServer"
             ],
             "description": "IPv6 LISP Mapping and Location Repository",
             "summary": "LISP IPv6 Map Resolvers",
             "web_endpoint": "/technology/routing/lisp/map-resolvers/ipv6"
         }
     },
     "tables/routing/protocols/lisp/ipv6-routes": {
         "api_endpoint": "/tables/routing/protocols/lisp/ipv6-routes",
         "get": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/lisp/ipv6-routes",
             "columns": [
                 "siteName",
-                "hostname",
+                "id",
                 "instanceId",
-                "registeredIp",
                 "sn",
-                "id",
+                "registeredIp",
+                "hostname",
                 "eidPrefix"
             ],
             "description": "IPv6 LISP table, Address mapping and routing",
             "summary": "LISP IPv6 Routes",
             "web_endpoint": "/technology/routing/lisp/routes/ipv6"
         }
     },
     "tables/routing/protocols/ospf-v3/interfaces": {
         "api_endpoint": "/tables/routing/protocols/ospf-v3/interfaces",
         "get": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/ospf-v3/interfaces",
             "columns": [
-                "timerWait",
-                "siteName",
-                "instanceId",
-                "sn",
-                "timerDead",
+                "id",
+                "priority",
                 "cost",
-                "neiCount",
                 "timerRetransmit",
+                "processId",
+                "intName",
                 "area",
                 "networkType",
                 "timerHello",
+                "timerWait",
                 "hostname",
-                "intName",
-                "addressFamily",
-                "processId",
-                "priority",
                 "routerId",
                 "state",
-                "id"
+                "sn",
+                "addressFamily",
+                "siteName",
+                "timerDead",
+                "instanceId",
+                "neiCount"
             ],
             "description": "Open Shortest Path First v3 (OSPFv3) interfaces inventory",
             "summary": "OSPF v3 Interfaces",
             "web_endpoint": "/technology/routing/ospf-v3/interfaces"
         }
     },
     "tables/routing/protocols/ospf-v3/neighbors": {
         "api_endpoint": "/tables/routing/protocols/ospf-v3/neighbors",
         "get": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/ospf-v3/neighbors",
             "columns": [
-                "localAddress",
-                "siteName",
-                "sn",
+                "neiHostname",
+                "localCost",
+                "id",
+                "priority",
+                "neiSiteName",
+                "neiSn",
                 "neiDevType",
+                "intName",
+                "neiAddress",
+                "neiIntName",
+                "localAddress",
                 "neiCost",
-                "bdr",
-                "target",
+                "hostname",
                 "dr",
-                "neiAddress",
-                "neiId",
-                "vrf",
-                "localCost",
-                "neiHostname",
                 "subnet",
-                "hostname",
-                "intName",
-                "currStateTime",
-                "addressFamily",
-                "neiSn",
-                "neiIntName",
-                "neiSiteName",
-                "priority",
-                "neiArea",
                 "state",
+                "source",
+                "neiArea",
+                "sn",
+                "target",
+                "addressFamily",
+                "siteName",
+                "currStateTime",
                 "localArea",
                 "devType",
-                "id",
-                "source"
+                "bdr",
+                "vrf",
+                "neiId"
             ],
             "description": "Open Shortest Path First v3 (OSPFv3) neighbors inventory",
             "summary": "OSPF v3 Neighbors",
             "web_endpoint": "/technology/routing/ospf-v3/neighbors"
         }
     },
     "tables/routing/protocols/ospf/interfaces": {
         "api_endpoint": "/tables/routing/protocols/ospf/interfaces",
         "get": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/ospf/interfaces",
             "columns": [
-                "timerWait",
-                "neiCount",
                 "siteName",
-                "hostname",
-                "intName",
+                "routerId",
+                "timerDead",
+                "area",
+                "id",
+                "priority",
+                "state",
                 "timerRetransmit",
+                "timerHello",
                 "sn",
-                "area",
-                "timerDead",
                 "networkType",
                 "processId",
-                "timerHello",
+                "neiCount",
                 "cost",
-                "routerId",
-                "state",
-                "id",
-                "priority"
+                "timerWait",
+                "hostname",
+                "intName"
             ],
             "description": "Open Shortest Path First (OSPF) interfaces inventory",
             "summary": "OSPF Interfaces",
             "web_endpoint": "/technology/routing/ospf/interfaces"
         }
     },
     "tables/routing/protocols/ospf/neighbors": {
         "api_endpoint": "/tables/routing/protocols/ospf/neighbors",
         "get": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/ospf/neighbors",
             "columns": [
-                "localAddress",
-                "siteName",
-                "sn",
+                "neiHostname",
+                "localCost",
+                "id",
+                "priority",
+                "neiSiteName",
+                "neiSn",
                 "neiDevType",
+                "intName",
+                "neiAddress",
+                "neiIntName",
+                "localAddress",
                 "neiCost",
-                "bdr",
-                "target",
+                "hostname",
                 "dr",
-                "neiAddress",
-                "neiId",
-                "vrf",
-                "localCost",
-                "neiHostname",
                 "subnet",
-                "hostname",
-                "intName",
-                "currStateTime",
-                "neiSn",
-                "neiIntName",
-                "neiSiteName",
-                "priority",
-                "neiArea",
                 "state",
+                "source",
+                "neiArea",
+                "sn",
+                "target",
+                "siteName",
+                "currStateTime",
                 "localArea",
                 "devType",
-                "id",
-                "source"
+                "bdr",
+                "vrf",
+                "neiId"
             ],
             "description": "Open Shortest Path First (OSPF) neighbors inventory",
             "summary": "OSPF Neighbors",
             "web_endpoint": "/technology/routing/ospf/neighbors"
         }
     },
     "tables/routing/protocols/rip/interfaces": {
         "api_endpoint": "/tables/routing/protocols/rip/interfaces",
         "get": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/rip/interfaces",
             "columns": [
-                "neiCount",
+                "timerHolddown",
                 "siteName",
-                "hostname",
-                "intName",
+                "timerUpdate",
                 "verReceive",
-                "timerInvalid",
-                "sn",
-                "timerHolddown",
                 "verSend",
-                "timerUpdate",
+                "timerInvalid",
                 "id",
+                "sn",
+                "neiCount",
+                "hostname",
+                "intName",
                 "timerFlush"
             ],
             "description": "Routing Information Protocol (RIP) interfaces inventory",
             "summary": "RIP Interfaces",
             "web_endpoint": "/technology/routing/rip/interfaces"
         }
     },
     "tables/routing/protocols/rip/neighbors": {
         "api_endpoint": "/tables/routing/protocols/rip/neighbors",
         "get": null,
         "post": {
             "api_endpoint": "tables/routing/protocols/rip/neighbors",
             "columns": [
-                "localAddress",
-                "hostname",
-                "intName",
+                "neiHostname",
                 "neiAddress",
-                "siteName",
+                "neiIntName",
                 "currStateTime",
-                "subnet",
-                "neiSn",
+                "localAddress",
+                "siteName",
+                "id",
+                "neiSiteName",
+                "devType",
+                "source",
                 "sn",
+                "neiSn",
                 "target",
-                "vrf",
-                "neiIntName",
                 "neiDevType",
-                "neiSiteName",
-                "neiHostname",
-                "devType",
-                "id",
-                "source"
+                "vrf",
+                "hostname",
+                "subnet",
+                "intName"
             ],
             "description": "Routing Information Protocol (RIP) neighbors inventory",
             "summary": "RIP Neighbors",
             "web_endpoint": "/technology/routing/rip/neighbors"
         }
     },
     "tables/scopes/api": {
         "api_endpoint": "/tables/scopes/api",
         "get": null,
         "post": {
             "api_endpoint": "tables/scopes/api",
             "columns": [
-                "path",
                 "method",
+                "path",
                 "id"
             ],
             "description": "",
             "summary": "POST /tables/scopes/api",
             "web_endpoint": null
         }
     },
     "tables/scopes/attributes": {
         "api_endpoint": "/tables/scopes/attributes",
         "get": null,
         "post": {
             "api_endpoint": "tables/scopes/attributes",
             "columns": [
-                "attributeFilters",
-                "id"
+                "id",
+                "attributeFilters"
             ],
             "description": "",
             "summary": "POST /tables/scopes/attributes",
             "web_endpoint": null
         }
     },
     "tables/sdwan/links": {
         "api_endpoint": "/tables/sdwan/links",
         "get": null,
         "post": {
             "api_endpoint": "tables/sdwan/links",
             "columns": [
-                "encapsulation",
-                "endpointIp",
+                "slug",
                 "siteName",
-                "hostname",
                 "port",
-                "interfaces",
+                "endpointIp",
+                "id",
+                "encapsulation",
                 "sn",
                 "name",
-                "slug",
                 "linkName",
-                "id",
-                "organization"
+                "organization",
+                "hostname",
+                "interfaces"
             ],
             "description": "Versa SD-WAN transport links inventory",
             "summary": "Versa Transport links",
             "web_endpoint": "/technology/sdwan/transport-links"
         }
     },
     "tables/sdwan/sites": {
         "api_endpoint": "/tables/sdwan/sites",
         "get": null,
         "post": {
             "api_endpoint": "tables/sdwan/sites",
             "columns": [
-                "uptime",
-                "siteName",
-                "hostname",
-                "sn",
-                "name",
-                "status",
                 "slug",
                 "remoteMgmtIp",
-                "id",
+                "siteName",
                 "type",
-                "organization"
+                "id",
+                "uptime",
+                "sn",
+                "name",
+                "organization",
+                "hostname",
+                "status"
             ],
             "description": "Versa SD-WAN sites inventory",
             "summary": "Versa Sites",
             "web_endpoint": "/technology/sdwan/sites"
         }
     },
     "tables/security/aaa/accounting": {
         "api_endpoint": "/tables/security/aaa/accounting",
         "get": null,
         "post": {
             "api_endpoint": "tables/security/aaa/accounting",
             "columns": [
                 "siteName",
-                "hostname",
-                "nextMethods",
-                "primaryMethod",
-                "sn",
-                "name",
                 "secondaryMethod",
                 "type",
                 "id",
-                "params"
+                "name",
+                "params",
+                "primaryMethod",
+                "sn",
+                "nextMethods",
+                "hostname"
             ],
             "description": "Authentication, Authorization and Accounting (AAA) accounting methods configured on managed network devices",
             "summary": "AAA Accounting",
             "web_endpoint": "/technology/management/aaa/accounting"
         }
     },
     "tables/security/aaa/authentication": {
         "api_endpoint": "/tables/security/aaa/authentication",
         "get": null,
         "post": {
             "api_endpoint": "tables/security/aaa/authentication",
             "columns": [
                 "siteName",
-                "hostname",
-                "nextMethods",
-                "primaryMethod",
-                "sn",
-                "name",
                 "secondaryMethod",
                 "type",
                 "id",
-                "params"
+                "name",
+                "params",
+                "primaryMethod",
+                "sn",
+                "nextMethods",
+                "hostname"
             ],
             "description": "Authentication, Authorization and Accounting (AAA) authentication methods configured on managed network devices",
             "summary": "AAA Authentication",
             "web_endpoint": "/technology/management/aaa/authentication"
         }
     },
     "tables/security/aaa/authorization": {
         "api_endpoint": "/tables/security/aaa/authorization",
         "get": null,
         "post": {
             "api_endpoint": "tables/security/aaa/authorization",
             "columns": [
                 "siteName",
-                "hostname",
-                "nextMethods",
-                "primaryMethod",
-                "sn",
-                "name",
                 "secondaryMethod",
                 "type",
                 "id",
-                "params"
+                "name",
+                "params",
+                "primaryMethod",
+                "sn",
+                "nextMethods",
+                "hostname"
             ],
             "description": "Authentication, Authorization and Accounting (AAA) authorization methods configured on managed network devices",
             "summary": "AAA Authorization",
             "web_endpoint": "/technology/management/aaa/authorization"
         }
     },
     "tables/security/aaa/lines": {
         "api_endpoint": "/tables/security/aaa/lines",
         "get": null,
         "post": {
             "api_endpoint": "tables/security/aaa/lines",
             "columns": [
-                "type",
-                "siteName",
-                "hostname",
-                "idType",
-                "outTransports",
-                "sn",
                 "authenServiceList",
-                "inAclAllVrfs",
+                "siteName",
                 "authorServiceList",
-                "idList",
-                "inAcl",
-                "inTransports",
+                "type",
                 "outAcl",
                 "id",
-                "accntServiceList"
+                "idList",
+                "inAclAllVrfs",
+                "outTransports",
+                "accntServiceList",
+                "sn",
+                "inTransports",
+                "idType",
+                "inAcl",
+                "hostname"
             ],
             "description": "Authentication, Authorization and Accounting (AAA) lines configured on managed network devices",
             "summary": "AAA Lines",
             "web_endpoint": "/technology/management/aaa/lines"
         }
     },
     "tables/security/aaa/password-strength": {
         "api_endpoint": "/tables/security/aaa/password-strength",
         "get": null,
         "post": {
             "api_endpoint": "tables/security/aaa/password-strength",
             "columns": [
                 "siteName",
-                "hostname",
-                "passwordStrengthCheck",
+                "id",
                 "sn",
-                "id"
+                "passwordStrengthCheck",
+                "hostname"
             ],
             "description": "Inventory of managed network devices with enabled/disabled passowrd strength check",
             "summary": "Password Strength",
             "web_endpoint": "/technology/management/aaa/password-strength"
         }
     },
     "tables/security/aaa/servers": {
         "api_endpoint": "/tables/security/aaa/servers",
         "get": null,
         "post": {
             "api_endpoint": "tables/security/aaa/servers",
             "columns": [
-                "port",
-                "hostname",
-                "intName",
+                "dstHostname",
+                "cfgName",
                 "siteName",
+                "port",
+                "type",
+                "id",
                 "srvGroupName",
-                "cfgName",
+                "protocol",
                 "sn",
-                "srcIp",
                 "ip",
-                "protocol",
-                "dstHostname",
-                "type",
-                "id"
+                "srcIp",
+                "hostname",
+                "intName"
             ],
             "description": "Authentication, Authorization and Accounting (AAA) configured on managed network devices",
             "summary": "AAA Servers",
             "web_endpoint": "/technology/management/aaa/servers"
         }
     },
     "tables/security/aaa/users": {
         "api_endpoint": "/tables/security/aaa/users",
         "get": null,
         "post": {
             "api_endpoint": "tables/security/aaa/users",
             "columns": [
-                "privilege",
                 "siteName",
-                "hostname",
+                "privilege",
+                "id",
                 "sn",
-                "username",
                 "groups",
-                "id"
+                "hostname",
+                "username"
             ],
             "description": "Authentication, Authorization and Accounting (AAA) loca configured on managed network devices",
             "summary": "AAA Local Users",
             "web_endpoint": "/technology/management/aaa/local-users"
         }
     },
     "tables/security/acl": {
         "api_endpoint": "/tables/security/acl",
         "get": null,
         "post": {
             "api_endpoint": "tables/security/acl",
             "columns": [
-                "interfaceOutZone",
-                "siteName",
-                "ruleNameNumeric",
-                "tcpFlags",
-                "ipSrcRegion",
-                "interfaceIn",
-                "sn",
-                "others",
-                "udpDst",
+                "vxlanSrcGrp",
                 "ipTtl",
-                "ipSrc",
-                "interfaceOut",
+                "id",
+                "l4Dst",
+                "tcpFlags",
+                "actionOriginal",
+                "udpSrc",
+                "description",
+                "ipProtocol",
+                "referencedTests",
+                "l4Src",
+                "active",
+                "ipDscp",
+                "l7Application",
                 "ipPacketLength",
+                "icmpType",
+                "ipPrecedence",
+                "mplsLabelIn",
+                "hostname",
+                "ipTos",
+                "ipSrc",
                 "srcPorts",
+                "policyName",
+                "interfaceOut",
+                "ipSrcRegion",
                 "ipv6Src",
-                "vxlanVni",
+                "tcpDst",
+                "icmpCode",
                 "ruleName",
-                "actionOriginal",
-                "ipDst",
-                "mplsLabelIn",
-                "ipFragmentOffset",
+                "interfaceOutZone",
                 "tcpSrc",
-                "icmpCode",
-                "referencedTests",
-                "icmpIcmpv6",
+                "optionsTracked",
+                "ipDstRegion",
+                "interfaceIn",
+                "vxlanVni",
+                "others",
+                "vxlanDstGrp",
+                "sn",
+                "udpDst",
+                "interfaceIntraZone",
+                "siteName",
+                "ipv6Dst",
                 "dstPorts",
-                "hostname",
-                "ipProtocol",
-                "interfaceInterZone",
                 "uid",
-                "l7Application",
-                "ipv6Dst",
-                "ipPrecedence",
-                "tcpDst",
-                "interfaceIntraZone",
-                "interfaceInZone",
-                "ipDstRegion",
-                "vxlanSrcGrp",
-                "ipDscp",
-                "l4Src",
-                "icmpType",
-                "description",
-                "ipTos",
+                "icmpIcmpv6",
+                "ipFragmentOffset",
+                "ruleNameNumeric",
+                "interfaceVrf",
                 "action",
+                "interfaceInZone",
                 "ruleNumber",
-                "policyName",
-                "interfaceVrf",
-                "l4Dst",
-                "vxlanDstGrp",
-                "optionsTracked",
-                "active",
-                "udpSrc",
-                "id"
+                "interfaceInterZone",
+                "ipDst"
             ],
             "description": "Detailed network access control list (ACL) information on managed network devices",
             "summary": "Access Control List Entries",
             "web_endpoint": "/technology/security/access-list"
         }
     },
     "tables/security/acl/global-policies": {
         "api_endpoint": "/tables/security/acl/global-policies",
         "get": null,
         "post": {
             "api_endpoint": "tables/security/acl/global-policies",
             "columns": [
                 "siteName",
-                "hostname",
-                "sn",
-                "outputPolicy",
                 "inputPolicy",
-                "id"
+                "outputPolicy",
+                "id",
+                "sn",
+                "hostname"
             ],
             "description": "Global access control list (ACL) policies configured on managed network devices",
             "summary": "Global ACL policies",
             "web_endpoint": "/technology/security/acl/global-acl-policies"
         }
     },
     "tables/security/acl/interfaces": {
         "api_endpoint": "/tables/security/acl/interfaces",
         "get": null,
         "post": {
             "api_endpoint": "tables/security/acl/interfaces",
             "columns": [
                 "siteName",
-                "hostname",
-                "intName",
-                "sn",
                 "outAcl",
+                "id",
+                "sn",
                 "inAcl",
-                "id"
+                "hostname",
+                "intName"
             ],
             "description": "Interfaces with packet filters or access control lists (ACL) applied",
             "summary": "ACL and Filter Interfaces",
             "web_endpoint": "/technology/security/acl-interfaces"
         }
     },
     "tables/security/dhcp/bindings": {
         "api_endpoint": "/tables/security/dhcp/bindings",
         "get": null,
         "post": {
             "api_endpoint": "tables/security/dhcp/bindings",
             "columns": [
-                "leaseIp",
-                "type",
+                "leaseTimeout",
                 "siteName",
-                "hostname",
-                "intName",
-                "vlanId",
+                "type",
+                "id",
+                "leaseIp",
                 "sn",
-                "leaseTimeout",
+                "vlanId",
                 "mac",
-                "id"
+                "hostname",
+                "intName"
             ],
             "description": "DHCP Snooping binding database inventory",
             "summary": "DHCP Snooping Binding Database",
             "web_endpoint": "/technology/security/dhcp-snooping/bindings-v4"
         }
     },
     "tables/security/dhcp/snooping": {
         "api_endpoint": "/tables/security/dhcp/snooping",
         "get": null,
         "post": {
             "api_endpoint": "tables/security/dhcp/snooping",
             "columns": [
-                "macVerification",
-                "dbWriteDelay",
+                "trustedPortList",
+                "dbLocation",
                 "siteName",
-                "hostname",
+                "circuitId",
+                "remoteId",
+                "insertion",
+                "id",
+                "enabled",
                 "vendorId",
                 "packetsDropped",
                 "sn",
-                "enabledVlanList",
-                "untrustedPolicy",
+                "hostname",
                 "packetsTotal",
-                "insertion",
-                "dbLocation",
-                "enabled",
-                "circuitId",
-                "trustedPortList",
-                "id",
-                "remoteId"
+                "macVerification",
+                "untrustedPolicy",
+                "enabledVlanList",
+                "dbWriteDelay"
             ],
             "description": "DHCP Snooping configuration parameters for managed network devices",
             "summary": "DHCP Snooping",
             "web_endpoint": "/technology/security/dhcp-snooping/configuration-v4"
         }
     },
     "tables/security/dmvpn": {
         "api_endpoint": "/tables/security/dmvpn",
         "get": null,
         "post": {
             "api_endpoint": "tables/security/dmvpn",
             "columns": [
+                "peerNbma",
                 "siteName",
-                "hostname",
-                "intName",
+                "id",
+                "state",
                 "peerTunnel",
                 "sn",
-                "peerNbma",
                 "time",
-                "attrb",
-                "state",
-                "id"
+                "hostname",
+                "intName",
+                "attrb"
             ],
             "description": "dynamic multipoint virtual private network (DMVPN) tunnels inventory ",
             "summary": "DMVPN Summary",
             "web_endpoint": "/technology/security/dmvpn"
         }
     },
     "tables/security/enabled-telnet": {
         "api_endpoint": "/tables/security/enabled-telnet",
         "get": null,
         "post": {
             "api_endpoint": "tables/security/enabled-telnet",
             "columns": [
+                "image",
+                "siteName",
+                "id",
                 "uptime",
                 "loginIp",
-                "siteName",
-                "hostname",
-                "sn",
                 "processor",
-                "configReg",
-                "loginType",
                 "reload",
                 "version",
-                "id",
-                "image"
+                "sn",
+                "loginType",
+                "configReg",
+                "hostname"
             ],
             "description": "Managed network devices with enabled Telnet access",
             "summary": "Telnet Access",
             "web_endpoint": "/technology/management/telnet-access"
         }
     },
     "tables/security/ipsec/gateways": {
         "api_endpoint": "/tables/security/ipsec/gateways",
         "get": null,
         "post": {
             "api_endpoint": "tables/security/ipsec/gateways",
             "columns": [
-                "deadPeerDetection",
-                "siteName",
-                "intDscr",
-                "sn",
+                "peerId",
                 "profileName",
+                "remoteGwAddressV6",
+                "type",
                 "natTraversal",
-                "dhGroup",
-                "role",
+                "id",
                 "version",
+                "intName",
+                "keyLifeBytes",
                 "neighbors",
+                "remoteGwAddress",
+                "deadPeerDetection",
+                "keyLifeSeconds",
+                "localGwAddressV6",
                 "hostname",
+                "sn",
+                "dhGroup",
                 "encryption",
-                "intName",
-                "localGwAddress",
                 "status",
-                "type",
-                "authentication",
-                "keyLifeBytes",
+                "siteName",
+                "intDscr",
                 "mode",
                 "localId",
                 "authType",
-                "peerId",
-                "keyLifeSeconds",
-                "id",
-                "remoteGwAddress"
+                "authentication",
+                "localGwAddress",
+                "role"
             ],
             "description": "Internet Protocol Security (IPsec) gateways inventory",
             "summary": "IPsec gateways",
             "web_endpoint": "/technology/security/ipsec/gateways"
         }
     },
     "tables/security/ipsec/tunnels": {
         "api_endpoint": "/tables/security/ipsec/tunnels",
         "get": null,
         "post": {
             "api_endpoint": "tables/security/ipsec/tunnels",
             "columns": [
-                "encapsulation",
+                "remoteGwAddressV6",
+                "profileName",
+                "id",
+                "selectorRemoteAddress",
+                "selectorRemoteAddressV6",
+                "selectorRemotePort",
+                "protocol",
                 "ikeGateway",
-                "siteName",
+                "intName",
+                "keepAlive",
+                "keyLifeBytes",
+                "neighbors",
                 "routeBased",
-                "intDscr",
+                "remoteGwAddress",
+                "selectorProtocol",
+                "encapsulation",
+                "selectorLocalAddressV6",
+                "keyLifeSeconds",
+                "localGwAddressV6",
                 "selectorLocalAddress",
-                "selectorRemotePort",
+                "hostname",
+                "tunnelIntDscr",
+                "tunnelIntName",
                 "sn",
-                "selectorLocalPort",
-                "selectorRemoteAddress",
-                "profileName",
-                "keepAlive",
                 "dhGroup",
-                "tunnelIntName",
-                "neighbors",
-                "hostname",
+                "autoUp",
                 "encryption",
-                "intName",
-                "tunnelIntDscr",
-                "localGwAddress",
-                "selectorProtocol",
                 "status",
-                "protocol",
-                "autoUp",
+                "siteName",
+                "intDscr",
+                "selectorLocalPort",
                 "authentication",
-                "keyLifeBytes",
-                "keyLifeSeconds",
-                "id",
-                "remoteGwAddress"
+                "localGwAddress"
             ],
             "description": "Internet Protocol Security (IPsec) tunnels inventory",
             "summary": "IPsec tunnels",
             "web_endpoint": "/technology/security/ipsec/tunnels"
         }
     },
     "tables/security/nat44": {
         "api_endpoint": "/tables/security/nat44",
         "get": null,
         "post": {
             "api_endpoint": "tables/security/nat44",
             "columns": [
-                "interfaceOutZone",
-                "siteName",
-                "ruleNameNumeric",
+                "natUdpSrc",
+                "vxlanSrcGrp",
+                "ipTtl",
+                "id",
+                "l4Dst",
                 "tcpFlags",
+                "actionOriginal",
+                "udpSrc",
+                "description",
+                "ipProtocol",
+                "referencedTests",
+                "natTcpDst",
+                "l4Src",
+                "active",
                 "natTcpSrc",
-                "ipSrcRegion",
-                "natIpDst",
-                "interfaceIn",
-                "sn",
-                "others",
+                "ipDscp",
+                "l7Application",
+                "natL4Src",
                 "natUdpDst",
-                "udpDst",
-                "ipTtl",
-                "ipSrc",
-                "interfaceOut",
                 "ipPacketLength",
+                "icmpType",
+                "ipPrecedence",
+                "mplsLabelIn",
+                "hostname",
+                "ipTos",
+                "ipSrc",
                 "srcPorts",
+                "natIpPortDst",
+                "policyName",
+                "interfaceOut",
+                "ipSrcRegion",
                 "ipv6Src",
-                "vxlanVni",
+                "tcpDst",
+                "icmpCode",
                 "ruleName",
-                "natIpPortDst",
-                "actionOriginal",
-                "ipDst",
                 "natIpSrc",
-                "mplsLabelIn",
-                "ipFragmentOffset",
+                "natIpDst",
+                "interfaceOutZone",
                 "tcpSrc",
-                "natL4Src",
-                "icmpCode",
-                "referencedTests",
-                "natTcpDst",
-                "icmpIcmpv6",
+                "optionsTracked",
+                "ipDstRegion",
+                "interfaceIn",
+                "vxlanVni",
+                "others",
+                "vxlanDstGrp",
+                "sn",
+                "udpDst",
+                "interfaceIntraZone",
+                "natInterfaceSrc",
+                "siteName",
+                "ipv6Dst",
                 "dstPorts",
-                "hostname",
-                "ipProtocol",
-                "interfaceInterZone",
-                "uid",
-                "l7Application",
                 "natL4Dst",
-                "ipv6Dst",
-                "ipPrecedence",
-                "tcpDst",
-                "interfaceIntraZone",
-                "interfaceInZone",
-                "ipDstRegion",
-                "vxlanSrcGrp",
-                "ipDscp",
-                "l4Src",
-                "icmpType",
-                "description",
-                "ipTos",
+                "uid",
+                "icmpIcmpv6",
+                "ipFragmentOffset",
+                "ruleNameNumeric",
+                "interfaceVrf",
                 "action",
+                "interfaceInZone",
                 "ruleNumber",
-                "policyName",
-                "interfaceVrf",
-                "l4Dst",
-                "natInterfaceSrc",
-                "vxlanDstGrp",
-                "optionsTracked",
-                "active",
-                "udpSrc",
-                "natUdpSrc",
-                "id"
+                "interfaceInterZone",
+                "ipDst"
             ],
             "description": "Network Address Translation (IPv4 to IPv4)",
             "summary": "Network Address Translation",
             "web_endpoint": "/technology/addressing/nat"
         }
     },
     "tables/security/object-groups": {
         "api_endpoint": "/tables/security/object-groups",
         "get": null,
         "post": {
             "api_endpoint": "tables/security/object-groups",
             "columns": [
-                "description",
-                "value",
+                "isLiteralValue",
                 "siteName",
-                "hostname",
-                "sn",
+                "id",
                 "name",
+                "sn",
                 "category",
-                "id",
-                "isLiteralValue"
+                "value",
+                "hostname",
+                "description"
             ],
             "description": "Security object groups and address books inventory",
             "summary": "Security Object Groups",
             "web_endpoint": null
         }
     },
     "tables/security/pbr": {
         "api_endpoint": "/tables/security/pbr",
         "get": null,
         "post": {
             "api_endpoint": "tables/security/pbr",
             "columns": [
-                "interfaceOutZone",
-                "siteName",
-                "ruleNameNumeric",
-                "tcpFlags",
-                "ipSrcRegion",
-                "interfaceIn",
-                "sn",
-                "others",
-                "udpDst",
+                "vxlanSrcGrp",
                 "ipTtl",
-                "ipSrc",
-                "interfaceOut",
-                "ipPacketLength",
-                "srcPorts",
-                "ipv6Src",
-                "vxlanVni",
-                "ruleName",
+                "id",
+                "l4Dst",
+                "tcpFlags",
                 "actionOriginal",
-                "ipDst",
-                "mplsLabelIn",
-                "ipFragmentOffset",
-                "tcpSrc",
-                "pbrActions",
-                "icmpCode",
-                "referencedTests",
-                "icmpIcmpv6",
-                "dstPorts",
-                "hostname",
+                "udpSrc",
+                "description",
                 "ipProtocol",
-                "interfaceInterZone",
-                "uid",
+                "referencedTests",
+                "l4Src",
+                "active",
+                "ipDscp",
                 "l7Application",
-                "ipv6Dst",
+                "ipPacketLength",
+                "icmpType",
                 "ipPrecedence",
+                "mplsLabelIn",
+                "pbrActions",
+                "hostname",
+                "ipTos",
+                "ipSrc",
+                "srcPorts",
+                "policyName",
+                "interfaceOut",
+                "ipSrcRegion",
+                "ipv6Src",
                 "tcpDst",
-                "interfaceIntraZone",
-                "interfaceInZone",
+                "icmpCode",
+                "ruleName",
+                "interfaceOutZone",
+                "tcpSrc",
+                "optionsTracked",
                 "ipDstRegion",
-                "vxlanSrcGrp",
-                "ipDscp",
-                "l4Src",
-                "icmpType",
-                "description",
-                "ipTos",
+                "interfaceIn",
+                "vxlanVni",
+                "others",
+                "vxlanDstGrp",
+                "sn",
                 "evalAclTests",
+                "udpDst",
+                "interfaceIntraZone",
+                "siteName",
+                "ipv6Dst",
+                "dstPorts",
+                "uid",
+                "icmpIcmpv6",
+                "ipFragmentOffset",
+                "ruleNameNumeric",
+                "interfaceVrf",
                 "action",
+                "interfaceInZone",
                 "ruleNumber",
-                "policyName",
-                "interfaceVrf",
-                "l4Dst",
-                "vxlanDstGrp",
-                "optionsTracked",
-                "active",
-                "udpSrc",
-                "id"
+                "interfaceInterZone",
+                "ipDst"
             ],
             "description": "Policy Based Routing (syntax search)",
             "summary": "Policy Based Routing",
             "web_endpoint": "/technology/routing/policy/pbr"
         }
     },
     "tables/security/secure-ports/devices": {
         "api_endpoint": "/tables/security/secure-ports/devices",
         "get": null,
         "post": {
             "api_endpoint": "tables/security/secure-ports/devices",
             "columns": [
-                "siteName",
-                "hostname",
-                "usersCount",
-                "sn",
-                "intTotalNetCount",
                 "intSecNetCount",
-                "intSecEdgeCount",
+                "intTotalNetCount",
+                "siteName",
                 "intTotalEdgeCount",
                 "id",
+                "intSecEdgeCount",
+                "sn",
+                "usersCount",
+                "hostname",
                 "methods"
             ],
             "description": "",
             "summary": "802.1x Secure ports - Devices",
             "web_endpoint": "/technology/security/secure-ports/devices"
         }
     },
     "tables/security/secure-ports/interfaces": {
         "api_endpoint": "/tables/security/secure-ports/interfaces",
         "get": null,
         "post": {
             "api_endpoint": "tables/security/secure-ports/interfaces",
             "columns": [
-                "siteName",
-                "usersCount",
-                "intDscr",
-                "sn",
-                "vendor",
-                "model",
-                "voiceVlan",
+                "id",
                 "dynamicMacCount",
                 "method",
-                "hostname",
+                "vendor",
                 "intName",
-                "platform",
                 "monitorMode",
+                "platform",
                 "edge",
                 "switchportMode",
+                "hostname",
                 "state",
+                "sn",
                 "accVlan",
-                "devType",
-                "id"
+                "usersCount",
+                "model",
+                "siteName",
+                "intDscr",
+                "voiceVlan",
+                "devType"
             ],
             "description": "Network access control interfaces inventory",
             "summary": "802.1x Secure ports - Interfaces",
             "web_endpoint": "/technology/security/secure-ports/interfaces"
         }
     },
     "tables/security/secure-ports/users": {
         "api_endpoint": "/tables/security/secure-ports/users",
         "get": null,
         "post": {
             "api_endpoint": "tables/security/secure-ports/users",
             "columns": [
-                "userMac",
                 "siteName",
-                "hostname",
-                "intName",
                 "userState",
+                "id",
+                "state",
                 "sn",
                 "username",
                 "userMethod",
-                "state",
-                "id"
+                "hostname",
+                "intName",
+                "userMac"
             ],
             "description": "Network access control users inventory",
             "summary": "802.1x Secure ports - Users",
             "web_endpoint": "/technology/security/secure-ports/users"
         }
     },
     "tables/security/zone-firewall/interfaces": {
         "api_endpoint": "/tables/security/zone-firewall/interfaces",
         "get": null,
         "post": {
             "api_endpoint": "tables/security/zone-firewall/interfaces",
             "columns": [
                 "siteName",
+                "id",
+                "isDefault",
+                "sn",
                 "hostname",
                 "intName",
-                "zone",
-                "sn",
-                "isDefault",
-                "id"
+                "zone"
             ],
             "description": "Security gateway interfaces participating in zone firewall policies",
             "summary": "Zone Firewall - Interfaces",
             "web_endpoint": "/technology/security/zone-firewall/interfaces"
         }
     },
     "tables/security/zone-firewall/policies": {
         "api_endpoint": "/tables/security/zone-firewall/policies",
         "get": null,
         "post": {
             "api_endpoint": "tables/security/zone-firewall/policies",
             "columns": [
-                "interfaceOutZone",
-                "siteName",
-                "ruleNameNumeric",
-                "tcpFlags",
-                "ipSrcRegion",
-                "interfaceIn",
-                "sn",
-                "others",
-                "udpDst",
+                "vxlanSrcGrp",
                 "ipTtl",
-                "ipSrc",
-                "interfaceOut",
+                "id",
+                "l4Dst",
+                "tcpFlags",
+                "actionOriginal",
+                "udpSrc",
+                "description",
+                "ipProtocol",
+                "referencedTests",
+                "l4Src",
+                "active",
+                "ipDscp",
+                "l7Application",
                 "ipPacketLength",
+                "icmpType",
+                "ipPrecedence",
+                "mplsLabelIn",
+                "hostname",
+                "ipTos",
+                "ipSrc",
                 "srcPorts",
+                "policyName",
+                "interfaceOut",
+                "ipSrcRegion",
                 "ipv6Src",
-                "vxlanVni",
+                "tcpDst",
+                "icmpCode",
                 "ruleName",
-                "actionOriginal",
-                "ipDst",
-                "mplsLabelIn",
-                "ipFragmentOffset",
+                "interfaceOutZone",
                 "tcpSrc",
-                "icmpCode",
-                "referencedTests",
-                "icmpIcmpv6",
+                "optionsTracked",
+                "ipDstRegion",
+                "interfaceIn",
+                "vxlanVni",
+                "others",
+                "vxlanDstGrp",
+                "sn",
+                "udpDst",
+                "interfaceIntraZone",
+                "siteName",
+                "ipv6Dst",
                 "dstPorts",
-                "hostname",
-                "ipProtocol",
-                "interfaceInterZone",
                 "uid",
-                "l7Application",
-                "ipv6Dst",
-                "ipPrecedence",
-                "tcpDst",
-                "interfaceIntraZone",
-                "interfaceInZone",
-                "ipDstRegion",
-                "vxlanSrcGrp",
-                "ipDscp",
-                "l4Src",
-                "icmpType",
-                "description",
-                "ipTos",
+                "icmpIcmpv6",
+                "ipFragmentOffset",
+                "ruleNameNumeric",
+                "interfaceVrf",
                 "action",
+                "interfaceInZone",
                 "ruleNumber",
-                "policyName",
-                "interfaceVrf",
-                "l4Dst",
-                "vxlanDstGrp",
-                "optionsTracked",
-                "active",
-                "udpSrc",
-                "id"
+                "interfaceInterZone",
+                "ipDst"
             ],
             "description": "Security gateways zone policies details",
             "summary": "Zone Firewall - Policies",
             "web_endpoint": "/technology/security/zone-firewall/policies"
         }
     },
     "tables/serial-ports": {
         "api_endpoint": "/tables/serial-ports",
         "get": null,
         "post": {
             "api_endpoint": "tables/serial-ports",
             "columns": [
-                "mode",
-                "parameters",
                 "siteName",
-                "hostname",
-                "pinout",
                 "flowControl",
                 "label",
+                "loggingLevel",
+                "id",
+                "connector",
+                "mode",
+                "pinout",
+                "parameters",
                 "sn",
                 "name",
-                "connector",
-                "loggingLevel",
-                "id"
+                "hostname"
             ],
             "description": "Serial Ports",
             "summary": "Serial Ports",
             "web_endpoint": "/technology/serial-ports"
         }
     },
     "tables/settings": {
@@ -8651,384 +8671,384 @@
     },
     "tables/settings/jumphosts": {
         "api_endpoint": "/tables/settings/jumphosts",
         "get": null,
         "post": {
             "api_endpoint": "tables/settings/jumphosts",
             "columns": [
-                "address",
-                "label",
-                "exclude",
-                "loginType",
                 "subnets",
                 "running",
+                "id",
                 "enabled",
-                "id"
+                "address",
+                "loginType",
+                "label",
+                "exclude"
             ],
             "description": "",
             "summary": "POST /tables/settings/jumphosts",
             "web_endpoint": null
         }
     },
     "tables/settings/ports": {
         "api_endpoint": "/tables/settings/ports",
         "get": null,
         "post": {
             "api_endpoint": "tables/settings/ports",
             "columns": [
-                "port",
-                "label",
-                "excludeSubnets",
                 "subnets",
+                "port",
+                "id",
                 "protocol",
-                "id"
+                "label",
+                "excludeSubnets"
             ],
             "description": "",
             "summary": "POST /tables/settings/ports",
             "web_endpoint": null
         }
     },
     "tables/snapshot-attributes": {
         "api_endpoint": "/tables/snapshot-attributes",
         "get": null,
         "post": {
             "api_endpoint": "tables/snapshot-attributes",
             "columns": [
-                "hostname",
-                "sn",
-                "name",
                 "id",
-                "value"
+                "name",
+                "sn",
+                "value",
+                "hostname"
             ],
             "description": "",
             "summary": "POST /tables/snapshot-attributes",
             "web_endpoint": null
         }
     },
     "tables/snapshot-devices": {
         "api_endpoint": "/tables/snapshot-devices",
         "get": null,
         "post": {
             "api_endpoint": "tables/snapshot-devices",
             "columns": [
-                "type",
-                "parentId",
-                "siteName",
-                "hostname",
-                "platform",
-                "sn",
-                "vendor",
-                "ipString",
                 "vTask",
-                "isSelected",
-                "version",
-                "model",
                 "settingsStates",
                 "family",
+                "model",
+                "siteName",
+                "type",
+                "platform",
+                "ipString",
                 "id",
+                "version",
+                "source",
+                "sn",
                 "isApiTask",
-                "source"
+                "isSelected",
+                "hostname",
+                "vendor",
+                "parentId"
             ],
             "description": "",
             "summary": "POST /tables/snapshot-devices",
             "web_endpoint": null
         }
     },
     "tables/spanning-tree/bridges": {
         "api_endpoint": "/tables/spanning-tree/bridges",
         "get": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/bridges",
             "columns": [
-                "mode",
                 "siteName",
-                "hostname",
+                "id",
+                "mode",
+                "sn",
                 "stpDomain",
-                "changeRate",
                 "virtPorts",
-                "sn",
-                "id",
-                "vlans"
+                "hostname",
+                "vlans",
+                "changeRate"
             ],
             "description": "Overview of all Spanning-Tree Protocol (STP) bridges, protocol types, VLANs",
             "summary": "STP Bridges",
             "web_endpoint": "/technology/spanning-tree/stp-bridges"
         }
     },
     "tables/spanning-tree/guards": {
         "api_endpoint": "/tables/spanning-tree/guards",
         "get": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/guards",
             "columns": [
+                "model",
+                "bpduGuard",
                 "siteName",
-                "hostname",
-                "intName",
-                "stpDomain",
                 "platform",
+                "id",
                 "voiceVlan",
-                "bpduGuard",
                 "bpduFilter",
                 "dynamicMacCount",
+                "devType",
+                "vendor",
                 "sn",
+                "stpDomain",
                 "switchportMode",
-                "vendor",
-                "portfast",
-                "model",
                 "accVlan",
-                "devType",
+                "portfast",
+                "hostname",
                 "rootGuard",
-                "id"
+                "intName"
             ],
             "description": "Overview of all Spanning-Tree Protocol (STP) guards applied to interfaces",
             "summary": "STP Guards",
             "web_endpoint": "/technology/spanning-tree/stp-guards"
         }
     },
     "tables/spanning-tree/inconsistencies/multiple-stp": {
         "api_endpoint": "/tables/spanning-tree/inconsistencies/multiple-stp",
         "get": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/inconsistencies/multiple-stp",
             "columns": [
-                "dstSn",
+                "dstHostname",
                 "siteName",
+                "id",
+                "srcSn",
                 "srcHostname",
                 "stpCount",
-                "dstHostname",
-                "srcSn",
-                "id"
+                "dstSn"
             ],
             "description": "Detected multiple Spanning-Tree Protocol (STP) instances between two devices",
             "summary": "Multiple STPs",
             "web_endpoint": "/technology/spanning-tree/inconsistencies/multiple-stp"
         }
     },
     "tables/spanning-tree/inconsistencies/neighbor-ports-vlan-mismatch": {
         "api_endpoint": "/tables/spanning-tree/inconsistencies/neighbor-ports-vlan-mismatch",
         "get": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/inconsistencies/neighbor-ports-vlan-mismatch",
             "columns": [
-                "dstSn",
-                "srcVlanCount",
+                "dstHostname",
                 "siteName",
-                "srcHostname",
-                "srcIntName",
+                "id",
                 "dstVlanCount",
-                "dstHostname",
-                "dstIntName",
                 "srcSn",
-                "id"
+                "srcHostname",
+                "dstIntName",
+                "srcVlanCount",
+                "dstSn",
+                "srcIntName"
             ],
             "description": "Neighbor trunk ports where there is a different number of VLANs on each side of the link",
             "summary": "STP Ports VLAN Mismatch",
             "web_endpoint": "/technology/spanning-tree/inconsistencies/neighbor-ports-vlan-mismatch"
         }
     },
     "tables/spanning-tree/inconsistencies/ports-multiple-neighbors": {
         "api_endpoint": "/tables/spanning-tree/inconsistencies/ports-multiple-neighbors",
         "get": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/inconsistencies/ports-multiple-neighbors",
             "columns": [
-                "dstSn",
+                "dstHostname",
                 "siteName",
+                "id",
+                "srcSn",
                 "srcHostname",
-                "srcIntName",
-                "dstHostname",
                 "dstIntName",
-                "srcSn",
-                "id"
+                "dstSn",
+                "srcIntName"
             ],
             "description": "Neighbor switchports where multiple Spanning-Tree Protocol (STP) peerings are detected",
             "summary": "STP Ports Multiple Neighbors",
             "web_endpoint": "/technology/spanning-tree/inconsistencies/ports-multiple-neighbors"
         }
     },
     "tables/spanning-tree/inconsistencies/stp-cdp-ports-mismatch": {
         "api_endpoint": "/tables/spanning-tree/inconsistencies/stp-cdp-ports-mismatch",
         "get": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/inconsistencies/stp-cdp-ports-mismatch",
             "columns": [
                 "siteName",
-                "hostname",
-                "intName",
-                "stpHostname",
-                "sn",
-                "stpSn",
+                "id",
                 "cdpHostname",
                 "cdpIntName",
+                "stpSn",
+                "sn",
+                "stpHostname",
                 "cdpSn",
                 "stpIntName",
-                "id"
+                "hostname",
+                "intName"
             ],
             "description": "Port connections with mismatched hostname or interface name in STP and CDP protocols reading",
             "summary": "STP/CDP Mismatch",
             "web_endpoint": "/technology/spanning-tree/inconsistencies/stp-cdp-ports-mismatch"
         }
     },
     "tables/spanning-tree/instance-members": {
         "api_endpoint": "/tables/spanning-tree/instance-members",
         "get": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/instance-members",
             "columns": [
-                "rootHostname",
+                "id",
                 "vlanId",
-                "rootId",
                 "vlanName",
-                "members",
-                "id"
+                "rootHostname",
+                "rootId",
+                "members"
             ],
             "description": "",
             "summary": "POST /tables/spanning-tree/instance-members",
             "web_endpoint": null
         }
     },
     "tables/spanning-tree/instances": {
         "api_endpoint": "/tables/spanning-tree/instances",
         "get": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/instances",
             "columns": [
+                "rootPriority",
                 "siteName",
-                "hostname",
-                "stpDomain",
-                "changeRate",
-                "edgesSum",
                 "virtPorts",
-                "vlanId",
+                "id",
+                "edgesSum",
+                "devs",
                 "sn",
-                "rootId",
+                "vlanId",
+                "stpDomain",
                 "vlanName",
-                "rootPriority",
-                "devs",
-                "id"
+                "rootId",
+                "hostname",
+                "changeRate"
             ],
             "description": "Spanning-Tree Protocol (STP) instances, root bridges and associated VLANs",
             "summary": "STP Instances",
             "web_endpoint": "/technology/spanning-tree/stp-instances"
         }
     },
     "tables/spanning-tree/neighbors": {
         "api_endpoint": "/tables/spanning-tree/neighbors",
         "get": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/neighbors",
             "columns": [
-                "siteName",
-                "sn",
-                "portRole",
-                "portStatus",
-                "vlanId",
-                "portRoleDst",
-                "portId",
-                "portIdDst",
                 "snDst",
-                "vlanName",
-                "portStatusDst",
+                "portIdDst",
+                "id",
                 "portPathCost",
-                "rootId",
-                "hostnameDst",
-                "hostname",
+                "vlanName",
                 "intName",
-                "intNameDst",
+                "hostnameDst",
                 "stpDomain",
+                "portId",
+                "hostname",
+                "portRole",
+                "portStatusDst",
+                "sn",
+                "vlanId",
+                "siteName",
                 "portPathCostDst",
-                "id"
+                "intNameDst",
+                "portRoleDst",
+                "rootId",
+                "portStatus"
             ],
             "description": "Spanning-Tree Protocol (STP) peering relationships of connected bridges",
             "summary": "STP Peerings",
             "web_endpoint": "/technology/spanning-tree/stp-neighbors"
         }
     },
     "tables/spanning-tree/ports": {
         "api_endpoint": "/tables/spanning-tree/ports",
         "get": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/ports",
             "columns": [
-                "portStatus",
+                "portRole",
                 "siteName",
+                "id",
+                "portPathCost",
+                "sn",
                 "hostname",
-                "intName",
                 "stpDomain",
                 "vlanId",
-                "portId",
-                "sn",
-                "rootId",
                 "vlanName",
-                "portRole",
-                "portPathCost",
-                "id"
+                "portStatus",
+                "rootId",
+                "portId",
+                "intName"
             ],
             "description": "Spanning-Tree Protocol (STP) virtual ports inventory",
             "summary": "STP Virtual Ports",
             "web_endpoint": "/technology/spanning-tree/stp-virtual-ports"
         }
     },
     "tables/spanning-tree/radius": {
         "api_endpoint": "/tables/spanning-tree/radius",
         "get": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/radius",
             "columns": [
-                "srcDev",
-                "stpDomain",
-                "dstDev",
                 "stpMode",
                 "distance",
-                "id"
+                "id",
+                "stpDomain",
+                "srcDev",
+                "dstDev"
             ],
             "description": "",
             "summary": "POST /tables/spanning-tree/radius",
             "web_endpoint": "/technology/spanning-tree/stp-radius"
         }
     },
     "tables/spanning-tree/topology": {
         "api_endpoint": "/tables/spanning-tree/topology",
         "get": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/topology",
             "columns": [
-                "root",
-                "stpDomain",
                 "siteName",
+                "id",
                 "vlanId",
-                "changeRate",
+                "stpDomain",
                 "vlanName",
-                "id"
+                "root",
+                "changeRate"
             ],
             "description": "Spanning-Tree Protocol (STP) instances with topology change compared to the last snapshot",
             "summary": "STP Stability",
             "web_endpoint": "/technology/spanning-tree/stp-stability"
         }
     },
     "tables/spanning-tree/vlans": {
         "api_endpoint": "/tables/spanning-tree/vlans",
         "get": null,
         "post": {
             "api_endpoint": "tables/spanning-tree/vlans",
             "columns": [
-                "bridgeId",
+                "rootPriority",
+                "bridgePriority",
                 "siteName",
-                "hostname",
-                "stpDomain",
-                "changeRate",
                 "virtPorts",
-                "vlanId",
+                "id",
                 "sn",
-                "rootId",
-                "bridgePriority",
                 "rootCost",
-                "rootPriority",
+                "stpDomain",
+                "vlanId",
                 "vlanName",
-                "id"
+                "bridgeId",
+                "rootId",
+                "hostname",
+                "changeRate"
             ],
             "description": "Spanning-Tree Protocol (STP) VLANs inventory",
             "summary": "STP VLANs",
             "web_endpoint": "/technology/spanning-tree/stp-vlans"
         }
     },
     "tables/url": {
@@ -9055,397 +9075,397 @@
     },
     "tables/users": {
         "api_endpoint": "/tables/users",
         "get": null,
         "post": {
             "api_endpoint": "tables/users",
             "columns": [
-                "domainSuffixes",
-                "ldapId",
-                "ssoProvider",
-                "username",
-                "email",
                 "timezone",
-                "roleIds",
                 "isLocal",
                 "id",
-                "roleNames"
+                "roleIds",
+                "domainSuffixes",
+                "email",
+                "roleNames",
+                "ldapId",
+                "username",
+                "ssoProvider"
             ],
             "description": "",
             "summary": "POST /tables/users",
             "web_endpoint": "/settings/administration/local-users"
         }
     },
     "tables/vlan/device": {
         "api_endpoint": "/tables/vlan/device",
         "get": null,
         "post": {
             "api_endpoint": "tables/vlan/device",
             "columns": [
+                "stdStatus",
                 "siteName",
-                "hostname",
-                "stpDomain",
-                "vlanId",
+                "id",
                 "sn",
+                "vlanId",
+                "stpDomain",
                 "vlanName",
-                "stdStatus",
-                "status",
-                "id"
+                "hostname",
+                "status"
             ],
             "description": "Virtual LAN (VLAN) inventory",
             "summary": "VLANs - Device Detail",
             "web_endpoint": "/technology/vlans/device-detail"
         }
     },
     "tables/vlan/device-summary": {
         "api_endpoint": "/tables/vlan/device-summary",
         "get": null,
         "post": {
             "api_endpoint": "tables/vlan/device-summary",
             "columns": [
                 "siteName",
-                "hostname",
-                "totalVlanCount",
-                "sn",
+                "id",
                 "activeVlanCount",
-                "id"
+                "sn",
+                "hostname",
+                "totalVlanCount"
             ],
             "description": "Virtual LAN (VLAN) per managed network device",
             "summary": "VLANs - Device Summary",
             "web_endpoint": "/technology/vlans/device-summary"
         }
     },
     "tables/vlan/l3-gateways": {
         "api_endpoint": "/tables/vlan/l3-gateways",
         "get": null,
         "post": {
             "api_endpoint": "tables/vlan/l3-gateways",
             "columns": [
-                "vlanId",
-                "stpDomain",
-                "rootId",
                 "id",
-                "networks"
+                "networks",
+                "stpDomain",
+                "vlanId",
+                "rootId"
             ],
             "description": "Layer 3 Gateways to VLAN mappings",
             "summary": "L3 Gateways",
             "web_endpoint": "/technology/vlans/l3-gateways"
         }
     },
     "tables/vlan/network-summary": {
         "api_endpoint": "/tables/vlan/network-summary",
         "get": null,
         "post": {
             "api_endpoint": "tables/vlan/network-summary",
             "columns": [
-                "vlanId",
-                "devCount",
                 "dscr",
+                "id",
+                "vlanId",
                 "vlanName",
-                "id"
+                "devCount"
             ],
             "description": "Virtual LANs (VLAN) configured in network grouped by VLAN ID",
             "summary": "VLANs - Network Summary",
             "web_endpoint": "/technology/vlans/network-summary"
         }
     },
     "tables/vlan/site-summary": {
         "api_endpoint": "/tables/vlan/site-summary",
         "get": null,
         "post": {
             "api_endpoint": "tables/vlan/site-summary",
             "columns": [
                 "siteName",
-                "devCount",
-                "vlanId",
                 "dscr",
+                "id",
+                "vlanId",
                 "vlanName",
-                "id"
+                "devCount"
             ],
             "description": "Virtual LANs (VLAN) configured in network grouped by VLAN ID with site information",
             "summary": "VLANs - Summary per Site",
             "web_endpoint": "/technology/vlans/site-summary"
         }
     },
     "tables/vrf/detail": {
         "api_endpoint": "/tables/vrf/detail",
         "get": null,
         "post": {
             "api_endpoint": "tables/vrf/detail",
             "columns": [
                 "siteName",
-                "hostname",
                 "rd",
+                "id",
+                "intCount",
                 "sn",
                 "vrf",
-                "intCount",
-                "id"
+                "hostname"
             ],
             "description": "Virtual Routing and Forwadring instances per devices",
             "summary": "VRF Devices",
             "web_endpoint": "/technology/routing/vrf/detail"
         }
     },
     "tables/vrf/interfaces": {
         "api_endpoint": "/tables/vrf/interfaces",
         "get": null,
         "post": {
             "api_endpoint": "tables/vrf/interfaces",
             "columns": [
                 "siteName",
-                "hostname",
-                "intName",
                 "rd",
+                "id",
                 "sn",
+                "networks",
                 "vrf",
-                "id",
-                "networks"
+                "hostname",
+                "intName"
             ],
             "description": "Virtual Routing and Forwadring instances per interfaces",
             "summary": "VRF Interfaces",
             "web_endpoint": "/technology/routing/vrf/interfaces"
         }
     },
     "tables/vrf/summary": {
         "api_endpoint": "/tables/vrf/summary",
         "get": null,
         "post": {
             "api_endpoint": "tables/vrf/summary",
             "columns": [
-                "vrf",
                 "id",
-                "devices"
+                "devices",
+                "vrf"
             ],
             "description": "Virtual Routing and Forwadring instances per devices summary",
             "summary": "VRF Summary",
             "web_endpoint": "/technology/routing/vrf/summary"
         }
     },
     "tables/vxlan/interfaces": {
         "api_endpoint": "/tables/vxlan/interfaces",
         "get": null,
         "post": {
             "api_endpoint": "tables/vxlan/interfaces",
             "columns": [
-                "sourcePrimaryIp",
-                "sourcePrimaryIpv6",
                 "siteName",
-                "hostname",
-                "intName",
-                "sourceSecondaryIpv6",
+                "hostLearningMode",
+                "sourcePrimaryIp",
                 "localRouterMac",
+                "id",
+                "sourceSecondaryIp",
+                "controlPlane",
                 "sn",
-                "sourceInt",
                 "encap",
-                "hostLearningMode",
-                "controlPlane",
-                "id",
-                "sourceSecondaryIp"
+                "sourceInt",
+                "sourceSecondaryIpv6",
+                "sourcePrimaryIpv6",
+                "hostname",
+                "intName"
             ],
             "description": "Virtual Tunnel End Point (VTEP) interfaces inventory",
             "summary": "VTEP Interfaces",
             "web_endpoint": "/technology/sdn/vxlan/interfaces"
         }
     },
     "tables/vxlan/peers": {
         "api_endpoint": "/tables/vxlan/peers",
         "get": null,
         "post": {
             "api_endpoint": "tables/vxlan/peers",
             "columns": [
-                "localAddress",
-                "siteName",
-                "sn",
-                "neiDevType",
-                "learnType",
-                "uptime",
-                "target",
-                "neiAddress",
-                "vni",
                 "neiHostname",
+                "id",
+                "uptime",
+                "neiSiteName",
                 "eVni",
-                "subnet",
-                "hostname",
-                "intName",
                 "neiSn",
+                "neiDevType",
+                "intName",
+                "neiAddress",
                 "neiIntName",
-                "neiSiteName",
                 "flags",
-                "routerMac",
+                "localAddress",
+                "hostname",
+                "subnet",
                 "state",
+                "source",
+                "sn",
+                "siteName",
+                "vni",
                 "devType",
-                "id",
-                "source"
+                "learnType",
+                "routerMac",
+                "target"
             ],
             "description": "Virtual Tunnel End Point (VTEP) peers matrix",
             "summary": "VTEP Peers",
             "web_endpoint": "/technology/sdn/vxlan/peers"
         }
     },
     "tables/vxlan/vni": {
         "api_endpoint": "/tables/vxlan/vni",
         "get": null,
         "post": {
             "api_endpoint": "tables/vxlan/vni",
             "columns": [
                 "bd",
-                "mode",
                 "siteName",
-                "intName",
-                "hostname",
-                "vniState",
+                "type",
+                "id",
                 "vni",
+                "mode",
                 "sn",
-                "vrf",
-                "mcastGroup",
+                "vniState",
                 "cfg",
-                "type",
-                "id"
+                "vrf",
+                "hostname",
+                "intName",
+                "mcastGroup"
             ],
             "description": "VXLAN network identifier (VNI) inventory",
             "summary": "VXLAN Network Identifier",
             "web_endpoint": "/technology/sdn/vxlan/vni"
         }
     },
     "tables/vxlan/vtep": {
         "api_endpoint": "/tables/vxlan/vtep",
         "get": null,
         "post": {
             "api_endpoint": "tables/vxlan/vtep",
             "columns": [
                 "siteName",
-                "hostname",
-                "vniCount",
-                "sn",
-                "peersCount",
                 "id",
-                "interfacesCount"
+                "sn",
+                "vniCount",
+                "interfacesCount",
+                "hostname",
+                "peersCount"
             ],
             "description": "VXLAN tunnel endpoint (VTEP) inventory",
             "summary": "VXLAN Tunnel Endpoints",
             "web_endpoint": "/technology/sdn/vxlan/vtep"
         }
     },
     "tables/wireless/access-points": {
         "api_endpoint": "/tables/wireless/access-points",
         "get": null,
         "post": {
             "api_endpoint": "tables/wireless/access-points",
             "columns": [
+                "switchPort",
+                "clientCount",
                 "siteName",
                 "avgRssi",
-                "controllerSn",
-                "controller",
-                "apMac",
-                "clientCount",
-                "switchHostname",
                 "avgSignalToNoiseRatio",
-                "switchPort",
-                "bssidCount",
-                "ssid",
                 "switchSn",
-                "apName",
-                "apSn",
                 "id",
+                "apSn",
+                "bssidCount",
+                "apMac",
+                "controller",
+                "ssid",
+                "controllerSn",
                 "apPort",
-                "impact"
+                "apName",
+                "impact",
+                "switchHostname"
             ],
             "description": "Wireless access points inventory",
             "summary": "Wireless Access Points",
             "web_endpoint": "/technology/wireless/access-points"
         }
     },
     "tables/wireless/clients": {
         "api_endpoint": "/tables/wireless/clients",
         "get": null,
         "post": {
             "api_endpoint": "tables/wireless/clients",
             "columns": [
-                "siteName",
-                "inPktsRate",
                 "client",
-                "ssid",
-                "bytesRate",
-                "policyManagerState",
-                "pktsRate",
+                "id",
+                "inPktsRate",
                 "signalToNoiseRatio",
-                "inBytesRate",
                 "frequency",
+                "pktsRate",
                 "bssid",
-                "apName",
+                "outPktsRate",
+                "policyManagerState",
+                "ssid",
                 "controllerSn",
+                "apName",
+                "clientIp",
+                "inBytesRate",
+                "uniqId",
+                "state",
                 "apSn",
-                "controller",
-                "outPktsRate",
+                "siteName",
                 "rssi",
-                "outBytesRate",
-                "state",
-                "uniqId",
-                "clientIp",
-                "id"
+                "bytesRate",
+                "controller",
+                "outBytesRate"
             ],
             "description": "Wireless clients inventory",
             "summary": "Wireless Clients",
             "web_endpoint": "/technology/wireless/clients"
         }
     },
     "tables/wireless/controllers": {
         "api_endpoint": "/tables/wireless/controllers",
         "get": null,
         "post": {
             "api_endpoint": "tables/wireless/controllers",
             "columns": [
-                "apCount",
-                "siteName",
                 "clientCount",
-                "ssid",
-                "controllerSn",
+                "siteName",
+                "apCount",
                 "id",
-                "controller"
+                "controller",
+                "ssid",
+                "controllerSn"
             ],
             "description": "Wireless controllers inventory",
             "summary": "Wireless Controllers",
             "web_endpoint": "/technology/wireless/controllers"
         }
     },
     "tables/wireless/radio": {
         "api_endpoint": "/tables/wireless/radio",
         "get": null,
         "post": {
             "api_endpoint": "tables/wireless/radio",
             "columns": [
                 "radioFreq",
-                "radioMac",
-                "radioDscr",
-                "siteName",
-                "wlanBssid",
+                "wlanSsid",
                 "clientCount",
-                "radioStatus",
-                "apName",
+                "siteName",
                 "id",
                 "apSn",
+                "radioDscr",
+                "wlanBssid",
+                "apName",
                 "mac",
-                "wlanSsid"
+                "radioStatus",
+                "radioMac"
             ],
             "description": "Wireless Radios & BSSID inventory",
             "summary": "Wireless Radios & BSSID",
             "web_endpoint": "/technology/wireless/radios/radios-detail"
         }
     },
     "tables/wireless/ssid-summary": {
         "api_endpoint": "/tables/wireless/ssid-summary",
         "get": null,
         "post": {
             "api_endpoint": "tables/wireless/ssid-summary",
             "columns": [
-                "radioCount",
-                "apCount",
                 "clientCount",
-                "ssid",
+                "apCount",
                 "id",
+                "radioCount",
+                "ssid",
                 "wlcCount"
             ],
             "description": "Wireless service set identifier (SSID) summary",
             "summary": "Wireless SSID Summary",
             "web_endpoint": "/technology/wireless/radios/ssid-summary"
         }
     },
```

### Comparing `mini_ipfabric-6.7.2/pyproject.toml` & `mini_ipfabric-6.8.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mini-ipfabric"
-version = "v6.7.2"
+version = "v6.8.0"
 description = "Mini Python package for interacting with IP Fabric using requests."
 authors = [
     "Justin Jeffery <justin.jeffery@ipfabric.io>",
     "Cristian Cordero <cristian.cordero@ipfabric.io>",
     "Solution Architecture <solution.architecture@ipfabric.io>"
 ]
 license = "MIT"
```

### Comparing `mini_ipfabric-6.7.2/README.md` & `mini_ipfabric-6.8.0/README.md`

 * *Files identical despite different names*

### Comparing `mini_ipfabric-6.7.2/PKG-INFO` & `mini_ipfabric-6.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mini-ipfabric
-Version: 6.7.2
+Version: 6.8.0
 Summary: Mini Python package for interacting with IP Fabric using requests.
 Home-page: https://gitlab.com/ip-fabric/integrations/mini-ipfabric
 License: MIT
 Keywords: ipfabric,ip-fabric,community-fabric
 Author: Justin Jeffery
 Author-email: justin.jeffery@ipfabric.io
 Requires-Python: >=3.7,<4.0
```

