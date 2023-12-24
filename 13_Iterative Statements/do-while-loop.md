* In this case the operation is different.first the statements are executed and then condition is checked.If the condition is false,then statements are not executed again.
* Do while loop statements are executed atleast once event if the condition is not true for the first statement.
Ex:-
```cpp
int i = 10;
do{
   cout<<i<<endl;
}while(i<0);
```

* in the above example loop is executed atleast onece event the i is grater then 10.

**Example of while loop**

* write a program to print table of 2.

```c++
#include <iostream>

using namespace std;
int main()
{
    int i = 1;
    do{
        cout << i * 2 << endl;
        i++;
    } while (i <= 10);

    return 0;
}
```