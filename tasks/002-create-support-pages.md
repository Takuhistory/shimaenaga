# 002: 補助ページ静的プロトタイプ作成

## 目的

stay側の予約前不安を減らす共通ページと、company側の信頼形成・問い合わせ導線を補強するページを追加する。

## 作成ページ

### stay側

- [x] `prototype/stay/faq/index.html`
  - 予約
  - チェックイン
  - 設備
  - キャンセル
  - アクセス
  - Beds24空室検索仮UI

- [x] `prototype/stay/access/index.html`
  - ニセコ・札幌のアクセス概要
  - 空港、駅、車、公共交通の掲載方針
  - 地図埋め込み予定エリア
  - Beds24空室検索仮UI

### company側

- [x] `prototype/company/company/index.html`
  - 会社概要
  - 事業方針
  - 事業内容
  - 会社情報
  - 信頼材料

- [x] `prototype/company/contact/index.html`
  - 問い合わせ専用ページ
  - フォーム仮UI
  - 相談前に分かるとよい情報
  - サービス詳細への導線

## 実装方針

- 予約機能は作らず、Beds24設置領域のみを置く
- 送信処理は作らず、フォーム仮UIのみを置く
- WordPress/SWELL化しやすいように、各セクションへ`data-wp-section`を付ける
- stay側とcompany側のCTAを混ぜない

## 次のタスク

- [ ] ルートのブランド分岐トップを、新しい`prototype`構成に合わせて再整理する
- [ ] GitHub Pages公開用に`prototype`を公開対象へ接続する
- [ ] Beds24の実URL・埋め込みコード仕様を反映する
- [ ] 画像提供後に写真差し替えとalt文の最終調整を行う
