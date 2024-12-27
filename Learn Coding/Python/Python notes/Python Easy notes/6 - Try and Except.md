#Python 
### -The idea of try and except  is that you know that some sequence of instruction(s) may have a problem and we want to add some statements to be executed if an error occurs.

```python
try:
	x = int(input("Enter x: "))
	print(f"x is {x}")
except ValueError: #except only is still OK for many situations
	print("x is not an integer")
```

### -Combining Try and Except with Else:

```python
try:
	x = int(input("Enter x: "))
except ValueError: #except only is still OK for many situations
	print("x is not an integer")
else:
	print(f"x is {x}")
```

### -Forcing the user to enter the right value using Try/Except and While loop:

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

### Let's combine all the things using Functions:

```python
def main():
	x = get_int("Enter x: ")
	print(f"x is {x}")
	
def get_int(prompt):
	while True:
		try:
			return int(input("Enter x: "))
		except ValueError: #except only is still OK for many situations
			print("x is not an integer, please enter an integer.")
		else:
			break
main()
```