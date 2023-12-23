# Constant Variables In C++
The const keyword in C++ is a type qualifier that indicates that an object, variable, or function parameter is constant, and its value cannot be changed after initialization. Here are some common uses of the const keyword in C++

### Constant Variables:
it helps in creating symbolic names for values that should not be modified during the program's execution.

#### syntax
```cpp
const <datatype> <variable_name> = <value>;
```

#### examples
1. int
```cpp
const int MAX_Salary = 5000;

cout<<MAX_Salary;

MAX_Salary = 10000; ❌
```

2. float
```cpp
const float Intrest = 15.63;

cout<<Intrest;

Intrest = 10000; ❌
```

2. char
```cpp
const char Cname = 'A';

cout<<Cname;

Cname = `B`; ❌
```