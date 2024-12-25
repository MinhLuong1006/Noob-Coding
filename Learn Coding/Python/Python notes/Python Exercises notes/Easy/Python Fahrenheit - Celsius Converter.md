#Python 
```Python
print("-----Fahrenheit - Celsius Converter-----")
print("Press F for converting from C degree to F degree.")
print("Press C for converting from F degree to C degree.")
while True:
    tp = input("What do you choose? ")
    if (tp.lower() == "f" or tp.lower() == "c"):
        break
    else:
        print("You didn't enter the right keyword! Try again.")
if (tp.lower() == "f"):
    while True:
        try:
            c = float(input("Enter the temperature in C degrees: "))
        except ValueError:
            print("You didn't enter a number! Try again.")
        else:
            break
    f = (c * 9/5) + 32
    print(f"{c:.2f} C degrees is {f:.2f} F degrees") #cant use :02 cuz its a float so we have to use .2f. See the rules at Lesson 9 - Format Specifiers
    
if (tp.lower() == "c"):
    while True:
        try:
            f = float(input("Enter the temperature in F degrees: "))
        except ValueError:
            print("You didn't enter a number! Try again.")
        else:
            break
    c = (f - 32) / 1.8
    print(f"{f:.2f} F degrees is {c:.2f} C degrees")
```

