# コーディング規約

## TypeScript

- 型は domain / database / UI の責務に合わせて分けます。
- `any` は避け、外部入力は Zod で検証します。
- nullable な関連は型で表現します。

## React Native

- 画面は Expo Router のルーティングに沿って配置します。
- UI は NativeWind と React Native Reusables を基本にします。
- アイコンは Lucide React Native を優先します。

## ドキュメント

- 新しいカテゴリを追加したら `docs/INDEX.md` を更新します。
- カテゴリ内にファイルを追加したら、そのカテゴリの `INDEX.md` を更新します。
- 設計判断が後から参照される場合は ADR を追加します。

