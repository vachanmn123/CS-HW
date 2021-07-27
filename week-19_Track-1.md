1. **Explain class definition and declaration with syntax and example.**
***

> **class**:  It is a user-defined data type, which holds its own data members and member functions, which can be accessed and used by creating an instance of that class. A C++ class is like a blueprint for an object  

Syntax for Class definition:
```cpp
class classname {
    Access Specifiers:
    data members;
    member functions(arguments) {}
};
```  
Example of class definition:
```cpp
class Student {
    public:
        string stdname;
        int stdid;

        void print_name();
};

void Student::print_name() {
    cout << stdname;
}
```  
***
***
2. **Explain with example member function definition inside the class .**
***  
> **definition inside the class:** The class member's definition is entirely inside the class body.  
```cpp
class ClassName {
    public:
    int number;

    void print_number() {
        cout << "Number is " << number << endl;
    };

};
```  
> **Definition outside the class:** The class member's definition is completely outside the class body  
```cpp
class ClassName {
    public:
    int number;

    void print_number();
};

void ClassName::print_number() {
    cout << "The number is " << number << endl;
}
```
***
***