# reimagined-design-patterns

Give a summary description of Four design patterns that you choose from the following design patterns: **Adapter,  Builder, Composite, Decorator, Observer, Interpreter, State, Mediator, Memento, Prototype, Proxy**. In your summaries say:

- what kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example
- how the pattern works, what the basic idea of the pattern is
- what the main advantage and what the the main disadvantage is of using this pattern
- Write a short summary for each of the four patterns, about half a page for each pattern (rather less than more). 

> Do not add diagrams, and do not try to give a complete description of the patterns as found in the books. Rather think of how you would explain the essential ideas of these patterns in a few sentences to a colleague while drinking coffee.


1. Observer Design Pattern : 
	The observer design pattern is an behaviour design pattern. Observer design pattern basically used when there is one to many relationship between objects.
	We use this pattern when we want to notify other dependent objects when there is a change happening in one Object(i.e objects property changes, when object does
	something).
	
	Example : 
  A Company updates to all of their employees of any change in the policy. Here Company is an subject object and employees are observer object. 	

	Advantages :
  	1. Supports loose coupling between objects
    2. Addition of removal of subscribers at runtime  	
    
	Dis-advantages : 
  	1. Order of the notifications to subscribers can not be controlled
	
2. Proxy Design pattern : 
	The proxy design pattern is an structural design pattern. Proxy design pattern is basically used when you to want to add some more additional behaviour to the object
	with the intent of controlling the original object.
	It is also used when you need to create a  wrapper to cover the original object's complexity and to implement lazy initialization.
	Proxy controlls the access to the original object.
	
	Proxy design patter usecases - Security around the original object, caching the information of the original object.	
	
	Example : A Company wants to block the non work related websites using proxy
	
	Advantages :
    1. Security to the original object
    2. Supports lazy initialization, so that we can use it only when we need them.
    3. Controlling the original object without caller knowing about that

	Dis-advantages:
    1. May be complicated if we introduce mulitple proxies
	
3. Adaptor Design pattern:
	The adaptor design pattern is an structural pattern. The adaptor pattern acts as an connector between two intefaces which are not compatible with each other and make them
  interoperable. The intension of adaptor design pattern is not add,remove or alter the behaviour
    	
	Example : AC power adaptors where the power supply ports are different in different countries

	Adavantages : 
	1. Follows Open/Closed principle where it is possible to add new adaptors without disturbing the existing client code.
	2. Follows Single Responsibility Principle where you can separate the interface from the business logic.
	
	Dis-advantages :	
	1. Introducing more chain adaptors to reach the actual type will become an cumbersome

4. Mediator Design Pattern :
    The mediator design pattern is an behavioural design pattern.
	
	A mediator design pattern facilitates the communication between other components without them necessarily being aware of each other or having direct reference or access to each other.
	
	Mediator follows the loosly couple communication between the objects and it helps in reducing the direct references to the each other.
	
	

	Example : Chat room participants
	
	Adavantages :
	1. The biggest advantage is it reduces the communication channels needed between components from many to many to just many to one
	2. Loose coupling, where the component depends only on the mediator
	3. Reusability
	
	Dis-advantages :
	1. Since it has to know many things it may become an god object
	2. Since mediator has to be talk with many different classes it can become extermely complex and can make difficult to maintain

	
