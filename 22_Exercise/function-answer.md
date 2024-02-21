## C++ Functions Answers

1. Create two functions in C++ - one to convert Celsius to Fahrenheit and another to convert Fahrenheit to Celsius.
**answer:**
```c++
#include <iostream>

using namespace std;

int C2F(int celsius){
    int Fahrenheit = (celsius * 1.8) + 32;
    return Fahrenheit;
}

int main(){
    int inputCelsius,outputFahrenheit;

    cout<<"Enter Celsius:- ";
    cin>>inputCelsius;

    outputFahrenheit = C2F(inputCelsius);
    
    cout<<inputCelsius<<" Celsius is equal to "<<outputFahrenheit<<" Fahrenheit";
    return 0;
}
```

2. Write a C++ function to find the sum of all elements in an integer array.
**answer:**

```c++
#include <iostream>

using namespace std;

int ArrSum(int sumArr[],int len)
{
    int sum = 0;
    for (int i = 0; i < len; i++)
    {
        sum += sumArr[i];
    }
    
    return sum;
}
int main()
{

    int arr[10] = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10};
    int arrLen = sizeof(arr) / sizeof(arr[0]);

    int arraySum = ArrSum(arr,arrLen);

    cout<<"Sum Of Given Arrray:- "<< arraySum;
    return 0;
}
```

3. Write a C++ function to check whether a given integer is a prime number or not. Test this function with different inputs.
**answer:**
```c++
#include <iostream>

using namespace std;

bool isPrime(int num) {
    if (num <= 1) {
        return false; // Numbers less than or equal to 1 are not prime
    }
    for (int i = 2; i * i <= num; ++i) {
        if (num % i == 0) {
            return false; // If num is divisible by any number less than or equal to its square root, it's not prime
        }
    }
    return true; // If the loop completes without finding a divisor, num is prime
}

int main() {
    int num;
    cout << "Enter a number: ";
    cin >> num;

    if (isPrime(num)) {
        cout << num << " is a prime number." << endl;
    } else {
        cout << num << " is not a prime number." << endl;
    }

    return 0;
}

```

4. Write a C++ function to addition of tow array.
**answer:**

```c++
#include <iostream>

using namespace std;

void ArrayAddition(const int arr1[], const int arr2[], int result[], int size) {
    for (int i = 0; i < size; ++i) {
        result[i] = arr1[i] + arr2[i];
    }
}

int main() {
    const int size = 5;
    int arr1[size] = {1, 2, 3, 4, 5};
    int arr2[size] = {6, 7, 8, 9, 10};
    int result[size];

    ArrayAddition(arr1, arr2, result, size);

    cout << "Resultant array after addition: ";
    for (int i = 0; i < size; ++i) {
        cout << result[i] << " ";
    }
    cout << endl;

    return 0;
}


```

###### Explanation:

* The function ArrayAddition takes two input arrays arr1 and arr2, their size size, and an output array result.
* It iterates over the arrays arr1 and arr2 and adds corresponding elements, storing the result in the result array.
In the main function, two arrays arr1 and arr2 are declared and initialized.
* The ArrayAddition function is called with these array result.


5. Create a recursive function to find the nth Fibonacci number.
**answer**

```c++
#include <iostream>

using namespace std;

int Fibonacci(int n) {
    if (n <= 1)
        return n;
    return Fibonacci(n - 1) + Fibonacci(n - 2);
}

int main() {
    int n;
    cout << "Enter the value of n to find the nth Fibonacci number: ";
    cin >> n;
    
    if (n < 0) {
        cout << "Invalid input. Please enter a non-negative integer." << endl;
        return 1;
    }

    cout << "The " << n << "th Fibonacci number is: " << Fibonacci(n) << endl;

    return 0;
}

```

6. Develop a recursive function to check if a given word is a palindrome.

```c++
#include <iostream>
#include <cstring>
#include <cctype>

using namespace std;

bool isPalindrome(const char *word, int start, int end) {
    // Base case: if start and end pointers cross each other or become equal
    if (start >= end)
        return true;

    // Ignore non-alphanumeric characters and convert to lowercase
    while (!isalnum(word[start]))
        start++;
    while (!isalnum(word[end]))
        end--;

    // If characters at start and end positions are not the same, it's not a palindrome
    if (tolower(word[start]) != tolower(word[end]))
        return false;

    // Recursive call with updated start and end pointers
    return isPalindrome(word, start + 1, end - 1);
}

int main() {
    char word[100];
    cout << "Enter a word to check if it's a palindrome: ";
    cin.getline(word, 100);

    if (isPalindrome(word, 0, strlen(word) - 1))
        cout << "\"" << word << "\" is a palindrome." << endl;
    else
        cout << "\"" << word << "\" is not a palindrome." << endl;

    return 0;
}

```