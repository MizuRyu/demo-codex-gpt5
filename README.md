⚠️ 注意: このレポジトリはすべてGPT-5が作成しています。

# demo-codex-gpt5

このリポジトリはデモ用のプロジェクトです。

## とりあえずやること

- 参考: https://gpt5-coding-examples.vercel.app/ のサンプルアプリをまず作成する。
- 下記のプロンプトを試して、単一HTMLのサンプルを生成・実装する。

### プロンプト: Esports Tournament

```
Title: Esports Tournament
Prompt:
Create a single-page app, in a single HTML file, for a neon, high-contrast esports tournament landing page.
Hero: animated 3D/Canvas backdrop with subtle scanlines; bold headline, date, and CTA buttons (“Register Team”, “Get Tickets”, “Watch Live”).
Interactive bracket: 8/16-team bracket with hover states, team logos, and match times; auto-advance demo mode.
Schedule section: timezone-aware match list with filters (stage, day) and an “Add to calendar” button (ICS export).
Team cards: roster, roles, country flags, recent form; responsive grid with quick compare.
Stream preview: embedded placeholder player with “Now/Next” ticker and sponsor carousel.
Venue & travel: map image, directions links, hotels list; accessibility and safety notes.
Social proof: testimonials, follower counts, and recent highlights carousel.  
Footer: FAQs, rules PDF link, code of conduct, contact form; sticky “Buy Tickets” CTA on mobile.  
Performance: lazy-loaded images, prefers-reduced-motion support; clean, modern, fully responsive.
```

## 使い方（ローカルプレビュー）

- 直接開く: macOS は `open index.html`、Windows は `start index.html`。
- 簡易サーバーで開く（推奨）:
  - `python3 -m http.server` を実行し、ブラウザで `http://localhost:8000/index.html` を開く。

## 備考

- アニメーション: OSの「動きを減らす」設定に対応（軽減）。
- 画像: `loading="lazy"` で遅延読み込みに対応。
- カレンダー: スケジュールの「Add to calendar」はICSファイルを生成・ダウンロードします。
- ルールPDF: 簡易プレースホルダのPDFをダウンロードします。
