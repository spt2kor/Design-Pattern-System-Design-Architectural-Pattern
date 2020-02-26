# Design-Pattern-System-Design-Architectural-Pattern
## Design-Pattern-System-Design-Architectural-Pattern

# [Object Oriented Design](https://www.oodesign.com/singleton-pattern.html)

## Design Principles
* Open Close Principle
		Software entities like classes, modules and functions should be open for extension but closed for modifications.
  
* Dependency Inversion Principle:
	* High-level modules should not depend on low-level modules. Both should depend on abstractions.
		Abstractions should not depend on details. Details should depend on abstractions.
		The Template Design Pattern is an example where the DIP principle is applied.

* Interface Segregation Principle
		Clients should not be forced to depend upon interfaces that they don't use.
		If the design is already done fat interfaces can be segregated using the Adapter pattern.
		
* Single Responsibility Principle
		A class should have only one reason to change.

* Liskov's Substitution Principle
		Derived types must be completely substitutable for their base types.

-------------------------------------------------------
## Creational Patterns
* Singleton
		Ensure that only one instance of a class is created.
		Provide a global point of access to the object.
		Example 1 - Logger Classes
		Example 2 - Configuration Classes
		Example 3 - Accesing resources in shared mode : multiple thread reading from single port 
		Example 4 - Factories implemented as Singletons
		
		Thread-safe implementation for multi-threading use.
		Lazy instantiation using double locking mechanism.
		Abstract Factory and Factory Methods implemented as singletons.
		
* Factory
		creates objects without exposing the instantiation logic to the client.
		refers to the newly created object through a common interface

* Factory Method
* Abstract Factory
* Builder
* Prototype
* Object Pool

## Behavioral Patterns
* Chain of Responsibility
* Command
* Interpreter
* Iterator
* Mediator
* Memento
* Observer
* Strategy
* Template Method
* Visitor
* Null Object

## Structural Patterns
* Adapter
* Bridge
* Composite
* Decorator
* Flyweight
* Proxy



