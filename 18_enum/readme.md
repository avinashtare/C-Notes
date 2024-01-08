# Enum In C++

* An enumeration (enum) in C++ is a user-defined data type that consists of a set of named integral constants.
* Enums are used to make code more readable and maintainable by giving meaningful names to constant values.

##### 
```cpp Declaration 
enum EnumName {
    enumerator1,
    enumerator2,
    // ... additional enumerators
};
```
* EnumName: The name of the enum.
* enumerator1, enumerator2, ...: Constants or enumerators representing integral values.

##### Initializing Enumerators
Enumerators are implicitly assigned integral values starting from 0. You can explicitly assign values to enumerators if needed.

```c++
enum Days {
    Sunday,    // 0
    Monday,    // 1
    Tuesday,   // 2
    // ... and so on
};

```

##### Display Enums
```cpp
Days d1 = Sunday;
cout<<d1;
```

#### Example
```cpp
#include <iostream>

using namespace std;
int main()
{   
    // declaration 
    enum numbers {
        zero,
        one,
        tow,
        three,
        four,
        five
    };

    // add values 
    numbers n0 = zero;
    numbers n1 = one;
    numbers n2 = tow;
    numbers n3 = three;
    numbers n4 = four;
    numbers n5 = five;

    // values 
    cout<<n0<<endl; // 0
    cout<<n1<<endl; // 1
    cout<<n2<<endl; // 2
    cout<<n3<<endl; // 3
    cout<<n4<<endl; // 4
    cout<<n5<<endl; // 5
    return 0;
}
```