# What is OOP?

* **Object Oriented Programming** as the name syes gives more significance to the object which has data and functions built around it.

* The data of the object can be accessed by the function associated with it.The functions of one object can access the data of another object through the function of that object.

* Object Oriented programming uses bottom up approach where the smaller task are first dealt in detail and gradually creating the entire hug system.

* Programs are divided into objects, the objects contain data and functions required to access them.

* More emphasis is given to data rather than procedure. It is seen in the real world problems that the data or the objects are more important than the procedure or the method to perform a task.Hance, in Object Oriented Programming, Object is given more importance compared to the procedure of doing it.

* Data is hideen or can't be access by external function. The data of an object can be accessed only by the functions of the same object.

* Objects communicate with  each other through functions.If a function of an object wants the data of another object then it can be accessed only through the functions. * New data and functions are easily added when required.Whenever new data is to be added,all the functions need not be changed only that functions are to be changed which required to access the data. * It follow a bottom-up approach. In this type of approach each element is first specified in detail and them the entire system is made using these elements. You will notice in the programming of C++, that this approach of bottom-up approach makes the programming very simple.

### The main principles of OOP include:

#### class
* Class It is a type or a category of things. It is similar to a structure with the difference that it can also have functions besides data items.
* A structure, we have seen, can have only data variables but class can have data members as well as funciton members.

#### Object
* It is an instance of a class. You can imagine it to be similar to a variable of class like we have a variable of a structure.

#### Data Abstraction
* Data abstraction is like defining or abstracting the object according to the required parameters. For example: if there is a class for car we have to just define the fule of the object of this class.
* We need not bother about anyting else of the object.

#### Data Encapsulation
* The data of an object is hidden from other objects. This is called as encapsulation.
* Encapsulation is achieved by putting data and functions associated with it into a class.
* The advantage of the data encapsulation is that the data is hidden from other functions and hence they can't access it or changed it directly.Thus the unexpected changes isn the data is not possible.

#### Inheritance
*Allowing a class (called a subclass or derived class) to inherit properties and behavior from another class (called a superclass or base class), facilitating code reuse and creating a hierarchy of classes.

#### Polymorphism
*  The ability for objects of different classes to be treated as objects of a common superclass, enabling a single interface to represent multiple types of objects. Polymorphism can be achieved through method overriding and method overloading.


## OOP VS POP

| Feature             | Procedural-Oriented Programming (POP)                                   | Object-Oriented Programming (OOP)                                            |
|---------------------|-------------------------------------------------------------------------|------------------------------------------------------------------------------|
| Main Focus          | Procedures and functions                                                | Objects and classes                                                          |
| Data and Functions	 | Data and functions are separate entities                                | Data and functions are encapsulated within objects                           |
| Code Organization   | Typically organized around functions                                    | Organized around objects and classes                                         |
| Reusability         | Functions can be reused, but often require passing multiple parameters	 | Objects and classes promote code reuse through inheritance and polymorphism  |
| Encapsulation       | Limited support for encapsulation                                       | Strong support for encapsulation                                             |
| Inheritance         | Not a built-in concept                                                  | Supports inheritance for code reuse                                          |
| Polymorphism        | Achieved through function overloading                                   | Supports polymorphism through method overriding and overloading              |
| Code Complexity     | Tends to become complex for large systems                               | Offers better manageability and scalability for large systems                |
| Examples            | C, Pascal, BASIC                                                        | C++, Java, Python, Ruby, C#                                                  |


|[Back: Exercise 22](../22_Exercise/readme.md)|[Next: Classes Object](../24_Classes_Object/readme.md)|
|--|--|