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

## The len() Function
You can pass the len() function a string value (or a variable containing a string), and the function evaluates to the integer value of the number of characters in that string. 

### Example
len('hello')

The output is 5 since there are  letters in the word hello.

## The str(), int(), and float() Functions
If you want to concatenate an integer such as 29 with a string to pass to print(), you’ll need to get the value '29', which is the string form of 29. 

str(29)

The str(), int(), and float() functions will evaluate to the string, integer, and floating-point forms of the value you pass, respectively. 

## Examples
1. int('42') will evaluate to 42
2. float('3.14') will evaluate to 3.14
3. float(10) will evaluate to 10.0
4. int(7.7) will evaluate to 7

The str() function is handy when you have an integer or float that you want to concatenate to a string. The int() function is also helpful if you have a number as a string value that you want to use in some mathematics. For example, the input() function always returns a string, even if the user enters a number.  The int() function is also useful if you need to round a floating-point number down. 





