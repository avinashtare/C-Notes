# Strings
C++ strings provide a convenient and powerful way to handle sequences of characters. Unlike traditional C-style strings, C++ strings are part of the Standard Template Library (STL) and are implemented as a class called `std::string`. 

## 1. Including the <string> Header
Before using C++ strings, include the <string> header in your program:

```cpp
#include <string>
```

## 2. Creating Strings
###  Initialization
* direct Initialization
```c++
std::string str1;                 // Default initialization (empty string)
std::string str2 = "Hello, World!";     // Initialization with a C-style string
```
* using Std Initialization
```c++
using namespace std
int main(){
string str1;                 // Default initialization (empty string)
string str2 = "Hello, World!";     // Initialization with a C-style string
}
```

### Input from the User
```cpp
#include <iostream>
#include <string>

int main(){
string userInput;
cout << "Enter a string: ";
cin >> userInput;
return 0;
}
```

## 3. String Operations

### Concatenatio: add tow string
```cpp
string str1;
string result = str2 + "World!";   // Concatenation
cout<<result;

str1 += "Append ";                      // Append to an existing string
cout<<str1;
```
### Accessing Characters: Accessing individual characters
```cpp
string strval = "My Name Is John";
string firstChar = strval[0]; // Accessing individual using index of characters. 
cout<<firstChar; // M
```

### Substring: Accessing specific using index
```cpp
string strval = "My Name Is John";
string sub = strval.substr(0, 7); // Extract substring starting from index 0 with length 5
cout<<sub; // output: My Name
```
### Length: get the length of the string
```cpp
string strval = "My Name Is John";
string sub = strval.substr(0, 7); // Get a substring starting from index 0 with length 7
cout << sub;                      // Output: My Name
```