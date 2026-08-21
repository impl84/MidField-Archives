# MidField Archives

MidField System の旧リリース、取扱説明書、SDK資料、利用事例を保存する歴史的アーカイブです。現在のソースをビルドするための依存物ではなく、Ver.1.32c～4.01の配布物と、2003～2010年頃の開発・利用状況を参照する目的で保管しています。

> [!WARNING]
> 収録されたインストーラーは古いWindows、Java、DirectX、DirectShow、Windows Media環境を前提としています。EXE 12件とZIP内のMSI 2件はいずれもデジタル署名されていません。現行PCへ直接インストールせず、ネットワークから隔離した使い捨ての仮想マシンで内容とハッシュを確認してから扱ってください。

## ディレクトリ構成

```text
MidField-Archives/
├── Installers/                 Ver.1.32c～4.01の旧配布物
├── Manuals/                    Ver.2.00/3.00の説明書と仕様書
└── UseCases_2003-2008.pdf      2003～2008年の利用事例
```

リポジトリ全体は21ファイル、約459 MiBです。実行ファイルやPDFの内容を更新するリポジトリではないため、保存済みファイルの再圧縮・改変・上書きは避けてください。

## 配布物

### Ver.1.32c～3.00

| ファイル | サイズ | 内容 |
| --- | ---: | --- |
| [`MFS132c.exe`](Installers/MFS132c.exe) | 22.90 MiB | MidField System Ver.1.32c 自己解凍形式配布物 |
| [`MFS132cSDK.exe`](Installers/MFS132cSDK.exe) | 42.25 MiB | Ver.1.32c SDK 自己解凍形式配布物 |
| [`MFS200BETA.exe`](Installers/MFS200BETA.exe) | 24.24 MiB | Ver.2.00 BETA 配布物 |
| [`MFS200APAN.exe`](Installers/MFS200APAN.exe) | 25.42 MiB | Ver.2.00系の追加配布物。ファイル名を原形のまま保存 |
| [`MFS200.exe`](Installers/MFS200.exe) | 23.63 MiB | Ver.2.00 配布物 |
| [`MFS200SDK.exe`](Installers/MFS200SDK.exe) | 33.15 MiB | Ver.2.00 SDK 配布物 |
| [`MFS300ALPHA.exe`](Installers/MFS300ALPHA.exe) | 25.31 MiB | Ver.3.00 ALPHA 配布物 |
| [`MFS300ALPHA_REV1.exe`](Installers/MFS300ALPHA_REV1.exe) | 25.31 MiB | Ver.3.00 ALPHA revision 1 |
| [`MFS300ALPHA_REV2.exe`](Installers/MFS300ALPHA_REV2.exe) | 26.47 MiB | Ver.3.00 ALPHA revision 2 |
| [`MFS300ALPHA_REV3.exe`](Installers/MFS300ALPHA_REV3.exe) | 26.47 MiB | Ver.3.00 ALPHA revision 3 |
| [`MFS300BETA.exe`](Installers/MFS300BETA.exe) | 26.37 MiB | Ver.3.00 BETA 配布物 |
| [`MFS300.exe`](Installers/MFS300.exe) | 25.69 MiB | Ver.3.00 配布物 |

これら12件は自己解凍形式のWindows実行ファイルです。PEファイルのバージョン情報に表示される `5.01` / `5.21` は自己解凍ツール側の情報であり、MidField Systemの製品バージョンとして使用しないでください。

### Ver.4.00/4.01

| ファイル | サイズ | ZIP内の構成 |
| --- | ---: | --- |
| [`MFS400-R0-en.zip`](Installers/MFS400-R0-en.zip) | 55.82 MiB | `MFS400-R0.msi`、`setup.exe`、x86 Visual C++再頒布可能パッケージ |
| [`MFS401-R0-ja.zip`](Installers/MFS401-R0-ja.zip) | 59.96 MiB | `MFS401-R0.msi`、`setup.exe`、x86 Visual C++再頒布可能パッケージ |

MSIのプロパティから、Ver.4.00は製品バージョン `4.00.00`・英語（language 1033）、Ver.4.01は `4.01.00`・日本語（language 1041）であることを確認できます。どちらも製造者は `Koji Hashimoto`、UpgradeCodeは共通です。

