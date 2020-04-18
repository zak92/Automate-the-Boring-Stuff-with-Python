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

## Storing Values in Variables with Assignment Statements
An assignment statement consists of a variable name, an equal sign (called the assignment operator), and the value to be stored. If you enter the assignment statement spam = 42, then a variable named spam will have the integer value 42 stored in it. 

## Variable Names
A good variable name describes the data it contains. A a descriptive name will help make your code more readable. 
You can name a variable anything as long as it obeys the following three rules:
• It can be only one word with no spaces.

• It can use only letters, numbers, and the underscore (_) character.

• It can’t begin with a number.

## Comments
The following line is called a comment.

#This program says hello and asks for my name.

Python ignores comments, and you can use them to write notes or remind yourself what the code is trying to do.

## The print() Function
The print() function displays the string value inside its parentheses on the screen. 

## The input() Function
The input() function waits for the user to type some text on the keyboard and press ENTER. 

myName = input()

This function call evaluates to a string equal to the user’s text, and the line of code assigns the myName variable to this string value.
