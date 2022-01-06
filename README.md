# Design Patterns

## What are design patterns?
Design patterns are typical solutions to commonly occurring problems in software design.

The concept of design patterns in software design was popularized in the Gang of four's book: "Design Patterns: Elements of Reusable Object-Oriented Software". In this book they describe 23 patterns and categorized these patterns into three groups: Creational, Structural, and Behavioral. 

**Note:** Outside of the Gang of Four's design patterns, there are many other patterns that have been identified.

## Creational Patterns

| Pattern          | Description                                           |
|------------------|-------------------------------------------------------|
| Abstract Factory | Creates an instance of several families of classes    |
| Builder          | Separates object construction from its representation |
| Factory Method   | Creates an instance of several derived classes        |
| Prototype        | A fully initialized instance to be copied or cloned   |
| Singleton        | A class of which only a single instance can exist     |


## Structural Patterns

| Pattern   | Description                                             |
|-----------|---------------------------------------------------------|
| Adapter   | Match interfaces of different classes                   |
| Bridge    | Separates an object’s interface from its implementation |
| Composite | A tree structure of simple and composite objects        |
| Decorator | Add responsibilities to objects dynamically             |
| Facade    | A single class that represents an entire subsystem      |
| Flyweight | A fine-grained instance used for efficient sharing      |
| Proxy     | An object representing another object                   |


## Behavioral Patterns

| Pattern         | Description                                           |
|-----------------|-------------------------------------------------------|
| Chain of Resp.  | A way of passing a request between a chain of objects |
| Command         | Encapsulate a command request as an object            |
| Interpreter     | A way to include language elements in a program       |
| Iterator        | Sequentially access the elements of a collection      |
| Mediator        | Defines simplified communication between classes      |
| Memento         | Capture and restore an object's internal state        |
| Observer        | A way of notifying change to a number of classes      |
| State           | Alter an object's behavior when its state changes     |
| Strategy        | Encapsulates an algorithm inside a class              |
| Template Method | Defer the exact steps of an algorithm to a subclass   |
| Visitor         | Defines a new operation to a class without change     |


## Resources
* [Dofactory](https://www.dofactory.com/net/design-patterns)
* [Refactoring Guru](https://refactoring.guru/design-patterns)


## Notes
Some other design patterns to document

**Publisher-Subscriber**
*Similar to Observer pattern but with 2 key differences:
1. pub/sub is mostly asynchronous whereas observer is mostly synchronous
2. Observers are aware of the observable whereas publishers and subscribers don't need to know each other. They simply communicate with the help of message queues.
