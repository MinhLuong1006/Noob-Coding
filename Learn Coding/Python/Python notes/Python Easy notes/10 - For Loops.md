#Python 
### For Loops are used to execute a block of code a fixed number of times. You can iterate over a range, string, sequence, etc.
```python
#use for loop to print from 1 to 5

for x in range(1,6): #since the 2nd number is exclusive so we write 11 
	print(x)

#Output:1
#       2
#       3
#       4
#       5
---------------------------------------------------------------------------------
#use for loop to print odd numbers only from 1 to 10
for x in range(1,11,2): #since the 2nd number is exclusive so we write 11 
	print(x)

#Output:1
#       3
#       5
#       7
#       9
```

### Iterating backwards
```python
for x in range(10, 0, -1):
	print(x)
---------------------------------------------------------------------------------
for x in reversed(range(1,11)): 
	print(x)
```

### Continue
```python
for x in range(1,6):
	if x == 3:
		continue
	else:
		print(x)

#Ouutput:1
#        2
#        4
#        5
```

### Break
```python
for x in range(1,6):
	if x == 3:
		break
	else:
		print(x)

#Ouutput:1
#        2
```

### Nested Loop
```Python
for x in range(...,...): 
	for x in range(...,...): 
		do...
```