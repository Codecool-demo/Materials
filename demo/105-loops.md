# Loops

Loops are used to perform the same block of code given amount of times. Thanks to that we don't need to repeat very similar parts of the code.
In Python, there are two types of loops - for loop and while loop 

Let's say we've got a list (my_list = ['cat', 'dog', 'bird', 'elephant']) and we want to display every element of that list on the screen, one after another.


### For loop, 'iterate through elements' approach:
```python
for <inner_variable> in <sequence>:
	<statement(s)>
```
Example:
```python
for element in my_list:
	print(element)
```
Everything in the above code looks super easy and nice, print() built-in function will print every element, but... What is the element variable? We didn't initialize it!
Well, we didn't, did we? Python did it for us. 
It's working like this:
Python checks what variable is between 'in' keyword and a colon (in our case - my_list)
Based on 1) Python will assign first component from my_list to element variable and execute <statement(s)> code
Next, Python will assign the second component from my_list to element variable and execute <statement(s)> code again.
This will be repeated as many times as there are components in my_list     


### While loop:
```python
while <expression>:
		<statement(s)>
```
Example:
```python
	index = 0
	while index < len(my_list):
		print(my_list[index])
		index = index + 1
```
OK, while loop looks more complicated than for loop, but don't worry! I'll explain everything :)

First, we need to create a variable outside while loop - in this case, index, that will hold indexes of elements from my_list. In beginning, I'm assigning a zero value to it because I'd like to start from first element. 

Next, Python will check if <expression> returns True. If so, it will execute <statement(s)> code. Otherwise no <statement(s)> will be executed.

The len() built-in function returns the information about how many elements there are in my_list collection. In our case there are four elements, zero is lesser than four, so the <statement(s)> block will be executed. In it, I'm accessing an element by its index and print that element (first line) and incrementing the index variable (second line). 

Why am I incrementing that variable? Because having executed all code in <statement(s)> block Python will get back to <expression> and check if while loop should be executed one more time. The second time index variable will be equal to one, so <expression> will still return True.
