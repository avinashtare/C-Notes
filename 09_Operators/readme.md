# Operators In C++
* Operators are used to perform operations on variables and values.
* Operators perform some action on. 
* Operators are symbols that represent computations or operations on variables and values.
* In C++ There are 3 types of Operators as Below:-

    1. Unary Operator 
    2. Binary Operator
    3. Ternary Operator

##  1. Unary Operator
* Unary operators in C++ are operators that operate on only one operand. 
* In other words, they perform an operation with a single variable or value
* There are several unary operators in C++, and here are some of the most common ones:
    1. Unary Plus (+):
    * unary plus operator is used to indicate the positive value of an expression
    Example:-
    ```cpp
         int x = -10;
        cout << x << " "; // Output: -10

        +x;

        cout << x << endl; // Output: 10

    ```
    2. Unary Minus (-):
    * The unary minus operator negates the value of its operand
    Example:-
    ```cpp
         int x = 10;
        cout << x << " "; // Output: 10
        
        -x;
        
        cout << x << endl; // Output: -10

    ```
    3. Increment (++):
    * The increment operator (++) is used to increase the value of its operand by 1.
    Example:-
    ```cpp
         int x = 10;
        cout << x << " "; // Output: 10
        
        x++;

        cout << y << endl; // Output: 11

    ```
    4. Decrement  (--):
    * The Decrement operator (--) is used to decrement the value of its operand by 1.
    Example:-
    ```cpp
        int x = 10;
        cout << x << " "; // Output: 10

        x--;

        cout << x << endl; // Output: 9
    ```




##  1. Binary Operator
* Unary operators in C++ are operators that operate on only tow operand. 
* In other words, they perform an operation with a two variables or value
* There are several binary operators in C++, and here are some of the most common ones:
### Types Of Binary Operator
##### 1. Arithmetic Operators.
##### 2. Relational Operators.
##### 3. Logical Operators.
##### 4. Assignment Operator

#### Arithmetic Operator
  1. ` + ` (addition).
 Example:
```c++
int x = 10;
int y = 30;
int z = x + y; // output:- 40
cout<<z;
```
  2. ` - ` (subtraction).
 Example:
```c++
int x = 50;
int y = 30;
int z = x - y; // output:- 20
cout<<z;
```
  3. ` * ` (multiplication).
 Example:
```c++
int x = 5;
int y = 3;
int z = x * y; // output:- 15
cout<<z;
```
  4. ` / ` (division).
 Example:
```c++
int x = 15;
int y = 3;
int z = x - y; // output:- 5
cout<<z;
```
  5. ` % ` (modulas) returns reminders.
 Example:
```c++
int x = 15;
int y = 3;
int z = x % y; // output:- 0
cout<<z;
```
6. ` ! `(Not Operator): it's returns true if the operand is false, and false if the operand is true.
```c++
 bool x = true;
 cout<<x<<endl; // output: 1
 cout<<!x<<endl; // output: 0
```

#### Relational Operator
relational operators are used to compare two values. These operators return a Boolean result, which is either true (1) or false (0)

* Types Of ` Relational  Operator. `
    1. ` == `(equal to): to compare two value are equal or not.
    2. ` != ` (Not equal to): Checks if the values on both sides are not equal.
    3. ` < ` (Less Then): Checks if the value on the left is less than the value on the right.
    4. ` <= ` (Less Then Equal): Checks if the value on the left is Less Then equal the value on the right.
    5. ` > ` (Greater Then): Checks if the value on the left is greater than the value on the right.
    6. ` >= ` (Greater Then Equal): Checks if the value on the left is greater than equal the value on the right.

#### Logical Operator
Logical operators in C are used to perform logical operations on Boolean values (true or false).

* Types Of ` Logical  Operator. `
    1. ` && `(END Operator): The logical AND operator returns true if both operands are true. otherwise, it returns false.
    2. ` || `(Or Operator): The logical OR operator returns true if  at least one operands are true.it returns false only if both operands are false.
    3. ` ! `(Not Operator): it's returns true if the operand is false, and false if the operand is true.

#### Assignment Operator
* Assignment operators are used to assign values to variables.
* Types Of Assignment Operator.
    1. `=` (assignment)
    2. `+=` (add and assign)
    3. `-=` (subtract and assign)
    4. `*=` (multiply and assign)
    5. `/=` (divide  and assign)
    6. `%=` (modulus  and assign)
    ` syntax `
    ```c++
    variable = expression;
    ```
* Example of Assignment Operator.
```c++
int a = 10;
int b = a; // its assigment operator 
cout<<b; // output: 10
```
* Example of add and assign.
```c++
int a = 10;
int b = 20;
b += a; // its add and assigment operator
cout<<b; // output: 30
```

#### Ternary Operator
The ternary operator, also known as the conditional operator, is a shorthand way of writing an if-else statement in C and many other programming languages. It is called "ternary" because it takes three operands. The basic syntax of the ternary operator is

syntax
```c++
condition ? expression_if_true : expression_if_false;
```
Here's how it works:
* The condition is evaluated first.
* If the condition is true, the expression immediately following the ? is evaluated and becomes the result of the entire expression.
* If the condition is false, the expression immediately following the : is evaluated and becomes the result.
Here's an example:
```cpp
    int x = 10;
    int y = 20;

    int result = (x > y) ? x : y; // result:- 20 
    cout<<result;
```