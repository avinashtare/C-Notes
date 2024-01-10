# Unions: Answers

1. Declare a union named 'Number' with members 'integer' and 'floatingPoint'. Initialize and print the values of both members.
```cpp
// 1. Declare a union named 'Number' with members 'integer' and 'floatingPoint'. Initialize and print the values of both members.
#include <iostream>

using namespace std;

union Number
{
    int integer;
    float floatingPoint;
};

int main()
{
    // Create an instance of the 'Number' union
    union Number myNum;

    // Initialize the values of both members
    myNum.integer = 20;
    myNum.floatingPoint = 34.44;

    // Print the values of both members
    cout << "a: " << myNum.integer << endl;
    cout << "b: " << myNum.floatingPoint << endl;

    return 0;
}
```
2. a union to represent a value as either an integer or a character. Accept user input for the value and print both representations.
```cpp
#include <iostream>

// Declare the union named 'Value'
union Value {
    int integerValue;
    char charValue;
};

int main() {
    // Create an instance of the 'Value' union
    union Value myValue;

    // Accept user input for the value
    std::cout << "Enter an integer value: ";
    std::cin >> myValue.integerValue;

    // Print the integer representation
    std::cout << "Integer Representation: " << myValue.integerValue << std::endl;

    // Print the character representation
    std::cout << "Character Representation: " << myValue.charValue << std::endl;

    return 0;
}

```