---
title: Linux と Windows (MSYS2) の相互変換
tags: [bash, msys2, linux]
---

| 操作                                         | コマンド                | Windows 限定 |
| -------------------------------------------- | ----------------------- | ------------ |
| Windows 形式のカレントディレクトリを表示する | `pwd -W`                | o            |
| Windows 形式のパスを Unix 形式に変換         | `cygpath -u (パス)`     | o            |
| Unix 形式のパスを Windows 形式に変換         | `cygpath -d (パス)`     | o            |
| CRLF を LF に変換する                        | `dos2unix (ファイル名)` | x            |
| LF を CRLF に変換する                        | `unix2dos (ファイル名)` | x            |
