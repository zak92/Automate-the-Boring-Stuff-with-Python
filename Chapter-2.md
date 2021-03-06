# Flow Control

## Boolean Values
The Boolean data type has only two values: True and False. They always start with a capital T or F, with the rest of the word in lowercase. 
### Example
spam = True
print(spam)

**Output**: True

## Comparison Operators
Comparison operators, compare two values and evaluate down to a single Boolean value.

![Comparison Operators]()

### Examples
1. 42 == 99        **Output: False**
2. 2 != 2          **Output: False**
3. 'dog' != 'cat   **Output: True**

## Boolean Operators
The three Boolean operators (and, or, and not) are used to compare Boolean values.

The and and or operators always take two Boolean values (or expressions)
* The and operator evaluates an expression to True if both Boolean values are True; otherwise, it evaluates to False. 
* The or operator evaluates an expression to True if either of the two Boolean values is True. If both are False, it evaluates to False.
* The not operator operates on only one Boolean value (or expression). The not operator simply evaluates to the opposite Boolean value.

## Examples
1. (4 < 5) and (5 < 6)
**Output: True**
2. (1 == 2) or (2 == 2)
**Output: True**

## Blocks of Code
Lines of Python code can be grouped together in blocks. You can tell when a block begins and ends from the indentation of the lines of code. There are three rules for blocks.

* Blocks begin when the indentation increases.
* Blocks can contain other blocks.
* Blocks end when the indentation decreases to zero or to a containing block’s indentation.

## if Statements
The most common type of flow control statement is the if statement. An if statement’s clause (that is, the block following the if statement) will execute if the statement’s condition is True. The clause is skipped if the condition is False.

## else statements
An if clause can optionally be followed by an else statement. The else clause is executed only when the if statement’s condition is False. In plain English, an else statement could be read as, “If this condition is true, execute this code. Or else, execute that code.” 

## elif Statements
While only one of the if or else clauses will execute, you may have a case where you want one of many possible clauses to execute. The elif statement is an “else if” statement that always follows an if or another elif statement. It provides another condition that is checked only if all of the previous conditions were False. 

![if elif else]()

## while Loop Statements
You can make a block of code execute over and over again using a while statement. The code in a while clause will be executed as long as the while statement’s condition is True.

## break Statements
There is a shortcut to getting the program execution to break out of a while loop’s clause early. If the execution reaches a break statement, it immediately exits the while loop’s clause.

## continue Statements
Like break statements, continue statements are used inside loops. When the program execution reaches a continue statement, the program execution immediately jumps back to the start of the loop and reevaluates the loop’s condition. (This is also what happens when the execution reaches the end of the loop.)

![while, break, continue]()

## for Loops and the range() Function
The while loop keeps looping while its condition is True, but what if you want to execute a block of code only a certain number of times? You can do this with a for loop statement and the range() function.

## The Starting, Stopping, and Stepping Arguments to range()
The first argument will be where the for loop’s variable starts, and the second argument will be up to, but not including, the number to stop at. The third argument is the amount that the variable is increased by after each iteration. The start and step arguments are optional. If the start argument is not specified, it will begin at 0. The stop argument will be up to, but not including, the number to stop at. You can even use a negative number for the step argument to make the for loop count down instead of up.

![for and range]()

So calling range(0, 10, 2) will count from zero to eight by intervals of two. The output will be 0, 2, 4, 6, 8

## Importing Modules
Python also comes with a set of modules called the standard library. Each module is a Python program that contains a related group of functions that can be embedded in your programs. For example, the math module has mathematics-related functions, the random module has random number-related functions, and so on.

Before you can use the functions in a module, you must import the module with an import statement. In code, an import statement consists of the following:

* The import keyword
* The name of the module
* Optionally, more module names, as long as they are separated by commas

Here’s an example of an import statement that imports four different modules:

import random, sys, os, math

Now we can use any of the functions in these four modules in our program.

## Ending a Program Early with the sys.exit() Function

The last flow control concept to cover is how to terminate the program. Programs always terminate if the program execution reaches the bottom of the instructions. However, you can cause the program to terminate, or exit, before the last instruction by calling the sys.exit() function. Since this function is in the sys module, you have to import sys before your program can use it.

### Example

![sys.exit]()

The user must enter exit in order to stop the program.








