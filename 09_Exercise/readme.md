# Exercise 9

### 1. Write a program to accept tow number from user and print sum of that number.
` Solution:- `
```c++
#include <iostream>

using namespace std;
int main(void)
{
    int x, y,s;

    cout<<"Enter First Number:- ";
    cin>>x;

    cout<<"Enter Second Number:- ";
    cin>>y;

    s = x+y;

    cout<<"Sum:- "<<s;
    return 0;
}
```


### 2. Write a program to accept tow number from user and print multiplication of that number.
` Solution:- `
```c++
#include <iostream>

using namespace std;
int main(void)
{
    int x, y,m;

    cout<<"Enter First Number:- ";
    cin>>x;

    cout<<"Enter Second Number:- ";
    cin>>y;

    m = x*y;

    cout<<"Addition:- "<<m;
    return 0;
}
```
### 3. Write a program to a accept number from user and print cube of that number.
` Solution:- `
```c++
#include <iostream>

using namespace std;
int main(void)
{
    int x,m;

    cout<<"Enter Number:- ";
    cin>>x;

    m = x*x*x;

    cout<<"Cube:- "<<m;
    return 0;
}
```
### 4. Write a program to a accept width and height from user and print area of rectangle.
` Solution:- `
```c++
#include <iostream>

using namespace std;
int main(void)
{
    int width,height,area;

    cout<<"Enter Width Of Reactangle:- ";
    cin>>width;

    cout<<"Enter Height Of Reactangle:- ";
    cin>>height;

    area = width*height;

    cout<<"Area Of Reactangle:- "<<area;
    return 0;
}
```
### 5. Write a program to a accept a number from user and check it's odd or even using ternary operator.
` Solution:- `
```c++
#include <iostream>

using namespace std;
int main(void)
{
    int num;

    cout<<"Enter a number- ";
    cin>>num;

    num%2==0?cout<<num<<" is even number":cout<<num<<" is odd number";
    return 0;
}
```