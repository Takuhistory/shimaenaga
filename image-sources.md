# 施設写真ソースメモ

シマエナガニセコ、シマエナガ札幌の施設ページで使う写真の取得元と、差し替え運用のメモ。

## 配置先

- ニセコ：`assets/facilities/niseko/airbnb/gallery-01.jpg` から `gallery-06.jpg`
- 札幌：`assets/facilities/sapporo/airbnb/gallery-01.jpg` から `gallery-06.jpg`

施設ページはこのファイル名を参照しているため、正式写真を受け取ったら同じファイル名で置き換えるだけで反映できる。旧来の仮写真は比較・退避用として `assets/facilities/{niseko|sapporo}/gallery-01.jpg` から `gallery-06.jpg` に残す。

## 取得元

### シマエナガニセコ

- Airbnb 掲載写真を優先使用
- `https://www.airbnb.jp/rooms/1323051985756787596`
- `https://www.airbnb.jp/rooms/1573871746227407424`
- 2026-05-20時点で、上記2ページから取得できる施設写真を `airbnb/` 配下に保存

### シマエナガ札幌

- Airbnb 掲載写真を優先使用
- `https://www.airbnb.jp/rooms/1382461147484335396`
- 2026-05-20時点で、上記ページから取得できる施設写真を `airbnb/` 配下に保存

## 運用メモ

- Airbnb画像は公開ページの直リンクをHTMLに埋め込まず、ローカルの `assets/` に保存して参照する
- 施設運営者から元写真を受け取ったら、同じファイル名で上書きするか、WordPressメディアライブラリへアップロードして差し替える
- 画像の権利確認は、運営者提供写真として扱う前提で進める

## WordPress実装時の扱い

- 最終実装ではWordPressメディアライブラリへアップロードし、各施設ページのギャラリーとして管理する
- 画像の順序は、1枚目を施設ページのメインビジュアル、2枚目以降をギャラリーに使う
- ファイル名は施設名と用途が分かる命名に変更してよい
- 例：`niseko-private-room-01.jpg`, `sapporo-living-01.jpg`
- 画像の代替テキストは「施設名 + 写っている場所」で設定する
