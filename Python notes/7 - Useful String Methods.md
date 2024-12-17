
## I) len()  | Calculate the length of the string

```python
name = input()
result = len(name)
print(result)

#Input:Minh Luong
#Output:10
```

## II) find() | Find the first occurrence of an element in the string

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

## IV) capitalize()  | Only capitalize the FIRST element of the string
```python
name = input()
result = name.capitalize()    #capitalize() takes no argument
print(result)

#Input:minh luong
#Output:Minh luong
```

