# スキーマ概要

## リレーション

```text
Bucket
  ↓
Project
  ↓
Todo
```

Todo は Project なしでも作成できます。Project は Bucket なしでも作成できます。

## Bucket

```text
id
title
description
deadline
status
createdAt
updatedAt
```

## Project

```text
id
bucketId nullable
title
description
deadline
status
createdAt
updatedAt
```

## Todo

```text
id
projectId nullable
title
description
priority
deadline
completed
createdAt
updatedAt
```

## Deadline

```text
value
precision
```

Precision:

```text
none
year
month
day
datetime
```

表示例:

| 保存値 | 表示 |
| --- | --- |
| `2030` | 2030年まで |
| `2028-06` | 2028年6月まで |
| `2026-07-03` | 7/3まで |
| `2026-07-03 18:00` | 7/3 18:00まで |

