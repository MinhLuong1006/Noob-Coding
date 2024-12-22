#Python 
## Format specifiers f"{value:flags}" format a value based on what flags are inserted.
### *** MUST USE A FORMATTED STRING f"{value}"

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

print(f"{price1:<10}") #Left justify
print(f"{price2:^10}") #Center align
print(f"{price3:>10}") #Right justify

#Output:5.26------              -: space
#       ---8.96---
#       -----6.157
```

### IV) value:+  | To indicate positive and negative values 
```python
price1 = 5.26
price2 = -8.96

print(f"{price1:+}") 
print(f"{price2:+}") 

#Output:+5.26
#       -8.96
----------------------------------------------------------------------------------
#value:space to add a space before a positive value, just to make it cleaner
price1 = 5.26
price2 = -8.96
price3 = 4.55
price4 = -5.25

print(f"{price1: }") 
print(f"{price2: }")
print(f"{price3: }") 
print(f"{price4: }")

#Output: 5.26
#       -8.96
#        4.55
#       -5.25
```

### V) value:,  | Comma separator
```python
n = 3000000

print(f"{n:,}")


#Output:3,000,000
```

### VI) Mix and Match Format Specifiers
```python
n1 = 3000.14159
n2 = -947584.65
n3 = -1200.35

print(f"{n1:+,.2f}")
print(f"{n2:+,.2f}")
print(f"{n3:+,.2f}")

#Output: +3,000.14
#        -947,584.65
#        -1,200.35
```