# Run Raw SQL from the Console

```ruby
sql = "select * from p13n_offers" # The raw sql goes here.
result = ActiveRecord::Base.connection.execute(sql)
result[0] # This is an array
```
