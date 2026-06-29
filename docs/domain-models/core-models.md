# コアモデル

## Bucket

人生でやりたいことや長期目的を表します。

制約:
- title は必須
- Project と Todo の進捗集計対象になる
- deadline は任意

## Project

Bucket と Todo の中間にある計画を表します。

制約:
- title は必須
- bucketId は nullable
- Todo のグルーピングとして使える

## Todo

日々の具体的な行動を表します。

制約:
- title は必須
- projectId は nullable
- 完了状態を持つ
- Project / Bucket と関連がない単独 Todo も許可する

## Deadline

期限の値と粒度をセットで扱います。

制約:
- precision が `none` の場合、value は空を許可する
- value の解釈は precision に従う
- 表示変換は UI 層またはフォーマット用ヘルパーに閉じ込める

