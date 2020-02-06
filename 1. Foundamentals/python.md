<a href="../1. Foundamentals">Back to Foundamentals</a>

# Python
Basic python data structures
* List (mutable)
* Tuples (immutable lists)
* Set (list with no duplications)
* Dictionary (key-value pairs)

For each of the data structure, understand how to 
* add items
* remove items
* count items
* check whether item exist in data structure

## Iterables
Any items that can be used in a `for` loop. (eg. all data structure)

*Iterator* - goes through the iterable one by one, often expendable (can only tranverse over the item once)

*List Comprehension* - sends the outputs into a list (Iterable + Operation, eg. `[2*i for i in mylist]`)

*Zip* - combines serveral iterables into one iterable object
* unequal iterable sizes (length) reuslt in zip of the len of shortest iterable
* Unzip / reverse operation: `zip(*iterable)`
* Process to DataFrame: `list()` :arrow_right: `zip()` :arrow_right: `dict()` :arrow_right:`DataFrame()`

*Generators* - function created iterable object having `yield` keyword in body

## Functions
```
def func(arg1, arg2, *args, kwarg1, kwarg2, **kwargs):
    ...
```
**Positional arguments** - defined/inputted by user 

**Keyword arguments** - default defined by function but can be overridden

**Lambda** - short functions to perform a small task
```
lambda arg1, arg2, ...: expression(arg1, arg2, ...)
```
* think of this as a way to quickly check/perform an operation on each element of an iterable