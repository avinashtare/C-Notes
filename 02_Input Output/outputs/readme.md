# Output in C++.
### What is An Output?
* Output it's a value or data that you can print your screen.
## `cout`
* If we need to show some data on screen we used `cout` syntax.
* cout is alrady `defind` in header file in `iostream`.
* Hance,We Can't use cout as Identifiers. like variable name and function name etc.
## print text
```cpp
#include <iostream> 

int main() { 
    std::cout << "Hello, World!"; 
    return 0; 
}
```
* `syntax` std::cout << "Hello, World!"; 
* `Output` Hello, Word!

* we must use std:: it defind in iostream file to print text of any datatype
* you mast use `<<` for output.

### use without std
```cpp
#include <iostream> 

using namespace std;
int main() { 
    cout << "Hello, World!"; 
    return 0; 
}
```
* here we direct use without writing std.
* we have include std before the output.
* now we can write code without using std.

### way to write cout
1. multiple lines
```
#include <iostream>

using namespace std;
int main() {
    // Output to the console
    cout << "text1";
    cout << "text2";
    return 0;
}
```
* output:- ``text1text2``
### New Line
1. New line using endl
```
#include <iostream>

using namespace std;
int main() {
    // Output to the console
    cout << "text1"<<endl;
    cout << "text2";
    return 0;
}
```
* output:- 
```shell
text1
text2
```

* you must add `<<endl;` for new line.
* semicolon is required after endl;

2. New line without using endl

```cpp
#include <iostream>

using namespace std;
int main() {
    // Output to the console
    cout << "text1\n";
    cout << "text2";
    return 0;
}
```
* output:- 
```shell
text1
text2
```

* `\n` escape sequence used to new line.


## Practice Examples With Output
 1.
 ```cpp
#include <iostream>

using namespace std;
int main() {
    // Output to the console
    cout << "text 1"<<endl;
    cout << "text 2"<<endl;
    cout << "text 3"<<endl;
    return 0;
}
```
* Output 
```shell
text 1
text 2
text 3
```
2.
 ```cpp
#include <iostream>

using namespace std;
int main() {
    // Output to the console
    cout << "Avinash"<<endl<<endl;
    cout << "Rahul"<<endl;
    cout << "Rahul"<<endl;
    return 0;
}
```
* Output 
```shell
Avinash

Rahul
Rahul

```
 3.
 ```cpp
 #include <iostream>

using namespace std;
int main() {
    // Output to the console
    cout << "text1\n text2\n";
    cout << "text3";
    return 0;
}
```
* Output 
```shell
text1
text2
text3
```

 4.
 ```cpp
#include <iostream>

using namespace std;
int main() {
    // Output to the console
    cout << "Avinash"<<endl<<"avinash";
    cout << "Rahul"<<endl;
    cout << "Shubahm";
    return 0;
}
```
* Output 
```shell
Avinash
avinashRahul
Shubahm
```


 5.
 ```cpp
#include <iostream>

using namespace std;
int main() {
    // Output to the console
    cout << "Avinash"<<endl<<" Tare "<<endl;
    cout << "Rahul Tare"<<endl;
    cout << "Shubahm Babu";
    return 0;
}
```
* Output 
```shell
Avinash
 Tare
Rahul Tare
Shubahm Babu
```

#### Thanks for reading