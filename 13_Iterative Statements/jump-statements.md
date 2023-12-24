# Jump Statements

* In C++, jump statements are special commands that allow the program to transfer control to different parts of the code.
* The jump main jump statements are:
    - break 
    - continue 
    - goto
    - return
* each serving a specific purpose in altering the flow of execution. While the `goto` statement also allows control transfer, its use is discouraged in modern C++ programming due to concerns about code readability and maintainability.

## break Jump Statement

* The break statement is used to exit from a loop or switch statement prematurely.
* It is commonly used in switch statements and loops (such as for, while, and do-while).

**syntax**
```cpp
break;
```
**Example**
```cpp
    for (int i = 0; i < 10; ++i)
    {
        if (i == 5)
        {
            break; // skip the rest of the loop when i is 5
        }
        // rest of the loop code
        cout << i << endl;
    }
```



## Continue Jump Statement

* The continue statement is used to skip the rest of the code inside a loop and jump to the next iteration of the loop.

**syntax**
```cpp
continue;
```
**Example**
```cpp
    for (int i = 0; i < 10; ++i)
    {
        if (i == 5)
        {
            continue; // skip the rest of the loop when i is 5
        }
        // rest of the loop code
        cout << i << endl;
    }
```


## goto Jump Statement
* The goto statement allows jumping to a labeled statement in the same function.
* While goto can be powerful, its use is generally discouraged as it can lead to unreadable and hard-to-maintain code. It can make the flow of the program less clear.

**syntax**
```cpp
goto:
    // statments
```
```cpp
void exampleFunction() {
    int i = 0;
    start:
        if (i < 5) {
            // do something
            ++i;
            goto start;  // jump to the 'start' label
        }
    // rest of the function code
}
```

## return Jump Statement
* The return statement is used to exit a function and return a value (if the function has a return type).

```cpp
int add(int a, int b) {
    return a + b;  // exit the function and return the sum of a and b
}
```