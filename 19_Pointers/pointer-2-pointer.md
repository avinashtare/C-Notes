## Pointer
* a pointer to a pointer, commonly known as a double pointer, is a variable that holds the memory address of another pointer.
* It provides an additional level of indirection, allowing manipulation of pointers themselves. Pointers to pointers are particularly useful in scenarios where a function needs to modify the value of a pointer.

##### Syntax Of Pointer Declaration:
```cpp
DataType **ptr_name = &Pointer;
```


##### Store Values and display address and values
```cpp
int main()
{
    int x = 34;
    int *b = &x;
    int **c = &b; //<-- store value of pointer in pointer

    // & <-- Address Of Variable
    cout<<"Address Of x: "<<&x<<endl;
    cout<<"Address Of b: "<<b<<endl;
    cout<<"Address Of c: "<<c<<endl<<endl;

    
    // * <-- Value Of Variable
    cout<<"Value Of x: "<<x<<endl;
    cout<<"Value Of b: "<<*b<<endl;
    cout<<"Value Of c: "<<**c<<endl; // <-- print value
     return 0;
}
```


| [Back: Pointer](./readme.md) |
| ---------------------------- |