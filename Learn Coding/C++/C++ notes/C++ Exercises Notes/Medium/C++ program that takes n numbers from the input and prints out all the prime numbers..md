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
	for (int i = 0; i < n; i++) 
	{ 
		cin >> arr[i]; 
	} 
		for (int i = 0; i < n; i++) 
	{ 
		int num = arr[i]; 
		bool isPrime = true; 
		if (num <= 1) 
		{ 
			isPrime = false; 
		} 
		else 
		{ 
			for (int i = 2; i <= num/2; i++) 
			{ 
				if (num % i ==0) 
				{ 
					isPrime = false; 
				} 
			} 
		} 
		if(isPrime) 
		{ 
			cout << num << " "; 
		}
	}	 	
}
```