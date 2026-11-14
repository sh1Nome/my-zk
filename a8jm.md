---
title: Docker Sandboxes の kit を起動できないとき
tags: [sbx]
---

以下のエラーが出たときは Docker Desktop の設定で General の「Use containerd for pulling and storing images」を有効にする。

```
exit status 1 ERROR: failed to build: OCI exporter is not supported for the docker driver. Switch to a different driver, or turn on the containerd image store, and try again. Learn more at https://docs.docker.com/go/build-exporters/
```
