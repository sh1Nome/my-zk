---
title: コマンドの実行結果を標準出力とファイルに出力する
tags: [linux, command, bash]
---

tee コマンドで実現できる。

```
$ echo hello | tee output.txt
hello
$ cat output.txt
hello
```
