# kansai.pm.org

`kansai.pm.org`のウェブサイトのビルドシステムです。

[Riji](https://github.com/Songmu/p5-Riji)を使用しています。

# 使い方

## 初期設定

CartonおよびDaikuを使用します。必要に応じてインストールしてください。

```
$ cpanm Carton Daiku
```

githubからcloneしたあと、`daiku setup`で環境を整えます。（必要なモジュールはプロジェクトのディレクトリにインストールされます。）

```
$ git clone https://github.com/kansai-pm/website.git
$ cd /path/to/website
$ daiku setup
```

## 記事の作成

新しい記事を作成するには`daiku new`を実行します。

```
$ daiku new
```

Markdownのファイルが作成されますので、そのファイルを編集してください。

## 記事を確認

記事を作成したら、ローカル環境で正しく表示されているか確認してください。

```
$ daiku serve
```

記事の作成者などは公開時に自動で設定されますので、空欄になっていても問題ありません。

## 記事を公開

記事を確認して問題なければ、記事を公開してください。

```
$ daiku deploy
```

リポジトリの状態も自動的に更新され、githubにpushされます。
