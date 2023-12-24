# for Loop
* for loop is an iterative statement.
* It is used to repeat a set of statements number of times.
* In the entry control loop number of iteration is known.
* In an entry controlled loop, the test condition is checked before entering the loop body.

**syntax**
```cpp
for(initilizations;condition;increment / decrement / updating)
{


  // statements;


}
```
* The sequence of excecution of the for loop is such that initialization statements are executed first.These initilization statements are executed only onec.They are used to initilize the values of the variables.
* The second step is checking the condition specified.There can be only one condition.if more then one conditions are required they can be combined using the logincal AND,Or operator.If the condition is false the execution of the loop will be terminated.
* The third step is to execute all the statements inside the curly braces.These statements will be executed sequentially.The number of statements can be of any count.
* The fourth step is the increment/decrement or updating control variable.These operations are not necessarily increment or decrement operations,but monstly these are increment decrement.
* At the last control goes back to the second step.As said the first step is executed only ones,the steps that are repeated continuously are the second,third and fourth steps.Afte the fourth step the condition is checked again.If the condition is true the execution continues,else the condition goes outside of the loop.

**Example Of For loop**
* write a program to print your name 10 times

```c++
#include <iostream>

using namespace std;
int main()
{

    for (int i = 0; i < 10; i++){
        cout << "Avinash" << endl;
    }
    return 0;
}
```


## Nested Loop 
* Loop Within Loop is Called As Nested Loop
* Nested for loops in C++ are used when you need to iterate over multiple dimensions of data

```cpp
#include <iostream>

using namespace std;
int main()
{
    for (int i = 0; i < 3; i++)
    {
        for (int j = 0; j < 3; j++)
        {
            cout << i;
        }
        cout << endl;
    }

    return 0;
}
```