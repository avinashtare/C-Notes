# Switch Case: Answers

### 1. Implement a basic calculator using a switch statement for addition, subtraction, multiplication, and division.
```cpp
#include <iostream>

using namespace std;
int main()
{
    // initialization
    int num1, num2, answer;
    char operation;

    // input first number
    cout << "Enter First Number:- ";
    cin >> num1;

    // input operation number
    cout << "Enter Operation Number:- ";
    cin >> operation;

    // input second number
    cout << "Enter First Second:- ";
    cin >> num2;

    switch (operation)
    {
    case '+':
        answer = num1 + num2;
        cout << "Answer:- " << answer;
        break;

    case '-':
        answer = num1 - num2;
        cout << "Answer:- " << answer;
        break;
    case '*':
        answer = num1 * num2;
        cout << "Answer:- " << answer;
        break;
    case '/':
        answer = num1 / num2;
        cout << "Answer:- " << answer;
        break;
    default:
        cout << "Invalid operation";
        break;
    }
    return 0;
}
```
### 2. Display the day of the week based on a user-provided number (1-7) using a switch statement.
```cpp
#include <iostream>

using namespace std;
int main()
{
    int day;

    cout << "Enter day of week:- ";
    cin >> day;

    switch (day)
    {
    case 1:
        cout << "It's Monday.";
        break;
    case 2:
        cout << "It's Tuesday.";
        break;
    case 3:
        cout << "It's Wednesday.";
        break;
    case 4:
        cout << "It's Thursday.";
        break;
    case 5:
        cout << "It's Friday.";
        break;
    case 6:
        cout << "It's Saturday.";
        break;
    case 7:
        cout << "It's Sunday.";
        break;

    default:
        cout << "This Day Not Exist In The Week.";
        break;
    }

    return 0;
}
```
### 3. Implement a program to convert temperature from Celsius to Fahrenheit and vice versa using a switch statement.
```cpp
#include <iostream>

using namespace std;
int main()
{
    int option;
    double celsius, fahrenheit;

    // goto statement
    start: 
        cout << "Choose Number Below:" << endl;
        cout << "1. Celsius to Fahrenheit." << endl;
        cout << "2. Fahrenheit to Celsius." << endl;
        cout << "> ";
        cin >> option;


    switch (option)
    {
    case 1:
        cout << "Enter Celsius:- ";
        cin >> celsius;

        fahrenheit = celsius * 9 / 5 + 32;
        cout << celsius << " Celsius is equal to " << fahrenheit << " Fahrenheit";
        break;
    case 2:
        cout << "Enter Fahrenheit:- ";
        cin >> fahrenheit;

        celsius = (fahrenheit - 32) * 5 / 9;
        cout << fahrenheit << " Fahrenheit is equal to " << celsius << " Celsius";
        break;

    default:
        goto start;
        break;
    }

    return 0;
}
```