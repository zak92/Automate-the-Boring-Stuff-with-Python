# PYTHON BASICS

## Math Operators in Python
![Operators](https://github.com/zak92/Automate-the-Boring-Stuff-with-Python/blob/master/Images/operators.png)

## The Integer, Floating-Point, and String Data Types
A data type is a category for values, and every value belongs to exactly one data type.

![Data Types](https://github.com/zak92/Automate-the-Boring-Stuff-with-Python/blob/master/Images/Data%20Types.png)

Always surround your string in single quote (') characters. For example ‘Hello World!’. You can even have a string with no characters in it, '', called a blank string or an empty string. 

## String Concatenation and Replication
The meaning of an operator may change based on the data types of the values next to it. For example, + is the addition operator when it operates on two integers or floating-point values. However, when + is used on two string values, it joins the strings as the string concatenation operator. 

**Example:**

'Alice' + 'Bob'

Output will be 'AliceBob' 

If you try to use the + operator on a string and an integer value, Python will not know how to handle this, and it will display an error message since you can’t add an integer to a string.

The * operator multiplies two integer or floating-point values. But when the * operator is used on one string value and one integer value, it becomes the string replication operator.  

**Example:**

'Alice' * 5

Output will be 'AliceAliceAliceAliceAlice' 

The * operator can be used with only two numeric values (for multiplication), or one string value and one integer value (for string replication).  

