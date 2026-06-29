# MVP 仕様

## スコープ

MVP は次の 5 つに絞ります。

- Bucket 管理
- Project 管理
- Todo 管理
- Focus モード
- ローカル保存

## 画面構成

```text
Splash
  ↓
Home
├── Focus
├── Todo 一覧
│   └── Todo 詳細
└── Bucket 一覧
    └── Bucket 詳細
        └── Project 詳細
```

Bottom Navigation:
- Home
- Todo
- Bucket

## 作成フロー

Todo 追加:

```text
+ ボタン
  ↓
タイトル
  ↓
詳細（任意）
  ↓
期限（任意）
  ↓
Project 選択（任意）
  ↓
保存
```

Project 未設定でも Todo は保存できます。

## Home

- 今日やることを表示
- Focus を開始できる
- Bucket の進捗を表示
- 最近完了した Todo を表示

## Todo 一覧

フィルター:
- 今日
- 今週
- 期限なし
- 完了済み
- Project 別
- タグ

## Bucket 詳細

- Bucket の説明、期限、進捗を表示
- 紐づく Project を表示
- 関連 Todo を表示
- Project 作成へ遷移できる

