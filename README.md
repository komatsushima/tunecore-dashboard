# TuneCore Japan Report Dashboard

A drag-and-drop dashboard for visualizing TuneCore Japan CSV reports — streaming revenue, YouTube monetization, Meta (Instagram), and TikTok/UGC — all in a single HTML file.

![Dashboard Preview](screenshots/preview.png)

## Features

- **Drag & drop** CSV files to instantly visualize your music revenue data
- **4 report types** supported: Streaming/DL, YouTube Monetization, Meta, TikTok/UGC
- **Multi-month merge** — drop multiple months of the same report type and data is automatically aggregated
- **Auto-detect encoding** — handles both SHIFT_JIS and UTF-8 CSV files from TuneCore Japan
- **100% client-side** — no data is sent to any server. Everything runs in your browser
- **Single HTML file** — no build tools, no dependencies to install, no server required
- **Store-level insights** — per-store streaming unit price, revenue breakdowns, play count comparisons
- **YouTube Shorts breakdown** — creation count, view count, and per-song ranking for Shorts
- **Responsive design** — works on desktop and mobile

## Supported Report Types

| Report | File Pattern | Key Metrics |
|--------|-------------|-------------|
| Streaming/DL | `report_distribution_jisseki_*.csv` | Revenue, play count, DL count, per-store unit price |
| YouTube | `report_youtube-monetization_jisseki_*.csv` | Views, revenue, Shorts breakdown, video count |
| Meta | `report_facebook-music-product_jisseki_*.csv` | Plays, revenue by platform/event |
| TikTok/UGC | `report_another_ugc_jisseki_*.csv` | Views, creations, revenue |

## Usage

1. Open `index.html` in your browser (or visit the [live demo](https://tunecore-dashboard.netlify.app))
2. Download your monthly CSV reports from [TuneCore Japan](https://www.tunecore.co.jp/)
3. Drag and drop 1–4 CSV files onto the drop zone
4. Explore your revenue data!

You can also drop multiple months of the same report type to see aggregated data across months.

## Deploy Your Own

Since this is a single HTML file with no build step, deployment is simple:

### Netlify (recommended)

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/komatsushima/tunecore-dashboard)

Or manually:
1. Fork this repository
2. Connect to [Netlify](https://app.netlify.com)
3. Set publish directory to `/` (root)
4. Deploy

### GitHub Pages

1. Go to repo Settings → Pages
2. Set source to `main` branch, root `/`
3. Save

### Local

Just open `index.html` in any modern browser. That's it.

## Tech Stack

- Vanilla HTML/CSS/JavaScript (no framework)
- [Chart.js 4.4.1](https://www.chartjs.org/) (loaded from CDN)
- [Noto Sans JP](https://fonts.google.com/noto/specimen/Noto+Sans+JP) (Google Fonts)

## Privacy

This dashboard processes all CSV data entirely in your browser. **No data is ever uploaded or transmitted to any server.** The CSV files never leave your machine.

## License

[MIT](LICENSE)

## Author

**Ko Matsushima (arne)**
- GitHub: [@komatsushima](https://github.com/komatsushima)

---

# TuneCore Japan レポート ダッシュボード

TuneCore Japanの確定レポート（CSV）をドラッグ＆ドロップするだけで、収益・再生数を可視化できるダッシュボードです。

## 特徴

- **ドラッグ＆ドロップ**でCSVを投入するだけ
- **4種類のレポート**に対応：ストリーミング・DL / YouTube収益化 / Meta / TikTok・UGC
- **複数月まとめて投入**可能（同タイプは自動合算）
- **SHIFT_JIS / UTF-8 自動判定**
- **完全ローカル処理** — データはサーバーに一切送信されません
- **単一HTMLファイル** — ビルド不要、サーバー不要
- **ストア別再生単価**、YouTube Shorts内訳など詳細な分析

## 使い方

1. `index.html` をブラウザで開く（または[ライブデモ](https://tunecore-dashboard.netlify.app)にアクセス）
2. TuneCore Japanから確定レポート（CSV）をダウンロード
3. ダッシュボードにドラッグ＆ドロップ
4. 収益データを確認！
