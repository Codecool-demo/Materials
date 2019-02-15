# Script Examples


S1. Write a script that asks a user about their name and greets them ("Hello <entered_name>!") If the user doesn't enter their name program should print "Hello stranger!"

A1. OK, we should split our program into two sections. First, we need to ask a user about their name and store that information in a variable. Next, we need to display some text based on that variable's value.

To ask the user we can use built-in function input(). That function displays on the screen message that is between brackets and returns whatever the user enters. That data will be stored in a variable called name.
```python
name = input('What is your name?')
```
So far, so good :)
 
Now, we need to check if the user entered their name or just pressed [ENTER] and acted as an anonymous user. To do so we can use 'if-else' conditional statement and check if the value of the variable name is equal to an empty string. If so, we will greet that user as a stranger. Otherwise, we'll say hello and add the user's name. A built-in print() function will be used to display our greeting on screen.
```python
if name == '':
print('Hello stranger!')
else:
print('Hello ' + name + '!')
```

Our full script can be found below:
```python
name = input('What is your name?')
if name == '':
print('Hello stranger!')
else:
print('Hello ' + name + '!')
```


S2. Write a script that will ask a user about the food they love. The script should store that information into a list. Only unique answers should be stored. The user should be asked several times unless they enter 'quit' as an answer. In such situation script should write all entered information, one food after another, line after line.

A2. Again, we should start with splitting our script into smaller parts. First, we need to ask the user several times about food. We don't know how many times they will provide us with food answer, so 'while' loop is the best candidate here.

Let's create two variables: list_of_food to store our food - as an empty list - and keep_asking that will control our 'while' loop - we assign starting value of True (because we want that loop to be executed at least once) to keep_asking variable.
```python
list_of_food = []
keep_asking = True
```
Next, we create a while loop that will check if the value of keep_asking variable is still True and our script should ask the user a question. If yes, we'll ask a question using built-in input() function and store an answer into a food variable. Then, we check the value of the food variable - if it's equal to 'quit' we will assign a False value to keep_asking variable. If it's not equal to 'quit' we'll check if that value is not on our list already and then add the food variable to list_of_food list.  
```python
while keep_asking == True:
	food = input('Please enter food you like: ')
	if food == 'quit':
		keep_asking = False
	else:
		if food not in list_of_food:
			list_of_food.append(food)
```
Great :) Now, we'll be asking the user as long as they won't enter 'quit'. When it happens we need to display all food names from our list_of_food. We'd like to print every food, so for loop is perfect here!

So, first we display on the screen information for the user that they'll see their favourite food:
```python
	print('Your favourite food: ')
```
And for loop:
```python
for food in list_of_food:
	print(food)
```
That's it, easy-peasy! :)
Our scripts looks like:

```python  
list_of_food = []
keep_asking = True

while keep_asking == True:
	food = input('Please enter food you like: ')
	if food == 'quit':
		keep_asking = False
	else:
		list_of_food.append(food)


print('Your favourite food: ')
for food in list_of_food:
	print(food)
```