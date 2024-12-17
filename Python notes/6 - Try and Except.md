##### -The idea of try and except  is that you know that some sequence of instruction(s) may have a problem and we want to add some statements to be executed if an error occurs.

```python
try:
	x = int(input("Enter x: "))
	print(f"x is {x}")
except ValueError: #except only is still OK for many situations
	print("x is not an integer")
```

##### -Combining Try and Except with Else:

```python
try:
	x = int(input("Enter x: "))
except ValueError: #except only is still OK for many situations
	print("x is not an integer")
else:
	print(f"x is {x}")
```

##### -Forcing the user to enter the right value using Try/Except and While loop:

```python
while True:
	try:
		x = int(input("Enter x: "))
	except ValueError: #except only is still OK for many situations
		print("x is not an integer")
	else:
		break
		
print(f"x is {x}")
```