# 📊 TuneCore Japan レポート ダッシュボード

TuneCore Japanから届く**確定レポート（CSV）**をドラッグ＆ドロップするだけで、収益・再生数を自動分析・可視化するダッシュボードです。

---

## ✨ 機能

- **CSVをドラッグ＆ドロップ**するだけで即分析（アップロード不要・完全ブラウザ処理）
- **4種類の確定レポート**に対応（著作権収益は現在未対応）
- **複数月まとめて投入**すると自動で合算して表示
- **楽曲別・アーティスト別・国別**の収益ランキング
- **ストア別の再生単価**（1再生あたりいくらか）の比較
- **YouTube Shorts** の作成数・再生数の内訳

---

## 🔒 プライバシーについて

CSVデータは**外部サーバーに一切送信されません**。すべてブラウザ内で処理されます。

---

## 🚀 使い方

### 方法① そのままブラウザで使う（一番かんたん）

👉 **[ダッシュボードを開く](https://tcj-report.netlify.app/)**

1. 上のリンクを開く
2. TuneCore Japanから届いたCSVをドラッグ＆ドロップ
3. 自動で分析されます

> 複数月のCSVをまとめて投入すれば、年間集計などもできます。

---

### 方法② 自分でホスティングする

1. このリポジトリをForkする
2. [Netlify](https://netlify.com) でGitHubと連携してデプロイ
3. 以降はGitHubにファイルをアップするだけで自動反映

> `index.html` をダウンロードしてブラウザで開くだけでも使えます。

---

## 📄 対応CSVについて

TuneCore Japanが発行する以下の確定レポートに対応しています：

| レポート種別 | CSVファイル名の例 | わかること |
|:---|:---|:---|
| ストリーミング・DL | `report_distribution_jisseki_YYYYMM.csv` | ストア別収益、再生回数、DL数、再生単価 |
| YouTube 収益化 | `report_youtube-monetization_jisseki_YYYYMM.csv` | 視聴回数、収益、Shorts内訳、動画数 |
| Meta（Instagram等） | `report_facebook-music-product_jisseki_YYYYMM.csv` | 再生数、プラットフォーム別・イベント別収益 |
| TikTok・UGC | `report_another_ugc_jisseki_YYYYMM.csv` | 視聴回数、作成数、収益 |

> ⚠️ 他社のレポートや、TuneCore Japanの著作権収益レポートには現在対応していません

---

## 🛠 技術情報

| 項目 | 内容 |
|------|------|
| 使用ライブラリ | Chart.js (v4.4.1), Noto Sans JP (Google Fonts) |
| 動作環境 | モダンブラウザ（Chrome / Firefox / Safari / Edge） |
| サーバー不要 | 完全クライアントサイド処理 |
| 文字コード | SHIFT_JIS / UTF-8 自動判定 |

---

## 📝 ライセンス

MIT License — 自由に使用・改変・再配布していただいて構いません。

---

## 👤 作者

**松島 功（arne）**
[@komatsushima](https://github.com/komatsushima)
