# Array With Loops
In C++, you can loop through an array using various constructs. The most common methods are using a for loop or a range-based for loop. Here's an example of both:

1. Using a for loop:

```cpp
#include <iostream>

using namespace std;
int main() {
    const int size = 5;
    int myArray[size] = {1, 2, 3, 4, 5};

    for (int i = 0; i < size; ++i) {
        cout << myArray[i] << " ";
    }

    return 0;
}

```

* In the above example, the for loop initializes an index variable i to 0, and it increments i in each iteration until i is equal to the size of the array. Inside the loop, myArray[i] accesses each element of the array.

### Insert table of 2 value in array and print it using for loop

```cpp
#include <iostream>

using namespace std;
int main()
{
    int table_2[10];

    // inserting value 
    for (int i = 0; i < 10; i++)
    {
        table_2[i] = (i + 1) * 2;
    }

    // printing value
    for (int i = 0; i < 10; i++)
    {
        cout<<table_2[i]<<"\n";
    }

    return 0;
}
```

* print below array values using loop
values 10,83,93,73,45,84,78,15,12,45

```cpp
#include <iostream>

using namespace std;
int main()
{

    int data[10] = {10, 83, 93, 73, 45, 84, 78, 15, 12, 45};

    for (int i = 0; i < 10; i++)
    {
        cout << data[i] << " ";
    }

    return 0;
}
```


| [Back: Strings](./strings.md) | [Next: Operation](./operation.md) |
| ----------------------------- | --------------------------- |