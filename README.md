# Design Patterns

## What are design patterns?
Design patterns are typical solutions to commonly occurring problems in software design.

The concept of design patterns in software design was popularized in the Gang of four's book: "Design Patterns: Elements of Reusable Object-Oriented Software". In this book they describe 23 patterns and categorized these patterns into three groups: Creational, Structural, and Behavioral. 

**Note:** Outside of the Gang of Four's design patterns, there are many other patterns that have been identified.

## Criticism of patterns

**Workaround for a weak programming language**

The need for patterns often arise when using a programming language that lacks the necessary level of abstraction. Patterns become a workaround that make up for lacking features.

For example, the Strategy pattern can be implemented with a simple anonymous (lambda) function in most modern programming languages.

**Inefficient solutions**

Patterns try to systematize approaches that are already widely used. This unification is viewed by many as a dogma and they implement patterns “to the point”, without adapting them to the context of their project.

**Unjustified use**

If all you have is a hammer, everything looks like a nail. Typically, once a novice first becomes familiar with design patterns they tend to overuse them.

**May Increase Complexity**

Using inappropriate patterns can be like trying to force a square peg into a round hole: adding additional work and unnecessary dependencies.


## Patterns
### Creational Patterns
Creational patterns provide object creation mechanisms that increase flexibility and reuse of existing code.

| Pattern          | Description                                           |
|------------------|-------------------------------------------------------|
| Abstract Factory | Creates an instance of several families of classes    |
| Builder          | Separates object construction from its representation |
| Factory Method   | Creates an instance of several derived classes        |
| Prototype        | A fully initialized instance to be copied or cloned   |
| Singleton        | A class of which only a single instance can exist     |


### Structural Patterns
Structural patterns explain how to assemble objects and classes into larger structures, while keeping the structures flexible and efficient.



| Pattern   | Description                                             |
|-----------|---------------------------------------------------------|
| Adapter   | Match interfaces of different classes                   |
| Bridge    | Separates an object’s interface from its implementation |
| Composite | A tree structure of simple and composite objects        |
| Decorator | Add responsibilities to objects dynamically             |
| Facade    | A single class that represents an entire subsystem      |
| Flyweight | A fine-grained instance used for efficient sharing      |
| Proxy     | An object representing another object                   |


### Behavioral Patterns
Behavioral patterns take care of effective communication and the assignment of responsibilities between objects.

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



**Object Pool**

Creational Pattern

Uses a set of initialized objects kept ready to use – a "pool" – rather than allocating and destroying them on demand. A client of the pool will request an object from the pool and perform operations on the returned object. When the client has finished, it returns the object to the pool rather than destroying it.

Object pooling can offer a significant performance boost in situations where the cost of initializing a class instance is high and the rate of instantiation and destruction of a class is high – in this case objects can frequently be reused, and each reuse saves a significant amount of time. 

https://en.wikipedia.org/wiki/Object_pool_pattern

**Publisher-Subscriber**

Behavioral pattern

Similar to Observer pattern but with 2 key differences:
1. pub/sub is mostly asynchronous whereas observer is mostly synchronous
2. Observers are aware of the observable whereas publishers and subscribers don't need to know each other. They simply communicate with the help of message queues.

**Null Object**

Behavioral pattern

https://www.c-sharpcorner.com/article/null-object-design-pattern/
