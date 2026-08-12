---
title: dnf の使い方
tags: [linux, rhel, package]
---

| 操作                                                       | コメント                                                  |
| ---------------------------------------------------------- | --------------------------------------------------------- |
| アップデート可能なパッケージを確認する                     | `dnf check-update`                                        |
| インストール済みパッケージを更新する                       | `dnf upgrade`                                             |
| パッケージを検索する                                       | `dnf search (パッケージ名)`                               |
| パッケージ名にパターンマッチングで検索する                 | `dnf repoquery '*bash*'`                                  |
| パッケージの依存関係を表示する                             | `dnf repoquery --requires (パッケージ名)`                 |
| パッケージの逆依存関係を表示する                           | `dnf repoquery --whatrequires (パッケージ名)`             |
| ユーザーが明示的にインストールしたパッケージのみを表示する | `dnf repoquery --userinstalled`                           |
| パッケージの詳細情報を表示する                             | `dnf info (パッケージ名)`                                 |
| 指定したファイルを含むパッケージを表示する                 | `dnf provides (ファイルパス)`                             |
| パッケージをインストールする                               | `dnf install (パッケージ名)`                              |
| パッケージを削除する                                       | `dnf remove (パッケージ名)`                               |
| 依存されていない自動インストールパッケージを削除する       | `dnf autoremove`                                          |
| COPR（コミュニティリポジトリ）を有効化する                 | `dnf copr enable (ユーザー名/リポジトリ名)`               |
| 有効なリポジトリ一覧を表示する                             | `dnf repo list`                                           |
| 既知のリポジトリにないけどインストールしてるパッケージ一覧 | `dnf list --extras`, `dnf repoquery --installed --extras` |

