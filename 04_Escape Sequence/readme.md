## Escape Sequence
* An escape sequence is a sequence of characters that does not represent itself when used inside a string literal or character constant.
* It is a sequence of characters that begins with the backslash character `(/)`.
* The backslash character is used to tell the compiler that the character that follows it should be treated specially.
* Escape Sequence used especially perform some special operations like going to new line, providing a horizontal tab,vertical tab etc.

### Escape Sequence Type in c++

| syntax |      Action      | 
| :----- | | :------------- | 
|   \n   |  New Line        | 
|   \t   |  Horizontal Tab  | 
|   \v   |  Vertical Tab    | 
|   \\   |  Backslash       |   
|   \b   |  Backspace       |   
|   \'   |  Single Quote    |
|   \"   |  Double Quote    |
|   \?   |  Question Mark   | 
|   \0   |  Null Value      | 
|   \r   |  Carriage Return | 
|   \f   |  Form Feed       | 
|   \a   |  Audible Alert   |

### some example

1. New Line `(/n)`
```cpp
#include <iostream>

using namespace std;
int main()
{
    cout<<" one \n two!";
    return 0;
}
```

* `Output`
```cpp
 one
 two!
```

2. Horizontal Tab `(/t)`
```cpp
#include <iostream>

using namespace std;
int main()
{
    cout<<" one \t two!";
    return 0;
}
```

* `Output`
```cpp
 one     two!
```

3. Print a Number 1 to one line by line without using multiple cout
```cpp
#include <iostream>

using namespace std;
int main()
{
    cout<<"Here is 1 to 100 Numbers\n";
    cout<<"\n1\n2\n3\n4\n5\n6\n7\n8\n9\n10";
    return 0;
}
```

* `Output`
```cpp
Here is 1 to 100 Numbers
1
2
3
4
5
6
7
8
9
10
```

* Thanks For Reading...