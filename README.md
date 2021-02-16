# テーブル設計

## usersテーブル

| Column             | Type   | Options                   |
| ----------         | ------ | ------------------------- |
| nickname           | string | null: false               |
| email              | string | null: false, unique: true |
| encrypted_password | string | null: false               |

## Association
- has_many :posts


## postテーブル

| Column              | Type       | Options                          |
| ------------------- | ---------- | -------------------------------- |
| athletes            | string     |                                  |
| elements1           | string     |                                  |
| elements2           | string     |                                  |
| elements3           | string     |                                  |
| elements4           | string     |                                  |
| elements5           | string     |                                  |
| elements6           | string     |                                  |
| elements7           | string     |                                  |
| elements8           | string     |                                  |
| elements9           | string     |                                  |
| elements10          | string     |                                  |
| elements11          | string     |                                  |
| elements12          | string     |                                  |
| user                | references | null: false, foreign_key: true   |


## Association

- belongs_to :user