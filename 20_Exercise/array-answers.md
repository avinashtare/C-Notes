# Structures: Answers

1.Declare a structure named 'Person' with members 'name' and 'age'.Accept user input for name and age and display it.

```cpp
#include <iostream>

using namespace std;

// person struct
struct Person
{
    string name;
    int age;
};

int main()
{
    struct Person p1;

    // accept values
    cout << "Enter Person Name:- ";
    cin >> p1.name;

    cout << "Enter Person Age:- ";
    cin >> p1.age;

    cout<<"Name:- "<<p1.name<<endl;
    cout<<"Age:- "<<p1.age<<endl;

    return 0;
}
```

2.Write a program uses a structure to represent a rectangle. Accept user input for the length and width, and then calculate and print the area of the rectangle.

```c++
#include <iostream>

using namespace std;

struct Rectangle
{
    int width;
    int height;
    int area;
};

int main()
{
    struct Rectangle rect1;

    cout << "Width:- ";
    cin >> rect1.width;

    cout << "Height:- ";
    cin >> rect1.height;

    cout << "Area Of Reactangle:- "<<rect1.width*rect1.height;

    return 0;
}
```

3.create a structure named 'Book' with members 'title', 'author', and 'publicationYear'.Accept user input for the title,author and publicatonYear and display the details of a book.

```cpp
#include <iostream>

using namespace std;

struct Book
{
    string title;
    string author;
    int publicationYear;
};

int main()
{
    struct Book book1;

    // get values 
    cout << "Book Title:- ";
    cin >> book1.title;

    cout << "Book Author:- ";
    cin >> book1.author;

    cout << "Book Publication Year:- ";
    cin >> book1.publicationYear;

    // print
    cout << "Book Title:- " << book1.title<<endl;
    cout << "Book Author:- " << book1.author<<endl;
    cout << "Book Publication Year:- " << book1.publicationYear;
    return 0;
}
```

4.Define a structure named 'Point' to represent a point members 'x' and 'y'. Calculate the distance between two points.
```cpp
#include <iostream>
#include <math.h>

// Declare the structure named 'Point'
struct Point
{
    double x;
    double y;
};
using namespace std;
int main()
{
    // Create instances of the 'Point' structure for two points
    struct Point point1, point2;

    // Initialize the coordinates of the first point
    cout << "Enter the coordinates of Point 1 (x y): ";
    cin >> point1.x>>point1.y;

    // Initialize the coordinates of the second point
    cout << ("Enter the coordinates of Point 2 (x y): ");
    cin >> point2.x>>point2.y;

    // Calculate and display the distance between the two points
    double distance = sqrt(pow(point2.x - point1.x, 2) + pow(point2.y - point1.y, 2));
    cout << "Distance between Point 1 and Point 2:- " << distance;

    return 0;
}
```

5.Create a structure named 'Employee' with members 'name', 'id', and 'salary'. Write a function to read an array of employees and find the employee with the highest salary.
```cpp
#include <iostream>

using namespace std;

struct Employee
{
    int id;
    string name;
    int salary;
};
int main()
{
    struct Employee employees[5];

    // insert values
    employees[0] = {1, "Rahul", 60000};
    employees[1] = {2, "Shubham", 40000};
    employees[2] = {3, "Jhon", 30000};
    employees[3] = {4, "Alex", 50000};
    employees[4] = {5, "Aysha", 70000};

    int highestSalary = 0;

    for (int i = 0; i < 5; i++)
    {
        int salary = employees[i].salary;

        // one line if statement
        if (salary > highestSalary)highestSalary = salary;
    }

    cout << "Highest Is Salary:- " << highestSalary;

    return 0;
}
```