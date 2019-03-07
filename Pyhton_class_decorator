ClassDecorator Example
======================


No args
-------

""" In this example the decorator is implemented as a class"""

class mydecorator(object):

    def __init__(self, f):
        print("mydecorator __init__")
        self.f = f


    def __call__(self, pos):
        print("mydecorator __call__")
        self.f(pos)


@mydecorator
def actualfunction(pos):
    print("Hi")


if __name__ == "__main__":
    actualfunction("Hi")
    print ("finished calling")


With Args
---------

class mydecorator(object):
    def __init__(self,f):
        print("I amd in mydecorator __init__")

    def __call__(self,pos):
        print("I am in mydecorator __call__")
        f(pos)


@mydecorator
def actualfunction(pos):
    print(pos)

if __name__ == "__main__":
    actualfunction("Hi i am actual function")
