#Cpp 

```C++
#include <iostream> 
using namespace std; 
int main() 
{ 
	int n; 
	cout<< "How many numbers would you like to enter? "; 
	cin >> n;
	int num[n]; 
	int size = sizeof(num) / sizeof(num[0]);
	for (int i = 0; i < size; i++) 
	{ 
		cin >> num[i]; 
	} 
	int index = 0; 
	int result[n]; 
	for (int i = 0; i < n; i++) 
	{ 
		if (num[i] % 2 == 0) 
		{ 
			result[index] = num[i]; 
			index++; 
		} 
	} 
	for (int i = 0; i < n; i++) 
	{ 
		if (num[i] % 2 != 0) 
		{ 
			result[index] = num[i]; 
			index++; 
		} 
	} 
	for (int i = 0; i < n; i++)
	{
		cout << result[i];
	} 
	return 0;
}
	
```