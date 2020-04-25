# Functions
![function]()

The first line is a def statement ➊, which defines a function named hello(). The code in the block that follows the def statement ➋ is the body of the function. This code is executed when the function is called, not when the function is first defined.The hello() lines after the function ➌ are function calls. 

## def Statements with Parameters
When you call the print() or len() function, you pass them values, called arguments, by typing them between the parentheses. You can also define your own functions that accept arguments. 

## Return Values and return Statements
When you call the len() function and pass it an argument such as 'Hello', the function call evaluates to the integer value 5, which is the length of the string you passed it. In general, the value that a function call evaluates to is called the return value of the function.

## The None Value
In Python, there is a value called None, which represents the absence of a value. The None value is the only value of the NoneType data type. (Other programming languages might call this value null, nil, or undefined.) Just like the Boolean True and False values, None must be typed with a capital N.

This value-without-a-value can be helpful when you need to store something that won’t be confused for a real value in a variable. One place where None is used is as the return value of print(). The print() function displays text on the screen, but it doesn’t need to return anything in the same way len() or input() does. But since all function calls need to evaluate to a return value, print() returns None. 

![none]()

## Keyword Arguments and the print() Function
Some functions have optional keyword arguments that can be specified when the function is called.

keyword arguments are identified by the keyword put before them in the function call. Keyword arguments are often used for optional parameters. For example, the print() function has the optional parameters end and sep to specify what should be printed at the end of its arguments and between its arguments (separating them), respectively.

![print]()

The two outputted strings appear on separate lines because the print() function automatically adds a newline character to the end of the string it is passed. However, you can set the end keyword argument to change the newline character to a different string.

![end]()

Similarly, when you pass multiple string values to print(), the function will automatically separate them with a single space.

![print2]()

But you could replace the default separating string by passing the sep keyword argument a different string.

![sep]()

## Local and Global Scope
* Parameters and variables that are assigned in a called function are said to exist in that function’s local scope. 
* Variables that are assigned outside all functions are said to exist in the global scope.

A variable that exists in a local scope is called a local variable, while a variable that exists in the global scope is called a global variable.

Scopes matter for several reasons:
* Code in the global scope, outside of all functions, cannot use any local variables.
* However, code in a local scope can access global variables.
* Code in a function’s local scope cannot use variables in any other local scope.

## The global Statement
If you need to modify a global variable from within a function, use the global statement. If you have a line such as global eggs at the top of a function, it tells Python, “In this function, eggs refers to the global variable, so don’t create a local variable with this name.” 

![global statement]()

Because eggs is declared global at the top of spam() ➊, when eggs is set to 'spam' ➋, this assignment is done to the globally scoped eggs. No local eggs variable is created.

## Exception Handling
Right now, getting an error, or exception, in your Python program means the entire program will crash. You don’t want this to happen in real-world programs. Instead, you want the program to detect errors, handle them, and then continue to run.

Errors can be handled with try and except statements. The code that could potentially have an error is put in a try clause. The program execution moves to the start of a following except clause if an error happens.

![try and except]()
When code in a try clause causes an error, the program execution immediately moves to the code in the except clause. After running that code, the execution continues as normal. The output of the previous program is as follows:

![try output]()

Functions are the primary way to compartmentalize your code into logical groups. Since the variables in functions exist in their own local scopes, the code in one function cannot directly affect the values of variables in other functions. This limits what code could be changing the values of your variables, which can be helpful when it comes to debugging your code.

## Practice Projects
[The Collatz Sequence]()




