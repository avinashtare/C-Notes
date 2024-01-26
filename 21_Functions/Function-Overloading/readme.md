# Function Overloading In C++

* Function overloading is c++ is techonic two or more functions can have the same name but different parameters.
* When same function name is overloaded with different jobs it is called Function Overloading. 
* In Function Overloading `Function` name should be the same and the arguments should be different.
* it's differ arguments and datatype.

#### Example
```cpp
#include <iostream>

using namespace std;

int sum(int a,int b){
    cout<<"Calling 2 arguments int \n";
    return a+b;
}
int sum(int a,int b,int c){
    cout<<"Calling 3 arguments int \n";
    return a+b+c;
}
float sum(float a,float b){
    cout<<"Calling 3 arguments float \n";
    return a+b;
}
int main()
{
    int a1 = 10;
    int a2 = 20;
    int a3 = 30;

    float b1 = 2.20;
    float b2 = 18.80;
    // calling same name 
    cout<<sum(a1,a2)<<endl;
    // diffrent datatype
    cout<<sum(b1,b2)<<endl;

    // 3 arguments
    cout<<sum(a1,a2,a3)<<endl;


    return 0;
}
```


|[Back: cctype](../User-Defined/Pre-Defined/cctype.md)|[Next: Recursion](../Recursion/readme.md)|
|--|--|