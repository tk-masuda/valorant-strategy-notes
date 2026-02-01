# Re:VIEW Document for Valorant Strategy Notes

このプロジェクトは[Re:VIEW](https://github.com/kmuto/review)を使用して執筆されています。

## Re:VIEWとは

Re:VIEWは技術書執筆のための軽量マークアップ言語およびツールチェーンです。
HTML、PDF、EPUBなど複数のフォーマットで出力できます。

## ファイル構成

- `config.yml` - Re:VIEWの設定ファイル
- `catalog.yml` - 章構成を定義するファイル
- `01-hogehoge.re` - 第1章のソースファイル
- `02-fugafuga.re` - 第2章のソースファイル
- `Gemfile` - Rubyの依存関係
- `Rakefile` - ビルドタスク定義

## セットアップ

```bash
# 依存関係のインストール
bundle install
```

## ビルド方法

### HTMLの生成

```bash
rake html
```

### PDFの生成

```bash
rake pdf
```

### EPUBの生成

```bash
rake epub
```

## 執筆方法

Re:VIEWの基本的な記法:

- `= 章タイトル` - 章(Chapter)
- `== セクションタイトル` - セクション
- `=== サブセクションタイトル` - サブセクション
- `//list[id][タイトル]{ ... //}` - ソースコードリスト
- `//table[id][タイトル]{ ... //}` - 表
- `//note{ ... //}` - ノート(補足)
- `//tip{ ... //}` - ヒント
- `//warning{ ... //}` - 警告

詳細は[Re:VIEW公式ドキュメント](https://github.com/kmuto/review)を参照してください。
