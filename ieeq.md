---
title: herdr と docker sandboxes を連携する
tags: [sbx, terminal]
---

1. `sbx setup ssh` でサンドボックスに ssh 接続できるようにする
    * `sbx setup ssh remove` で設定を戻せる
    * `ssh sandbox-name.sbx` で接続できるようになる
1. `herdr machine add sandbox-name.sbx` で herdr にサンドボックスを設定する
