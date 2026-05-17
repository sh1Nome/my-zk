---
title: Systemd の使い方
tags: [linux, command]
---

| 操作                                                 | コマンド                                                   |
| ---------------------------------------------------- | ---------------------------------------------------------- |
| systemdのデーモン設定を再読み込みする                | `systemctl daemon-reload`                                  |
| 指定したサービスを自動起動するように設定する         | `systemctl enable (サービス名)`                            |
| 指定したサービスを起動する                           | `systemctl start (サービス名)`                             |
| 指定したサービスを停止する                           | `systemctl stop (サービス名)`                              |
| サービスの状態を確認する                             | `systemctl status (サービス名)`                            |
| 指定したサービスが自動起動に設定されているか確認する | `systemctl is-enabled (サービス名)`                        |
| 指定したサービスのユニットファイルの内容を表示する   | `systemctl cat (サービス名)`                               |
| 自動起動設定済みのサービス一覧                       | `systemctl list-unit-files --type=service --state=enabled` |
