```C++
#include <iostream>
#include <cmath>
using namespace std;
int main()
{
    int i = 0;
    int n;
    int remain;
    cin >> n;
    int sum = 0;
    while(n!=0)
    {
        remain = n % 10;
        n = n /10;
        sum = sum + remain * pow(2,i);
        i++;
    }
   cout << sum;
    return 0;
}
```