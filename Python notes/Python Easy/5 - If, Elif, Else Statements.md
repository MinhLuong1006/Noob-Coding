## I) Conditional Execution

##### Conditional statements give us the ability to check conditions and change the behavior of the program accordingly. The simplest form is the **if statement:**

```python
if (condition):
	actions
```

## II) Alternative Execution

##### A second form of the if statement is alternative execution, in which there are two possibilities and the condition determines which one gets executed:

```python
if (condition):
	action1
else:
	action2
```

## III) Chained Conditionals

##### Sometimes there are more than two possibilities so we need more than 2 branches:

```python
if (condition1):
	action1
elif (condition2):
	action2
else (condition3):
	action3
```

## IV) Nested Conditionals

##### One conditional can also be nested within another. We could have written the three-branch example like this:

```python
if (condition1):
	action1:
else:
	if (condition2):
		action2
	else:
		action3
```

