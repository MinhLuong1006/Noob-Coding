#Cpp
```C++

#include <iostream>
using namespace std;
int main()
{
    int n;
    int arr[n+1];
    cout << "How many numbers would you like to enter? ";
    cin >> n;
    if (n<=1)
    {
        cout << "Not enough numbers to compare!";
        return 1;
    }
    for (int i = 0; i < n; i++)
    {
        cin >> arr[i];
        
    }
    int smallest = arr[0]; 

    for (int i = 1; i < n; i++) 
    {
        if (arr[i] < smallest)
        {
            smallest = arr[i];
        }
    }
    cout << smallest;
   return 0;
}
```