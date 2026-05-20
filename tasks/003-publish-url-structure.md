# 003: GitHub Pages向けURL構造へ反映

## 目的

`prototype/`配下で確認していた静的プロトタイプを、GitHub Pagesで共有しやすい公開用URLへ反映する。

## 実装済み

- [x] ルートトップを表示せず、`/stay/`へリダイレクトする構成へ更新
- [x] `stay/`配下を最新の宿泊者向けプロトタイプへ更新
- [x] `stay/niseko/`を最新の施設詳細プロトタイプへ更新
- [x] `stay/sapporo/`を最新の施設詳細プロトタイプへ更新
- [x] `stay/faq/`を公開用URLへ追加
- [x] `stay/access/`を公開用URLへ追加
- [x] `company/`配下を民泊相談トップとして追加
- [x] `company/management/`を追加
- [x] `company/startup-support/`を追加
- [x] `company/beds24-ota/`を追加
- [x] `company/company/`を追加
- [x] `company/contact/`を追加
- [x] 旧`owners/`を`company/`への案内ページに変更
- [x] 共通CSSを公開用`styles.css`へ反映

## URL方針

- `/` はトップページとして使わず、`/stay/`へリダイレクト
- `/stay/` は宿泊者向けトップ
- `/company/` は物件オーナー向け民泊相談トップ
- `/owners/` は旧URL互換として `/company/` へ誘導

## 次のタスク

- [x] GitHub Pagesへ公開するためにコミット・pushする
- [x] 公開URLで主要リンクを確認する
- [ ] Beds24の実URL・埋め込みコードが決まり次第、仮UIを差し替える
- [ ] Airbnb掲載写真を優先して施設写真を差し替える
- [ ] 姉から受け取る実写真がAirbnb掲載写真より適切な場合は、用途別に差し替える
