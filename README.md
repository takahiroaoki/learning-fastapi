# api

本リポジトリ[FastAPI入門](https://zenn.dev/sh0nk/books/537bb028709ab9)を学習する際に書いたコードを保管しています。

ライブラリのバージョン、環境や学習のために、配布されたコードと異なる箇所が複数あります。

## 実行環境

本レポジトリのコードの実行環境は以下です。

- Windows 10
- [Docker Desktop for Windows](https://www.docker.com/products/docker-desktop) 4.2.0
- VSCode

## 動作確認

1. 本プロジェクトのディレクトリで、以下のコマンドを実行し、コンテナを起動します。

```
$ docker-compose up -d
```
2. 初めてコンテナを作成した場合は、データベースを初期化します。

```
$ docker-compose exec fast_api poetry run python -m api.migrate_db
```

3. http://localhost:8000/docs にアクセスする。

## 参考文献
- [FastAPI入門](https://zenn.dev/sh0nk/books/537bb028709ab9)
