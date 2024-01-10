## 3. Without Parameters With Return Value Function.
**syntax** 
```cpp
returnType FunctionName(){
    // statements

    return <value>
}

FunctionName()
```

**Example** 
* sum of tow numbers using function.
```cpp
#include <iostream>

using namespace std;

// declear
int sum()
{
    int a, b;
    cout << "Enter Two Numbers:- ";
    cin >> a >> b;
    int c = a + b;
    // return addition 
    return c;
}

int main()
{
    // calling function
    int c = sum();
    cout << "Sum:-  "<< c;
    return 0;
}
```

* we only return that value we written before function name.i.e. int,float.
* if we created int function we can't return value type of float or string.
* we can create any return type functions like int float,bool etc.



| [2. Parameters return without value ](../User-Defined/with-para-no-return-function.md)  | [ 4. Parameters with return value ](./with-para-with-return-function.md) | 
| ------------------------------- | ------------------------------------------------------------------------------------ |
