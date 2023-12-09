# Inputs In C++.
`before learn input you must know datatype and variables. first learn that then leran this.`
### What is Input?
* When we want to get a value from user we used input.
* Value will be a intiger or string or image anything.
* Here we get value from user using `cin` utility.

### what is cin?
* we know cout is used to print output like this cin used to get value from user.
* like that cin used to get/accept values from user.
* is alrady `defind` in header file in `iostream`.
* Hance,We Can't use `cin` as Identifiers. like variable name and function name etc.
* it's a keyword.
### how to use
* `syntax:` cin>>(Identifier);
* you must user for store value in variable `>>`
* must use semicolon (;) after Identifier.
### Write a code to get a number from user and print it.

```cpp
#include <iostream>

using namespace std;
int main() {
    int number; // <-- difind a int variable
    
    cout << "Enter a number:-"; // <-- it's print only text
    cin>>number;// <-- store text
    cout<<"You Number is:- "<<number; //<-- print stored text
    return 0;
}
```
* `output:-`
```shell
Enter a number:-100
You Number is:- 100
````

# Examples
1. write a accept program two number and print that number

``` cpp
#include <iostream>

using namespace std;
int main(){
    int a;
    int b;

    // accept 1st number 
    cout<<"Enter First Number:-";
    // store fisrt number 
    cin>>a;
    
    // accept 2nd number
    cout<<"Enter Second Number:-";
    // store 2nd number
    cin>>b;

    // print tow numbers
    cout<<"First Number:- "<<a<<endl;
    cout<<"Second Number:- "<<b;
    
    return 0;
}
```
* `output:-`
```shell
Enter First Number:-40
Enter Second Number:-23
First Number:- 40
Second Number:- 23
````