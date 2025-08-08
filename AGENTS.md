# AGENTS — Constraints & Division of Work

本ファイルはエージェント（Codex）に対する制約や役割分担を記述します。

## Constraints（現時点）
- Design固定: 初期に作成したWebサイトのネオン/高コントラストのデザインに準拠する。
  - 詳細は `notes/design.md` を参照。
- 入力方法: ターミナルに本文を貼り付ける（URLからの直接取得は行わない）。
- 生成物: 単一HTMLの「一枚スライド」。ブラウザで開き、スクリーンショットを取得する前提。
- コンポーネント見た目: タイトル/サブタイトルなどの細部はエージェントに委任。ただしテーマ準拠。
- オフライン/ローカル: 外部APIや外部フォントへの依存は避ける。
- アニメーション: `prefers-reduced-motion` に配慮し、過剰な動きを避ける。

## Roles / Flow（想定）
1. User: 記事本文をこのターミナルに貼り付ける。
2. Agent: 要約（抽出型）→ テンプレ適用 → 単一HTMLを生成（例: `slides/slide-<timestamp>.html`）。
3. User: 生成HTMLをブラウザで開き、キャプチャを取得。

## References
- Plan/タスク: `notes/plan.md`
- Design仕様: `notes/design.md`

