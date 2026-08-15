# MidField-Archives

MidField System の旧リリース、取扱説明書、SDK 資料、利用事例を保存するアーカイブリポジトリです。現在のソースをビルドするための依存ではなく、Ver.2.00～4.01 の配布物と歴史的資料を参照するために使用します。

## 収録ファイル

| ファイル | 内容 |
| --- | --- |
| `MFS200-Overview.pdf` | MidField System Ver.2.00 概要（2ページ） |
| `MFS200.pdf` | Ver.2.00 取扱説明書（46ページ） |
| `MFS200RC.pdf` | Ver.2.00 遠隔コマンド仕様（36ページ） |
| `MFS200SDK.pdf` | Ver.2.00 SDK 概要説明書（12ページ） |
| `MFS200.exe` | Ver.2.00 インストーラー |
| `MFS200SDK.exe` | Ver.2.00 SDK インストーラー |
| `MFS300-Overview.pdf` | MidField System Ver.3.00 機能概要（2ページ） |
| `MFS300.pdf` | Ver.3.00 取扱説明書（48ページ） |
| `MFS300.exe` | Ver.3.00 インストーラー |
| `MFS400-R0-en.zip` | Ver.4.00 R0 英語版。MSI、`setup.exe`、x86 Visual C++ 再頒布可能パッケージを収録 |
| `MFS401-R0-ja.zip` | Ver.4.01 R0 日本語版。MSI、`setup.exe`、x86 Visual C++ 再頒布可能パッケージを収録 |
| `UseCases.pdf` | 2003～2008年の利用事例（6ページ） |

`MFS300-Overview.pdf` と `MFS300.pdf` の PDF メタデータには Ver.2.00 の表題が残っていますが、表紙と本文は Ver.3.00 です。

## 資料から確認できる製品概要

MidField System は、IP ネットワーク上の多地点映像・音声通信を支援するミドルウェア/アプリケーションとして開発されました。旧版資料には次の機能が記録されています。

- DV/HDV、WMV、PCM、MIDI 等のストリーム送受信と変換。
- 単方向映像配信、双方向映像通話、複数拠点間通信。
- 映像タイル、Picture in Picture、映像・音声ミキサー。
- 中継・トランスコーディング、IP マルチキャスト、IPv6。
- 遠隔コマンドと遠隔デスクトップ。
- 遠隔授業、TV 会議、映像中継、防災・医療教育、遠隔楽器レッスン等への利用。

現在のコードは [MidField-Core](https://github.com/impl84/MidField-Core)、[MidField-Ui](https://github.com/impl84/MidField-Ui)、[MidField-Application](https://github.com/impl84/MidField-Application)、[MidField-System](https://github.com/impl84/MidField-System) に分割されています。開発用統合環境は [MidField-Development](https://github.com/impl84/MidField-Development)、実行スナップショットは [MidField-Runtime](https://github.com/impl84/MidField-Runtime) を参照してください。

## 取り扱い

- 旧インストーラーは現行 Windows、ドライバー、JRE での動作を保証するものではありません。
- EXE/MSI は信頼できる隔離環境で検証し、署名、ハッシュ、依存ランタイム、管理者権限の要否を確認してから実行してください。
- ZIP 内の Visual C++ 再頒布可能パッケージは x86 であり、現在の開発版 x64 バイナリとは世代・アーキテクチャが異なります。
- アーカイブの再圧縮や上書きは避け、更新が必要な場合は新しい版名のファイルとして追加してください。

## ライセンス

このリポジトリには独立した `LICENSE` や EULA のテキストファイルがありません。旧インストーラー内の条件、および現行配布環境の [MidField-Development/EULA.txt](https://github.com/impl84/MidField-Development/blob/main/EULA.txt) を確認してください。文書・画像・実行ファイルの再配布条件が不明な場合は権利者へ確認してください。
