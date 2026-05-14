---
title: GitHub の通知バッジを削除する方法
tags: [github]
---

原因は不明だが、通知がないのに通知バッジだけ残ることがある。  
GitHub APIを使用して通知バッジを削除できる。

```bash
curl -L \
  -X PUT \
  -H "Accept: application/vnd.github+json" \
  -H "Authorization: Bearer <YOUR-TOKEN>" \
  -H "X-GitHub-Api-Version: 2022-11-28" \
  https://api.github.com/notifications \
  -d '{"last_read_at":"2025-11-10T00:00:00Z","read":true}'
```

参考: https://docs.github.com/ja/rest/activity/notifications?apiVersion=2022-11-28#mark-notifications-as-read
