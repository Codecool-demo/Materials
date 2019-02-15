# Lists

Lists are kind of containers for storing other variables. They can even store other collections inside! 

Lists - it's a collection that is changeable (you can add, remove or edit their elements) and it keeps order of elements. It also allows duplicate members.
```python 
	my_list = [2, 4, 3.14, 'dog']
```
As you can see there may be different types of variables in a single list. 

Each element has an index - it's position inside a given list. Indexes are integers and they start at 0. So, element 2 is at 0 index, element 4 is at 1 index, 3.14 is 2 and 'dog' is 3.  

   
You can access an element by it's index. To do so we use the name of a list and then we put an index number in square brackets '[]'.  Let's say, we want to print 4th element  - 'dog'. Its index is 3, so:
```python
print(my_list[3])   # displays 'dog' on screen  
```

To display every element on a given list we can use a loop. Loops are described in details in [here](demo/105-loops.md)

While loop:
```python
	i = 0
	while i < len(my_list):
		print(my_list[i])
```
For loop, iterating through elements:
```python
	for element in my_list:
		print(element)
```
For loop, using indexes:
```python
	for index in range(len(my_list)):
			print(my_list[index])
```

Lists are editable, so we can add new elements to them. 
It can be done by adding new element at the end of our list, i.e.:
```python
my_list = [2, 4, 3.14, 'dog']
new_element = “burger”
my_list.append(new_element)
print(my_list)   # displays [2, 4, 3.14, 'dog', 'burger']
my_list.append(111)
print(my_list)   # displays  [2, 4, 3.14, 'dog', 'burger', 111]
```
We can also insert a new element at given index, which results in moving some existing elements further down that list. So if there is already an element on a given index it will be moved one index further, 
```python
my_list = [2, 4, 3.14, 'dog']
new_element = 'water'
my_list.insert(2, new_element)   # first param is an index, second - new elem.
print(my_list) # displays  [2, 4, 'water', 3.14, 'dog']
```
As you can see, the new element 'water' has been inserted on index 2, which moved element 3.14 from position 2 to 3 and element 'dog' from position 3 to 4.

If you'll try to insert the new element in a position that doesn't exist, like index 10 in an example below, Python will add that element at the end of our list:
```python 
my_list = [2, 4, 3.14, 'dog']
new_element = 'tea'
my_list.insert(10, new_element)   # our list has only 4 indexes, but...
print(my_list) # displays  [2, 4, 3.14, 'dog', 'tea']
```

Next, we can change element at given index. New element can be of different type than the former one. Let's change second element - 4 (second element so it's index is 1):
```python
my_list = [2, 4, 3.14, 'dog']
my_list[1] = 'beer'
print(my_list)   # displays  [2, 'beer', 3.14, 'dog']
```
So, we basically have assigned (using '=' sign) a new value to the element at that index.
 

Finally, we can delete some elements from our list.
Let's delete element 3.14 - it's index is 2, so:  
```python
my_list = [2, 4, 3.14, 'dog']
my_list.pop(2)
print(my_list)    # displays  [2, 4, 'dog']
```
As you can see there is no “hole” in our list as a result of deletion - element at index 3 has been moved to index 2, and the one at index 4 to index 3. Our list is now shorter a bit :)

OK, let's delete something else, this time by telling the value of an element we want to delete. We don't need the 'dog' anymore (poor bastard...), so:
```python
my_list = [2, 4, 3.14, 'dog']
my_list.remove('dog')
print(my_list)    # displays  [2, 4, 3.14]
```
	And the 'dog' is gone…

One last note about deletion by specifying an element's value. The .remove() method will get rid of the first occurrence of a given value. So, if we have more than one element of the same value, only the first will be deleted, i.e.:
```python
my_list = [2, 4, 'dog', 3.14, 'dog']
my_list.remove('dog')
print(my_list)    # displays  [2, 4, 3.14, 'dog'] - only the first dog is no more!
```