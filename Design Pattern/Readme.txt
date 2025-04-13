-OO Basics:
 -encapsulation : Encapsulation is the technique of making the fields in a class private and providing access to the fields via public methods. If a field is declared private, it cannot be accessed by anyone outside the class, thereby hiding the fields within the class. For this reason, encapsulation is also referred to as data hiding.Encapsulation can be described as a protective barrier that prevents the code and data being randomly accessed by other code defined outside the class. Access to the data and code is tightly controlled by an interface.The main benefit of encapsulation is the ability to modify our implemented code without breaking the code of others who use our code. With this feature Encapsulation gives maintainability, flexibility and extensibility to our code.
 
 -inheritance : Inheritance can be defined as the process where one object acquires the properties of another. With the use of inheritance the information is made manageable in a hierarchical order.When we talk about inheritance, the most commonly used keyword would be extends and implements. These words would determine whether one object IS-A type of another. By using these keywords we can make one object acquire the properties of another object.
 
 -polymorphism : Polymorphism is the ability of an object to take on many forms. The most common use of polymorphism in OOP occurs when a parent class reference is used to refer to a child class object.Any Java object that can pass more than one IS-A test is considered to be polymorphic. In Java, all Java objects are polymorphic since any object will pass the IS-A test for their own type and for the class Object.It is important to know that the only possible way to access an object is through a reference variable. A reference variable can be of only one type. Once declared, the type of a reference variable cannot be changed.The reference variable can be reassigned to other objects provided that it is not declared final. The type of the reference variable would determine the methods that it can invoke on the object.A reference variable can refer to any object of its declared type or any subtype of its declared type. A reference variable can be declared as a class or interface type.
 
 -Abstraction : Abstraction refers to the ability to make a class abstract in OOP. An abstract class is one that cannot be instantiated. All other functionality of the class still exists, and its fields, methods, and constructors are all accessed in the same manner. You just cannot create an instance of the abstract class.If a class is abstract and cannot be instantiated, the class does not have much use unless it is subclass. This is typically how abstract classes come about during the design phase. A parent class contains the common functionality of a collection of child classes, but the parent class itself is too abstract to be used on its own.
 
 -Association: Association is a relationship between two objects. In other words, association defines the multiplicity between objects. You may be aware of one-to-one, one-to-many, many-to-one, many-to-many all these words define an association between objects. Aggregation is a special form of association. Composition is a special form of aggregation. Example: A Student and a Faculty are having an association.
 
 -Aggregation: Aggregation is a special case of association. A directional association between objects. When an object ‘has-a’ another object, then you have got an aggregation between them. Direction between them specified which object contains the other object. Aggregation is also called a “Has-a” relationship.
 
 
 -composition: Composition is a special case of aggregation. In a more specific manner, a restricted aggregation is called composition. When an object contains the other object, if the contained object cannot exist without the existence of container object, then it is called composition. Example: A class contains students. A student cannot exist without a class. There exists composition between class and students.

-OO Principles:
 -Encapsulate what changes
 -Favor composition over inheritance
 -program to interface not to inheritance
 -strive for loosely coupled design between objects that interact


-Strategy  pattern: Defines a set of encapsulated algorithms that can be swapped to carry out a specific behaviour.

-Observer pattern: The observer pattern defines a one-to-many dependency between objects so that when one object changes state, all of its dependents are notified and updated automatically.

-Decorator pattern: Decorator design pattern is used to enhance the functionality of a particular object at run-time or dynamically.  At the same time other instance of same class will not be affected by this so individual object gets the new behavior.  Basically we wrap the original object through decorator object.   Decorator design pattern is based on abstract classes and we derive concrete implementation from that classes. It’s a structural design pattern and most widely used.
http://javapapers.com/design-patterns/decorator-pattern/
http://javarevisited.blogspot.in/2011/11/decorator-design-pattern-java-example.html


-Factory pattern:Factory pattern is one of most used design pattern in Java. This type of design pattern comes under creational pattern as this pattern provides one of the best ways to create an object.In Factory pattern, we create object without exposing the creation logic to the client and refer to newly created object using a common interface.
http://www.tutorialspoint.com/design_pattern/factory_pattern.htm
http://javarevisited.blogspot.in/2011/12/factory-design-pattern-java-example.html

-singleton pattern: There should be only one instance allowed for a class and, we should allow global point of access to that single instance.
http://javapapers.com/design-patterns/singleton-pattern/
http://www.javaworld.com/article/2073352/core-java/simply-singleton.html

-command pattern

-Adapter and Facade pattern:

-Template method pattern

-Iterator and composite pattern

-state pattern

-proxy pattern

-compound pattern

-MVC
