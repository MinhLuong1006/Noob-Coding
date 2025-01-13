#Python 
## I) The Basics
#### Delcaring An Array Using NumPy

```Python
import numpy as np
arr = np.array([1,2,3])
print arr

#Output: [1,2,3]
---------------------------------------------------------------------------------
import numpy as np
arr = np.array([1,2,3], [4,5,6])
print arr

#Output: [[1,2,3]
#         [4,5,6]]
```

#### Get Dimension

```Python
import numpy as np
arr = np.array([1,2,3])
print (arr.ndim)

#Output: 1
----------------------------------------------------------------------------------
import numpy as np
arr = np.array([1,2,3], [4,5,6])
print (arr.ndim)

#Output: 2
----------------------------------------------------------------------------------
import numpy as np
arr = np.array([[1,2,3], [4,5,6]], [[10,11,12],[13,14,15]])
print (arr.ndim)

#Output: 3
-----------------------------------------------------------------------------------
import numpy as np
arr = np.array(20)
print (arr.ndim)

#Output: 0
```

#### DTYPE
##### Use this when we know that we don't need something that is too big in order to make the program run faster.

```Python
import numpy as np
arr = np.array([1,2,3], dtype='int16') #default is int32
arr.itemsize

#Output: 2
```

## II) NumPy Array Indexing

### Get a specific element

```Python
import numpy as np
arr = np.array([1,2,3])
print (arr[1])

#Output: 2
----------------------------------------------------------------------------------
import numpy as np
arr = np.array([1,2,3], [4,5,6])
print (arr.[1,2])

#Output: 6
----------------------------------------------------------------------------------
import numpy as np
arr = np.array([[1,2,3], [4,5,6]], [[10,11,12],[13,14,15]])
print (arr.[1,1,1])

#Output: 14
```