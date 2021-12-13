**const keyword**
-Whenever const keyword is attached with any method(), variable, pointer variable and
with the object of a class it prevents that specific object/method()/variable to modify its data items value.


-constant variables: need to be initialized at the time of declaration as the const variable cannot remain un-initialized
ex "const int x=3 ;"



Const Keyword With Pointer Variables:

1) pointer pointing to a const value
   Syntax: "const data_type* var_name;"
   You can modify pointer itself but the object pointed to by pointer shall not be modified.
   used to make string or an array of elements unchangeable
       ~~~
            const int x=1 ;
            const int* ptr = &x;  
            *ptr = 5; // error
            ptr++;    // right
     ~~~

2) const pointer pointing to a value
   Syntax:"data_type* const var_name;"
   You are not allowed to modify the pointer but the object pointed to can be modified.
    ~~~
            int x = 1;
            int *const ptr = &x;  
            *ptr = 5; // right
            ptr++;    // error  
  ~~~

3) const pointer pointing to a const variable
   Syntax: "const data_type* const var_name;"
   in this case no change can happen to the pointer or the variable.


-A function() parameters and return type of function() can be declared as constant.

-constant member functions
The const member functions are the functions which are declared as constant in the program. The object called by these functions cannot be modified.
const keyword is usually used  so that accidental changes to object are avoided.
A const member function can be called by any type of object while non-const functions can be called by non-const objects only.

-the const nature of any object can be changed by const casting
 The syntax :
 "const_cast<type name>(expression) "





**The & operator **

-The ampersand symbol & is used in C++ as a reference declarator .
-Pointer operator & returns the address of a variable. For example &a; will give actual address of the variable.
~~~
         int target;
         int &rTarg = target;  // rTarg is a reference to an integer.
         // The reference is initialized to refer to target.
          void f(int*& p);      // p is a reference to a pointer
~~~
-You can use the & operator with overloaded functions only in an initialization or assignment where
 the left side uniquely determines which version of the overloaded function is used.


-&& is a logical operator AND , it returns true only when the 2 operands are true.

-In Bitwise operators supported by C++ language
 & >> Binary AND Operator copies a bit to the result if it exists in both operands.
 
ex -> Assume if A = 60; and B = 13; now in binary format they will be as follows −
      A = 0011 1100
      B = 0000 1101
      A&B = 0000 1100















#Refrences:


https://www.ibm.com/docs/en/i/7.2?topic=expressions-address-operator
https://www.tutorialspoint.com/cplusplus/cpp_operators.htm
https://www.geeksforgeeks.org/const-keyword-in-cpp/
https://stackoverflow.com/questions/21476869/constant-pointer-vs-pointer-to-constant
https://www.tutorialspoint.com/const-cast-in-cplusplus







