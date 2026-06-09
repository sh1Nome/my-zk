---
title: よく使う Docker コマンド
tags: [docker, command]
---

| 操作                                                                                                        | コマンド                             |
| ----------------------------------------------------------------------------------------------------------- | ------------------------------------ |
| 起動しているコンテナ一覧を出力する                                                                          | `docker ps`                          |
| すべてのコンテナ一覧を出力する                                                                              | `docker ps -a`                       |
| イメージ一覧を出力する                                                                                      | `docker image ls`                    |
| カレントディレクトリの compose.yml に従い、コンテナを起動する（バックグラウンド実行、ビルド）               | `docker compose up -d --build`       |
| カレントディレクトリの compose.yml に従い、コンテナを停止する（ローカルのイメージを削除、ボリュームを削除） | `docker compose down --rmi local -v` |
| コンテナで bash を実行する                                                                                  | `docker exec -it (コンテナid) bash`  |
| 使用していないすべてのリソースを強制削除する                                                                | `docker system prune -af`            |
| Docker のディスク使用状況を詳細表示する                                                                     | `docker system df -v`                |
| イメージのビルドログを出力する                                                                              | `docker history (イメージid)`        |
| コンテナのログを出力する                                                                                    | `docker logs (コンテナID)`           |
| Docker の実行ホストとコンテナ内でファイルをやり取りする、コンテナのパスは `(コンテナID):(パス)` と表記する  | `docker cp (パスA):(パスB)`          |

