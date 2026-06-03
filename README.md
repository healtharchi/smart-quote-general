# スマート見積（汎用版） — HEALTH ARCHI

白紙から自由に見積を作れる汎用の見積ツール。リフォーム・修繕・解体など、工事種別を問わず使えます。
よく使う内訳は「テンプレート」に登録してワンタッチで呼び出せます。

- 公開URL（予定）: https://healtharchi.github.io/smart-quote-general/
- 姉妹ツール: スマート見積システム（木造新築・在来工法専用） https://healtharchi.github.io/smart-quote/

## 特長（v1.1）
- **物件（案件）レイヤー**：物件（お客様・現場）ごとに見積を管理。1物件に複数見積。
- **確定 → 請求書**：見積を確定（編集ロック・解除可）すると請求書を発行（番号自動・振込先表示）。
- 金額は「数量 × 単価」のみ（坪数連動などの自動計算式は持たない＝あらゆる工種に汎用）
- お気に入りテンプレート（カテゴリ・項目・標準単価）の登録／呼び出し
- 見積書3様式（① シンプル ② 内訳付き ③ 正式・押印欄付き）＋請求書を印刷・PDF保存
- 会社情報・印鑑画像・振込先を登録して見積書／請求書に自動表示
- 全データ localStorage（外部送信なし）／JSONエクスポート・インポート（旧v1データは自動移行）

## 技術
- 単一HTML（React 18 + Tailwind CDN + Babel standalone）
- データ保存: ブラウザ localStorage（キー: `ha_general_quote_v1`）
- HEALTH ARCHI ツールUI規約 v1.1 準拠（紺#1B2B4B／オレンジ#F08300・#C85400／本文18px／48pxボタン）

## ファイル
- `index.html` — ツール本体
- `guide.html` — 使い方ガイド
- `README.md` — 本ファイル

## デプロイ
GitHub Pages（静的）。`main` ブランチへ push で自動公開。

---
© HEALTH ARCHI
