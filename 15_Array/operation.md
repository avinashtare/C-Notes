# Array [Operation](../09_Operators/readme.md)
* We can perform any type of like arithmetic [operation](../09_Operators/readme.md) on array. For Ex:- +,-,*,/,% etc.
* you can perform various type of operation like `arithmetic`,`unary`,`binary`,`turnary`,`logical`,`relational` etc.

## 1. [Arithmetic](../09_Operators/readme.md) Operations:

* Addition Of Tow Array 
```cpp
int array1[2] = {1, 2};
int array2[2] = {6, 7};

// Addition
// first index addtion
int result_1 = array1[0] + array2[0];
// first second addtion
int result_2 = array1[2] + array2[2];

// result 
cout<<result_1<<"\n";
cout<<result_2;

// Subtraction, Multiplication, Division, Modulus
// Similar loops for other arithmetic operations
```

* Subtraction Of Tow Array 
```cpp
int array1[2] = {1, 2};
int array2[2] = {6, 7};

// Addition
// first index Subtraction
int result_1 = array1[0] - array2[0];
// first second Subtraction
int result_2 = array1[2] - array2[2];

// result 
cout<<result_1<<"\n";
cout<<result_2;

// Subtraction, Multiplication, Division, Modulus
// Similar loops for other arithmetic operations
```

* you can use loops.
```cpp
int array1[] = {1, 2, 3, 4, 5};
int array2[] = {6, 7, 8, 9, 10};
int result[5];

// Addition and store in result 
for (int i = 0; i < 5; ++i) {
    result[i] = array1[i] + array2[i];
}

// print value 
for (int i = 0; i < 5; ++i) {
   cout<<result[i];
}

// Subtraction, Multiplication, Division, Modulus
// Similar loops for other arithmetic operations
```

## 2. Comparison Operations:
* Similar loops for other comparison operations
* below code check value of array1 and array2 in equal by index;
```cpp
int array1[] = {1, 2, 2, 4, 5};
int array2[] = {6, 7, 2, 9, 5};

// Comparing arrays for equality
for (int i = 0; i < 5; i++) {
    if (array1[i] != array2[i]) {
        cout<<array[i]<<"\n";
        break;
    }
}
```

## 4.Other Operations:
* Finding the minimum or maximum element in an array.
* Reversing the order of elements in an array.
* Searching for a specific value in the array.
* Computing the sum, average, or other statistical measures.

| [Back: Loop Of Array](./loops.md) | [Next: Method](./method.md) |
| ----------------------------- | --------------------------- |

