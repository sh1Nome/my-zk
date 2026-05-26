---
title: git の author と committer について
tags: [git]
---

git のコミットには author と committer がいる。  
author はコードを書いた人で committer はコミットした人のこと。  
rebase でコミットハッシュが変わる場合、 author は変わらないが、 commiter が変わる。

`git merge --squash` の場合、 author が merge コマンドを実行した人になってしまうらしい。  
`git rebase -i` で squash した場合は、 squash の最初のコミットの author が、  
まとまったコミットの author となる。  
どちらも貢献が消える可能性があるので、できる限り使わないほうがいい。
