# テーブル設計
=============================================================================
## users ユーザ情報テーブル
| Column                   | Type          | Options                        |
| ------------------------ | ------------- | ------------------------------ |
| name                     | string        | null: false                    |
| email                    | string        | null: false, unique: true      |
| encrypted_password       | string        | null: false                    |

## Association
--has_many :comments
=============================================================================
## comments 投稿情報テーブル
| Column                   | Type          | Options                        |
| ------------------------ | ------------- | ------------------------------ |
| comment                  | text          | null: false                    |