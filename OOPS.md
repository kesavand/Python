OOPS Terminology:

Class :
A user-defined prototype for an object that defines a set of attributes that characterize any object of the class. 
The attributes are data members (class variables and instance variables) and methods, accessed via dot notation.
By convention class names starts with a capital letter.
Example:
class MyClass(object): 
    pass  #pass is keyword, equals to do nothing
    
    
Data member:
A class variable or instance variable that holds data associated with a class and its objects.

Method − A special kind of function that is defined in a class definition.

Class variable:
 A variable that is shared by all instances of a class. Class variables are defined within a class but outside any of the class's methods. Class variables are not used as frequently as instance variables are Since the OOPs princeples encourage data encapsulation usually the class variables are accessed by using get and set methods.
 
Private Attributes:
An attribute starting with one underscores inside a class is private attribute(a class variable, instance variable and an instance method can be made private), Remember that in python nothing is private, but is a convention to use underscore for private members so that coders dont access the attribute directly and implement appropirate methods to access the private attributes,
NOTE: when an attribute is preceeded with double underscores, it is not  convention; it has a specific meaning to the interpreter.The double underscore before an attribute name makes the interpreter to add class name before the attribute, This isused to avoid name clashes when the same name is used in other classes and sub classess.


Instance variable :
  A variable that is defined inside a method and belongs only to the current instance of a class.
 
  
Object :
 A unique instance of a data structure that's defined by its class. An object comprises both data members (class variables and instance variables) and methods.
 
 Object:
  A unique instance of a data structure that's defined by its class. An object comprises both data members 
 
 New and Init methods:
 The magic method __new__ will be called when instance is being created. Using this method you can customize the instance creation. 
 This is only the method which will be called first then __init__ will be called to initialize instance when you are creating instance.


what are class methods static methods and instance methods ?
In Python, classes can have three different types of methods. Such as 
instance methods, static methods and class methods.

Instance method:
 A method that is called on an instance of a class. Instance methods are defined inside class body.

Unlike instance methods, static and class are not bound to instance of a class.
They can be called without creating an instance of a class.
Class methods
Class methods are used to work with class attributes.

They can be called without creating an instance.

similar to instance methods classmethods take a reference to class,

as first argument. Usually ‘cls’ is used as class reference.

Class methods are created, by using @classmethod decorator

Example

Creating Class methods
?
class Employee(object):
             
    @classmethod
    def i_am_class_method(cls):
 
        pass
Notice ‘cls‘ reference passed while defining it.

Python implicitly passes ‘cls’ reference when classmethod is called.

Calling class methods
Class methods can be called by using class name or instance.

?
Employee.i_am_class_method()
 
or
 
emp_1 = Employee()
 
emp_1 .i_am_class_method()
static method
A static method is like a normal module level function, defined inside a class.

But they never receive an automatic self, or cls argument.

Static methods are also can be called by using class name or instance.

static methods are created, by using @staticmethod decorator

Creating static methods
?
class Employee(object):       
  
    @staticmethod
    def i_am_static_method():
 
        pass
Calling static methods
Static methods can also be called by using class name or instance.

?
Employee.i_am_static_method()
 
 
or
 
emp_1 = Employee()
 
emp_1.i_am_static_method()
Generally static methods are used to,

perform utility functions related to class.




What every object has ?
Every object has,
1.Type
2.Id
3.Attribute(s), some of them are Method(s)
4. Value(s), of attributes.
 
 
What are the difference between modules and class ?
Python modules are files containing Python code.
Modules can be executed individually, or imported in some other module and get executed.
A module may contain, classes, properties or functions any of these or all of these.

 

Where as a class is Python code inside a module.
 
 Pillars of OOPS:
   
Encapsulation & Abstraction:
----------------------------
The terms encapsulation and data abstraction are often interchangeable.Actually, the data abstraction is achieved through encapsulation.
Encapsulation in general, is a mechanism,to restrict the direct access of some of objects attributes. That is, to hide internal implementation of an object, from outside its definition.Typically access to attributes is only allowed, through setters and getters methods.

Inheritance:
------------
 
 Polymorphism
