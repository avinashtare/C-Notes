# Array: Answers

1.Declare an integer array named 'numbers' with a size of 5 and initialize it with values 1, 2, 3, 4, and 5. Print the elements of the array.

```cpp
#include <iostream>

using namespace std;
int main(){
    int numbers[5] = {1,2,3,4,5};

    for(int i =0;i<5;i++){
        cout<<"Index: "<<i<<" Value: "<<numbers[i]<<endl;
    }
}
```


2.Print reverse array.
```cpp
#include <iostream>

using namespace std;
int main()
{
    int arrSize = 10;
    int arr[arrSize] = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};

    for (int i = arrSize - 1; i >= 0; i--)
    {
        cout << "Value: " << arr[i] << endl;
    }

    return 0;
}
```


3.Given two sorted arrays, 'arr1' and 'arr2', merge them into a new array named 'mergedArr' while maintaining the sorted order. Assume 'mergedArr' has enough space to accommodate all elements.

```cpp
// Given two sorted arrays, 'arr1' and 'arr2', merge them into a new array named 'mergedArr' while maintaining the sorted order. Assume 'mergedArr' has enough space to accommodate all elements.
#include <iostream>

using namespace std;
int main()
{
    int arr1[] = {1, 3, 5, 7};
    int size1 = sizeof(arr1) / sizeof(arr1[0]);

    int arr2[] = {2, 4, 6, 8};
    int size2 = sizeof(arr2) / sizeof(arr2[0]);

    // size of array
    int arrSize = size1;
    if (size1 == size2)
    {

        int mergedArr[arrSize];

        // merge array
        for (int i = 0; i < arrSize; i++)
        {
            mergedArr[i] = arr1[i] + arr2[i];
        }

        // Print the merged array
        for (int i = 0; i < arrSize; ++i)
        {
            cout << arr1[i]<<" + "<<arr2[i]<<" = "<<mergedArr[i] << endl;
        }
    }
    else{
        cout<<"arr1 not equal to arr2";
    }

    return 0;
}
```
4.Write a program in C++ to find and print the largest element in an array.
```cpp
#include <iostream>

using namespace std;
int main()
{

    int arr[] = {34, 23, 532, 3112, 53, 12};
    int arrSize = sizeof(arr) / sizeof(arr[0]);
    int largeArray = 0;

    for (int i = 0; i < arrSize; i++)
    {
        // one line statement
        if (largeArray < arr[i])
            largeArray = arr[i];
    }
    cout << "Largest Element: " << largeArray;

    return 0;
}
```

5.Find Out Largest Sum In Array. Example:- Input: {1,2,3,4,34,3,69,6} Output:[69,69]

```cpp
#include <iostream>

using namespace std;
int main()
{

    int arr[] = {1, 2, 3, 4, 34, 3, 69, 6};
    int arrSize = sizeof(arr) / sizeof(arr[0]);

    int largSum[2] = {0, 0};

    for (int i = 0; i < arrSize; i++)
    {
        for (int j = 0; j < arrSize; j++)
        {
            // previous sum
            int preSum = largSum[0] + largSum[1];
            // current sum
            int nowSum = arr[i] + arr[j];

            // one line if statement
            if (preSum < nowSum)
            {
                largSum[0] = arr[i];
                largSum[1] = arr[j];
            }
        }
    }

    cout << largSum[0] << " " << largSum[1];

    return 0;
}
```