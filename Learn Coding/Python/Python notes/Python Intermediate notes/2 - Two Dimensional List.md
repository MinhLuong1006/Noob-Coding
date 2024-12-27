#Python 
```Python
fruits =     ["apple", "orange", "banana", "coconut"]
vegetables = ["celery", "carrots", "potatoes"]
meats =      ["chicken", "fish", "turkey"]

groceries = [fruits, vegetables, meats]
print(groceries[0])

#Output: ["apple", "orange", "banana", "coconut"]
-------------------------------------------------------------------------------
print(groceries[0][0])
print(groceries[2][1])

#Output: apple
#        fish
```

```Python
groceries = [["apple", "orange", "banana", "coconut"],
			["celery", "carrots", "potatoes"],
			["chicken", "fish", "turkey"]]

for collection in groceries:
	for item in collection:
		print(item, end = " ")

#Output: apple orange banana coconut celery carrots potatoes chicken fish turkey 
```
