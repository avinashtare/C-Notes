# For Loop: Answers
   
1. Print the first 10 natural numbers in reverse order using a for loop.
```cpp
#include <iostream>

using namespace std;
int main()
{

    for (int i = 10; i > 0; i--)
    {
        cout<<i<<"\n";
    }
    
    return 0;
}
```
2. Calculate the factorial of a given number using a for loop.
```cpp
#include <iostream>

using namespace std;
int main()
{
    int n = 5;
    cout<<"Which Number You Want To Find Factorail:-";
    cin>>n;
    int factorial = 1;
    for (int i = 1; i <= n; i++)
    {
        factorial *= i;
    }

    cout<<"Factorial Of "<<n<<":- "<<factorial;
    
    return 0;
}
```
3. Print the multiplication table of a given number using a for loop.

```cpp
#include <iostream>

using namespace std;
int main()
{
    int n = 5;
    cout<<"Which Number You Want To Find Table:-";
    cin>>n;
    for (int i = 1; i <= 10; i++)
    {
        int table = n*i;
        cout<<table<<endl;
    }

    return 0;
}
```

4.  Print Below Output.
```cpp
- output

*
**
***
```

```cpp
#include <iostream>

using namespace std;
int main()
{

    for (int i = 0; i < 3; i++)
    {
        for (int j = 0; j <= i; j++)
        {
            cout << "*";
        }

        // newline 
        cout << endl;
    }

    return 0;
}
```

5.  Print Below Output.
```cpp
output

***
**
*
```

```cpp
#include <iostream>

using namespace std;
int main()
{

  
    for (int i = 0; i < 3; i++)
    {
        for (int j = 1; j <= 3-i; j++)
        {
            cout << "*";
        }

        // newline 
        cout << endl;
    }

    return 0;
}
```


6.  Print a pattern of stars in the shape of a right-angled triangle using a for loop.
```cpp
- output

  *
 * *
* * * 
```

```cpp
#include <iostream>

using namespace std;
int main()
{

    for (int i = 0; i < 3; i++)
    {
        for (int j = 1; j < 3 - i; j++)
        {
            cout << " ";
        }

        for (int j = 0; j <= i; j++)
        {
            cout << " *";
        }

        cout << endl;
    }

    return 0;
}
```
