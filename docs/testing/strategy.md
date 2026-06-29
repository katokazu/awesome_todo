# テスト方針

## 優先対象

- Deadline の precision と表示変換
- Todo の作成、完了、編集、削除
- Project / Bucket の nullable な関連
- Focus で次に表示する Todo の選択
- DB マイグレーション

## ツール

- Vitest
- React Native Testing Library

## 方針

ドメインロジックとフォーマット処理はユニットテストを優先します。画面テストは Home、Todo、Bucket、Focus の主要フローから追加します。

