## Format specifiers {value:flags} format a value based on what flags are inserted.

### I) value:.(number)f  | Round to that many decimal places (fixed point)
```python
x = 3.14111215464
y = 2.1
print(f"x equals to: {x:.2f}")
print(f"y equals to: {y:.2f}")

#Output:3.14
#       2.10
```

### II) value:(number)  | Allocate that many spaces
```python
x = 3.14
y = -2.1
print(f"x equals to: {x:10}")
print(f"y equals to: {y:10}")

#Output:      3.14
#             -2.1
---------------------------------------------------------------------------------
x = 3.14
y = -2.1
print(f"x equals to: {x:010}")
print(f"y equals to: {y:010}")
#Each number will be "0" padded
#Output:00000003.14
#       -00000002.1
```

### III) Left Justify, Center Align, Right Justify
```python
price1 = 5.26
price2 = 8.96
price3 = 6.157

print(price1:<10) #Left justify
print(price1:^10) #Center align
print(price1:>10) #Right justify

#Output:5.26------              -: space
#       ---8.96---
#       -----6.157
```