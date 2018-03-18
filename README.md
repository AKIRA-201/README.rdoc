## members table

|Column|Type|Options|
|------|----|-------|
|member_id|integer|null:false, foreign_key: true|
|member_name|text|null:false, foreign_key:true|

|message|text|null: false, foreign_key: true|
|image|string|null :false, foregin_key: true|

### Association
- has_nany :group
- belongs_to :user

##group table
|Column|Type|Options|
|------|----|-------|
|group_id|integer|null: false, foreign_key: true|
|group_name|type|null:false, foreign_key: true|


### Association
- belongs_to :group
- belongs_to :user

##users table
|Column|Type|Options|
|------|----|-------|
|user_id|integer|null:false, foreign_key: true|
|user_name|text|null:false, foreign_key:true|

### Association
- has_many :group
- belongs_to :menmber
