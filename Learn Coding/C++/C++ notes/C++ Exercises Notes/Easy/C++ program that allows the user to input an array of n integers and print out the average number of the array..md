#Cpp
```C++
#include <iostream>
using namespace std;
int main()
{
    int arr[1000]; //This is what the lecturer wants.
    int ans;
    int sum = 0;
    
    int n;
    cout << "How many numbers would you like to enter? ";
    cin >> n;
    for (int i = 0; i < n; i++)
    {
        cin >> arr[i];
        sum = sum + arr[i];
    }
    ans = sum / n;
    cout << ans;
   return 0;
}
```
##### ----------------------------------------------------------------------------------------------

```C++
#include <iostream>
using namespace std;
int main()
{
    int ans;
    int sum = 0;
    int n;
    int arr[n+1]; //This is what we want.
    cout << "How many numbers would you like to enter? ";
    cin >> n;
    for (int i = 0; i < n; i++)
    {
        cin >> arr[i];
        sum = sum + arr[i];
    }
    ans = sum / n;
    cout << ans;
   return 0;
}
```