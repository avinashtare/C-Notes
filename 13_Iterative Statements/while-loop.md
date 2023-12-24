# while Loop
* while loop is an iterative statement.
* It is used to repeat a set of statements number of times.
* In the entry control loop number of iteration is known.
* In an entry controlled loop, the test condition is checked before entering the loop body.


**syntax**
```cpp
// initilization
while(condition)
{

  // statements;

  // increment / decrement / updating
}
```
* The operation of the while loop is such that,first the condition is checked.If the condition is true,then the statements are executed.Once the statements are executed.the condition is again checked and this keeps on repeting,until the condition is false.If the condition is false,the statements inside the loop are not executed,instead the control directly comes out of the loop

**Example**
* write a program to print 1 to 100 using while loop

```cpp
#include <iostream>

using namespace std;
int main(){
    int i = 1;

    while(i<=10){
        cout<<i<<endl;
        // increment i by 1
        i++;
    }
    return 0;
}
```