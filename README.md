##usersテーブル

|  Column   |  Type       | Options       |
|-----------|-------------|---------------|
|   email   |  string     | NOT  NULL     |
| password  |  string     | NOT  NULL     |
|   name    |  string     | NOT  NULL     |
|  profile  |  text       | NOT  NULL     |
| occupation|  text       | NOT  NULL     |
| position  |  text       | NOT  NULL     |

##prototypesテーブル

|  Column   |  Type       | Options       |
|-----------|-------------|---------------|
|   title   |  string     | NOT  NULL     |
|catch_copy |  text       | NOT  NULL     |
| concept   |  text       | NOT  NULL     |
|  image    |ActiveStorage|               |
|  user     | references  |               |
| position  |  text       |               |


##commentsテーブル

|  Column   |  Type       | Options       |
|-----------|-------------|---------------|
|  text     |  text       | NOT  NULL     |
|  user     | references  |               |
| prototype | references  |               |

