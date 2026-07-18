---
title: Route 53 で管理してるサブドメインで Lambda を呼び出す方法
tags: [aws, infra]
---

1. Lambda 関数を作る
1. API Gateway と Lambda をつなげる
1. サブドメインの証明書を ACM で発行する
1. API Gateway のカスタムドメインを作成する
    * ACM で作成した証明書を指定する
1. API マッピングを作成する
    * 対象の API とステージを指定する
1. Route 53 にエイリアスレコードを作成する
