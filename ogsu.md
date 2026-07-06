---
title: Debian インストール時の設定
tags: [linux, debian]
---

こんな感じで設定してみた。

- パーティショニング: LVM 有効化、全ファイルを 1 パーティションに
- ファイルシステム: ext4
- パッケージ: Debian デスクトップ環境と Xfce のみ
- ブートローダー: `/dev/sda`に GRUB をインストール
