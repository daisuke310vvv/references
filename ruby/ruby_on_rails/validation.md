## Model validation references

##バリデーション一覧

|バリデーション名|内容|
|:---------------|--------------------------:|
|validates_associated|関連先のレコードがvalidであること|
|confirmation|emailなどのように、確認フィールドと内容が一致すること|
|exclusion|ある値でないこと|
|format|あるフォーマットを満たすこと|
|inclusion|ある値のうちに含まれること|
|length|ある長さを満たすこと|
|numericality|数値であること、オプションでゼロ以上、偶数かなどを検査|
|presence|存在すること|
|absence|存在しないこと|
|uniqueness|値が一意であること。scopeオプションで一意性の範囲を指定|

##独自でバリデーションする場合
  
```ruby
class Book < ActiveRecord::Base
  validate do |book|
    #do something
  end
```
