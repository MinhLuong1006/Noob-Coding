#Python 
```Python
import time

tm = int(input("Enter the number of seconds: "))
for i in range (tm, 0, -1):
    sec = i % 60
    mi = int(i / 60) % 60
    h = int(i / 3600)
    print(f"{h:02}:{mi:02}:{sec:02}")
    time.sleep(1)
    
print("Time's up!")
```