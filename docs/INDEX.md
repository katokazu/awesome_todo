# ドキュメントマップ

タスクに関連するディレクトリの `INDEX.md` を最初に読み、必要なファイルのみ参照してください。

| ディレクトリ | 内容 | いつ参照するか |
| --- | --- | --- |
| `architecture/` | システム全体設計、画面構成、技術構成 | 新機能設計、構成理解時 |
| `adr/` | アーキテクチャ意思決定記録 | 設計判断の背景を知りたい時 |
| `api/` | API 仕様、外部連携、将来同期の境界 | API や同期設計時 |
| `database/` | スキーマ設計、ローカル DB、マイグレーション方針 | DB 操作時 |
| `domain/` | プロダクト概要、用語、ビジネスルール | 仕様理解、要件整理時 |
| `domain-models/` | ドメインモデルの振る舞い・制約 | モデル実装・修正時 |
| `patterns/` | 実装パターン、設計方針 | コード実装時 |
| `specs/` | 機能単位の要件・設計 | 機能追加・修正時 |
| `testing/` | テスト戦略、テスト観点 | テスト追加・修正時 |
| `standards/` | コーディング規約、Git 運用、ドキュメント運用 | コード記述時全般 |

## 主要ドキュメント

- `docs/domain/product-overview.md`: アプリのコンセプト、価値、ロードマップ
- `docs/specs/mvp.md`: MVP のスコープと主要画面
- `docs/architecture/overview.md`: Expo / React Native 前提の全体構成
- `docs/database/schema.md`: Bucket / Project / Todo / Deadline のモデル
- `docs/domain-models/core-models.md`: コアモデルの責務と制約

