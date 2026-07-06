# アイギス・アーク エンブレム

単色SVGのエンブレムをブラウザ上でカスタマイズし、PNGまたはSVGとして保存できる静的HTMLツールです。

## 公開URL

- Cloudflare Pages: `https://arc-emblem.pages.dev`
- GitHub Pages: 廃止

## 主な機能

- `base.svg`の単色カラー変更
- 単色、線形グラデーション、円形グラデーションの切り替え
- SVG全体基準のグラデーション表示
- 土台比率 `3:4` / `9:16`
- サイズ `S` / `M` / `L` / `XL`
- 背景色と透明度の指定
- 透明背景がわかるチェック柄プレビュー
- PNG保存
- SVG保存
- iPhone向け保存表示

## 使い方

1. ページを開く
2. カラー方式、色、比率、サイズ、背景を調整する
3. `PNG保存`または`SVG保存`で書き出す
4. iPhoneでは`iPhone保存`を押し、表示された画像を長押しして写真アプリへ保存する

## ローカル確認

`index.html`は`fetch("base.svg")`でSVGを読み込むため、ローカルファイルを直接開くよりHTTPサーバー経由で確認します。

```sh
python3 -m http.server 8000
```

ブラウザで開く:

```text
http://localhost:8000/
```

## Cloudflare Pages設定

このプロジェクトはビルド不要の静的サイトです。

| 項目 | 設定値 |
| --- | --- |
| Project name | `arc-emblem` |
| Production branch | `main` |
| Framework preset | `None` |
| Build command | 空欄 |
| Build output directory | 空欄または `/` |
| Root directory | 未設定 |

## ファイル構成

```text
.
├── base.svg
├── index.html
├── README.md
└── docs/
    └── 2026年7月6日_要件定義/
        └── 20260706_task.md
```

## 開発メモ

- `base.svg`は塗り指定なしの単色SVGとして扱い、ページ側で`fill`を差し替えています。
- グラデーションは`gradientUnits="userSpaceOnUse"`を使い、複合パスごとではなくSVG全体の`viewBox`基準で描画します。
- PNG書き出しでは、選択中の土台サイズ、背景、余白をCanvasへ描画します。
- SVG書き出しでは、土台サイズ、背景、余白、カスタム済みエンブレムを含む完成版SVGを書き出します。
