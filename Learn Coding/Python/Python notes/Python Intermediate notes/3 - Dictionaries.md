#Python 
```Python
Dictionary is a collection of {key:value} pairs. Dictionaries are ordered and changeable. No duplicates.
```
## I) Dictionaries

### 1) dict.get() | Get the value of a key

```Python
capitals = {"USA": "Washington D.C.",
		    "China": "Beijing",
		    "Russia": "Moscow"}
		    
print(capitals.get("USA"))

#Output: Washington D.C.
```

### 2) dict.update({key:value}) | Update the dictionary

```Python
capitals = {"USA": "Washington D.C.",
		    "China": "Beijing",
		    "Russia": "Moscow"}
		    
capitals.update({"USA": "New York"})
capitals.update({"Germany": "Berlin"})

print(capitals)


#Output: {'USA': 'New York', 'China': 'Beijing', 'Russia': 'Moscow', 'Germany': 'Berlin'}
```

### 3) dict.pop() | Eleminate an element in a dictionary

```Python
capitals = {"USA": "Washington D.C.",
		    "China": "Beijing",
		    "Russia": "Moscow"}
		    
capitals.pop({"China"})


print(capitals)


#Output: {'USA': 'New York','Russia': 'Moscow', 'Germany': 'Berlin'}
```

### 4) dict.clear() | Clear all the elements in a dictionary

```Python
capitals = {"USA": "Washington D.C.",
		    "China": "Beijing",
		    "Russia": "Moscow"}
		    
capitals.clear()


print(capitals)


#Output: {}
```

### 5) Using loops with dictionaries

```Python
capitals = {"USA": "Washington D.C.",
		    "China": "Beijing",
		    "Russia": "Moscow"}
		    
keys = capitals.keys()
print(keys)
print()
for key in keys:
	print(key)


#Output: dict_keys(['USA', 'China', 'Russia'])
#
#        USA
#        China
#        Russia

--------------------------------BETTER VERSION:---------------------------------

capitals = {"USA": "Washington D.C.",
		    "China": "Beijing",
		    "Russia": "Moscow"}
for capital in capitals:
	print(capital)
	
#Same output
|||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||

capitals = {"USA": "Washington D.C.",
		    "China": "Beijing",
		    "Russia": "Moscow"}
		    
values = capitals.values()
print (values)
print()
for value in values:
	print(value)

#Output: dict_values(['Washington D.C.', 'Beijing', 'Moscow'])
#
#        Washington D.C.
#        Beijing
#        Moscow

--------------------------------BETTER VERSION:-----------------------------------

capitals = {"USA": "Washington D.C.",
		    "China": "Beijing",
		    "Russia": "Moscow"}
for capital in capitals:
	print(capitals[capital])
	
#Same output
||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||

capitals = {"USA": "Washington D.C.",
		    "China": "Beijing",
		    "Russia": "Moscow"}
items = capitals.items()
print(items)
print()
for key, value in items:
	print(f"{key}: {value}")


#Output: dict_items([('USA', 'Washington D.C.'), ('China', 'Beijing'), ('Russia', 'Moscow')])
#	
#        USA:Washington D.C.
#        China:Beijing
#        Russia:Moscow

--------------------------------BETTER VERSION:-----------------------------------

capitals = {"USA": "Washington D.C.",
		    "China": "Beijing",
		    "Russia": "Moscow"}
for capital in capitals:
	print(capital, capitals[capital], sep=": ")
	
#Same output
```

## II) Lists of Dictionaries

```Python
Use Lists of Dictionaries when there is a lot of information.
```

```Python
countries = [{"name": "USA", "capital": "Washington D.C.", "pact":"NATO"},
			 {"name": "Soviet Union", "capital": "Moscow", "pact":"Warsaw"},
			 {"name": "East Germany", "capital": "Berlin", "pact":"Warsaw"}]
for country in countries:
	print (country["name"], country["capital"], country["pact"], sep = ": ")


#Output: USA: Washington D.C.: NATO
#        Soviet Union: Moscow: Warsaw
#        East Germany: Berlin: Warsaw
			 
```