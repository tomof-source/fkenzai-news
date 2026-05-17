# Fkenzai Staff Notes — 社内通信リポジトリ

フクシマ建材の会議・社内コミュニケーションを、議事録の一段上のフォーマットで残すための静的サイト。GitHub Pagesで配信される。

## 用途
- 議事録を、社内・パートナーが「読み物」として消化できる形に整える
- 検索エンジン除外（`noindex, nofollow`）で、URLを知っている関係者だけが閲覧できる
- 修正・削除のご要望は、フクシマ建材 AI秘書経由で対応

## フォルダ構成
```
fkenzai-news/
├── index.html                ← トップページ（記事一覧）
├── about/index.html          ← このサイトについて（後日整備）
├── marketing/                ← 広報・マーケティング定例
│   └── 2026-04-12/index.html
├── staff-meeting/            ← スタッフ会議（未着手）
├── exec/                     ← 経営会議（未着手）
├── consulting/               ← コンサル会議（未着手）
├── .nojekyll                 ← GitHub Pages の Jekyll を無効化
└── README.md
```

カテゴリは必要に応じて追加。URLは `カテゴリ/YYYY-MM-DD/` で統一。

## 作り方
1. 会議の議事録（`04_出力/048_議事録/`）を素材として用意
2. AI秘書スキル `/議事録報告書HTML` を実行（将来）
3. 生成された `index.html` をローカルでプレビュー
4. 問題なければ `git push` で GitHub Pages に反映

## 配信
- ホスティング：GitHub Pages
- 公開URL：`https://<アカウント名>.github.io/fkenzai-news/`
- 検索エンジン除外：各HTMLに `<meta name="robots" content="noindex, nofollow">`

## デザイン
- ベース色：墨色 `#1F1B16` × テラコッタ `#C46330`
- 紙質背景：`#FAF6EE`
- フォント：Noto Serif JP（見出し）／ Noto Sans JP（本文）／ Cormorant Garamond（英字装飾）
- 1記事 = 1フォルダ + `index.html`（必要に応じて `photos/` を同梱）

## 参考にしたサンプル
- マネゼミ講師会通信：https://izumicoinzoom-hash.github.io/manasemi/koshikai-news/1-5/
- 作り方ガイド：https://izumicoinzoom-hash.github.io/manasemi/koshikai-news/about-making/
