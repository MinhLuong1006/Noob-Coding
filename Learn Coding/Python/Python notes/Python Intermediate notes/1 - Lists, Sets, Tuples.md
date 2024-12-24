#Python 
```Python
Lists = [] ordered and changeable. Duplicates are OK. 
-When you need a collection of ordered items that can be changed (mutable).

Set = {} unordered and immutable. Add or Remove is OK. No Duplicates.
-When you need a collection of unique items and do not care about order.

Tuple = () ordered and unchangeable. Duplicates are OK. Faster.
-When you want a fixed, ordered collection of items that shouldn't be changed. Useful for passing data as a single entity.

***use help() function to see the descryption of methods: print(help(fruits))***

```

| Feature    | List                         | Set                        | Tuple                      |
| ---------- | ---------------------------- | -------------------------- | -------------------------- |
| Order      | Maintains order              | No order                   | Maintains order            |
| Mutability | Mutable (changeable)         | Mutable (add/remove items) | Immutable (cannot change)  |
| Duplicates | Allowed                      | Not allowed                | Allowed                    |
| Usage      | Dynamic, ordered collections | Unique, unordered items    | Fixed, ordered collections |


### I) List
##### 1) List indexing
```Python
fruits = ["apple", "orange", "banana", "coconut"]
print(fruits[2:])

#Output: ['banana', 'coconut']

---------------------------------------------------------------------------------

print(fruits[::-1])

#Output: ['coconut', 'banana', 'orange', 'apple']

```

##### 2) index() | Show the index of an element
```Python
fruits = ["apple", "orange", "banana", "coconut"]
print(fruits.index("orange"))

#Output: 1

```

##### 3) List with loops
```Python
fruits = ["apple", "orange", "banana", "coconut"]
for x in fruits:
	print(x) #x represent the elemts in the lists so fruits[x] is incorrect
	
#Output: apple
#		 orange
#        banana
#        coconut
```

##### 4) len()
```Python
fruits = ["apple", "orange", "banana", "coconut"]
print(len(fruits))

#Output: 4
```

##### 5) insert()
```Python
fruits = ["apple", "orange", "banana", "coconut"]
fruits.insert(0, "pineapple") #or fruits[0] = "sussy" 
for x in fruits:
	print(x)
	
#Output: sussy
#		 orange
#        banana
#        coconut
```

##### 6) append() | Add an element at the end of the list
```Python
fruits = ["apple", "orange", "banana", "coconut"]
fruits.append("sussy")

#Output: apple
#		 orange
#        banana
#        coconut
#        sussy

```

##### 7) sort()
```Python
fruits = ["apple", "orange", "banana", "coconut"]
fruits.sort() 
for x in fruits:
	print(x)
	
#Output: apple
#		 banana
#        coconut
#        orange
```

##### 8) reverse()
```Python
fruits = ["apple", "orange", "banana", "coconut"]
fruits.reverse()
print(fruits)

#Output: ['coconut', 'banana', 'orange', 'apple']
```

##### 9) clear() | Clear all the elements in the list
```Python
fruits = ["apple", "orange", "banana", "coconut"]
fruits.clear()
print(fruits)

#Output: []
```

##### 10) count() | Count how many times an element exists
```Python
fruits = ["apple", "orange", "banana", "coconut", "banana"]
print(fruits.count("banana"))

#Output: 2
```

##### 11) Check if an element is in a list or not with 'in' operator
```Python
fruits = ["apple", "orange", "banana", "coconut", "banana"]
print("banana" in fruits)

#Output: True
```

### II) Set
##### 1) add() | add an element to the set
```Python
fruits = {"apple", "orange", "banana", "coconut"}
fruits.add("sussy")
print(fruits)
#Output: {"orange", "banana", "apple", "coconut", "sussy"} Sets are unordered so the order would be random.
```

##### 2) remove() | remove an element from the set
```Python
fruits = {"apple", "orange", "banana", "coconut"}
fruits.add("apple")
print(fruits)
#Output: {"orange", "banana", "coconut"} Sets are unordered so the order would be random.
```

##### 3) pop() | remove the first element of the set
```Python
It is simmilar to remove() but it removes the first element of the set instead. However, since the orders in sets are unordered so the element will be removed will be random.
```

## III) Tuple
```Python
fruits = ("apple", "orange", "banana", "coconut")

The methods for working with Tuples are similar to those for Lists
```