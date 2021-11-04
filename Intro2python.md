# Learning Python for fun and profit

## Basic structure

A python script is sensitive to indentation, unlike java where curly braces define blocks of code, python relies on indentation.

    #
    # Example of python script
    #
    
    def main():
        print("Hello World, errrr... ")
        name = input("What's your name? ")
        print("Hello ", name)
        
    if __name__ == "__main__"
    main()
    
 This is an example of standalone python program.
 
 ## Variables
 
 You can dedicate a file to your variables, myprogram.py and variables.py, then refer to them from the main script.
 
     #
     # Examples of variable
     #
     
     # initial declaration
     n=1
     print(n)
     # re assigning a value to n
     n="Name"
     print(n)
     # Is n a number or a name ??
     print(n + str(123))
     def myFunction():
         n=123
         print(n)
     print(n)
     
The last lines of the script are tricky, in this example, the output is expected to be *123* then *Name*. If n is global, the function will overwrite the global n

    #
    # global variable
    #
    global n
    n=1
    myFunction():
        n=2
        print(n)
    print(n)
    
    In this case, the expected output is *2* then *2* as the value of n was overwritten.
    
## Functions
    
Functions are objects in python, you can execute or refer the them.    

    #
    # Functions
    #
    
    def myFunction():
        print("Hello")
        
    print(myFunction())
    print(myFunction)
    
The two outputs are different, the first print prints out the result of the function *Hello* and the second prints information about the object.

    #
    # Useful functions
    #
    
    def AddNumbers(arg1, arg2):
        return arg1 + arg2
        
    print(AddNumbers(3,5))
    
    def Power(num, x=1):
        result = 1
        for i in range(x):
            result = result * num
        return result
        
    print(Power(2,3))
    print(Power(x=3, num=2))
    
When using the argument names, the order does not matter. Output is expected to be *8* and *8*.

## Conditions

Be careful in logical bugs when using conditions as you could be surprised when using == or < or >

    #
    # Conditions
    #
    
    x, y = 100, 10
    
    if (x < y):
        st = "x is smaller than y"
    elif (x == y):
        st = "x is the same as y"
    else:
        st = "x must be greater than y... but is it?"
        
Python does not have a "switch" operand equivalent.

    #
    # One liner conditional statement
    #
    
    x, y = 100, 100 
    st = "x is smaller than y" if (x<y) else "x is either the same or greater than y"
    print(st)
    
## Loops

While loop

    #
    # while loop
    #
    x=0
    while(x<5):
    print(x)
    x=x+1
    
For loop, don't forget, arg2 is not included in the output of range()... arg1 is.

    #
    # for loop
    #
    x=0
    for x in range(5,10):
        print(x)
        
    days=["M", "T", "W", "T", "F", "S", "S"]
    for d in days:
        print(d)
        
    for x in range(5,10):
        if(xx7): break
        print(x)

    days=["M", "T", "W", "T", "F", "S", "S"]
    for i,d in enumerate(days):
        print(i,d)
        
## Object oriented programming

Classes... superclasses... methods... ???

## Modules

Python comes with a ton of librairies, or modules, to import

    #
    # importing modules
    #
    import math
    print("the sqare root of 16 is ", math.sqrt(16))
    print("Pi is = ", math.pi)
    
## Wrap around

    class Person:
        def __initialize(self, name, age)
        self.name = name
        self.age = age
        
