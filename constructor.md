## What is constructor?
Constructor is a similar to method which is called at the time of object creation.  
Constructor is similar to method but it don’t have return type.   
Name of the constructor should be same as class name.  
It is invoked at the time of object creation.  
If we don’t provided constructer JVM will provide default constructor.  

Syntax of Constructor:  
Class Student {  
	Int studentNo;  
	Student (int studentNumber) {  
	studentNo = studentNumber  
	}  
}  

### Why we need constructor? 
Constructor is used to initialize the instance variables to default values at the time of object creation.

### Constructors Types:
Default constructor :  Constructor without parameter and empty body.  
Class Calculator {  
	Calculator(){  
	}  
}  

Parameterized constructor: Provides specified values to object.  
Class Student {  
	Int studentNo;  
	String studentName;  
	Student (int studentNumber, String name) {  
	studentNo = studentNumber;  
	studentName = name;  
	}  
}  

