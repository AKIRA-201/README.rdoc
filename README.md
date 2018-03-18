## members table

|Column|Type|Options|
|------|----|-------|
|member_id|integer|null:false, foreign_key: true|
|member_name|text|null:false, foreign_key: true|

### Association
- has_nany :group
- belongs_to :user

## groups table

|Column|Type|Options|
|------|----|-------|
|group_id|integer|null: false, foreign_key: true|
|group_name|type|null:false, foreign_key: true|


### Association
- has_many :members through :users

## users table

|Column|Type|Options|
|------|----|-------|
|user_id|integer|null:false, foreign_key: true|
|user_name|text|null:false, foreign_key:true|

### Association
- has_many :messages
- belongs_to :menmber

### messages table
|Column|Type|Options|
|------|----|-------|
|message|text|null:false, foreign_key: true|
|image|string|null :false, foregin_key: true|

### Asscociation
- belongs_to :users

