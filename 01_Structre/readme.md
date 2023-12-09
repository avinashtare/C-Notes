### Structure Of C++

## hello word print code
```cpp

#include <iostream>

int main() {
    // Output to the console
    std::cout << "Hello, World!";
    return 0;
}

```

### `include` 
* using include we can add header file to our program.
* is used to add extra features  nd in-build functions into our code.
* it's must defind top of the file.
### `include <iostream>`
* `iostream` is a in build file that use to run c program.
* This header includes the declarations for the standard input/output stream objects (cin for input and cout for output) and other related functionality 

### `int main(){ return 0; }`
* In the c programming function start's with main function.
* In the above case our code start with main fuction with intiger data type that means this functions return int value.(we will learn fuction in detaild).
* All then code inside of then main function which is start with `{` and ends with `}` all the code inside will run first.

`std::cout << "Hello, World!";`
* `std` is the predefind utility in c programming.which used to get input or print output on the screen.
* `cout<<"Hello Word!";` used to print output or some data on your output screen.
* you must declear `std::` before `cout` and then `<<` and `your data`;
* must use coloumn semicolon (;) after "" this.
* `return 0;` is run end of the code to compiler know your code is ended.