---
title: Linux で WiFi に接続する方法
tags: [linux, command]
---

| 操作                                        | コマンド                              |
| ------------------------------------------- | ------------------------------------- |
| 接続情報を表示する                          | `nmcli connection show`               |
| 指定したSSIDのWi-Fiに接続する               | `nmcli device wifi connect (SSID)`    |
| Wi-Fiネットワークをスキャンして一覧表示する | `nmcli device wifi list --rescan yes` |
