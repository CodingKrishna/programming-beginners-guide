## What is class?
Class is used to represent a real time entity in a business usecase to feed into computor in java programing. 

Class is template of an real-time entity. Every entity in this real world has set of properties and it exhibits some behaviors.

We will bind the properties and behaviors into a class.

Class Human {  
	Sting name;  
	String gender;  
	void sleep() { 
  };  
	void walk() {  
  };  
}

#### Why we need class?
Actually class keyword is derived from word classification in java, every real entity in this world need to be classified to differentiate.   
Like humans classifies the things, systems also need classification. Java class classifies the real entity's to the system to understand the about entity.  
Ex: Car, Human, Animals, Restaurant etc.  
All this classification as a human we will understand.  

#### How we will tell to the system about this entity’s ?
Ans : through class we will define so that system will understand.

## What is object?
Object is nothing but actual instance of real time entity in the compute memory.  
How we create actual real entity structure in memory?  
Through class definition.  
Car sivaCar = new Car();  
Car raviCar = new Car();  

### Why we need object?
To represent real world objects in JVM.  
To manipulate with real object to get desire functionality's.  

### Characteristics of an object.
State : represent the data(values) of an object.   
Behavior : represent the behavior (functionality's )  of an object.  
Identity : every object in this world has identity to differentiate with others object.  
In java reference is used to identify the object as unique id.  
raviCar.color = “Red”;  
raviCar.transport(source, destination);  

