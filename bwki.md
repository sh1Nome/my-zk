---
title: fast-forward merge とは
tags: [git, command]
---

マージコミットを作成せずにマージすること。  
作業ブランチにマージ先ブランチの HEAD が含まれ、線形的な履歴になっているときに実行できる。  
`git merge --ff-only` を使うと fast-forward merge の場合のみマージを許可する。  
`git merge --no-ff` を使うと fast-forward merge を行わず、必ずマージコミットを作成する。
