# 施設写真ソースメモ

シマエナガニセコ、シマエナガ札幌の施設ページで使う写真の取得元と、差し替え運用のメモ。

## 配置先

- ニセコ：`assets/facilities/niseko/gallery-01.jpg` から `gallery-06.jpg`
- 札幌：`assets/facilities/sapporo/gallery-01.jpg` から `gallery-06.jpg`

施設ページはこのファイル名を参照しているため、正式写真を受け取ったら同じファイル名で置き換えるだけで反映できる。

## 取得元

### シマエナガニセコ

- 楽天トラベル 写真・動画ページ
- `https://travel.rakuten.co.jp/HOTEL/194445/gallery.html`

### シマエナガ札幌

- STAY JAPAN 掲載ページ
- `https://stayjapan.com/area/hokkaido/sapporo/pr/14753`

## WordPress実装時の扱い

- 最終実装ではWordPressメディアライブラリへアップロードし、各施設ページのギャラリーとして管理する
- 画像の順序は、1枚目を施設ページのメインビジュアル、2枚目以降をギャラリーに使う
- ファイル名は施設名と用途が分かる命名に変更してよい
- 例：`niseko-private-room-01.jpg`, `sapporo-living-01.jpg`
- 画像の代替テキストは「施設名 + 写っている場所」で設定する

