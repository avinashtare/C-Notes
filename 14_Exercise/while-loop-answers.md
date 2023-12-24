# While Loop: Answers
   
### 1. Determine if a given number is a prime number or using a while loop.
```cpp
#include <iostream>

using namespace std;
int main()
{

    int n = 0;
    int i = 2;
    bool isPrime = true;
    cout << "Enter a number:-";
    cin >> n;

    while (i <= (n / 2))
    {
        if (n % i == 0)
        {
            isPrime = false;
            break;
        }
        i++;
    }

    if (isPrime == true)
    {
        cout << n << " is a prime number";
    }
    else
    {
        cout << n << " is not a prime number";
    }

    return 0;
}
```

### 2. Print the [Fibonacci](https://en.wikipedia.org/wiki/Fibonacci_sequence) series up to the 20th term using a while loop.
```cpp
#include <iostream>
using namespace std;
int main() {
  int n1 = 0;
  int n2 = 1;

  int i = 0;
  while (i < 20) {
    cout << n1 << endl;

    int Fibonacci = n1 + n2;
    n1 = n2;
    n2 = Fibonacci;
    i++;
  }

  return 0;
}
```
### 3. Find the sum of digits of a given number using a while loop.
```cpp
input  output
121  : 4
564  : 15
13   : 4
```

```cpp
#include <iostream>
using namespace std;

int main()
{
    int n;
    int sum = 0;

    cout << "Enter a number:-";
    cin >> n;

    while (n != 0)
    {
        sum = sum + n % 10;
        n = n / 10;
    }
    cout << sum;
    return 0;
}

```