## What is method overriding?
Whenever same method name is existing in both base class and derived class with same types of parameters or same order of parameters is known as method Overriding. 

An instance method in a subclass with the same signature (name, plus the number and the type of its parameters) and return type as an instance method in the superclass overrides the superclass's method.

### Why we need method overriding?
Method Overriding is used to provide specific implementation of a method that is already provided by its super class.

Method Overriding is used for Runtime Polymorphism

```java
class Human { 
  void dressing(){
    System.out.println(“human dressing");
  }  
}  
 class Man extends Human{  
  void dressing(){
   System.out.println("Man dressing ”);
  }
}

class OverridingDemo{  
  public static void main(String args[]){  
    Man obj = new Man();  
    obj.dressing();  
    }
}

```
