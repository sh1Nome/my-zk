---
title: Docker Sandboxes に GitHub の読み取り権限だけ与える方法
tags: [sbx]
---

1. [GitHub の読み取り専用トークンを楽に作る方法](d0br.md) に従って読み取り専用トークンを作る
1. `sbx secret set github` でトークンを設定する
1. `sbx rm` で環境を削除する
1. `sbx run` で新しく環境を起動する
