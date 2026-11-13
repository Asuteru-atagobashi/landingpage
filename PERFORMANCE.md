# Web性能設計・実装記録

- 対象: Asuteru愛宕橋・1物件1LP
- 区分: 通常の静的サイト
- 初回HTML: 見出し、物件概要、賃料例、電話CTAを含む
- LCP候補: `assets/exterior.png`。初回HTMLで取得し、lazy-loadなし。fetchpriority=high。
- 下部画像: `assets/room.jpg` と `assets/floor-plan.png`。loading=lazy、表示寸法を指定。
- JavaScript、外部フォント、動画、WebGL、外部解析タグ: 使用なし
- CTA: `tel:09037500041`。スマートフォン幅では画面下に固定表示。
- 動作軽減設定: スムーススクロールとCSS遷移を抑制。本文・電話CTAは初期HTMLから利用可能。
- 元画像サイズ: 外観 2,612,050 bytes、洋室 332,683 bytes、間取り 50,827 bytes。変換せず利用。
- LCP・CLS・転送量・応答ヘッダー: 未計測。性能達成は未確認。
