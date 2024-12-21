#### A perfect number is equal to the sum of its divisors excluding itself

```C++
#include <iostream>
using namespace std;
int main()
{
    int n;
    int remain;
    cin >> n;
    int sum = 0;
    
    for (int i = 1; i < n/2; i++) 
    {
        if(n%i == 0)
        {
            sum = sum + i;
        }
    }
    
    if(sum == n)
    {
        cout << "perfect";
    }
    else
    {
        cout << "not perfect";
    }
    return 0;
}
//i must be above 0 because dividing by 0 is illegal in programming and math. i < n is OK but i < n/2 makes the program run faster. Any number that is greater than n/2 can't be a proper divisor expept n itself. 
```