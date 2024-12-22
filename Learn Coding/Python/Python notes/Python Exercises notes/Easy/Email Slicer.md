#Python 
```python
email = input("Please enter your email: ")
splitpos = email.index("@")
domain = email[splitpos:]
name = email[:splitpos]
print(f"The name is {name}")
print(f"The domain is {domain}")
```