---
title: GitHub の読み取り専用トークンを楽に作る方法
tags: [github]
---

URL パラメーターを使うことで事前入力できる。  
例えば 30 日限定の読み取り専用トークンなら以下。

https://github.com/settings/personal-access-tokens/new?expires_in=30&contents=read&issues=read&pull_requests=read&actions=read&discussions=read

詳細はこちらを確認。
https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens#pre-filling-fine-grained-personal-access-token-details-using-url-parameters

補足:（2026/11/15 時点）

* このトークンは自分のプロジェクトであれば Issue を作成できる
    * `gh issue create`
    * `gh api --method POST repos/sh1Nome/dotfiles/issues -f title='test' -f body='test'`
* `gh issue` の `close`, `comment`, `reopen` は使えない
* https://docs.github.com/en/rest/issues/issues?apiVersion=2026-03-10#create-an-issue には解釈が難しいことが書いてある
    * > “Issues” repository permissions (write)
    * > Any user with pull access to a repository can create an issue.
* 他の人のプロジェクトに作ろうとすると失敗する
    * > `GraphQL: Resource not accessible by personal access token (createIssue)`
