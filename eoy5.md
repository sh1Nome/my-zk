---
title: Linux で日付を操作する
tags: [linux, command]
---

NTP の自動同期を無効にし、手動設定

1. `timedatectl set-ntp false`
1. `timedatectl set-time "2026-07-01 12:00:00"`

戻したいときは NTP の同期を有効に

`timedatectl set-ntp true`

戻らないときは `set-ntp` を `false` → `true` と何度か切り替える
