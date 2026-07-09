# Future Product Lab Report System v1.1

展示会・海外視察・技術調査レポートを、単なる報告書ではなく、会社の知識資産へ育てるための Claude Code 用スキルセットです。

## 構成

```text
.claude/commands/
  make-report.md
  review-report.md
  publish-report.md
  archive-report.md
  build-report.md

  Config/
    FPL_STYLE.md
    report-config.yml

  Examples/
    SamplePrompt.md
```

## 推奨ワークフロー

```text
make-report.md
↓
review-report.md
↓
publish-report.md
↓
archive-report.md
```

一括実行する場合は `/build-report <フォルダー名>` を使う（上記4工程を順に統括実行する）。

## 各スキルの役割

### make-report.md

初稿作成。Nippou.txtと写真をもとにReport.mdを作る。

### review-report.md

編集者。写真・本文・構成を整える。

### publish-report.md

出版社。GitHub公開前の品質保証を行う。README.mdの更新バッジ（★/◎/△）もここで洗い直す。

### archive-report.md

知識アーキビスト。Report.mdから技術テーマ・企業・トレンド・アイデアを抽出し、`KnowledgeBase/` へ蓄積する。

### build-report.md

統括役。`Reports/<フォルダー名>/` を対象に、各工程を順番に実行する。差分ビルド（前回ビルド以降の変更分のみ処理）に対応。

## 配置

このリポジトリでは `.claude/commands/` 直下にフラットに配置しており、各ファイルがそのままスラッシュコマンド（`/make-report` 等）になります。

`Config/`・`Examples/` は補助資料であり、スキル本文から参照されます。

## 使い方

### 一括実行（推奨）

```text
/build-report 202604-HANNOVER
```

### 公開前チェックだけ行う場合

```text
publish-report.md のスキルを使って、現在の Report.md をGitHub公開前の品質で最終確認してください。画像リンク、Markdown表示、README.md、CHANGELOG.md、Release Notes、公開判定まで実施してください。
```

### 編集から公開まで行う場合

```text
review-report.md で Report.md を編集品質まで高めたあと、publish-report.md で公開前チェックを行ってください。
```

### 知識資産化まで行う場合

```text
build-report.md の考え方に従って、Report.md を公開品質に整えたうえで、archive-report.md により Knowledge、Companies、Trends、Ideas を更新してください。
```

## Version

v1.1
