1. **Write syntax and example for structure definition and declaration?**
Ans. ***Structure definition syntax:***
```cpp
struct structureName{
  member1;
  member2;
  member3;
  .;
  .;
  .;
  memberN; 
};
```
  ***Stucture definition example:***
```cpp
struct student_info {
  int studentID;
  int grade;
  char section;
};
```
2. **Difference between structure and class.**
ans.
    (i) Members of a class are private by default and members of a struct are public by default.
    (ii) Class can have null values but the structure can not have null values.
    (iii) Memory of structure is allocated in the stack while the memory of class is allocated in heap.
    (iv) Classes support polymorphism and also be inherited but the structure cannot be inherited.

3. **Write a Program for array of structure.**
ans. 
```cpp
#include <iostream.h>

struct student
{
  int roll_no;
  int phone_number;
};

int main(){

	struct student stud[5];
  	int i;

	for(i=0; i<5; i++){
		cout << "Student " << i + 1 << endl;
		cout << "Enter roll no" << endl;
		cin >> stud[i].roll_no;
		cout << "Enter phone number" << endl;
		cin >> stud[i].phone_number;
	}

	for(i=0; i<5; i++){
		cout << "Student " << i + 1 << endl;
		cout << "Roll no : " << stud[i].roll_no << endl;
		cout << "Phone no : " << stud[i].phone_number << endl;
	}
	return 0;
}
```