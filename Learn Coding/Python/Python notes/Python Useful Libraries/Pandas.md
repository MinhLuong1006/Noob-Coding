#Python 
## Intro to Dataframes

```Python
import pandas as pd
from pandas import DataFrame
df = DataFrame([[1,2,3],[4,5,6],[7,8,9]], columns=["A", "B", "C"], index = ["x","y","z"])
print(df)

# Output:    A  B  C
#         x  1  2  3
#         y  4  5  6
#         z  7  8  9
```

```Python
import pandas as pd
from pandas import DataFrame
df = DataFrame([[5,6,8],[9,2,1],[3,5,6]], columns=["A", "B", "C"], index = ["x","y","z"])
print(df.max())
print(df.min())
# Output: A    9
#         B    6
#         C    8
#         dtype: int64
#         A    3
#         B    2
#         C    1
#         dtype: int64
```

## Intro to Series
```Python
import pandas as pd
from pandas import Series
df = Series([1,2,3], index = ["x","y","z"], dtype="int32")
print(df)

# Output:  x    1
#          y    2
#          z    3
#          dtype: int32


```