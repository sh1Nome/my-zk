---
title: SSH サーバーのインストール
tags: [ssh]
---

Debian 系で systemd を使える場合。

```
sudo apt update
sudo apt install ssh
sudo systemctl restart sshd
```

