# cmath Library

the cmath library in C and C++ provides a set of functions that perform various mathematical operations. These functions cover a wide range of mathematical operations such as basic arithmetic operations, trigonometric functions, logarithmic functions, exponential functions, and more.
Here are some common functions provided by the cmath library:

1. Basic Arithmetic Functions:
* add(x, y): Adds two numbers.
* subtract(x, y): Subtracts one number from another.
* multiply(x, y): Multiplies two numbers.
* divide(x, y): Divides one number by another.

2. Trigonometric Functions:
* sin(x): Sine of x (x is in radians).
* cos(x): Cosine of x (x is in radians).
* tan(x): Tangent of x (x is in radians).

3. Exponential and Logarithmic Functions:
* exp(x): Calculates the exponential function e^x.
* log(x): Natural logarithm of x.
* log10(x): Logarithm base 10 of x.

4. Power Functions:
* pow(x, y): Raises x to the power y.

4. Square Root:
* sqrt(x): Square root of x.

5. Absolute Value:
* fabs(x): Absolute value of x.

#### example of find power of a number
```
#include <iostream>
#include <cmath>

using namespace std;

int main() {
    int num, power;
    cout << "Enter a number and power: ";
    cin >> num >> power;
    
    int result = pow(num, power);

    cout << "Power of " << power << " is " << result << endl;

    return 0;
}
```
|[Back: pre-defind function](./readme.md)|[Next: string.h](./string.md)|
|--|--|