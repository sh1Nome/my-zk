---
title: Linux でフォントを操作する
tags: [linux, font]
---

* `fc-list` - インストールしているフォントを一覧表示する
* `fc-list :spacing=mono` - 等幅フォントのリストを表示
* `fc-list :lang=ja` - 日本語対応のフォントを表示
* `fc-query /path/to/ttf | grep spacing` - 等幅フォントか確認
    * 100ならmono, 90ならdual
* `fc-cache -v` - フォントキャッシュを更新する（verbose）
    * `/usr/share/fonts` に入れてから実行するとフォントを追加できる
