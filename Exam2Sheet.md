
A `list` maintains order. The elements can be of any type (int, float, string, tuple, etc.)
Its elements are accessed through their index values.

A `dictionary` is an unordered collection of key-value parts. They're good for handling large amount of data.
Every element has a key-value pair. Its elements are accessed through it's key value.

- You can access data more quickly in a dictionary by using its key, whereas in a list, you need to iterate through the entire list until you find the item of interest.

Why is a base case critical to recursive functions?
- Function won't know how to terminate without a base case, leading to infinite recursion, a.k.a. "stack overflow"

```
def mult3(n):
    if n == 1:
        return 3
    else:
        return mult3(n-1) + 3
```
**Base case:**`n == 1`

Finding target in a sorted list using a binary search is faster than linear search because:
- You look at the value towards the middle, if not found, and ***discard the other half*** without ever searching through it. Repeat as needed until the target is found, ***halving your search space*** each time.

QuickSort without recursion?
- Yes, any recursive function can be implemented using loops, although the resulting code may be more complex.

`Syntax errors`: something wrong with the syntax of the program (Omitting a colon after if statement or else)

`Logic errors`: code runs fine, but produces an unexpected result (`sum_xy = x - y`)

`Runtime errors:` code is syntactically correct, but quits in execution (trying to access file which doesn't exist, using an identifier that has not be defined)

---

**Dictionaries** 

`fruits = {'fruit': 'apple', 'amount': 5}` defining a dictionary,  `print(fruits['fruit'])` gets value associated with key

`fruit_type = fruits.get('fruit')` using get() to retrieve the value `print(fruit_type)`

Looping through all the keys: `fruits.keys()`  Looping through all the values  `fruits.values()` in order `sorted(fruits.keys())`

`items()` returns a view object that displays a list of a given dictionary's (key value) tuple pair

**Files I/O**

`my_file = open(***filepath***)` Opens the file with given filepath for reading, returns file object

`my_file.close()` Closes file `my_file`

**Lists**

`list = []` creates an empty list

`list[start : end]` returns a sublist of list from index start to index end

`list.append(element)` adds the element to the end of list. returns **None**

`list.count(element)` returns the number of times element occurs in list

**Sets**

`{elmt(s)}, set(lst)` constructs a set of provided elmt(s), or of elements in lst
`my_set.add(elmt)` adds elmt to my_set. returns **None**

**Sorting**

`sorted(collection [,key=sort_key, reverse=bool_val]` returns a sorted copy of ***collection***, based on optional sort key (**key**) and optional order preference (**reverse**)

`lst.sort([key=sort_key, reverse=bool_val]` sorts the given list **lst**, based on sort key (**key**) and order prefernce (**reverse**) and returns **None**

