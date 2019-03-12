## What is final ?
Whenever there is no more changes in the value then we will make it as final.

In Java final is used in several different contexts to define an entity that can only be assigned once.

Final can be using in front of variable, method and class.

### Final variable
A final variable can only be initialized once, either via an initializer or an assignment statement.   
It does not need to be initialized at the point of declaration: this is called a "blank final" variable. 

A blank final instance variable of a class must be definitely assigned in every constructor of the class in which it is declared

similarly, a blank final static variable must be definitely assigned in a static initializer of the class in which it is declared,  
otherwise, a compile-time error occurs in both cases.

Unlike the value of a constant, the value of a final variable is not necessarily known at compile time.  
It is considered good practice to represent final constants in all uppercase, using underscore to separate words.

```java
public class Sphere {
    // pi is a universal constant, about as constant as anything can be.
    public static final double PI = 3.141592653589793;
    public final double radius;
    public final double xPos;
    public final double yPos;
    public final double zPos;
    Sphere(double x, double y, double z, double r) {
         radius = r;
         xPos = x;
         yPos = y;
         zPos = z;
    }
}
```
### Final method 
A final method cannot be overridden or hidden by subclasses.  
This is used to prevent unexpected behavior from a subclass altering a method that may be crucial to the function or consistency of the class.

```java
public class Base
{
    public       void m1() {...}
    public final void m2() {...}

    public static       void m3() {...}
    public static final void m4() {...}
}


public class Derived extends Base
{
    public void m1() {...}  // OK, overriding Base#m1()
    public void m2() {...}  // forbidden

    public static void m3() {...}  // OK, hiding Base#m3()
    public static void m4() {...}  // forbidden
}

```

### Final class 

if a final variable holds a reference to an object, then the state of the object may be changed by operations on the object,   
but the variable will always refer to the same object . This applies also to arrays, because arrays are objects.  

A final class cannot be subclassed. Doing this can confer security and efficiency benefits,   
so many of the Java standard library classes are final, such as java.lang.System and java.lang.String.  
```java
public final class MyFinalClass {...}

public class ThisIsWrong extends MyFinalClass {...} // forbidden

```

