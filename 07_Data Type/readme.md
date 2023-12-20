# Data Type

The type of values that can be stored in a variable depends on its data type. Data types in C++ define the nature of the data that a variable can hold, and they determine the range of values and operations that can be performed on those values. Choosing the appropriate data type for a variable is crucial as it influences the amount of memory allocated and the kind of operations that can be performed on the variable.

# Data Type In C++
- ## Fundamental/Pre-defined In Data Type
- ## User Defined Data Types 
- ## Derived Data Types

## Fundamental/Pre-defined In Data Type
fundamental or pre defind data type means which is alrady defind in a programming language.we can directly use those data types to store values.


| Type   | Typical Size | Typical Range                | Description                                       |
|--------|--------------|-----------------------------|---------------------------------------------------|
| int    | 4 Bytes      | -2,147,483,648 to 2,147,483,647 | Stores whole numbers, without decimals            |
| char   | 1 byte       | -128 to +127                 | Stores single characters.                         |
| float  | 4 bytes      | 1.2E-38 to 3.4E+38           | Stores decimal numbers. Sufficient for 6-7 decimal digits. |
| double | 8 bytes      | 2.3E-308 to 1.7E+308         | Stores decimal numbers. Storing 15 to 17 significant decimal digits. |
| bool | 1 bytes      | -         | Stores true or false |

Note:- c programming don't support string data type. 1 Byte is equal 4 bit.

### int Data Type
Range of the int data type is not strictly defined by the language standard, but it is commonly implemented as a 32-bit signed integer on many systems. The range of a 32-bit signed integer is typically from -2,147,483,648 to 2,147,483,647, inclusive.

Syntax
```c++
int <variable name> = value;
```
Example
```c++
int age = 21;
```

Note:- if we want to store big range of number we can user ` long int `

### char Data Type
char is a data type used to represent individual characters. It is one of the fundamental data types and is commonly used to store letters, digits, and other symbols. The char type is designed to hold a single character from the character set.

Syntax
```c++
char <variable name> = '<single character>';
```
Example
```c++
char First = 'A';
```

1. Size: In C++, the size of a char is always 1 byte.

2. Range: The range of values a char can represent depends on whether it is signed or unsigned. For a signed char, the typical range is from -128 to 127. For an unsigned char, the range is typically from 0 to 255. The signed or unsigned nature of char can vary between different systems.

3. Usage: char is commonly used to store individual characters, such as letters of the alphabet, digits, and special symbols.

4. Character Constants: In C++, character constants are enclosed in single quotes. Ex:- `'<value>'`


### float data type
float is a data type used to store decimal numbers. it's store 4 bytes of memory. Sufficient for 6-7 decimal digits.

Syntax
```c++
float <variable name> = value;
```
Example
```c++
float height = 4.12;
```
Note:- store more then 6-7 decimal values we used ` double `.

### bool data type
Bool is a data type used to store true or false. it's store only 1 bytes of memory.

Syntax
```c++
bool <variable name> = <true|false>;
```
Example
```c++
bool Earth_Is_Flat = false;
bool Earth_Is_Not_Flat = true;
```



## User Defined Data Types
use defind data type means user/programmer will create own data type which coming from pre-defind data type.

* structure
* union
* Enum

### Derived Data Types
Derived data tpe means those data type which derived from another data type & it can be predefine or  userdefind.

* array 
* function
* pointer


Checkout [Questions Of Datatype](./questions.md)