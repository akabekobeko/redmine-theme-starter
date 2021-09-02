# Starter kit for theme of Redmine

![Redmine](https://img.shields.io/badge/Redmine-4.2.2-brightgreen)

Redmine テーマを開発するためのスターター キットです。

## インストール

事前に [Node.js](https://nodejs.org/en/)、[Docker](https://www.docker.com/) ([Docker Compose](https://docs.docker.com/compose/))、Git を利用できるようにしてください。そのうえで以下のコマンドを実行します。

```
$ git clone https://github.com/akabekobeko/redmine-theme-starter.git
$ cd redmine-theme-starter
$ npm i
```

## 独自化

テーマをリリースする予定があるなら、以下のファイルに記述された `mytheme` という部分を独自の名前へ置き換えてください。

- `package.json`
- `docker-compose.yml`

## 開発

### ビルド

SCSS ファイルを CSS ファイルに変換します。

```
$ npm run build
```

### Watch build for CSS

SCSS ファイルの変更を検知して CSS ファイルへ変換するツールを起動します。

```
$ npm start
```

<kbd>Ctrl</kbd> + <kbd>C</kbd> でツールを停止します。

### Redmine 上での動作確認

テーマを Redmine 上でチェックするための手順です。

#### 確認開始

```
$ docker-compose up -d
```

1. Web ブラウザーで http://localhost:8080/ を開きます
2. 管理者として Redmine にログインします
3. 管理画面から自分のテーマを選択します
4. テーマの SCSS (CSS) ファイルが更新されたら Web ブラウザー上の Redmine ページを再読み込みします

#### 終了

```
$ docker-compose stop
```

## リリース

テーマをリリースする場合は以下のコマンドを実行してください。

```
$ npm run release
```

実行すると `package.json` の `name` に基づくテーマ ディレクトリーが生成されます。同時に `version` を付与した名前の ZIP アーカイブ ファイルが生成されます。

例 :

- `mytheme`
- `mytheme-1.0.0.zip`

## ライセンス

- [GNU GENERAL PUBLIC LICENSE Version 3](LICENSE)
