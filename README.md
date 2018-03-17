## members tabble

|Column|Type|Options|
|------|----|-------|
|user_id|integer|null:false, foreign_key: true|
|group_id|integer|null: false, foreign_key: true|

### Asociation
- belongs_to :group
- belongs_to :user

