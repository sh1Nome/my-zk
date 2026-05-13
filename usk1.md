---
title: ChromeOS で keyring ツールを使う方法
tags: [chrome, os, google]
---

## 概要

ChromeOS で Linux のキーリングツールを使う方法。  
VS Code で GitHub Copilot の認証情報を永続化するときに必要だった。

## 手順

1. `gnome-keyring`をインストールする
    - コマンド: `sudo apt install gnome-keyring seahorse`
2. `gnome-keyring`を利用してVSCodeを起動する
    - コマンド: `code . --password-store="gnome-libsecret"`
3. コマンドパレットで`Preferences: Configure Runtime Arguments`を選択する
4. `argv.json`に以下を追加する
    ```json
    "password-store": "gnome-libsecret"
    ```

## 説明

* `gnome-keyring`: パスワードマネージャーとして機能する
* `seahorse`: `gnome-keyring`に保存されたデータをGUIで操作するためのツールである
* `argv.json`: VSCodeを起動する際のデフォルト引数を設定するファイルである
  - 配置場所: `/home/(user)/.vscode`
  - 削除することで初期設定に戻すことが可能である

## 参考
https://code.visualstudio.com/docs/configure/settings-sync#_recommended-configure-the-keyring-to-use-with-vs-code