## 資料

| ファイル | ページ数 | 内容 |
| --- | ---: | --- |
| [`MFS200-Overview.pdf`](Manuals/MFS200-Overview.pdf) | 2 | MidField System Ver.2.00 概要 |
| [`MFS200.pdf`](Manuals/MFS200.pdf) | 46 | Ver.2.00 取扱説明書 |
| [`MFS200RC.pdf`](Manuals/MFS200RC.pdf) | 36 | Ver.2.00 遠隔コマンド仕様 |
| [`MFS200SDK.pdf`](Manuals/MFS200SDK.pdf) | 12 | Ver.2.00 SDK概要説明書。C++/Java APIとサンプルの構成を記載 |
| [`MFS300-Overview.pdf`](Manuals/MFS300-Overview.pdf) | 2 | MidField System Ver.3.00 機能概要 |
| [`MFS300.pdf`](Manuals/MFS300.pdf) | 48 | Ver.3.00 取扱説明書 |
| [`UseCases_2003-2008.pdf`](UseCases_2003-2008.pdf) | 6 | 遠隔教育、TV会議、映像中継、防災、医療教育、遠隔楽器レッスン等の利用事例 |

`MFS300-Overview.pdf` と `MFS300.pdf` のPDFメタデータにはVer.2.00の表題が残っていますが、表示される表紙と本文はVer.3.00です。

## 資料から確認できる機能

旧版資料には次の機能が記録されています。

- DV/HDV、WMV、PCM、MIDI等のストリーム送受信と変換
- 単方向映像配信、双方向映像通話、複数拠点間通信
- 映像タイル、Picture in Picture、映像・音声ミキサー
- 中継・トランスコーディング、IPマルチキャスト、IPv6
- 遠隔コマンドと遠隔デスクトップ
- 遠隔授業、TV会議、イベント中継、防災・医療教育、遠隔楽器レッスンでの利用

Ver.2.00はWindows XP/Vista 32-bit、DirectX 9.0c、Windows Media Player 11、Visual C++ 2005 SP1再頒布可能パッケージ（x86）、Java 6 Update 7を前提としています。Ver.3.00はWindows XP SP3/Vista SP2/Windows 7、Visual C++ 2010再頒布可能パッケージ（x86）、Windows Media Player 11/12、Java 6 Update 22を前提とし、映像ミキシングにOpenCV 2.1.0を使用しています。

## 安全な取り扱い

- 現行Windowsでの動作、互換性、安全性は保証されません。
- 実行前にウイルススキャンとハッシュ確認を行い、仮想マシンのスナップショットを作成してください。
- 検証用仮想マシンは原則オフラインにし、ホストとの共有フォルダやクリップボードも必要最小限にしてください。
- 管理者権限、古い再頒布可能パッケージ、Java、DirectShowフィルターの登録が必要になる可能性があります。
- 旧版が作成する設定、COM登録、ユーザーデータを残さないよう、検証後は仮想マシンを破棄またはスナップショットへ戻してください。
- ZIP内のx86ランタイムや旧バイナリを、現在のx64開発版と混在させないでください。

ファイルのSHA-256はPowerShellで確認できます。

```powershell
Get-FileHash .\Installers\MFS300.exe -Algorithm SHA256
```

## 現行版との関係

現在のMidField System Ver.4のソース、開発環境、実行スナップショットは、統合リポジトリ [MidField-System-Ver.4](https://github.com/impl84/MidField-System-Ver.4) を参照してください。このアーカイブの配布物を現行ソースのビルド依存として使用しないでください。

## ライセンス

このリポジトリには独立した `LICENSE` やEULAのテキストファイルがありません。Ver.2.00 SDK資料では、インストール後の配布物に「使用許諾契約書.txt」が含まれると説明されています。利用・再配布前に各インストーラー内の条件と、現行統合リポジトリの `MidField-Development/EULA.txt` を確認してください。

文書、画像、実行ファイル、および同梱された第三者ランタイムの権利・再配布条件が不明な場合は、権利者へ確認してください。

## READMEの作成

この `README.md` は、リポジトリ内の配布物、PDF資料、Git履歴を調査したうえで、OpenAI Codexが2026年8月21日に作成しました。
