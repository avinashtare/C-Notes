# enum: Answers

1. Declare an enumeration named 'Weekdays' to represent the days of the week (Monday, Tuesday, ..., Sunday). Print the values of Monday and Friday.
```c++
#include <iostream>

// Declare the enumeration named 'Weekdays'
enum Weekdays {
    Monday,
    Tuesday,
    Wednesday,
    Thursday,
    Friday,
    Saturday,
    Sunday
};

int main() {
    // Print the values of Monday and Friday from the 'Weekdays' enumeration
    std::cout << "Value of Monday: " << Monday << std::endl;
    std::cout << "Value of Friday: " << Friday << std::endl;

    return 0;
}
```

2. Write a program in C++ that uses an enum to represent traffic light colors (Red, Yellow, Green). Accept user input for the current color and print the next color.

```cpp
#include <iostream>

using namespace std;
enum Light
{
    Red,
    Yellow,
    Green
};
using namespace std;
int main()
{

    int currentColor;
    cout << "Enter the current traffic light color (0: Red, 1: Yellow, 2: Green): ";
    cin >> currentColor;

    switch (currentColor)
    {
    case Red:
        cout << "Yellow";
        break;
    case Yellow:
        cout << "Green";
        break;
    case Green:
        cout << "Red";
    }

    return 0;
}
```