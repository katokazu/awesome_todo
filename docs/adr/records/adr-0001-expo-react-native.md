# ADR 0001: Expo + React Native を採用する

## ステータス

Accepted

## 背景

iOS / Android 両対応、UI 開発速度、個人開発での DX、将来的な Web 対応を重視します。

## 決定

Framework は Expo + React Native + TypeScript を採用します。

## 結果

- Expo Router を前提に画面を構成します。
- ネイティブ API を深く触る必要が出た場合は、追加の ADR で再検討します。

