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
A common Python technique is to use range(len(someList)) with a for loop to iterate over the indexes of a list.
## Example 
supplies = ['pens', 'staplers', 'flamethrowers', 'binders']\
for i in range(len(supplies)):\
    print('Index ' + str(i) + ' in supplies is: ' + supplies[i])

Output:\
Index 0 in supplies is: pens\
Index 1 in supplies is: staplers\
Index 2 in supplies is: flamethrowers\
Index 3 in supplies is: binders

## The in and not in Operators
![in not in]()

## The Multiple Assignment Trick
The multiple assignment trick (technically called tuple unpacking) is a shortcut that lets you assign multiple variables with the values in a list in one line of code. So instead of doing this:

![multiple assignment]()

## Using the enumerate() Function with Lists
Instead of using the range(len(someList)) technique with a for loop to obtain the integer index of the items in the list, you can call the enumerate() function instead. On each iteration of the loop, enumerate() will return two values: the index of the item in the list, and the item in the list itself.

### Example
supplies = ['pens', 'staplers', 'flamethrowers', 'binders']/
for index, item in enumerate(supplies):/
    print('Index ' + str(index) + ' in supplies is: ' + item)/

Index 0 in supplies is: pens/
Index 1 in supplies is: staplers/
Index 2 in supplies is: flamethrowers/
Index 3 in supplies is: binders

## Using the random.choice() and random.shuffle() Functions with Lists
The random module has a couple functions that accept lists for arguments. The random.choice() function will return a randomly selected item from the list.

### Example
import random\
pets = ['Dog', 'Cat', 'Moose']\
random.choice(pets)\
Output: 'Dog'

The random.shuffle() function will reorder the items in a list. This function modifies the list in place, rather than returning a new list.

### Example
import random\
people = ['Alice', 'Bob', 'Carol', 'David']\
random.shuffle(people)\
Output: ['Carol', 'David', 'Alice', 'Bob']

## Augmented Assignment Operators

![Augmented Assignment]()

## Methods
A method is the same thing as a function, except it is “called on” a value. For example, if a list value were stored in spam, you would call the index() list method on that list like so: spam.index('hello').Each data type has its own set of methods. The list data type, for example, has several useful methods for finding, adding, removing, and otherwise manipulating values in a list.

### Finding a Value in a List with the index() Method
List values have an index() method that can be passed a value, and if that value exists in the list, the index of the value is returned. If the value isn’t in the list, then Python produces a ValueError error. 

