# Link Extractor

Webページからリンクを素早く抽出するツールです。

## 特徴

- **実際のWebページ対応**: CORS プロキシ経由でHTML取得
- **高度な解析機能**: 相対URL→絶対URL変換、リンクタイプ自動判定
- **位置情報フィルタリング**: ヘッダー・フッター・ナビゲーション等でリンクを分類・絞り込み
- **抽出設定**: 重複除去、件数制限の柔軟な設定
- **CSV出力**: BOM付きUTF-8でExcel対応
- **エラーハンドリング**: 日本語エラーメッセージ
- **レスポンシブデザイン**: モバイル対応
- **画像リンク対応**: alt属性・title属性からテキスト取得

## 使用方法

1. URLを入力（https://example.com）
2. 必要に応じて抽出設定を調整
3. 「リンクを抽出」ボタンをクリック
4. 結果をテーブルで確認
5. 位置フィルターで絞り込み
6. 必要に応じてCSV出力

## 抽出設定

- **重複除去**: 同じURLを1件のみ表示
- **件数制限**: 25～500件の範囲で制限設定
- **位置フィルタ**: ヘッダー、フッター、ナビゲーション等でフィルタリング

## 位置情報機能

リンクが配置されている場所を自動判定し、日本語で分類表示：

- ヘッダー / フッター
- ナビゲーション / メニュー
- メインコンテンツ / サイドバー
- テーブル内 / リスト内 / フォーム内
- その他の構造的位置

## 対応サイト例

- Wikipedia
- Google
- Example.com
- その他多数のWebサイト

## 技術スタック

- React 18 + TypeScript
- Vite
- GitHub Pages
- AllOrigins CORS プロキシ

## 機能一覧

- [x] URL入力・解析
- [x] リンクタイプ判定（external/internal/email/document/image/phone/anchor）
- [x] 位置情報自動判定・フィルタリング
- [x] 重複除去・件数制限設定
- [x] CSV出力機能
- [x] エラーハンドリング
- [x] レスポンシブデザイン
- [x] 画像リンクテキスト改善
- [x] 統計情報表示

## リンク

- [Live Demo](https://sakai-kai.github.io/link-extractor/)
- [Source Code](https://github.com/sakai-kai/link-extractor)

---

Made with React + TypeScript + Vite
