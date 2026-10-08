---
title: GitHub の読み取り専用トークンを楽に作る方法
tags: [github]
---

URL パラメーターを使うことで事前入力できる。  
例えば 30 日限定の読み取り専用トークンなら以下。

https://github.com/settings/personal-access-tokens/new?expires_in=30&contents=read&issues=read&pull_requests=read&actions=read&discussions=read

詳細はこちらを確認。
https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens#pre-filling-fine-grained-personal-access-token-details-using-url-parameters
