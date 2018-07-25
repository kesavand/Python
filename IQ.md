Differentiate between deep and shallow copy?

A deep copy copies an object into another. This means that if you make a change to a copy of an object,
it won’t affect the original object. In Python, we use the function deepcopy() for this, and we import the module copy.
We use it like: b=copy.deepcopy(a)

A shallow copy, however, copies one object’s reference to another. So, if we make a change in the copy, it will affect the original object. For this,
we have the function copy(). We use it like: copy.copy(a)

Differentiate between lists and tuples?
The major difference is that a list is mutable, but a tuple is immutable.
Tuple doesn't allow object deletion.

What are tuples ?
A tuple1 is a sequence of values much like a list. The values stored in a tuple can be any type, and they are indexed by integers. The important difference is that tuples are immutable. 
Tuples are also comparable and hashable so we can sort lists of them and use tuples as key values in Python dictionaries.

What are lists ?
lists are a list of values,and they are indexed by integers, They are mutable.


what are dictionaries ?
Dictionaries are a an unordered collection of key value pairs.The dictionaries are mutable.


