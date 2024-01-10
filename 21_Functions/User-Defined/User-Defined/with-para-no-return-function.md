## 2. Parameters Without Return Value Function.

**syntax** 
```cpp
returnType FunctionName(parameters){
    // statements
}

FunctionName(arguments)
```

**Example** 
* sum of tow numbers using function.
```cpp
#include <iostream>

using namespace std;

// declear with parameters
void sum(int x, int y)
{
    int z = x+y;

    cout << "\nSum Of " << x << " " << y << " = " << z;
}

int main()
{
    int a, b;
    cout << "Enter Two Numbers:- ";
    cin >> a>>b;
   
    // calling function and send arguemnts
    sum(a,b);

    return 0;
}
```

* In above function we sent arguemnts to the function add recived as parameters.
* we send a and b as argument ad recived as x and y respectively.
* we must add data tyep of parameters.


|  [ 1. No parameters and no return value ](./no-para-no-return-function.md) | [ 3. Without parameters return value ](./no-para-with-return-function.md) | 
| ------------------------------- | ------------------------------------------------------------------------------------ |
