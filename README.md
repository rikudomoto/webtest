# テーブル設計

## Helper_users テーブル

| Column             | Type    | Options     |
| ------------------ | ------- | ----------- |
| name               | string  | null: false |
| email              | string  | null: false |
| password           | string  | null: false |
| area               | integer |             |
| position           | string  |             |
| Experience_history | integer |             |
| appeal             | string  |             |

### Association
-
-
-

## operator_users テーブル

| Column            | Type   | Options     |
| ----------------- | ------ | ----------- |
| Team_name         | string | null: false |
| email             | string | null: false |
| password          | string | null: false |
| area              | string |             |
| Team_introduction | string |             |

### Association
-
-
-

## Postテーブル

| Column | Type | Options |
| ------ | ---- | ------- |
|        |      |         |