# Class Method

* Class Method are functions in class which can call when require.
* Class Method has power to manipulate variable of class.

##### In C++,There is tow why to defind a method in class:

- Inside class definition
- Outside class definition

### Inside class definition

* Defind Class Method Withen a class.
Example:
```
class MyClass_Inside {        // class
  public:              // Access specifier
    void customMethod() {  // Method/function defined inside the class
      cout << "Hello World!";
    }
};

int main() {
  MyClass_Inside myObj;     // Create an object of MyClass_Inside
  myObj.customMethod();  // Call the method
  return 0;
}
```

### Outside class definition
* Defind a class outside of a class using scope resolution `::` operator.
Example:

```
#include <iostream>

using namespace std;
class MyClass_Outside {        // The class
  public:              // Access specifier
  // Method/function declaration
    void Method();   
};

// Method/function definition outside the class
void MyClass_Outside::Method() {
  cout << "Hello World!";
}

int main() {
  MyClass_Outside myObj;     // Create an object of MyClass_Outside
  myObj.Method();  // Call the method
  return 0;
}
```