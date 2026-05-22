---
title: git で署名を SSH Key でする方法
tags: [git, command]
---

.config/git/config もしくは .gitconfig に以下の設定をする。

```
[user]
    name = sh1nome # Git のユーザー名
    email = shinodayo1024@gmail.com # Git のメールアドレス
    signingkey = ~/.ssh/id_ed25519.pub # Git の署名用の公開鍵のパス
[commit]
    gpgsign = true # すべてのコミットで署名する
[gpg]
    format = ssh # 署名時に使用するフォーマット
```

user.signingkey で設定した公開鍵を GitHub に署名用の鍵として登録する。
