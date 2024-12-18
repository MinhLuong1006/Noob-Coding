
## I) len()  | Calculate the length of a string

```python
name = input()
result = len(name)
print(result)

#Input:Minh Luong
#Output:10
```

## II) find() and index()| Find the first occurrence of an element in a string

```python
name = input()
result = name.find("L")
print(result)

#Input:Minh Luong
#Output:5
#If there is no result it will return -1
```

## III) rfind() | To find the last occurrence
```python
name = input()
result = name.rfind("L")
print(result)

#Input:Minh Luong
#Output:4
#If there is no result it will return -1
```

## IV) capitalize()  | Only capitalize the FIRST element of a string
```python
name = input()
result = name.capitalize()    #capitalize() takes no argument
print(result)

#Input:minh luong
#Output:Minh luong
```

## V) upper() and lower()  | To make all the elements of a string upper or lower

```python
name = input()
result = name.upper()    
print(result)

#Input:Minh Luong
#Output:MINH LUONG
---------------------------------------------------------------------------------
name = input()
result = name.lower()    
print(result)

#Input:Minh Luong
#Output:minh luong
```

## VI) title()  | Capitalize the first character of every words in a string
```python
name = input()
result = name.title()    
print(result)

#Input:minh luong
#Output:Minh Luong
```

## VII) isdigit() | Check if all elements in a string are digits
```python
x = input()
result = x.isdigit()    
print(result)

#Input:minh luong123                     #Input:2365546
#Output:False                            #Output:True
```

## VIII) isalpha() | Check if all elements in a string are alphabet letters
```python
x = input()
result = x.isalpha()    
print(result)

#Input:minhluong                 #Input:lol2365546  or   minh luong or   minh_luong
#Output:True                     #Output:False
```
## IX) count() | Count how many times an element exists in a string
```python
name = input()
result = name.count("n")    
print(result)

#Input:minh luong
#Output:2
```

## X) To see all the string methods in Python:
```python
print(help(str))
```