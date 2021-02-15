
The focus today is the Dependency in Software. You could explain that Dependency Injection is a concrete strategy to achieve Dependency Inversion.

## Connections

### Dependencies in Software

Ask the participants

* What is coupling?
* What are the drawbacks of high coupling?
* What are the advantages of loode coupling?

### Dealing with Dependencies Quizz

https://www.mentimeter.com/s/a708d73b675e16ded775f39ded162519/b889518b2732/edit


## Concepts: 

### Principles

* Inversion of Control
* SOLID
    * Single Responsibility Principle
    * Open Close Principle
    * Liskov Substitution Principle
    * Interface Segregation Principle
    * Dependency Inversion Principle
* KISS (Keep It Simple, Stupid)
* DRY (Don't repeat yourself)
* Composition over Inheritance
* POLS (Principle of least suprise)
* YAGNI (You Aren’t Gonna Need It)
* Tell Don't Ask
* Law of Demeter
* Different Levels of Abstractions
* Separation of concerns

### Patterns

* Creational design patterns
    * Abstract Factory
    * Builder
    * Factory Method
    * Object Pool
    * Prototype
    * Singleton
    * Dependency Injection
* Structural design patterns
    * Adapter
    * Bridge
    * Composite
    * Decorator
    * Facade
    * Flyweight
    * Private Class Data
    * Proxy
* Behavioral design patterns
    * Chain of responsibility
    * Command
    * Interpreter
    * Iterator
    * Mediator
    * Memento
    * Null Object
    * Observer
    * State
    * Strategy
    * Template method
    * Visitor



## Concrete

There is a kata with 2 classes in Azure: 
https://dev.azure.com/NagarroAT/Training%20ICAgile/_git/icagile-programming-class-2020admiral?version=GB05_DesignPrinciples&anchor=design-principle-exercises

* Introduce the example - goal is unit tests!
* Tell them that they are not allowed to change the code
* Split up in pairs
* Stop the breakout sessions when at least some pairs have discovered the problem and start asking you if they really are not allowed to change the code
* Ask someone to explain the problem to the group. (The dependency on the Sensor is awkward since you can’t control what pressure reading it gives). 
* Ask if anyone can relate this to the Dependency Inversion Principle. Hopefully someone will explain it to the group. If not, go through it yourself. (The Alarm has a dependency on a detail - Sensor - rather than an abstraction).
* Ask them to continue to work on the same exercise, but now they are allowed to change the code to solve the DIP violation. Let them create an abstraction for the TirePressureMonitor have the Alarm class depend on that instead of a concrete class. They should find it possible to write tests for the class now, using a stub implementation of the abstraction.

If that goes quickly, consider doing the TextConverter problem as well in a similar way.

## Conclusions

Recap the exercise in the group on a Miro board
