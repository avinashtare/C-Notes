# Pre-Defined Functions In C++
* Pre-defined functions often exist to carry out common tasks, such as: finding an average number. determining the length of a string.
* A pre-defind function used to reduce time and code complexity.
* we can make our own predefind-function and used in c++.
* before calling any pre-defind function we must include this function file in begining of the code.

**Syntax**
```
include <pre-defind.h>

function_name(arguments);
```

** example of find sqare root of number **
```
#include <iostream>
#include <math.h>

using namespace std;
int main()
{
    int n,s;
    cout << "Enter a number:- ";
    cin >> n;
    s = sqrt(n);
    cout<<"Sqare Root Of "<<n<<":- "<<s;
}
```
* in above example we used pre-defind library math.h it's give us additonal functions to play with maths.

#### Pre-Defnid Function Buit-In Library
1. [cmath](./cmath.md)
2. [string](./string.md)
3. [cctype](./cctype.md)

|[Back: UserDefin Function](../readme.md)|[Next: Function Overloading](../../Function-Overloading/readme.md)|
|--|--|