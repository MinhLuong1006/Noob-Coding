#Cpp 

```C++
#include <iostream>
using namespace std; 
bool check(string s1, string s2) 
{ 
	int count = 0; 
	for(int i = 0; i < s1.length(); i++) 
	{ 
		for(int j = 0; j < s2.length(); j++) 
		{ 
			if(s1[i] == s2[j]) 
			{ 
				count +=1; 
			} 
		} 
	} 
	if (count == s1.length()) 
	{ 
		return true; 
	} 
	else 
	{ 
		return false; 
	} 
} 

int main() 
{ 
	string s1; 
	string s2; 
	cout << "Please enter the first string: "; 
	cin >> s1; 
	cout << "Please enter the second string: ";
	cin >> s2;
	if (check(s1, s2)) 
	{ 
		cout << "YES"; 
	} 
	else 
	{ 
		cout << "NO"; 
	}
	return 0;
}
```