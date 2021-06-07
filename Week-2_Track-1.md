1. **Explain with example call by value and call by reference**  
***   
**__Call by value:__**  
>Call by value means to pass to the function only the value of the variable. A copy of the data in the variable is created when a function is called by value.  

***example***
```cpp
void func(int inp){     //Pass by value
    cout << inp;
    inp = inp + 1;
}
```
In the above example when the function is called by passing a value, the data in the variable is copied and used inside the function after the function exits, that copy is destroyed leaving the original value intact.  
***
**__Call by reference:__**
>Call by reference means to pass to the function the memory location of the variable. No copy of the value is created in this case.  

***example***  
```cpp
void func(int &inp){
    cout << inp;
    inp = inp + 1;
}
```
In the above example when the function is called the memory location of the variable is passed so even when this function exits the value of the variable remains changed.
***