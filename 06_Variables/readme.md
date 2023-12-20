# Variables in C++
* In C++, a variable is essentially a named storage location in the computer's memory. This allows you to refer to and manipulate data stored in that location using the variable's name.
* Variables act as containers to hold different types of datatype.
* In C++, all the variables must be declared before use.
* All the operations done on the variable effects that memory location.

### Rules for declare a Variable in C++
    1. It's Contains `A-Z` and `a-z` and `0-9`.
    2. We Can Use Key Word As Variable.
    3. It's Must `Start's With alphabet`.
    4. It's Can't Contains blank space (`` ``) and special characters like \,>,&,^,$,#, etc.
    5. We Can Use Underscores `_` as Variable.

### diffrent type of variables

| id |   names   |                            store                                       |
| :- |:--------- | :--------------------------------------------------------------------- |
|  1 |    int    |           stores integers, without decimals, like `123` or `-123`      |
|  2 |    char   | stores single characters, like `A` only single word                    |
|  3 |   double  |  stores floating point numbers, with decimals, such as 19.99 or -19.99 :
|  4 |   string  |                       stores text values like `"hello word'`           |
|  5 |    bool   |                             store true or false                        |

etc..

### syntax
`datatype variableName = value;`

## Declare Multiple Variables
syntax: `datatype variable1,variable2,variable3`

## examples

### single declaration
* store integers
`int num = 12;`

* store characters
`` char c = 'A';``

* store boolean
`bool b = true;`

`bool d = false;`
* store string
`string myText = "Hello";s

### Multiple declaration
* store integers
```cpp 
int num1,num2;
num1 = 10;
num2 = 20;
```

* store characters
```cpp 
char c1,c2;
c1 = 'R';
c2 = 't';
```


### Local & Global Variable
* Global Variable:- we can access any where from the code.
* Local Variable:- we can access withen a block.

Example:- 
```cpp

#include <iostream>

// it's a global variable 
int a = 10;

using namespace std;
int main(void)
{
    // it's a local variable/
    int b = 20;
    cout<<"Global:- "<<a<<endl;
    cout<<"Local:- "<<b;
    return 0;
}

```