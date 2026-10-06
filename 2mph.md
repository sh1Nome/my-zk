---
title: Docker Sandboxes で認証が必要なツールを使う方法
tags: [sbx, ai]
---

[v2 mixin kit](https://docs.docker.com/ai/sandboxes/customize/kits-v2/) でツールを入れ、以下の手順で起動する。

```bash
# ドメインを許可する
sbx polocy allow network example.com

# アクセストークンを環境変数に設定する
read -r -s -p 'token: ' TMP_TOKEN

# アクセストークンを sbx に設定する
sbx secret set-custom --host example.com --env EXAMPLE_TOKEN --value "$TMP_TOKEN"

# 環境変数に設定したアクセストークンを削除する
unset TMP_TOKEN

# sbx に設定したアクセストークンのプレースホルダーを確認する
sbx secret ls

# v2 mixin kit と sbx に設定したアクセストークンを使い codex を起動する
sbx run codex --kit ./example-kit -e EXAMPLE_TOKEN='<プレースホルダー>'
```

注: 上記はツールが `EXAMPLE_TOKEN` をアクセストークンとして扱う場合の手順
