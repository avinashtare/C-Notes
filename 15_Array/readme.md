# Array In C++
* Arrays are fundamental data structures in C++ that allow the storage of multiple elements of the same type in a contiguous block of memory. 
* It is a collection of multiple data of same data type.For Example we can have an array of int type data or float type data etc.
* Array can have data of same type only all elements of an array have to be same type only.
* We cannot have an array of combination of different data types.
* An array has static memory allocation memory size onece allocated for an array cannot be changed.
#### important points about array:
- The index of last element is n-1,where n is the size of the array.
- The starting index of the first element of an array is always zero.


**How Array Index And Value Works:**
| value | 1 | 20 | 3 |
|-------|---|----|---|
| index | 0 | 1 | 2  |

* you can access values using index.*
* if you want to access `20` you can access using `1` index.
**syntax:-**

- Declaration of array
```cpp
datatype <variablename>[size];
```
- Assign of array
```cpp
<variablename>[size] = {value1,value2};
```

- Access value of array.

```cpp
cout<<variablename[size];
```

**Example:-**
* Statically Declaration / Compile Time

```cpp
int data[3] = {1,2,3};

cout<<data[2]; // output:- 3
cout<<data[0]; // output:- 1
```


* Dynamically Declaration / Run Time
```cpp
int data[3];;

// declaration 
data[0] = 20;
data[1] = 5;
data[2] = 90;

cout<<data[2]; // output:- 90
cout<<data[0]; // output:- 20
cout<<data[1]; // output:- 5

// changed value dynamically run time 
data[1] = 45;
data[2] = 78;

cout<<data[1]; // output:- 45
cout<<data[0]; // output:- 20
cout<<data[2]; // output:- 78
```
* Note:- If you not declare any value in array it's stored default `garbage` value.

## Omit Array Size
* We don't have to specify the size of the array. The compiler is smart to determine the size of the array based on the number of added values
* No need to declare size.

```cpp
int marks[] = {343,342,234}; // Three array elements

cout<<marks[0] //output:- 343
cout<<marks[2] //output:- 342
cout<<marks[3] //output:- 234

````

| [Next:- Array Dimensions](./dimensions.md) |
| ------------------------------------------ |