#Cpp
#### Armstrong numbers are those numbers whose value is equal to the sum of digits of the number to their third power. Ex: 153 is an Armstrong number because 153 = 1^3 + 5^3 + 3^3.

```C++
#include <iostream>
#include <cmath>
using namespace std;
int main()
{
    int n;
    int sum = 0;
    int remain;
    cin >> n;
    int org = n;
    
    while(n!=0)
    {
        remain = n % 10;
        sum = sum + pow(remain,3);
        n = n /10;
    }
    
    if(sum == org)
    {
        cout << "armstrong";
    }
    else
    {
        cout << "not armstrong";
    }
    return 0;
}
```