#Cpp
```C++
include <iostream> 
using namespace std;
int main() 
{ 
	int result = 0; 
	int day, month, year; 
	cout << "Please enter the day "; 
	cin >> day; 
	cout << "Please enter the month "; 
	cin >> month; 
	cout << "Please enter the year "; 
	cin >> year; 
	
	if (day <= 0 || month <= 0 || month > 12 || year <= 0) 
	{ 
		cout << "Invalid input. Please enter positive integers for day, month,           and year." << endl; 
		return 1; 
	} 
	else 
	{ 
		bool isLeap = false;
		 
		if (year % 400 == 0) 
		{ 
			isLeap = true; 
		} 
		else if (year % 4 == 0 && year % 100 != 0 ) 
		{ 
			isLeap = true; 
		} 
		else 
		{ 
			isLeap = false; 
		} 
		if (isLeap) 
		{ 
			int days[] = {31,29,31,30,31,30,31,31,30,31,30,31}; 
			if (day > days[month]) 
			{ 
				cout << "Invalid value because the day you enter is greater than                 the number of the days in the month"; 
				return 1; 
		} 
		else 
		{ 
			for(int i = 0; i < month - 1; i++) 
		{ 
		result += days[i]; 
		} 
		} 
	} 
	else if (!isLeap) 
	{ 
		int days[] = {31,28,31,30,31,30,31,31,30,31,30,31}; 
		if (day > days[month]) 
		{ 
		cout << "Invalid value because the day you enter is greater than the             number of the days in the month"; 
		return 1;
	} 
		else 
		{ 
			for(int i = 0; i < month - 1; i++) 
		    { 
			    result += days[i]; 
		    } 
	    } 
    } 
    } 
	 result += day; 
	 cout << result; 
	 return 0; 
}
```