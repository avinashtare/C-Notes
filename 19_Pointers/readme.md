* Pointers are variables that are used to `store` the `address of another variable`.
* Address of a variable is the memeory location number which is allotted to the variable.
* The Memory addresses are 1,2,3... and so on up to the capacity of the memory.
* The address is normally displayed in hexadecimal form.
* pointers unlike other variables do not store values. As staned they store address of other variables.
* `&` is a address of operator in c++.
* `*` is a value of operator in c++.

##### Syntax Of Pointer Declaration:
```cpp
DataType *ptr_name = &AnotherVariable;
```

* Where *DataType* is the data type of the variable to which the pointer is supposed to point.If We want a pointer to point to an integer then,we need to have the data type of the pointer as *int*,for a float type data pointer should also be of the *float* type and so on.
* The `ptr_name` is an identifier the name of the pointer.The same rules of identifiers apply to the pointer name as to any other variable declaration.
* The most importent diffrence in the declaration of a pointer is the "*" sign given before the poiner name.
* Hence, according to the syntax seen above,if we want to declare a pointer `int` type data then we can declare it as given in the example below:

##### Store Values
```cpp
int main()
{
    int x = 34;
    int *b = &x; // <-- store address of anoter variable

    // & <-- Address Of Variable
    cout<<"Address Of x: "<<&x<<endl;
    cout<<"Address Of b: "<<b<<endl;
     return 0;
}
```

##### Display Values
* we can access value using `*` value of operator.
```cpp
int main()
{
    int x = 34;
    int *b = &x; // <-- store address of anoter variable

    // & <-- Address Of Variable
    cout<<"Value Of x: "<<x<<endl;
    cout<<"Value Of b: "<<*b<<endl;
     return 0;
}
```

#### change value
* any variable value change it's refelect to all variable.
* before change value you must add `*` value of oprator
##### example 1
```cpp
int main()
{
    int x = 34;
    int *b = &x; variable

    x = 11; // <-- here change value

    // & <-- Address Of Variable
    cout<<"Value Of x: "<<x<<endl;
    cout<<"Value Of b: "<<*b<<endl;
     return 0;
}
```.
##### example 2
```cpp
int main()
{
    int x = 34;
    int *b = &x; variable

    *b = 11; // <-- here change value

    // * <-- Address Of Variable
    cout<<"Value Of x: "<<x<<endl;
    cout<<"Value Of b: "<<*b<<endl;
     return 0;
}
```
| [Next: Pointer To Pointer](./pointer-2-pointer.md) |
| -------------------------------------------------- |