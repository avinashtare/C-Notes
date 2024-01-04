# Union In C++

* A union in C++ is a user-defined data type that allows storing different data types in the same memory location.
* Unlike structures, which allocate memory for each member independently, unions share the same memory space for all members. 
* **Only one member of the union can be active at a time.**

##### Declaration Syntax
```cpp
union UnionName {
    datatype1 Variablename1;
    datatype2 Variablename2;
    // ... additional members
};
```

* UnionName: The name of the union.

#### Accessing Union Values

Since all members share the same memory space, only one member should be accessed at a time. The active member can be accessed using the union name followed by a dot`.` and the member name.
```cpp
UnionName myUnion;
myUnion.Variablename = value;  // Accessing and assigning values
```

##### Example
```

#include <iostream>

using namespace std;
union carPrice
{
    int rupee;
    int punds;
    int doller;
    int euro;
};
int main()
{

    // case 1
    carPrice price1;
    price1.rupee = 1234;
    cout << price1.rupee << endl;  // 1234
    cout << price1.doller << endl; // 1234

    // case 2
    price1.rupee = 7878;
    cout << price1.rupee << endl;  // 7878
    cout << price1.doller << endl; // 7878

    return 0;
}
```