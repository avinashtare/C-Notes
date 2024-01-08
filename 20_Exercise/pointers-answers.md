# Pointers: Answers

1. Declare an integer variable 'num' and a pointer 'ptr' to store its address. Initialize 'num' to 42 and print both the value and the address.
```cpp
#include <iostream>

using namespace std;
int main() {
    int num = 42;
    int *ptr = &num;

    cout << "Value of num: " << num << endl;
    cout << "Address of num: " << ptr << endl;

    return 0;
}
```

2. Create an array of integers named 'arr' with values 1, 2, 3. Declare a pointer 'p' and use it to print the elements of the array.
```cpp
#include <iostream>

using namespace std;
int main() {
    int arr[] = {1, 2, 3};
    int *p = arr;

    for (int i = 0; i < 3; ++i) {
        cout << "Element " << i << ": " << *p << endl;
        p++;
    }

    return 0;
}

```
3. Declare an array of characters named 'str' with the value "Hello". Create a pointer 'charPtr' and use it to print each character of the string.
```cpp
#include <iostream>

using namespace std;
int main() {
    char str[] = "Hello";
    char *charPtr = str;

    while (*charPtr != '\0') {
        cout << *charPtr << " ";
        charPtr++;
    }

    return 0;
}
```