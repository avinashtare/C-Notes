## Comments In C Programming

### what is comments
*  comments are statment are not executed by the compiler or an interpreter
*. The comments are human-readable text or notes in the source code of a C program
* A comment makes the program easier to read and understand.

## Types Of Comments

| id | Type Of Comments|
| :- | :-------------- |
|  1 | Single Line     |
|  2 | Multiline Line  |

### 1. Single Line
* when we need to comment only a Single code we used Single line comments
* Single line comment begins with the `//`
* Any Text After `//` is ignored  by the compiler.
#### example 

```cpp
#include <iostream>

using namespace std;
int main()
{
    // i am a comment i will not execute
    cout<<"Hello, World!";
    return 0;
}
```

### 2. Multiline Line
* when we need to comment only a Multiple lines of code we used Single line comments.
* Single line comment begins with the `/*` and ends with `*/`.
* Any Text After `/*` and `*/` is ignored  by the compiler.
#### example 

```cpp
#include <iostream>

using namespace std;
int main()
{
    /* Bleow
    code
    is 
    print
    hello World
    in 
    screen 
    this all will ignoted by compiler
    */
    cout<<"Hello, World!";
    return 0;
}
```