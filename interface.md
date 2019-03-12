
## Why we need Interface?
To achieve fully Abstraction.   
Contract b/w modules with loosely coupling.  
Multiple  inheritance.  
To achieve Dynamic polymorphism.   
To remove Conditional Code for Business entities.  

Interface contains only abstracted methods.  
All methods in interface are by default public abstract methods.  
All variables are by default public static final.  
Whey all variables are public static final?   
At least on concrete class should implements interface.  
An interface can extend another interface.  

The signature of the interface method and the same return type or subtype should be maintained when overriding the methods.  
An implementation class itself can be abstract and if so interface methods need not be implemented.  
Checked exceptions should not be declared on implementation methods other than the ones declared by the interface method or subclasses of those declared by the interface method.  

A class can implement more than one interface at a time.  
A class can extend only one class, but implement many interfaces.   
An interface can extend another interface, similarly to the way that a class can extend another class.  
```java
Interface ATMWithDraw{
Double MAX_LIMIT= 500000.00;
	Public  boolean withDraw(int acNo,int amount);
}
```

Design Sending an email of statement.  
Design Printing an statement in different formats.  
Design Tax calculation for the Amount.  

```java
Interface ATMWithDraw{
Double MAX_LIMIT= 500000.00;
	Public  boolean withDraw(int acNo,int amount);
	Public void sendEmail(AccountInfo accInfo);
}
```
Is it good design?

###  Tagging Interfaces or Marker Interface 

Creates a common parent  
	you can use a tagging interface to create a common parent among a group of interfaces  
Adds a data type to a class  
A class that implements a tagging interface does not need to define any methods (since the interface does not have any), but the class becomes an interface type through polymorphism.  






