```C++
#include <iostream>
#include <cstdlib>
#include <ctime>
using namespace std;
int main()
{
    srand((unsigned int) time(NULL)); //seeds the random num generator using the current time, if we don't have this line of code the random num every time we play the game will be the same.
    //time(NULL) returns a value type of time_t, which is an integer. srand() expects an unsigned int as its argument. This will explicitly casts the value, avoiding some errors. srand(time(NULL)) is still OK in most cases tho.
    //unsigned: not having a + or - sign.
    int num = rand()%100 + 1; //If it is only rand() % 100, the num will likely be in the range of 0-99 so we plus 1 and then it will be in the range of 1-100.
    int x;
    
    while (true)
    {
        cin >> x;
        if (x < num)
        {
        cout << "Too low! " << endl;
        }
        else if (x > num)
        {
        cout << "Too high! " << endl;
        }
        else if (x == num)
        {
            cout << "Congrats! " << endl;
            break;
        }
    }
    return 0;
}
```