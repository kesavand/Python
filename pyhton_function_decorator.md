Pyhton Decorator function example:
=================================

No args
--------
'''This is an example to explain the python decorator'''

from functools import wraps
def mydecorator(func):
    @wraps(func)
    def wraper(*args, **kwargs):
        print("before calling the actual function")
        func(*args, **kwargs)
        print("after calling the function")
    return wraper


@mydecorator
def actualfunction(*args, **kwargs):
    print("..", args,kwargs["stuff"])

if __name__ == "__main__":
    actualfunction(["Hello ", "i " "am " "actual " "function "], stuff = "interesting" )

With Args
--------
''' Decorator function with the argumnets
1. The decorated function is passed with positional and variable arguments
2. The decorated function is also passed with the variable arguments
'''
from functools import wraps
def mydecorator(pos,*args,**kwargs): # arguments for the decorator

def innerfunction(func):
        print(pos, args, kwargs['name'])
        @wraps(func)
        def wrapper(pos,*args,**kwargs):  # arguments for the decorated function
            print("before calling the function")
            func(pos,*args,**kwargs)
            print("After calling the function")
        return wrapper
    return innerfunction


@mydecorator("Hi", ["I ","am"], name = "mydecorator" ) # passing arguments for the decorater
def actualfunction(pos,*args,**kwargs):
    print (pos , args, kwargs['name'])

if __name__ == "__main__" :
    actualfunction("Hi ", ["i ", "am "], name = "actualfunction") #passing arguments for the decorated function


