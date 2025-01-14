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
	for (int i = 0; i < n; i++) 
	{ 
		cin >> num[i]; 
	} 
	int index = 0; 
	int result[n]; 
	for (int i = n - 1; i >= 0; i--) 
	{ 
		result[index] = num[i]; 
		index++; 
	} 
	for (int i = 0; i <n; i++) 
	{ 
		cout << result[i] << " "; 
	} 
	return 0;
}
```