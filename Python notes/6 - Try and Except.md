##### -The idea of try and except  is that you know that some sequence of instruction(s) may have a problem and we want to add some statements to be executed if an error occurs.

```python
try:
	x = int(input("Enter x: "))
	print(f"x is {x}")
except ValueError:
	print("x is not an integer")

