
1.Functions can be reused which is a major advantage. it can be called anywhere multiple times.
2.when the function is called
3.the def keyword is used to create a function
4.In function definition, the code of the function is written and it is not executed at first. The function call will trigger the execution of the function and pass the value to the argument in the function
5.global scope - 1
  local scope - created whenever the function is called
6.it is destroyed
7.it is the value that function call evaluates to. it can be used in an expression
8.None is returned
9.Using global statement
10.NoneType
11.imports the module areallyourpetsnamederic
12.import the module named spam using "import spam" and then spam.bacon() can be used to call the function
13.placing the error causing peice of code in the try clause
14.in the try clause, the error causing line of code is written and the solution for that is given in the except clause

PRACTICE PROJECTS:

The collatz sequence

def collatz(number):
    if number%2==0:
        print(number//2)
        return number//2
    else:
        print(3*number+1)
        return 3*number+1
try:
    n = int(input("Enter a number : "))
    while n!=1:
        n=collatz(n)
except ValueError:
    print("Please enter a valid input")
