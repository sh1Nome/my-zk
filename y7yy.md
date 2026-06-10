---
title: Windows のコマンドライン
tags: [windows]
---

## 概要

cmd と powershell について、とりあえずこれだけ分かればなんとかなる。

## cmd

| 操作                       | コマンド          |
| -------------------------- | ----------------- |
| コマンドのヘルプを表示する | `(command) /h`    |
| コマンドのパスを表示する   | `where (command)` |

## PowerShell

| 操作                       | コマンド                                                            |
| -------------------------- | ------------------------------------------------------------------- |
| コマンドのヘルプを表示する | `help (command)`                                                    |
| コマンドのパスを表示する   | `Get-Command (command)`                                             |
| コマンドのパスを表示する   | `where.exe (command)`                                               |
| ps1 ファイルを実行         | `powershell -NoProfile -ExecutionPolicy Bypass -File /path/to/file` |

