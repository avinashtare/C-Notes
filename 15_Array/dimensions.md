# Dimensional Of Arrays In C++

Arrays can be one-dimensional, two-dimensional, three-dimensional, and so on.

## 1. One-Dimensional Arrays:
* A one-dimensional array is a linear collection of elements stored in contiguous memory locations.
* Declaration and Initialization:
```cpp
int arr[5] = {1, 2, 3, 4, 5};
cout<<arr[0]; //output:- 1
cout<<arr[1]; //output:- 2
cout<<arr[2]; //output:- 3
cout<<arr[3]; //output:- 4
cout<<arr[4]; //output:- 5
```

* graphical look
| value | 1 | 2 | 3 | 4 | 5 |
|-------|---|---|---|---|---|
| index | 0 | 1 | 2 | 3 | 4 |

## 2. Two-Dimensional Arrays:
* A two-dimensional array represents a matrix or table with rows and columns.

**syntax**
```cpp
// Declaration
<datatype> <variable_name>[size][size] = {{value_1,value_n},{value_1,value_n}};

// access values
cout<<variable_name[size][size];
```
* Declaration and Initialization:
```cpp
int matrix[2][2] = {{1,2},{3,4}};

cout<<matrix[0][0]; // output:- 1
cout<<matrix[0][1]; // output:- 2
cout<<matrix[1][0]; // output:- 3
cout<<matrix[1][1]; // output:- 4
```
* graphical look.
![2d image](../assets/images/2d%20E1.png)

* Another exmaple of 2d array

```cpp
int matrix[3][3] = {{1,2,3},{4,5,6},{7,8,9}};

cout<<matrix[0][0]<<"\n"; // output:- 1
cout<<matrix[0][1]<<"\n"; // output:- 2
cout<<matrix[0][2]<<"\n"; // output:- 3

cout<<matrix[1][0]<<"\n"; // output:- 4
cout<<matrix[1][1]<<"\n"; // output:- 5
cout<<matrix[1][2]<<"\n"; // output:- 6

cout<<matrix[2][1]<<"\n"; // output:- 7
cout<<matrix[2][1]<<"\n"; // output:- 8
cout<<matrix[2][2]<<"\n"; // output:- 9
```
* graphical look.
![2d image](../assets/images/2d%20E2.png)


## 3. Multi-Dimensional Array
* Arrays with more than two dimensions are termed multidimensional arrays.

**syntax:**
```cpp
<datatype> <variable_name>[size_1][size_2]...[size_n];
```

**Example**
```cpp
int data[2][3][2] = {
    {{34, 21}, {84, 59}, {23, 43}},
    {{78, 15}, {94, 35}, {28, 48}},
};
cout<<data[0][0][0]<<"\n"; // output:- 34

cout<<data[0][1][0]<<"\n"; // output:- 84
cout<<data[0][1][1]<<"\n"; // output:- 59

cout<<data[1][1][0]<<"\n"; // output:- 94
cout<<data[1][2][1]<<"\n"; // output:- 48
```

| [Back: Array](./readme.md) | [Next: String](./strings.md) |
| -------------------------- | ---------------------------- |