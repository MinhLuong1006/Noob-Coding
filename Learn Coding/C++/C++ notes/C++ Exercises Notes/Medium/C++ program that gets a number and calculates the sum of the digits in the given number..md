```C++
#include <iostream>
using namespace std;
int main()
{
    int n;
    int sum = 0;
    int remain;
    cin >> n;
    while(n!=0)
    {
        remain = n % 10;
        n = n /10;
        sum = sum + remain;
    }
    cout << sum;
    return 0;
}
```