# Classes Object In C++

* OOP stands for Object-Oriented Programming.
<br>

* Class:- A class is a user-defined data type.It is similar to a structure with the difference that it can also have functions besides data items. A structure, we have seen, can have only data variable but a class can have data members as well as functoin members.
<br>
* Object:- It is an instance or example of a class. You can imagine it to similar to a variable of class like we have a variable of a structure.

## Create a class
* In c++ To create class we used **class** key word:

##### syntax
```
class <Class_Name>{
    <Access_Specifier>:
    
    // variable 
    // methods/function
}
```

##### <Class_Name>:- Name Of The class name.

#### <Acess_Specifier>:
*  access specifiers are used to control the visibility of class members. 
* There are three access specifiers in C++: `public`, `private`, and `protected`. They determine how class members (variables and functions) can be accessed by other parts of the program.

* Public (public): Members declared as public are accessible from anywhere in the program. They can be accessed by objects of the class, as well as by non-member functions.

Example:
```
class MyClass {
public:
    int publicVar;
    void publicMethod() {
        // Code here
    }
};
```

* Private (private): Members declared as private are only accessible within the same class or by friend functions. They cannot be accessed by objects of the class or by non-member functions.

Example:
```
class MyClass {
private:
    int privateVar;
    void privateMethod() {
        // Code here
    }
};

```

* Protected (protected): Members declared as protected are similar to private members but have an additional level of access. They are accessible within the same class and by derived classes (classes that inherit from the base class). Protected members cannot be accessed by objects of the class or by non-member functions.
Example:
```
class BaseClass {
protected:
    int protectedVar;
    void protectedMethod() {
        // Code here
    }
};

```

#### Defind a class & object

```
#include <iostream>

using namespace std;
class car
{
private:
    int speed;

public:
    // method set speed
    void setSpeed(int s)
    {
        speed = s;
    }

    // method find speed
    int findSpeed()
    {
        return speed;
    }
};

int main()
{
    // Defind Class
    car suzuki;

    // call method 
    suzuki.setSpeed(20);

    // get method speed
    cout<<"Speed Of Car:- "<<suzuki.findSpeed();


    return 0;
}
```