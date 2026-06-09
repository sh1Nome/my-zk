---
title: docker-compose.yml の例
tags: [docker, command]
---

2026 年 6 月現在は compose.yaml が推奨されている。

```yml
services:
  debian:
    image: debian:latest
    # コンテナを起動し続けるためのコマンド
    command: tail -f /dev/null
    # インタラクティブモードとTTYを有効化
    tty: true
    # PID1にinitプロセスを設定
    init: true
    # ホストのディレクトリをマウント
    volumes:
      - ./mount:/root
    # 作業ディレクトリを指定
    working_dir: /root
```
