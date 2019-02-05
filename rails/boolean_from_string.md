# To Convert a String to a Boolean Value

To convert a string to a boolean value ...

```
[5] pry(main)> ActiveModel::Type::Boolean.new.cast("FALSE")
=> false
[6] pry(main)> ActiveModel::Type::Boolean.new.cast("False")
=> true
[8] pry(main)> ActiveModel::Type::Boolean.new.cast("False".downcase)
=> false
```

So ... since `False` retuns `true` (why?) you'll probably want to do a
downcase on the string as shown in the last example to get what you *really* want.

Only false values are checked and they are defined as ...

```
FALSE_VALUES = [false, 0, "0", "f", "F", "false", "FALSE", "off", "OFF"]
```
