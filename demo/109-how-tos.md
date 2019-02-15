# How to's

**Q: How can I display only odd/even numbers?**

A: You can use modulo operator - '%' - which returns the remainder of given division. Even numbers are divided by 2 without a remainder, and odd numbers are not ;) Example:
```python
number = 6
if number % 2 == 0:
print('{} is even'.format(number))
```

**Q: How can I check if a list contains (or doesn't contain) the given element?**

A: You can use 'in' (or 'not in') keyword(s), i.e.
```python
	first_element = 5
	second_element = 10
	my_list = [3, 5, 7, 11]

	If first_element in my_list:
		# do something

	If second_element not in my_list:
		# do something else
```

**Q: How can I check what type is given variable?**

A: Python has a built-in function type() that reveals information about the given variable. Usage:
```python
message = 'My secret message'
print(type(message))
```

**Q. How can I check the size of a list? Or length of a string?**

A. Python has a built-in function len() returns information about length/number of elements. Usage:
```python
my_list = [1, 56, 9, 12]
my_list_length = len(my_list)
print(my_list_length)

my_string = 'bicycle'
my_lstring_length = len(my_string)
print(my_string_length) 
```