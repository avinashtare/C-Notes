# Methods Of Array
* Array methods are functions that can be applied to arrays in C++. 
* They can perform calculations or changes to arrays.
* save time by avoiding the need to write common functions from scratch.

## List Of Inbuild Functions In C++
| Function                                    | Description                                                                                          |
| ------------------------------------------- | ---------------------------------------------------------------------------------------------------- |
| `size(arr)` or `sizeof(arr)/sizeof(arr[0])` | Returns the number of elements in the array.                                                         |
| `sort(begin, end)`                          | Sorts the elements in the range `[begin, end)` in ascending order.                                   |
| `reverse(begin, end)`                       | Reverses the order of elements in the range `[begin, end)`.                                          |
| `find(begin, end, value)`                   | Searches for the first occurrence of `value` in the range `[begin, end)`.                            |
| `min_element(begin, end)`                   | Returns an iterator pointing to the minimum element in the range `[begin, end)`.                     |
| `max_element(begin, end)`                   | Returns an iterator pointing to the maximum element in the range `[begin, end)`.                     |
| `copy(begin, end, dest)`                    | Copies elements from the range `[begin, end)` to the destination array `dest`.                       |
| `fill(begin, end, value)`                   | Sets all elements in the range `[begin, end)` to the specified value.                                |
| `swap(arr1, arr2)`                          | Swaps the contents of two arrays.                                                                    |
| `binary_search(begin, end, value)`          | Performs binary search in the sorted range `[begin, end)` for the specified value.                   |
| `accumulate(begin, end, init)`              | Computes the sum of the elements in the range `[begin, end)` starting with the initial value `init`. |
| `begin(arr)`                                | Returns an iterator pointing to the beginning of the array or container.                             |
| `end(arr)`                                  | Returns an iterator pointing to the end of the array or container.                                   |

## Size Of Array
* Get the size of an array, you can use the sizeof() operator.
* It's returns the size of in bytes.

* find size of one element in bytes or all element in bytes in array.

* **`find a single element size in array in bytes`**
```cpp
    int arr[] = {2,2,3,4,5,6,7,8,9,0};
    cout<<sizeof(arr);
````

* **`find a all element size in array in bytes`**
```cpp
    int arr[] = {2,2,3,4,5,6,7,8,9,0};
    cout<<sizeof(arr);
````

* **`Find Length of element `**
```cpp
    int arr[] = {23,2,3,4,5,6,7,8,9,0};
    int arrayLenght = sizeof(arr) / sizeof(arr[0]);
    cout<<arrayLenght;
```

## Sort Array
* using sort function we can sort array element in c++.
* for use this function we need to include `<algorithm>` header.
* it's takes two parameters, the first being the point of the array from where the sorting needs to begin.
* second parameter being the length up to which we want the array to get sorted. 
* third parameter is optional and can be used in if we want to sort the elements lexicographically.

* **`Below is a program to show how sort() working.`**
```cpp
    int data[] = {100, 0, 3, 89, 5, 6, 45, 25, 90, 80};
    int dataayLenght = sizeof(data) / sizeof(data[0]);

    // find length of dataay
    int n = sizeof(data) / sizeof(data[0]);

    // this sort function to sort
    sort(data, data + n);

    // print sort 
    for (int i = 0; i < n; i++){
        cout << data[i] << " ";
    }
```

## Reverse Array Element
* using sort function we can reverse array element in c++.
* for use this function we need to include `<algorithm>` header.
* it's takes two parameters, the first being the point of the array from where the reversing needs to begin.
* second parameter being the length up to which we want the array to get sorted. 

* **`Below is a program to show how reverse() working.`**
```cpp
int data[] = {1,2,3,4,5,6,7,8,9};
int dataayLenght = sizeof(data) / sizeof(data[0]);

// find length of dataay
int n = sizeof(data) / sizeof(data[0]);

// this reverce function
reverse(data, data + n);

// print reverce 
for (int i = 0; i < n; i++){
    cout << data[i] << " ";
}
```

## Find Element In Array
* In C++, you can use various built-in functions and algorithms to find elements in an array. 
* One commonly used function for this purpose is std::find, which is part of the C++ Standard Template Library (STL). Here's an example:
```cpp
#include <iostream>
#include <algorithm>

using namespace std;
int main()
{

    // Example array
    int arr[] = {1, 2, 3, 4, 5};

    // Size of the array
    int size = sizeof(arr) / sizeof(arr[0]);

    // Element to search for
    int target = 3;

    // Use std::find to search for the element in the array
    int *result = std::find(arr, arr + size, target);

    // Check if the element was found
    if (result != arr + size)
    {
        std::cout << "Element found at index: " << (result - arr) << std::endl;
    }
    else
    {
        std::cout << "Element not found in the array" << std::endl;
    }

    return 0;
}
```

[Learn More About It](https://cplusplus.com/reference/array/array/)


| [Back: Operation Of Array](./operation.md) |
| ----------------------------- |