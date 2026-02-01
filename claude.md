# Valorant戦略ノート

## プロジェクト概要
Valorantの戦略的思考をまとめる技術書プロジェクト。Re:VIEWを使用して執筆。

## 技術スタック
- Re:VIEW（技術書執筆フォーマット）
- Ruby（ビルドツール）

## ディレクトリ構造
- `*.re` - Re:VIEW形式の原稿ファイル
- `config.yml` - Re:VIEW設定
- `catalog.yml` - 章構成の定義
- `Rakefile` - ビルドタスク（html, pdf, epub）

## ビルド
```bash
bundle install
rake html   # HTML出力
rake pdf    # PDF出力
rake epub   # EPUB出力
```

## 執筆ルール
- 言語: 日本語
- 章の追加: `NN-title.re` を作成し `catalog.yml` に追記
