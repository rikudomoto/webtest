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

## Post テーブル

| Column         | Type    | Options     |
| -------------- | ------- | ----------- |
| Match_date     | integer | null: false |
| position       | string  | null: false |
| Position_years | string  | null: false |
| word           | string  | null: false |

### Association

-
-
-

### rooms テーブル

| Column | Type   | Options     |
| ------ | ------ | ----------- |
| name   | string | null: false |

### Association

-
-
-

## room_users テーブル

| Column | Type       | Options                        |
| ------ | ---------- | ------------------------------ |
| user   | references | null: false, foreign_key: true |
| room   | references | null: false, foreign_key: true |

### Association

-
-
-

## messages テーブル

| Column  | Type       | Options                        |
| ------- | ---------- | ------------------------------ |
| content | string     |                                |
| user    | references | null: false, foreign_key: true |
| room    | references | null: false, foreign_key: true |

### Association

-
-
-