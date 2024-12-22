#Python 
## Variable is a container for a value. A variable behaves as if it was the value it contains.

| Data Type | Definition                   |
| --------- | ---------------------------- |
| Text      | str                          |
| Numeric   | int, float, complex          |
| Sequence  | list, tuple, range           |
| Mapping   | dict                         |
| Set       | set, frozenset               |
| Boolean   | bool                         |
| Binary    | bytes, bytearray, memoryview |

## Operators

| Operators |  Definitions   |
| :-------: | :------------: |
|     +     |    Addition    |
|     -     |  Substraction  |
|     *     | Multiplication |
|     /     |    Division    |
|    //     | Floor Division |
|     %     |    Modulus     |
|    **     | Exponentiation |

## Asking for user inputs

```python
abc = input("Please enter a string: ")
n = int(input("Please enter a number: "))
```

## f-string Formatting

```python
h = int(input("Enter your height: "))
print(f"You are {h} tall")
```


## Built-in Function

### abs()     | Absolute Value (is the distance aways from 0 of a number)

```python
int a = -3
print (abs(a))
#Output: 3
```

### round()   | Round a number
```python
int a = 3.4
print(round(a))
#Output: 3
```

### pow()   | Calculate the power of a number, it raises a number to the power of another

```python
int x = 2
int y = 3
print(pow(x ,y))
#Output: 8
```

### min() and max()
```python
x = 1
y = 2
z = 3
print(min(x ,y, z))
print(max(x ,y, z))
#Output: 1
#        3
```
