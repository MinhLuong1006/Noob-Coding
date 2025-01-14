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
	cout << "Numbers that can be expressed by the sum of two prime numbers: " << endl; 
	for (int i = 0; i < n; i++) 
	{ 
		int num = arr[i]; 
		for (int p1 = 2; p1 < num; p1++) 
		{ 
			bool isPrime1 = true; 
			for (int j = 2; j <= p1 / 2; j++) 
			{ 
				if (p1 % j == 0) 
				{ 
					isPrime1 = false; 
					break; 
				} 
			} 
			if (isPrime1) 
			{ 
				int p2 = num - p1; 
				bool isPrime2 = true; 
				if (p2 > 1) 
				{ 
					for (int j = 2; j <= p2 / 2; j++) 
					{ 
						if (p2 % j == 0) 
						{ 
							isPrime2 = false; 
							break; 
					    } 
				    } 
			    } 
				else 
				{ 
					isPrime2 = false; 
				} 
				if (isPrime2) 
				{ 
					cout << num << " "; 
					break; 
				} 
			} 
	    } 
	} 
	return 0; 
}
```