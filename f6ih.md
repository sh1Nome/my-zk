---
title: msys2 について
tags: [windows, msys2]
---

## 概要

Windows向けのソフトウェア構築環境。LinuxライクなツールとCMakeなどのネイティブビルドツールが含まれる。

## インストール方法

1. https://www.msys2.org/ から以下の3つをダウンロード
    * `msys2-x86_64-yyyymmdd.exe`
    * `msys2-x86_64-yyyymmdd.exe.sig`
    * `msys2-x86_64-yyyymmdd.exe.sha256`
2. SHA256で整合性、GPGで信頼性をチェック
3. インストーラーを実行

## 設定

* `MSYS2_PATH_TYPE=inherit`
    * MSYS2 ルートディレクトリ直下の `.ini` ファイル（例：`C:\msys64\ucrt64.ini`）に `MSYS2_PATH_TYPE=inherit` を記述する
    * Windows の PATH 変数を MSYS2 シェルに継承し、Windows ネイティブツールへのアクセスが容易になる
* `/etc/nsswitch.conf`
    * MSYS2 ルートディレクトリ直下の `/etc/nsswitch.conf` ファイル（例：`C:\msys64\etc\nsswitch.conf`）の `db_home` を `windows` に設定する
    * ホームディレクトリを Windows のユーザープロフィール配下（`C:\Users\ユーザー名`）に変更でき、Windows ネイティブツールとの統合が容易になる

