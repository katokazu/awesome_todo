# AGENTS.md

このリポジトリは、Bucket List から Project、Todo、Focus へ落とし込むローカルファーストな Todo アプリです。

## 原則

- 基本的にドキュメントは日本語をベースとして作成すること。プログラミングに使うものや固有名詞などは英語で構わない。
- 文字エンコーディングはUTF-8を基本とすること。

## 最初に読むもの

作業前に、タスクに関係するドキュメントだけを辿ってください。

1. `docs/INDEX.md`
2. 関係するカテゴリの `docs/<category>/INDEX.md`
3. 必要な個別ドキュメント

巨大なコンテキストを一度に読み込まず、3ホップ以内で必要情報へ到達する構成を前提にします。

## プロダクトの軸

- コンセプトは「未来の目的と、今日の行動をつなぐ。」
- 最重要体験は Focus です。
- 判断に迷ったら「この機能は、ユーザーが今日の一歩を踏み出す助けになるか？」を基準にします。
- Todo は Bucket / Project と関連付けられるが、単独でも成立します。

## 技術方針

- Framework: Expo + React Native + TypeScript
- Navigation: Expo Router
- State: Zustand
- Local DB: SQLite (`expo-sqlite`) + Drizzle ORM
- Validation: Zod
- Date: dayjs
- UI: NativeWind + React Native Reusables
- Icons: Lucide React Native
- Notification: Expo Notifications
- Testing: Vitest + React Native Testing Library

## 作業ルール

- 既存の設計判断は `docs/adr/` を確認してから変更します。
- ドメイン用語や関係性は `docs/domain/` と `docs/domain-models/` を優先します。
- 機能要件は `docs/specs/` を更新してから実装します。
- DB スキーマ変更時は `docs/database/` とマイグレーション方針を揃えます。
- 実装パターンや規約に迷ったら `docs/patterns/` と `docs/standards/` を確認します。
- ドキュメントを更新したら、関連する `INDEX.md` も更新します。

