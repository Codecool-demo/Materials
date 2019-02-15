# Common mistakes


* Indentation error

TODO

* Use of addition sign '+' with different variables types.

Python uses '+' sign in a different way based on variables types. For example, it will sum up two integers, merge together two lists or concatenate two strings. But there is a limitation - it only works when both variables are of the same type. Otherwise, you'll see an error like below:
```python
a = 5
b = 'dog'
print(a+b)
TypeError: unsupported operand type(s) for +: 'int' and 'str'
``` 

* My error is not on that list! Halp! :(

Don't worry and stay calm :) In case of an error Python displays on last line the type of that error. Your first steps should be to google that error :)