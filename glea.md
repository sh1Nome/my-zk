---
title: apt リポジトリの設定
tags: [linux, debian, package]
---

`/etc/apt/sources.list` または `/etc/apt/sources.list.d/` 配下の `.list` ファイル を編集する  
`.list`ファイルにGPG鍵の場所が書かれている。  
以下に配置されることが多い。  

* `/etc/apt/keyrings/`
* `/etc/apt/trusted.gpg.d/`
* `/usr/share/keyrings/`

