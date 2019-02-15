# Conditional Expression

Conditional expressions are used to control a program flow based on conditions.

```python
if <expression>:
	<statement(s)>
```
In case <expression> is True Python will execute code in <statement(s)> block. <statement(s)> code must be indented (one Tab or four spaces). 
An example:
```python
if hour < 7:
	print('You should sleep!')
```
Expression body can have more than one condition checked, i.e.
```python
if hour >= 7 or hour <= 23:
	print('You should drink!')
```
You can also specify a block of code that should be executed in case the expression doesn't equal True:
```python
if <expression>:
	<statement(s)>
else:
	<statement(s)>
```
An example:
```python
if dog_is_hungry:
	print('feed him!')
	print('pet him!')
else:
	print('play with him!') 
```

Finally, we can combine many if-s into one, like:
```python
if <expression>:
	<statement(s)>
elif <expression>:
	<statement(s)>
else:
	<statement(s)>
```
An example:
```python
	if name == 'Marcin':
		print('Marcin, it's your coffee')
	elif name == 'Ewa':
		print('Hello Ewa!')
	elif name == 'Adam':
		print('Adam, are you hungry?')
	else:
		print('Hello stranger, nice to see you!')
```
Warning!
Elif is an abbreviation for 'else if'. 
Every if, elif or else must be ended by a colon.
You can put as many elif-s as you need.
Block of code in a next line(s) after if, elif or else must be intended.
