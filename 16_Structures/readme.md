# Structures In C++

* a structure is a user-defined data type that allows you to group together variables of different data types under a single variable name.
* Structure is a collection of multiple data elements that can be of different data types.
* Array is a Collection of data ites of same data type,while structure can have data items of different type.
* The memory space require to store one variable of sturcture is equal to the memory space required by all  the elements independently to be stored in memory.
### 1. Initialization
**syntax Initialization**
```cpp
struct StructureName {
    // Member variables (data members)
    DataType1 variable_NAME;
    DataType2 variable_NAME;
    // ... (add more VARIABLE as needed)
};
```

**Explanation**:
* `struct`: The keyword used to declare a structure.
* `Datatype`: You can add any type of datatype here.
StructureName: The name of the structure.

### 2. Struct declaration
**syntax:** of declaration of a variable of structure:
```cpp
struct structure_name structure_variableName;
```
**syntax:** beginning of initializationa variablename for structure:

```cpp
struct StructureName {
    // Member variables (data members)
    DataType1 variable_NAME;
    DataType2 variable_NAME;
    // ... (add more VARIABLE as needed)
} structure_variableName; // <---------- here
```
### 3. Store Values
**syntax:** of store value in struct using datatype:
```cpp
struct structure_name structure_variableName;

structure_variableName.variableName_1 = value;
structure_variableName.variableName_1 = value;
```
**syntax:** of store value in struct using brakets:
```cpp
struct structure_name structure_variableName = {value_1,value2,value_n};
```
### 4. Access Valeus (print)
**syntax:** of access value in struct:
```cpp
struct structure_name structure_variableName;

cout<<structure_variableName.variableName_1;
cout<<structure_variableName.variableName_1;
```

#### **Example Of Student In Structure:**

```cpp
#include <iostream>

using namespace std;

// initialization
struct student{
    int RollNo;
    int age;
    int height;
    float fess;
};

int main()
{
    // declaration of new struct for student 1
    struct student s1;

    // store values for student 1
    s1.RollNo = 501;
    s1.age = 34;
    s1.height = 160;
    s1.fess = 63323.67;

    // display all the values
    cout<<"RollNo:- "<<s1.RollNo<<endl;
    cout<<"age:- "<<s1.age<<endl;
    cout<<"height:- "<<s1.height<<endl;
    cout<<"fess:- "<<s1.fess<<endl;
    return 0;
}
```
* **Example: Store Multiple Student Data Using Struct Structure:**
```
#include <iostream>

using namespace std;

// initialization
struct student
{
    int RollNo;
    int age;
    int height;
    float fess;
};

int main()
{
    // declaration of new struct for student 1
    struct student s1;
    // declaration of new struct for student 2
    struct student s2;

    // store values for student 1
    s1.RollNo = 501;
    s1.age = 34;
    s1.height = 160;
    s1.fess = 63323.67;

    // store values for student 2
    s2.RollNo = 524;
    s2.age = 14;
    s2.height = 180;
    s2.fess = 45789.67;

    // display all values of student 1
    cout << "Student 1" << endl;
    cout << "RollNo:- " << s1.RollNo << endl;
    cout << "age:- " << s1.age << endl;
    cout << "height:- " << s1.height << endl;
    cout << "fess:- " << s1.fess << endl;

        // display all values of student 2
    cout << "Student 2" << endl;
    cout << "RollNo:- " << s2.RollNo << endl;
    cout << "age:- " << s2.age << endl;
    cout << "height:- " << s2.height << endl;
    cout << "fess:- " << s2.fess << endl;
    return 0;
}
```


| [Next: Structure With Array](./structure_array.md) |
| -------------------------------------------------- |