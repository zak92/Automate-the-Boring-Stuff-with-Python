# Lists
## The List Data Type
A list is a value that contains multiple values in an ordered sequence. The term list value refers to the list itself not the values in the list. A list value looks like this: ['cat', 'bat', 'rat', 'elephant']. Values inside the list are also called items. Items are separated with commas (that is, they are comma-delimited).

## Getting Individual Values in a List with Indexes
Say you have the list ['cat', 'bat', 'rat', 'elephant'] stored in a variable named spam. The Python code spam[0] would evaluate to 'cat', and spam[1] would evaluate to 'bat', and so on.

Lists can also contain other list values. The values in these lists of lists can be accessed using multiple indexes, like so:

![lists in lists]()

## Negative Indexes
While indexes start at 0 and go up, you can also use negative integers for the index. The integer value -1 refers to the last index in a list, the value -2 refers to the second-to-last index in a list, and so on.

![negative index]()

## Getting a List from Another List with Slices
Just as an index can get a single value from a list, a slice can get several values from a list, in the form of a new list. A slice is typed between square brackets, like an index, but it has two integers separated by a colon. 
### Example
spam = ['cat', 'bat', 'rat', 'elephant']

spam[1:3] is a list with a slice 

Output: ['bat', 'rat']

In a slice, the first integer is the index where the slice starts. The second integer is the index where the slice ends. A slice goes up to, but will not include, the value at the second index.

As a shortcut, you can leave out one or both of the indexes on either side of the colon in the slice. Leaving out the first index is the same as using 0, or the beginning of the list. Leaving out the second index is the same as using the length of the list, which will slice to the end of the list.
### Example
spam[:2]

Output: ['cat', 'bat']

## Getting a List’s Length with the len() Function
The len() function will return the number of values that are in a list value passed to it, just like it can count the number of characters in a string value.
### Example
spam = ['cat', 'dog', 'moose']\
len(spam)\
3

## Changing Values in a List with Indexes
You can also use an index of a list to change the value at that index.

### Example
spam = ['cat', 'bat', 'rat', 'elephant']\
spam[1] = 'aardvark'\
spam = ['cat', 'aardvark', 'rat', 'elephant']

## List Concatenation and List Replication
The + operator combines two lists to create a new list value and the * operator can be used with a list and an integer value to replicate the list.

### Examples
[1, 2, 3] + ['A', 'B', 'C']\
[1, 2, 3, 'A', 'B', 'C']

['X', 'Y', 'Z'] * 3\
['X', 'Y', 'Z', 'X', 'Y', 'Z', 'X', 'Y', 'Z']

## Removing Values from Lists with del Statements
The del statement will delete values at an index in a list. All of the values in the list after the deleted value will be moved up one index.

### Example
spam = ['cat', 'bat', 'rat', 'elephant']\
del spam[2]\
spam = ['cat', 'bat', 'elephant']

## Using for Loops with Lists
A common Python technique is to use range(len(someList)) with a for loop to iterate over the indexes of a list.\
## Example 
supplies = ['pens', 'staplers', 'flamethrowers', 'binders']\
for i in range(len(supplies)):\
    print('Index ' + str(i) + ' in supplies is: ' + supplies[i])

Output:\
Index 0 in supplies is: pens\
Index 1 in supplies is: staplers\
Index 2 in supplies is: flamethrowers\
Index 3 in supplies is: binders\

## The in and not in Operators
![in not in]()

## The Multiple Assignment Trick
The multiple assignment trick (technically called tuple unpacking) is a shortcut that lets you assign multiple variables with the values in a list in one line of code. So instead of doing this:

![multiple assignment]()

## Using the enumerate() Function with Lists




