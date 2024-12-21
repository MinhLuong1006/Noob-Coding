```C++
#include <iostream>
using namespace std;
int main()
{
    bool isPrime = true;
    int n;
    cin >> n;
    if (n <= 1)
    {
        cout << n << " is not a prime number";
        return 1;
    }
    for (int i = 2; i < n/2; i++)
    {
        if (n % i ==0)
        {
            isPrime = false;
        }
    }
    if(isPrime)
    {
        cout << n << " is a prime number";
    }
    else
    {
        cout << n << " is not a prime number";
    }

    return 0;
}
```