# CHANGELOG

## 2026-07-09 08:32 Publish Check

### Fixed
- 縦位置写真（IMG_4299.JPG）の表示幅を width="800" → width="500" に修正

### Checked
- Markdown構文：見出し階層（H1×1・H2のみ）、テーブル、`<p>`/`</p>`（28/28）、`<font>`/`</font>`（2/2）すべて正常
- 画像リンク：全29件（Images/直下27件＋OtherPictures/2件）を実ファイルと照合、欠落なし
- 画像サイズ：全て800px以下（IAI・GMO・SEER等の主要写真は800x600、リサイズ済み）
- EXIF orientation：全29枚 `<nil>`（sipsリサイズ時に消失）。縦位置写真2枚（IMG_4299・OtherPictures/IMG_4311）をReadで目視確認し、向き正常を確認
- READMEリンク：出張報告書テーブルに既存登録あり（2025年12月3日行、27枚・3.8MB、集計値と一致）
- GitHub表示互換：問題なし
- 日本語校正：表記揺れなし（AMR等の英数字表記は半角で統一済み）
- 「その他の写真」章：OtherPictures/（IMG_4295.JPG, IMG_4311.PNG）と内容一致

### Notes
- Report.md本文はmake-report段階で既に完成しており、Nippou.txtの内容は全て反映済み
- 本文の大幅な書き換えは行っていない