### Example 
spam = ['hello', 'hi', 'howdy', 'heyas'\/
spam.index('hello')\
Output: 0

When there are duplicates of the value in the list, the index of its first appearance is returned.

### Adding Values to Lists with the append() and insert() Methods
To add new values to a list, use the append() and insert() methods.

### Example
spam = ['cat', 'dog', 'bat']\
spam.append('moose')\
Output: ['cat', 'dog', 'bat', 'moose']

The previous append() method call adds the argument to the end of the list. The insert() method can insert a value at any index in the list. The first argument to insert() is the index for the new value, and the second argument is the new value to be inserted. 

### Example
spam = ['cat', 'dog', 'bat']\
spam.insert(1, 'chicken')\
output: ['cat', 'chicken', 'dog', 'bat']

### Removing Values from Lists with the remove() Method
The remove() method is passed the value to be removed from the list it is called on.

### Example
spam = ['cat', 'bat', 'rat', 'elephant']\
spam.remove('bat')\
Output: ['cat', 'rat', 'elephant']

If the value appears multiple times in the list, only the first instance of the value will be removed./
The del statement is good to use when you know the index of the value you want to remove from the list. The remove() method is useful when you know the value you want to remove from the list.

### Sorting the Values in a List with the sort() Method
Lists of number values or lists of strings can be sorted with the sort() method.

### Example
spam = [2, 5, 3.14, 1, -7]\
spam.sort()\
Output: [-7, 1, 2, 3.14, 5]

spam = ['ants', 'cats', 'dogs', 'badgers', 'elephants']\
spam.sort()\
Output: ['ants', 'badgers', 'cats', 'dogs', 'elephants']

You can also pass True for the reverse keyword argument to have sort() sort the values in reverse order/.
spam.sort(reverse=True)
Output: ['elephants', 'dogs', 'cats', 'badgers', 'ants']

There are three things you should note about the sort() method. First, the sort() method sorts the list in place; don’t try to capture the return value by writing code like spam = spam.sort().\
Second, you cannot sort lists that have both number values and string values in them, since Python doesn’t know how to compare these values.\
Third, sort() uses “ASCIIbetical order” rather than actual alphabetical order for sorting strings. This means uppercase letters come before lowercase letters. Therefore, the lowercase a is sorted so that it comes after the uppercase Z. 

If you need to sort the values in regular alphabetical order, pass str.lower for the key keyword argument in the sort() method call.
### Example
spam = ['a', 'z', 'A', 'Z']\
spam.sort(key=str.lower)\
Output: ['a', 'A', 'z', 'Z']

This causes the sort() function to treat all the items in the list as if they were lowercase without actually changing the values in the list.

### Reversing the Values in a List with the reverse() Method
If you need to quickly reverse the order of the items in a list, you can call the reverse() list method. 
### Example
spam = ['cat', 'dog', 'moose']\
spam.reverse()\
Output: ['moose', 'dog', 'cat']

## Sequence Data Types
The Python sequence data types include lists, strings, range objects returned by range(), and tuples. Many of the things you can do with lists can also be done with strings and other values of sequence types: indexing; slicing; and using them with for loops, with len(), and with the in and not in operators. 

### Examples
name = 'Zophie'\
name[0]\
Output: 'Z'

'Zo' in name\
Output: True

## Mutable and Immutable Data Types
A list value is a mutable data type: it can have values added, removed, or changed. However, a string is immutable: it cannot be changed.The proper way to “mutate” a string is to use slicing and concatenation to build a new string by copying from parts of the old string. Tuples are immutable.

## The Tuple Data Type
The tuple data type is almost identical to the list data type, except in two ways. First, tuples are typed with parentheses, (), instead of square brackets, []. But the main way that tuples are different from lists is that tuples, like strings, are immutable. Tuples cannot have their values modified, appended, or removed. 

### Example 
eggs = ('hello', 42, 0.5)\
eggs[0]\
Output: 'hello'

If you have only one value in your tuple, you can indicate this by placing a trailing comma after the value inside the parentheses. Otherwise, Python will think you’ve just typed a value inside regular parentheses. The comma is what lets Python know this is a tuple value. 

### Example 
type(('hello',))\
<class 'tuple'>

type(('hello'))\
<class 'str'>

You can use tuples to convey to anyone reading your code that you don’t intend for that sequence of values to change. If you need an ordered sequence of values that never changes, use a tuple.\
A second benefit of using tuples instead of lists is that, because they are immutable and their contents don’t change, Python can implement some optimizations that make code using tuples slightly faster than code using lists.

## Converting Types with the list() and tuple() Functions
The functions list() and tuple() will return list and tuple versions of the values passed to them.

![tuple-list]()

## Identity and the id() Function
All values in Python have a unique identity that can be obtained with the id() function. 

## Example 
id('Howdy') #The returned number will be different on your machine.\
Output: 44491136

When Python runs id('Howdy'), it creates the 'Howdy' string in the computer’s memory. The numeric memory address where the string is stored is returned by the id() function. Python picks this address based on which memory bytes happen to be free on your computer at the time, so it’ll be different each time you run this code.\
Like all strings, 'Howdy' is immutable and cannot be changed. If you “change” the string in a variable, a new string object is being made at a different place in memory, and the variable refers to this new string.

### Example
bacon = 'Hello'\
id(bacon)\
44491136\
bacon += ' world!' # A new string is made from 'Hello' and ' world!'.\
id(bacon) # bacon now refers to a completely different string.\
44609712

However, lists can be modified because they are mutable objects. The append() method doesn’t create a new list object; it changes the existing list object. We call this “modifying the object in-place.”

### Example
![id]()

If two variables refer to the same list and the list value itself changes, both variables are affected because they both refer to the same list. The append(), extend(), remove(), sort(), reverse(), and other list methods modify their lists in place.

## The copy Module’s copy() and deepcopy() Functions
Although passing around references is often the handiest way to deal with lists and dictionaries, if the function modifies the list or dictionary that is passed, you may not want these changes in the original list or dictionary value. For this, Python provides a module named copy that provides both the copy() and deepcopy() functions. The first of these, copy.copy(), can be used to make a duplicate copy of a mutable value like a list or dictionary, not just a copy of a reference. 

### Example 
![copy]()

Now the spam and cheese variables refer to separate lists, which is why only the list in cheese is modified when you assign 42 at index 1.

If the list you need to copy contains lists, then use the copy.deepcopy() function instead of copy.copy(). The deepcopy() function will copy these inner lists as well.


## Practice Projects
[Comma Code]()\
[Coin Flip Streaks]()\
[Character Picture Grid]()







