---
title: git で署名を SSH Key でする方法
tags: [git, command]
---

.config/git/config もしくは .gitconfig に以下の設定をする。

```
[user]
    name = sh1nome # Git のユーザー名
    email = shinodayo1024@gmail.com # Git のメールアドレス
    signingkey = ~/.ssh/id_ed25519 # Git の署名用の秘密鍵のパス
[commit]
    gpgsign = true # すべてのコミットで署名する
[gpg]
    format = ssh # 署名時に使用するフォーマット
[gpg "ssh"]
    allowedSignersFile = ~/.ssh/allowed_signers # 署名の検証をするための設定
```

user.signingkey で設定した公開鍵を GitHub に署名用の鍵として登録する。

allowed_signers はこんな感じで設定できる

```
echo "$(git config get user.email) namespaces=\"git\" $(eval cat "$(ssh -G github.com | awk '/^identityfile/ {print $2; exit}').pub")" >> ~/.ssh/allowed_signers
```
