# If-Else: Answers

1. Check if a given number is even or odd.
```cpp
#include <iostream>

using namespace std;
int main()
{
    int n;

    cout<<"Enter a number:-";
    cin>>n;

    if(n%2==0){
        cout<<n<<" is a even number";
    }
    else{
        cout<<n<<" is a odd number";
    }

    return 0;
}
```
2. Determine if a year is a leap year or not.

```cpp
#include <iostream>

using namespace std;
int main()
{

    int year;

    cout<<"Enter a year:-";
    cin>>year;

    if((year%400==0 || year%4==0) && year%100!=0){
        cout<<year<<" is leap year";
    }
    else{
        cout<<year<<" is not leap year";
    }
    return 0;
}
```
3. Determine the largest of three numbers using if-else statements.
```c++
// Determine the largest of three numbers using if-else statements.
#include <iostream>

using namespace std;
int main()
{

    int first = 10;
    int second = 20;
    int third = 5;

    if(first>second && first>third){
        cout<<first<<" is Max Value";
    }
    else if(second>first&&second>third){
        cout<<second<<" is Max Value";
    }
    else if(third>first&&third>second){
        cout<<third<<" is Max Value";
    }
    else{
        cout<<"All the values are equal";
    }

    return 0;
}
```
4. Check if three given numbers can form a triangle or not.

```cpp
#include <iostream>

using namespace std;

int main() {
    double a, b, c;

    cout << "Enter three numbers (side lengths): ";
    cin >> a >> b >> c;

    if ((a + b > c) && (a + c > b) && (b + c > a)) {
        cout << "The given numbers can form a triangle.\n";
    } else {
        cout << "The given numbers cannot form a triangle.\n";
    }

    return 0;
}
```
5. Check if a given year is a century year (ending with 00) and a leap year.
```c++
#include <iostream>

using namespace std;

int main() {
    int year;

    cout << "Enter a year: ";
    cin >> year;

    if (year % 100 == 0) {
        // Check if a century year
        if (year % 400 == 0) {
            cout << year << " is a leap year and a century year.\n";
        } else {
            cout << year << " is a century year but not a leap year.\n";
        }
    } else {
        // Check if a non-century year
        if (year % 4 == 0) {
            cout << year << " is a leap year but not a century year.\n";
        } else {
            cout << year << " is neither a leap year nor a century year.\n";
        }
    }

    return 0;
}
```