## What is this keyword?

This keyword refers to current class object. We mostly use for differentiate the instance variable and parameter.
```java
Class Product {
  	int productId;
  	void  Product (int productId){
      	this. productId = productId;
	}
}
```

### What is current class object?
Product p1 = new Product();  
Product p2 = new Product();  

When we are working with p1 reference p1 Object of Product is current class object similarly when we are dealing with p2 reference   
p2 Object of Product is current class object.

By using this keyword we can invoke current class method also because it refers Object. 

	p1.calculateDiscount();

By using this keyword we can call constructor from another constructor.
```java
Class Product {
  	int productId;
	String productName;
	void  Product (int productId){
      	this. productId = productId;
	}
	void  Product (int productId, Stirng productName ){
      	this(productId);
	this. productName = productName;
	}
}
```
