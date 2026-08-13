---
title: Docker Sandboxes とは
tags: [ai, docker]
---

AI エージェントのための microVM を基盤としたサンドボックス環境。  
`sbx` コマンドを使い操作する。  
サブコマンドやオプションの使用感は `docker` に似ている。

https://docs.docker.com/ai/sandboxes

サンドボックスからホスト OS 上のプロキシを経由する。  
プロキシで AI エージェントの認証情報を注入するため、  
サンドボックスは AI エージェントの認証情報にアクセスできない。

Windows は winget で導入できる。  
Fedora は GitHub Release の rpm で導入できる。
