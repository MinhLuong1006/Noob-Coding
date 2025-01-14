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
    int size = sizeof(arr)/sizeof(arr[0]); 
    cout << "Enter the numbers:" << endl;
    for(int i = 0; i < n; i++)
    {
        cin >> arr[i];
    }
    
    for(int i = 0; i < size-1; i++)                                     
    {
        for(int j = 0; j < size - 1 -i; j++) 
        {
            if(arr[j] > arr[j+1])
            {
                int temp = arr[j];
                arr[j] = arr[j+1];
                arr[j+1] = temp;
            }
        }
    }
    
    cout<< "Second largest number is: " << endl;
    cout << arr[n-2];
    
    return 0;
}
```