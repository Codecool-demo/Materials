## Frequently Used Built-in Functions

**input()** - takes in an input string which will be displayed to a user on the screen. Returns whatever the user enters - it's always a string! (even if the user enters number).
```python
	data_from_user = input('How are you?')
```
More information about int() can be found here -> https://www.w3schools.com/python/ref_func_input.asp



**int()** - convert other data type (i.e. string) into an integer.
```python
	age_as_string = '25'
	age = int(age_as_string)
```
More information about int() can be found here -> https://www.w3schools.com/python/ref_func_int.asp



**len()** - returns information about size/length of an input argument.
```python
	length = len('this is a very long string, who is curious how long it is?')
```
More information about len() can be found here -> https://www.w3schools.com/python/ref_func_len.asp



**print()** - displays an input argument on the screen. The difference between print() and input() is that print() doesn't retrieve any data from the user.
```python
	print('Hello world!')
```
More information about print() can be found here -> https://www.w3schools.com/python/ref_func_print.asp



**range()** - creates a sequence of numbers. In its basic form, when only one argument is used (see example below!) range() create a sequence starting from 0 up to (but not including!) given argument, i.e.:
```python
	for index in range(5):
		print(index)
	# prints:
	# 0
	# 1
	# 2
	# 3
	# 4
```
More information about range() can be found here -> https://www.w3schools.com/python/ref_func_range.asp
 

 
**str()** - convert other data type (i.e. int) into a string, i.e.:

OK, you may wonder why would you convert an integer into a string? Well, a very common situation is when you'd like to display some information in a print() function, you have a mix of strings and integers and want to create a single string using '+' sign, i.e.:
```python
my_age = 25
my_brother_age = 34
print(“I'm “ + str(my_age) + ' and he is ' + str(my_brother_age) + ' years old')
```



**type()** - returns information about a type of argument variable, i.e.:
```python	
	a = ['cat', 'dog', 'eagle']
	b = 23
	c = 'I want to break free!'

	print(type(a))
	print(type(b))
	print(type(c))
```