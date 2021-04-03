# テーブル設計

## users テーブル

|  Column     |  Type   |  options     |
|  ---------  |  ------ |  ----------- |
|  email      |  string |  null: false |
|  password   |  string |  null: false |
|  name       |  string |  null: false |
|  profile    |  text   |  null: false |
|  occupation |  text   |  null: false |
|  position   |  text   |  null: false |


## prototypesテーブル

|  column     |  type        |  options     |
|  ---------  |  ----------  |  ----------- |
|  title      |  string      |  null: false |
|  catch_copy |  text        |  null: false |
|  concept    |  text        |  null: false |
|  image      |              |              |
|  user       |  references  |              |


## commentsテーブル

|  column     |  type        |  options     |
|  ---------  |  ----------  |  ----------- |
|  text       |  text        |  null: false |
|  user       |  references  |              |
|  prototype  |  references  |              |