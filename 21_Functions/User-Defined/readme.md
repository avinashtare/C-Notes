# User Defind Functions In C++

* User defind function is written by programmer accordin to it's need.
* This functions can be modify and manipulate by the programmer.
* we can create this function and call.
* Now, we only learn `main` fucntion it's is a user defind function.

#### **Declare Function** 
*  **syntax**

    ```cpp
    returnType FunctionName(parameter){
        // statement
        return <value>;
    }
    ```
* `returnType :` it's a return datatype of function like int,flaot, etc.
* `FunctionName()`:- name of the function it's used to call a function.All [Identifiers](../../05_Identifiers/readme.md) rules apply for function name. 
* `(parameter):` accept all the variables in side function to perform some action.
* `return :` it's used to return values after some action.
Note:- void return type is not return any value.

**Example:**
```cpp
void sum(){
    int a = 10;
    int b = 20;
    cout<<"Sum:- "<<a+b;
}
```
#### **Calling Function** 
* before calling function it must be declare.
* we can pass arguments to the function.
* return value can be store inside of variable.
* don't forgot to  add `;` semocolon after calling function.
  **syntax**
    ```cpp
    FunctionName(arguments);
    ```
* `FunctionName(); :`name of function you want to call.
* `(arguments):` send variable values to function.we can send pointers also.

**Example:**
```cpp
sum();
```

## 4 Way To Write Function
1. No parameters and no return value.
2. Parameters return without value.
3. Without parameters return value.
4. Parameters with return value.

| [ 1. No parameters and no return value ](./User-Defined/no-para-no-return-function.md) | [2. Parameters return without value ](./User-Defined/with-para-no-return-function.md) |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------ |

| [ 3. Without parameters return value ](./User-Defined/no-para-with-return-function.md) | [ 4. Parameters with return value ](./User-Defined/with-para-with-return-function.md) |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------ |

