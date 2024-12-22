#Cpp 
```C++
#include <iostream>
using namespace std;
int main()
{
    cout<<"How many numbers? ";
    int n;
    cin >> n;
    int arr[n];
    int size = sizeof(arr)/sizeof(arr[0]); //Because an int has 4 bytes so we divide the size by a random element in the array, which is also an int, to get the correct count of elements.
    //we can also use vector<int> arr(x); then replace all the "size" with "x"
    for(int i = 0; i <=n-1; i++)
    {
        cin >> arr[i];
    }
    
    for(int i = 0; i < size-1; i++) //size-1 because the greatest number is always                                       at the bottom so no need to compare
    {
        for(int j = 0; j < size - 1 -i; j++) //size-1 and -i elements sorted
        {
            if(arr[j] > arr[j+1])
            {
                int temp = arr[j];
                arr[j] = arr[j+1];
                arr[j+1] = temp;
            }
        }
    }
    
    for(int i = 0; i < n; i++)
    {
        cout << arr[i] << " ";
    }
    return 0;
}

```