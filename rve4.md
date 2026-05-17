---
title: Linux でファイルを圧縮する方法
tags: [linux, command]
---

| 操作                                                         | コマンド                           |
| ------------------------------------------------------------ | ---------------------------------- |
| アーカイブを作成する（create, auto compress, verbose, file） | `tar cavf hoge.tgz hoge/`          |
| `/fuga`ディレクトリに移動してから`hoge/`を圧縮する           | `tar cavf hoge.tgz -C /fuga hoge/` |
| アーカイブを展開する（extract, verbose, file）               | `tar xvf hoge.tgz`                 |
| zipファイルを展開する                                        | `unzip (ファイル名).zip`           |
