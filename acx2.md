---
title: MSYS2 の bash 限定コマンド
tags: [bash, msys2]
---

| 操作                                         | コマンド            |
| -------------------------------------------- | ------------------- |
| Windows 形式のカレントディレクトリを表示する | `pwd -W`            |
| Windows 形式のパスを Unix 形式に変換         | `cygpath -u (パス)` |
| Unix 形式のパスを Windows 形式に変換         | `cygpath -d (パス)` |
