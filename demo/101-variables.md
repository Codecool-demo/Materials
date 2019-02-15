# Variables

Variables are "boxes", in which we can keep different kinds of data. They should be [proper named](demo/107-clean-code.md).

To assign a value to a variable one can use '=' sign, i.e.

```python
my_variable = 5
```

We can also assign one variable to another (in such situation both variables will have the same value), i.e.:
```python 
my_second_variable = my_variable
```

or perform an arithmetical operation before assigning, i.e.
```python
my_third_variable = (my_variable * 3) - 2
```  
Variables can hold a single value:
  * **Booleans** - for storing True or False
```python
is_available = True
```
  * **Integers** - for storing numbers (i.e. -100, 0, 12, 99)
```python
age = 33
```
  * **Floats** - for storing floating point numbers (i.e. 4.12, 0.123)
```python
result = 3,23
```
  * **Strings** - for string characters (i.e. "I don't want to miss a thing!")
```python
message = "User has been created" 
```