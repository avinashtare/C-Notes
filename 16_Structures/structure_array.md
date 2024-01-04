# Array With Structure
* We can store multiple structure in a single array in c++;

#### Array initialization
**syntax**
```cpp
    // create an array 
    structName arrayVariable[size];
```

#### Store Values
#### **syntax 1**
```cpp
   // create an array 
    structName arrayVariable[size];

    // declear sturct
    struct structName myStudent;

    // store value in struct
    myStudent.variableName_1 = value_1;
    myStudent.variableName_2 = value_2;

    // append value by index
    arrayVariable[0] = myStudent;
```

#### **syntax 2**
```cpp
   // create an array 
    structName arrayVariable[size];

    // store value in struct
    arrayVariable[0] = {value1,value2,value_n};
    arrayVariable[1] = {value1,value2,value_n};
```




#### Array Values Display
* Display Values Using Index
```syntax
   // create an array 
    structName arrayVariable[size];

    // store value in struct
    arrayVariable[0] = {value1,value2,value_n};
    arrayVariable[1] = {value1,value2,value_n};

    // display index 1 values
     arrayVariable[0].value1;
     arrayVariable[0].value2;
     arrayVariable[0].value3;

     
    // display index 2 values
     arrayVariable[2].value1;
     arrayVariable[2].value2;
     arrayVariable[2].value3;
```
## Example

* write a program to store Person values in Person Structure Array and print it.
```cpp
#include <iostream>
#include <string>

using namespace std;

struct person
{
    string name;
    int age;
    int height;
};

int main()
{
    person PersonArray[1];

    // add value {name,age,height}
    PersonArray[0] = {"aviansh",34,134};

    // print
    cout<<PersonArray[0].name<<endl;
    cout<<PersonArray[0].age<<endl;
    cout<<PersonArray[0].height<<endl;

    return 0;
}

```

** write a program to store `multiple` Person values in Person Structure Array and `print using loop` it.
```cpp
#include <iostream>
#include <string>

using namespace std;

struct person
{
    string name;
    int age;
    int height;
};

int main()
{
    person PersonArray[5];

    // add value {name,age,height}
    PersonArray[0] = {"Aviansh", 34, 134};
    PersonArray[1] = {"Jimmy", 43, 134};
    PersonArray[2] = {"Supra", 23, 134};
    PersonArray[3] = {"Michael", 12, 134};
    PersonArray[4] = {"Johan", 53, 134};

    // print
    for (int i = 0; i < 5; i++)
    {
        cout<<"-------- Persont "<<i+1<<"--------"<<endl;

        cout << "Name: "<<PersonArray[i].name << endl;
        cout << "Age: "<<PersonArray[i].age << endl;
        cout << "Height: "<<PersonArray[i].height << endl<<endl;
    }

    return 0;
}

```



| [Back: Structures](./readme.md) | [Next: Nested Structure](./nested%20structure.md) |
| ----------------------------- | --------------------------- |