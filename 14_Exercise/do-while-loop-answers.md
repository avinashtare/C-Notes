# Do-While Loop: Answers


### 1. Ask the user to guess a number between 1 and 100 using a do-while loop, and provide hints if the guess is incorrect.
```cpp
#include <iostream>

using namespace std;
int main()
{
    int n;
    int answer = 74;

    do
    {
        cout << "Guess The Number Between 1 to 100 :- ";
        cin >> n;

        if (answer < n)
        {
            cout << "You Guess Wrong Number Is Less Then " << n << endl;
        }
        else if(answer> n)
        {
            cout << "You Guess Wrong Number Is Grather Then " << n << endl;
        }
        else if(answer == n){
            cout << "You Guess Right Number Is " << n << endl;
        }
    } while (answer != n);

    return 0;
}
```
### 2. Let the user input a positive number. Repeat until a negative number is entered.
```cpp
#include <iostream>

using namespace std;
int main()
{
    int n;

    cout << "Enter The Positive Number :- ";
    cin >> n;

    do
    {
        cout << n << endl;
        n--;
    } while (n >= -1);

    return 0;
}
```
### 3. Ask the user to enter a password. Repeat until the correct password is entered using a do-while loop.
```cpp
#include <iostream>

using namespace std;
int main()
{
    string password = "@1234@pass";
    string EnteredPass;
    do
    {
        cout<<"Enter Your Correct Password:- ";
        cin>>EnteredPass;

        if(password!=EnteredPass){
            cout<<"Incorrect Password!"<<endl;
        }
        else if(password==EnteredPass){
            cout<<"You are login.";
        }
    } while (password!=EnteredPass);

    return 0;
}
```