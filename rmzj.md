---
title: WSL について
tags: [windows, wsl]
---

## 概要

Windows Subsystem for Linux の略。  
Windows で Linux の仮想環境を使える。  
WSL2 の場合の基盤は Hyper-V。

## インストール

```
wsl --install -d Debian
wsl --set-default Debian
```

## アンインストール

```
wsl --unregister Debian
```

## Windowsのエクスプローラーからアクセス

```
\\wsl$
```

