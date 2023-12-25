# Strings In Array

* We can declared a variable that holds an array of strings.
* To insert values to string array and also store value.
* learn more about [string](../08_Strings/readme.md)

**example**
```cpp
#include <iostream>

using namespace std;
int main()
{
     string student[5] = {"avinash", "john", "rahul", "rajesh", "sumit"};
     
     cout<<student[0]; // output:- avinash
     cout<<student[1]; // output:- john
     cout<<student[2]; // output:- rahul
     cout<<student[3]; // output:- rajesh
     cout<<student[4]; // output:- sumit

     return 0;
}
```

**Find Size Of String**
```cpp
#include <iostream>

using namespace std;

int main() {
    string student[5] = {"avinash", "john", "rahul", "rajesh", "sumit"};

    // Use the length() member function to get the length of the C++ string
    int student_1_size = student[0].length();

    cout << "Length of the first student's name: " << student_1_size << endl;

    return 0;
}
```

* You Can add more method 
* get name from user and store in student
```cpp
#include <iostream>

using namespace std;

int main() {
    string student[5];

    cout<<"Enter your name:-";
    cin>>student[0];

    cout<<"Your Name Is:-"<<student[0];
    return 0;
}
```

| [Back: Dimensions](./dimensions.md) | [Next: Loops](./loops.md) |
| ----------------------------------- | ------------------------- |