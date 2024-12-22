#Cpp
```C++
#include <iostream>
using namespace std;
int main()
{
    int n;
    int remain;
    cin >> n;
    while(n!=0)
    {
        remain = n % 10;
        n = n /10;
        cout << remain;
    }
    return 0;
}
```