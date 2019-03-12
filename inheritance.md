
## What are the relationships ?
In real word every entity has it own individual functionality's but to make a system all this should be related in a relationship 

Ex: Training system  
 Entity's : student, master , class room, chars and board.

To make meaning full training system all this entity's are should be in a relation and should communicate each other systematically.   

#### Relationships in java

In java relationship always makes to understand how to reuse the feature from one class to another class

* Is-A  
  In Is-A relationship one class is obtaining the features of another class by using inheritance concept with extends keywords.

* Has-A  
  In Has-A relationship an object of one class is created as data member in another class the relationship between these two classes is Has-A.

### What is inheritance ?
The process where one class acquires the properties (methods and fields) of another.  
A class that is derived from another class is called a subclass (also a derived class, extended class, or child class).   
The class from which the subclass is derived is called a superclass(also a base class or a parent class).
```java
class Super{
   .....
   .....
}

class Sub extends Super{
   .....
   .....

}
class Calcu{ 
   int z;	
  public void addition(int x, int y){
      z = x+y;
      System.out.println("The sum of the given numbers:"+z);
   }
	
   public void Subtraction(int x,int y){
      z = x-y;
      System.out.println("The difference between the given numbers:"+z);
   }
   
}
public class ScintCalcu extends Calculation{      
   public void power(int x, int y){
      z = x*y;
      System.out.println("The product of the given numbers:"+z);
   }
}
Class Test{
   public static void main(String args[]){
      int a = 20, b = 10;
      ScintCalcu demo = new ScintCalcu ();
      demo.addition(a, b);
      demo.Subtraction(a, b);
      demo.power(a, b);      
   }
}

```

### Different types of inheritance

* Single inheritance 
* Multi Level inheritance
* Hierarchical inheritance 
* Multiple inheritance 


