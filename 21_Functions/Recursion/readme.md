# Recursion Function In C++
* Recursion is a programming concept where a function calls itself in its own definition.
* A function that calls itself is called a recursive function, and the process is known as recursion. 
* In C++, recursion is a powerful technique that can be used to solve problems in a more elegant and concise way.

* A recursive function generally has two parts:

1. Base Case: This is the termination condition that stops the recursive calls. Without a base case, the recursion would continue indefinitely.

* Recursive Case: This is the part where the function calls itself with modified arguments, moving closer to the base case.

Here's a simple example of a recursive function in C++ that calculates the factorial of a number:

```
#include <iostream>

// Recursive function to calculate factorial
int factorial(int n) {
    // Base case: factorial of 0 is 1
    if (n == 0) {
        return 1;
    } else {
        // Recursive case: n! = n * (n-1)!
        return n * factorial(n - 1);
    }
}

int main() {
    // Example usage of the recursive factorial function
    int result = factorial(5);
    std::cout << "Factorial of 5 is: " << result << std::endl;

    return 0;
}

```

In this example:

* The factorial function calculates the factorial of a number n.
* The base case is when n is 0, in which case the function returns 1.
* The recursive case multiplies n with the factorial of (n-1).
* It's important to ensure that the recursive function moves towards the base case, and there's a condition that stops the recursion. Otherwise, you can end up with infinite recursion, causing a stack overflow.

Recursion is a powerful technique, but it may come with a trade-off in terms of memory usage, as each recursive call adds a new frame to the call stack. It's often used when the problem naturally exhibits a recursive structure or when it leads to cleaner and more readable code.

|[Back: Function Overloading](../Function-Overloading/readme.md)|[Next: Exercise 22](../../22_Exercise/redme.md)|
|--|--|