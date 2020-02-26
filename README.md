# Design-Pattern-System-Design-Architectural-Pattern
## Design-Pattern-System-Design-Architectural-Pattern

# [Object Oriented Design](https://www.oodesign.com/singleton-pattern.html)

## Design Principles
* Open Close Principle
	* Software entities like classes, modules and functions should be open for extension but closed for modifications.
  
* Dependency Inversion Principle:
	* High-level modules should not depend on low-level modules. Both should depend on abstractions.
	* Abstractions should not depend on details. Details should depend on abstractions.
	* The Template Design Pattern is an example where the DIP principle is applied.

* Interface Segregation Principle
	* Clients should not be forced to depend upon interfaces that they don't use.
	* If the design is already done fat interfaces can be segregated using the Adapter pattern.
		
* Single Responsibility Principle
	* A class should have only one reason to change.

* Liskov's Substitution Principle
	* Derived types must be completely substitutable for their base types.

-------------------------------------------------------
## Creational Patterns
* Singleton
	* Ensure that only one instance of a class is created.
	* Provide a global point of access to the object.
	* Example 1 - Logger Classes
	* Example 2 - Configuration Classes
	* Example 3 - Accesing resources in shared mode : multiple thread reading from single port 
	* Example 4 - Factories implemented as Singletons
		
	* Thread-safe implementation for multi-threading use.
	* Lazy instantiation using double locking mechanism.
	* Abstract Factory and Factory Methods implemented as singletons.
		
* Factory  :factory function
	* creates objects without exposing the instantiation logic to the client.
	* refers to the newly created object through a common interface
	* Class Registration - using reflection

* Factory Method
	* Defines an interface for creating objects, but let subclasses to decide which class to instantiate
	* Refers to the newly created object through a common interface
	* 	
	* 

* Abstract Factory
	* Abstract Factory offers the interface for creating a family of related objects, without explicitly specifying their classes.
	* Phone Number Example	
	* Pizza Factory Example
	* Look & Feel Example - Windows Themes		

* Builder
	* Defines an instance for creating an object but letting subclasses decide which class to instantiate
	* Refers to the newly created object through a common interface
	* text converting application: convert a document from RTF format to ASCII format	
	* Example 1 - Vehicle Manufacturer.
	* Example 1 - Students Exams.
	* Builder and Abstract Factory
	* Common interface for products
	* 
	* 

* Prototype
	* specifying the kind of objects to create using a prototypical instance
	* creating new objects by copying this prototype
	* 	
	* 

* Object Pool
	* reuse and share objects that are expensive to create.
	* 	
	* 

## Behavioral Patterns
* Chain of Responsibility
	* It avoids attaching the sender of a request to its receiver, giving this way other objects the possibility of handling the request too.
	* The objects become parts of a chain and the request is sent from one object to another across the chain until one of the objects will handle it.	
	* 	
	* 

* Command
	* 
	* 	
	* 

* Interpreter
	* 
	* 	
	* 

* Iterator
	* 
	* 	
	* 

* Mediator
	* 
	* 	
	* 

* Memento
	* 
	* 	
	* 

* Observer
	* 
	* 	
	* 

* Strategy
	* 
	* 	
	* 

* Template Method
	* 
	* 	
	* 

* Visitor
	* 
	* 	
	* 

* Null Object
	* 
	* 	
	* 

## Structural Patterns
* Adapter
	* 
	* 	
	* 

* Bridge
	* 
	* 	
	* 

* Composite
	* 
	* 	
	* 

* Decorator
	* 
	* 	
	* 

* Flyweight
	* 
	* 	
	* 

* Proxy
	* 
	* 	
	* 
	

