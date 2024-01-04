# Nested Structure In C++
* When a structure contains another structure, it is called nested structure. 
* A structure consisting of such complex elements is called a complex structure.

**Syntax Initialization**

```c++
struct StructName{
    .
    .
    .
    struct StructName{
        .
        .
        .
    } calingName;
};
```

**Syntax Calling**

```c++
StructName.InnerStruct.variable = value;
```

**Syntax Add Value**

```c++
StructName.InnerStruct.variable = value;
```
**Example:**
```cpp
#include <iostream>

using namespace std;
struct Student
{
    int id;
    string name;
    int age;
    struct FeesStructure
    {
        int fees;
        int paid;
    } feesDetails;
};

int main()
{
    struct Student myStudent;

    // add values
    myStudent.id = 1;
    myStudent.name = "Avinash";
    myStudent.age = 12;
    myStudent.feesDetails.fees = 12344;
    myStudent.feesDetails.paid = 342;

    // display
    cout<<"Id: "<<myStudent.id<<endl;
    cout<<"Name: "<<myStudent.name<<endl;
    cout<<"Age: "<<myStudent.age<<endl;
    cout<<"Fees: "<<myStudent.feesDetails.fees<<endl;
    cout<<"Paid: "<<myStudent.feesDetails.paid<<endl;
    return 0;
}
```


| [Back: Array With Structure](./structure_array.md) 
| ----------------------------------------------- |