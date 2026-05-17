---
title: firewalld の使い方
tags: [linux, bash, command]
---

| 操作                                               | コマンド                                          |
| -------------------------------------------------- | ------------------------------------------------- |
| ファイアウォールのポート8080/tcpを永続的に開放する | `firewall-cmd --permanent --add-port=8080/tcp`    |
| ファイアウォールのポート8080/tcpを永続的に削除する | `firewall-cmd --permanent --remove-port=8080/tcp` |
| ファイアウォールの設定を再読み込みする             | `firewall-cmd --reload`                           |
| 開放されているポートの一覧を表示する               | `firewall-cmd --list-ports`                       |
