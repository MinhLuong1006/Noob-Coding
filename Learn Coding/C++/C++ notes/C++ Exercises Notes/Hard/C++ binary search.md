#Cpp
```C++
#include <iostream>
using namespace std;
void sort(int arr[], int size);
int binarysearch(int value, int arr[], int first, int last);

int main()
{
    cout<<"How many numbers? ";
    int n;
    cin >> n;
    int arr[n];
    int size = sizeof(arr)/sizeof(arr[0]);
    for(int i = 0; i <=n-1; i++)
    {
        cin >> arr[i];
    }
    sort(arr, size);
    int value;
    cout << "Enter the value to search for: ";
    cin >> value;

    int result = binarysearch(value, arr, 0, n - 1);

    if (result != -1) 
    {
        cout << "Value " << value << " found at index " << result << "." << endl;
    } 
    else 
    {
        cout << "Value " << value << " not found in the array." << endl;
    }

    return 0;
}

void sort(int arr[], int size)
{
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

}

int binarysearch(int value, int arr[], int first, int last)
{
    if (first > last)
    {
        return -1;
    }
    while (first <= last) 
    {
        int middle = first + (last - first) / 2; 

        if (arr[middle] == value) 
        {
            return middle; 
        } 
        else if (arr[middle] < value) 
        {
            first = middle +1; 
        } 
        else
        {
            last = middle -1; 
        }
    }
    
}
```