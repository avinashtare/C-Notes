# string.h Library

The `string.h` library in C and C++ provides functions for manipulating C-style strings (character arrays). Here are some common functions:

### 1. String Copy (`strcpy`)

Copies the contents of one string to another.

```cpp
char destination[20];
char source[] = "Hello, World!";

strcpy(destination, source);
cout<<"\nOld: "<<destination<<"\nCopyed: "<<source;
```

### 2. String Concatenation (strcat)
Concatenates (appends) one string to the end of another.

```cpp
char str1[20] = "Hello, ";
char str2[] = "World!";
strcat(str1, str2);
cout<<str1;
```

### 3. String Length (strlen)
Returns the length of a string (excluding the null terminator).

```cpp
char myString[] = "Hello";
size_t length = strlen(myString);
cout<<(length);
```

### 4. String Comparison (strcmp)
* Compares two strings.
* if str equal then it's return 0 other wise -1.


```cpp
char str1[] = "apple";
char str2[] = "banana";
int result = strcmp(str1, str2);
if(result ==0){
   cout<<"Str1 is eqal to Str2"; 
}
else{
   cout<<"Str1 not eqal to Str2"; 
}
```

### 5. String Search (strstr)
Finds the first occurrence of a substring in a string.

```cpp
char sentence[] = "This is a sample sentence.";
char word[] = "is";
char *found = strstr(sentence, word);
cout<<(found);
```

### 6. String Tokenization (strtok)
Breaks a string into a sequence of tokens (substrings).


```cpp
char sentence[] = "This is a sample sentence.";
char *token = strtok(sentence, " ");
cout<<(token);
while (token != NULL) {
    // Process each token
    token = strtok(NULL, " ");
    cout<<" -- "<<token;
}
```

### 7. String Comparison (strncmp)
Compares the first n characters of two strings.

```cpp
const char str5[] = "apple";
const char str6[] = "apricot";
int result = strncmp(str5, str6, 3);  // Compare the first 3 characters
cout<<result;
```

### 8. String Reverse (strrev)
Reverses the characters in a string.

```cpp
char myString[] = "Hello";
cout<<strrev(myString);
```

|[Back: cmath function](./cmath.md)|[Next: cctype](./cctype.md)|
|--|--|