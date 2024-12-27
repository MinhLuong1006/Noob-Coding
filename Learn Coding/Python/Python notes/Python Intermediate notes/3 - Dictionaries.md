#Python 
### Dictionary is a collection of {key:value} pairs. Dictionaries are ordered and changeable. No duplicates.

##### I) dict.get() | Get the value of a key
```Python
capitals = {"USA": "Washington D.C.",
		    "China": "Beijing",
		    "Russia": "Moscow"}
		    
print(capitals.get("USA"))

#Output: Washington D.C.
```

##### II) dict.update({key:value}) | Update the dictionary
```Python
capitals = {"USA": "Washington D.C.",
		    "China": "Beijing",
		    "Russia": "Moscow"}
		    
capitals.update({"USA": "New York"})
capitals.update({"Germany": "Berlin"})

print(capitals)


#Output: {'USA': 'New York', 'China': 'Beijing', 'Russia': 'Moscow', 'Germany': 'Berlin'}
```