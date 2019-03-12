Abstract class is to achieve abstraction.

### What abstraction?
Abstract class will abstract the functionality.  
Abstract class holds the semi implementation.  
An abstract class is a class that is declared abstract.  
it may or may not include abstract methods.  
Abstract classes cannot be instantiated.  
they should be a sub classed to implement abstract class .  

### What is abstract methiod? 

An abstract method is a method that is declared without an implementation.

The class must also be declared abstract. If a class contains an abstract method, the class must be abstract as well.

Any child class must either override the abstract method or declare itself abstract.

```java
Interface Graphic {
 	Public void draw();
	Public int calArea();
}
Abstract class AGraphics implements Graphic {
	Public void draw(){
		// implementation 
	}

Public abstract int calArea();
}

Class Circle extends AGraphics {
	public int calArea(){
		//implementation 
	}
}

Graphics g= new Circle();
AGraphics ga = new Circle();
Circle c= new Circle(); 

```

