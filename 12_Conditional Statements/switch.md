# Switch Case Statement

* some time we need to check multiple case of a particular condition. In such cases we used switch if else statements.
* using switch statements we can implement ladder if else much better way.

**syntax of switch statement**
```cpp
switch(expression / variable) {
    case <option_1>:
        // Code to be executed for option_1
        break
    case <option_2>:
        // Code to be executed for option_2
        break
    |
    |
    |
    case <option_n>:
    // Code to be executed for option_n
    break
    default:
        // Code to be executed if none of the cases match
}
```

**Example of Switch Statement**
* write a program to accept day of week and print day if day is invalid print default anything.

```c++
#include <iostream>

using namespace std;
int main()
{

    int day;
    cout << "Enter a day of Week:-";
    cin >> day;
    switch (day)
    {
    case 1:
        cout<<"Monday";
        break;
    case 2:
        cout<<"Turesday";
        break;
    case 3:
        cout<<"Wednesday";
        break;
    case 4:
        cout<<"Thursday";
        break;
    case 5:
        cout<<"Friday";
        break;
    case 6:
        cout<<"Saturday";
        break;
    default:
        cout<<"It's Not Day Of Week!";
    }
    return 0;
}
```

## fall through switch case
* In C++ programming languages the fall-through behavior in a switch statement refers to the phenomenon where, once a case is matched and its code block is executed, control doesn't automatically exit the switch block. Instead, it continues to the next case unless a "break" statement is encountered. This allows for executing multiple case blocks sequentially.

**example of fall through**
* write a code to accept a character from user and find it's vowel or not.

```cpp
#include <iostream>

using namespace std;
int main(){
    char c;
    cout<<"Enter a character:-";
    cin>>c;

    switch(c){
        case 'a':
        case 'e':
        case 'i':
        case 'o':
        case 'u':
        case 'A':
        case 'E':
        case 'I':
        case 'O':
        case 'U':
            cout<<c<<" is a vowel";
            break;
        default:
            cout<<c<<" is not a vowel";
            break;
    }
    return 0;
}
```