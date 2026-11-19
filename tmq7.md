---
title: Docker Sandboxes でクリップボードを使う
tags: [sbx]
---

`sbx settings set clipboard.textCopy true` で codex cli の `/copy` などを使えるようになる。

画像を貼り付けたい場合は `sbx settings set clipboard.imagePaste true` で有効にする。

なぜデフォルトがオフかはここに書いてある。  
画像の貼り付けとはいえホストのデータがサンドボックス内に送信されるかららしい。  
https://docs.docker.com/ai/sandboxes/faq/#can-i-paste-images-into-an-agent
