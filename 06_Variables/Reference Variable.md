# Reference Variable In C++

* a reference variable is an alternative name for an existing variable.
* It provides a way to access the value of a variable through a different name.
* Reference variables are commonly used in functions for passing arguments by reference, allowing the function to modify the original values of the variables.

### Declaration and Initialization

* A reference variable is declared using the `&` symbol. The syntax for declaring a reference variable is as follows:

```cpp

data_type &reference_variable = original_variable;

```
Here, `data_type` is the type of the original variable, and reference_variable is the name given to the reference.

```cpp
int main() {
    int original = 42;
    int &ref = original;

    cout<<"Original: "<<original; // output 42
    cout<<"Reference: "<<ref; // output 42
    // Now 'ref' is an alias for 'original'
    return 0;
}
```