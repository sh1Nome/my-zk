---
title: pandoc の変換結果をクリップボードにコピーする
tags: [command, pandoc]
---

OSC 52 に対応のターミナルであれば、以下のコマンドで pandoc の変換結果を、  
クリップボードにコピーできる。  
MEMO: OSC 52 は base64 エンコード文字列を要求する。

```
printf '\e]52;c;%s\e\\' "$(pandoc -f markdown -t html README.md | base64)"
```
