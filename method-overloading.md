## What is method overloading ?
If a class have multiple methods with same name but with different number of parameter or different order of parameters or different types of parameters is known as method overloading.

method overloading is not possible by changing the return type of the method only.

Calss cal {  
int add(int x,int y) {  
  return x+y;  
    }
int add(int x, int y, int z){  
  return x+y+z;  
   }
}

###  Why we need method overloading ?
Suppose we have to perform addition of given number but there can be any number of arguments,   
if we write method such as a(int, int) for two arguments, b(int, int, int) for three arguments then it is very difficult for you   
and other programmer to understand purpose or behaviors of method they can not identify purpose of method.   
So we use method overloading to easily figure out the program. 

For example above two methods we can write sum(int, int) and sum(int, int, int) using method overloading concept.
