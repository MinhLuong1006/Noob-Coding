#Cpp 

```C++
#include <iostream> 
using namespace std; 
int main() 
{ 
	cout << "How many numbers would you like to enter? "; 
	int n; 
	cin >> n; 
	int arr[n]; 
	for (int i = 0; i <n; i++) 
	{ 
		cin >> arr[i]; 
	} 
	int res = arr[0]; 
	for (int i = 1; i <n; i++) 
	{ 
		if (arr[i] > arr[i-1]) 
		{ 
			res = arr[i]; 
		} 
	} 
	cout << "The biggest number is: " << res; return 0; 
}
```