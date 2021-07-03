# ELK-DEP-OPTIONS

This repository contains various deployment options to build a elasticsearch cluster for use. 

- Docker Only
- Docker Compose + No Auth [BASIC LICENSE]
- Docker Compose + AD Auth [BASIC LICENSE]
- Docker Compose + OpenID Connect Auth [BASIC LICENSE]
- Standard Kubernetes + Snapshot Plugin + No Auth [BASIC LICENSE]
- Standard Kubernetes using ECK + Snapshot Plugin + Basic Auth [BASIC LICENSE]
- Standard Kubernetes + Snapshot Plugin + OpenDistro Security Plugin + Basic Auth [BASIC LICENSE]
- Standard Kubernetes + Snapshot Plugin + OpenDistro Security Plugin + AD Auth [BASIC LICENSE]
- Standard Kubernetes + Snapshot Plugin + OpenDistro Security Plugin + OpenID Connect Auth [BASIC LICENSE]
- OpenDistro Elasticsearch

Apart from this repository contains examples of Elasticsearch deployment using OpenDistro Security plugin instead of X-Pack. 


Befor running any elasticsearch cluster on Kubernetes/Docker, make sure node has maximum number of memory map areas a process may have defined.

```
sysctl -w vm.max_map_count=262144

```







### OIDC 

```
curl https://login.microsoftonline.com/<TENANT_ID>/v2.0/.well-known/openid-configuration | jq
https://gist.github.com/paulgrav/31909667f96614a645b1ceec5b9b06b0
```
