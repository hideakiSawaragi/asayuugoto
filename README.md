# 朝夕事
## 暮らしに潤いをもたらす女性を輝かせるウェブサイト

### users table
users has many:contact
users has many:workshop
users has many:board references
users has many:proposal
|column|type|
|:--|--:|
|name|string|
|mail|text|
|age|integer|
|gender|string|
|regsidentail area|string|

### contact table
contact belongs_to:users
|column|type|
|:--|--:|
|name|string|
|mail|string|
|mail|text|
|tel|integer|
|getail|text|

### work shop
workshop belongs_to:users
|column|type|
|:--|--:|
|shopname|integer|
|tel|integer|
|mail|text|
|website|text|
|detail|text|
|image|text|

### proposal
proposal belongs_to:workshop
|column|type|
|:--|--:|
|users_id|references|
|term|boolean|
|detail|text|
|credit|text|
|card company|boolean|

### board references
board has many:users
board has many:question

|column|type|
|:--|--:|
|user_id|references|
|gruop_id|references|
|detail|text|

### question
question has many:answer

|column|type|
|:--|--:|
|user_id|integer|
|group_id|references|
|detail|text|

### answer
answer belongs_to:question

|column|type|
|:--|--:|
|user_id|references|
|group_id|references|
|detail|text|

