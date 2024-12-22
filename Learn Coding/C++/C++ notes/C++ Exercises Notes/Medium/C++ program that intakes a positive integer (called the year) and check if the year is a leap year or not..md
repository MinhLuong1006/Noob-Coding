#Cpp
###### A leap year has 366 days (the extra day is the 29th of February), and it comes after every four years. To check if a year is a leap year, divide the year by 4. If it is fully divisible by 4, it is a leap year. For example, the year 2016 is divisible 4, so it is a leap year, whereas, 2015 is not. However, Century years like 300, 700, 1900, 2000 need to be divided by 400 to check whether they are leap years or not.
```C++
#include <iostream> 
using namespace std; 
int main() 
{ 
 int year; 
 cout << "Enter a year: "; 
 cin >> year; 
 
 if (year < 0) 
 { 
	 cout << "The year need to be a positive number."; 
	 return 1;
 } 
 else 
 { 
	 if (year % 400 == 0) 
     { 
		 cout << year << " is a leap year."; 
     }
     else if (year % 4 == 0 && year % 100 != 0) 
     { 
		cout << year << " is a leap year."; 
     }
     else 
     { 
	     cout << year << " is not a leap year."; 
     }   
 }
 return 0; 
}
```

