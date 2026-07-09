# CHANGELOG

## v1.1 - 2026-07-09

### Added
- build-report.md：差分ビルドモード（前回ビルド以降の変更ファイルのみ処理、トークン消費最小化）〔7/6-7/7〕
- publish-report.md：README.md 更新バッジの自動更新（9.4節）〔7/8〕
- archive-report.md：KnowledgeBase 4テーブルのバッジ列・相対時間表記〔7/8〕
- archive-report.md：`effective_time()` — 未コミット編集分を mtime で判定（git履歴のみだと新規ファイルを誤判定するため）〔7/9〕

### Changed
- バッジ体系を3段階に変更：★=24時間以内・◎=3日以内・△=7日以内〔7/9〕（旧：★=3日以内・○=7日以内。○は視認性が低いため△へ変更）
- make-report.md：README 目次テーブルを6列形式（バッジ列＋ナレッジ化列）に更新
- build-report.md：対象フォルダーの場所を `Reports/` 直下に明記
- build-report.md：「変更なし」判定時の写真審査範囲を明確化（動画残存チェック・未分類確認のみ）
- publish-report.md：PUBLISH_SUMMARY.md 日付抽出に `head -1` を追加（差分ビルドの複数日付行対応）
- report-config.yml：KnowledgeBase パス・バッジ定義を現行構成に同期

### Fixed
- publish-report.md：末尾「コミットメッセージ形式」のコードフェンス閉じ忘れを修正（以降の見出しがコードブロックに飲み込まれていた）

## v1.0 - 2026-07-02

### Added
- publish-report.md を追加
- review-report.md を追加
- archive-report.md を追加
- build-report.md を追加
- FPL_STYLE.md を追加
- report-config.yml を追加
- README.md を追加

### Notes
- Future Product Lab Report System の初期バージョン。
