## cctype Library In C++

the cctype header provides functions that can be used to check and manipulate characters. These functions are similar to the ones available in the ctype.h header in C. Here are some commonly used functions from cctype.

#### 1. isalpha:
Checks if a character is an alphabetic character (A-Z or a-z).

```cpp
#include <iostream>
#include <cctype>

using namespace std;
int main() {
    char ch = 'A';

    if (isalpha(ch)) {
        cout << ch << " is an alphabetic character." << endl;
    } else {
        cout << ch << " is not an alphabetic character." << endl;
    }

    return 0;
}
```

#### 2. isdigit:
Checks if a character is a digit (0-9).

```cpp
#include <iostream>
#include <cctype>

using namespace std;
int main() {
    char ch = '5';

    if (isdigit(ch)) {
        cout << ch << " is a digit." << endl;
    } else {
        cout << ch << " is not a digit." << endl;
    }

    return 0;
}

```

#### 3. isalnum:
Checks if a character is an alphanumeric character (alphabetic or digit).

```cpp
#include <iostream>
#include <cctype>

using namespace std;
int main() {
    // allow:- 1,a,A etc...
    // not allow- @ % & * etc...
    char ch = '1';

    if (isalnum(ch)) {
        cout << ch << " is an alphanumeric character." << endl;
    } else {
        cout << ch << " is not an alphanumeric character." << endl;
    }

    return 0;
}
```

#### 4. isspace:

Checks if a character is a whitespace character (space, tab, newline).

```cpp
#include <iostream>
#include <cctype>

using namespace std;
int main() {
    char ch = ' ';

    if (isspace(ch)) {
        cout << ch << " is a whitespace character." << endl;
    } else {
        cout << ch << " is not a whitespace character." << endl;
    }

    return 0;
}
````

#### islower
check character is lower case or not.
```cpp
#include <iostream>
#include <cctype>

using namespace std;
int main() {
    char ch = 'A';

    if (islower(ch)) {
        cout << ch << " is a lower character." << endl;
    } else {
        cout << ch << " is not a lower character." << endl;
    }

    return 0;
}
```

#### isupper
check character is upper case or not.
```cpp
#include <iostream>
#include <cctype>

using namespace std;
int main() {
    char ch = 'A';

    if (isupper(ch)) {
        cout << ch << " is a upper character." << endl;
    } else {
        cout << ch << " is not a upper character." << endl;
    }

    return 0;
}
```

#### tolower
check character is lower is not convert into lower.

```cpp
#include <iostream>
#include <cctype>

using namespace std;
int main() {
    char ch = 'A';

    ch = tolower(ch);
    cout<<ch;

    return 0;
}
```
#### toupper
check character is upper is not convert into upper.
```cpp
#include <iostream>
#include <cctype>

using namespace std;
int main() {
    char ch = 'a';

    ch = toupper(ch);
    cout<<ch;

    return 0;
}
```

|[Back: string.h](./string.md)|[Next: Function Overloading](../../Function-Overloading/readme.md)|
|--|--|