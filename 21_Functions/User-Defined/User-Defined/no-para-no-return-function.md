## 1. Without Parameters Without Return Value Function.

**syntax** 
```cpp
returnType FunctionName(){
    // statements
}
```

**Example** 
* sum of tow numbers using function.
```cpp
#include <iostream>

using namespace std;

// declear
void sum()
{
    int a, b, c;
    cout << "Enter Two Numbers:- ";
    cin >> a>>b;
    c = a + b;

    cout << "\nSum Of " << a << " " << b << " = " << c;
}

int main()
{
    // calling function
    sum();

    return 0;
}
```

* In above example we have `void` data type. void data type use in function for don't return any value.


|  [ Back: Function ](../readme.md)| [Next: Parameters return without value ](./with-para-no-return-function.md) |
| ------------------------------- | ------------------------------------------------------------------------------------ |
