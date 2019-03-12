
# What is user defined data type?

Data types are two types one is pre-defined data type and second one is user defined data type.

We already saw predefined data types like int, char and float.

In real time application we need to capture complex businesses entities like product info or student info that time we need to make a custom data type.  

We can define our own data type like predefined data types so we call it as custom data type.

## How many User defined data types?
* Structure
* Array

* Structure is not directly supported in java but we are achieving the same thing with class 
* Structure is collection of heterogynous combination of predefined data types.

Class Product{

int id;

String name;

float price;

}

Above class is kind of data type which is made up of with predefined data types. This product data type can hold one product information.

Product product = new Product();  
   product.id = 2;  
   product.name = “T-shirt”;  
System.out.println(product.id) ;  
System.out.println(product.name) ;  

# Arrays
Array is homogeneous collection of data types and memory is allocated consecutively.  
When we want to store group of similar elements we use arrays   
Ex:  all id’s of students.  
Stytax: data type arrayName[arraysize] = {};  

Ex: int ids[] ={10,20,30,40}   
System.out.println(ids[2])   

int a[]=new int[3];//declaration and instantiation   
### How to Access array element?
Array element can be accessed using index.  
a[0]=10;//initialization    
a[1]=20;    
a[2]=70;    
System.out.println(a[0]);     

//printing array    
for(int i=0;i<a.length;i++)//length is the property of array    
System.out.println(a[i]);    




