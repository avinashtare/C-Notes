# if else
* This is very important statements used to check the condition and execute a set of statements,based on whether the condition is `true` or `false`.
* If condition is satisfied (true) run if block otherwice run else block.
* Hence it is called as `selective statements`. 

**syntax of if-else:**
```cpp

if(condition){

// if condition true execute this statements

}
else{

// if condition false execute this statements

}

```

* In c++ else statement is optional.we can have a if statement without the else statement.
**syntax of if:**
```cpp

if(condition){

// if condition true execute this statements

}

```

__if else example:__
* write a program to accept a number from user and find it's greater then 100.

```cpp
#include <iostream>

using namespace std;
int main()
{
    int n;
    cout << "Enter a number:-";
    cin>>n;

    if(n>100){
        cout<<n<<" is grather then 100";
    }
    else{
        cout<<n<<" is less then 100";
    }
    
    return 0;
}
```

# Ladder if-else
* some time we need to check multiple case of a particular condition. In such cases we used ladder if else statements.

**Syntax of Ladder if-else**

```cpp
if(condition){

}
else if(condition_1){
    // if satisfied condition 1
}
else if(condition_2){
    // if satisfied condition 2
}
|
|
else if(condition_n){
    // if satisfied condition n
}
else{
    // if not satisfied any condition
}
```
* In the above case compiler first check 1st condition if it's true then compiler execute code inside of the if statements.
* But if the condition is false it goes to the else if statement and check condition if ture execute statments inside else if. it's run antil the else if statments.
* At last if not satisfied any condition it's goes to else statement as default and run all then statments inside of then else statement.

__example of ladder if else statement__
* write a program to accept number between 1 to 5 and print word of the number.if the word is not between 1 to 5 print error.

```cpp

#include <iostream>

using namespace std;
int main()
{
    int n;
    cout << "Enter Number Between 1-5:- ";
    cin >> n;

    if (n == 1){
        cout << "One";
    }
    else if (n == 2){
        cout << "Two";
    }
    else if (n == 3){
        cout << "Three";
    }
    else if (n == 4){
        cout << "Four";
    }
    else if (n == 5){
        cout << "Five";
    }
    else{
        cout<<"Error";
    }

    return 0;
}
```