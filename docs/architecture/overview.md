# アーキテクチャ概要

## 方針

iOS / Android 両対応、UI 開発速度、個人開発の DX を重視し、Expo + React Native を採用します。将来的な Web 対応も視野に入れます。

## 技術スタック

| 領域 | 採用 |
| --- | --- |
| Framework | Expo, React Native, TypeScript |
| Navigation | Expo Router |
| State | Zustand |
| Local Database | SQLite (`expo-sqlite`) |
| ORM | Drizzle ORM |
| Validation | Zod |
| Date | dayjs |
| UI | NativeWind, React Native Reusables |
| Icons | Lucide React Native |
| Notification | Expo Notifications |
| Storage | Expo Secure Store, AsyncStorage |
| Testing | Vitest, React Native Testing Library |

## レイヤー

```text
UI / Screens
  ↓
Application State / Hooks
  ↓
Domain Models / Use Cases
  ↓
Repository / Database Layer
  ↓
SQLite
```

## データ方針

最初はローカルファーストで構築します。クラウド同期、ログイン、Web 対応は Phase 3 以降の拡張として扱います。

