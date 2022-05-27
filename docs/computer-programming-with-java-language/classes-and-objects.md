# 1.0 Classes and Objects

[zh-CN](classes-and-objects-zh-CN.md)

# 1.1 What is a class? What is the object?

As mentioned earlier, Java is an object-oriented programming language, and when we start learning a certain language, we are not only able to write programs, but also learn how to `design`, and the ability of such `design` is very convenient. That's the beauty of programming.

I believe you can definitely find such definitions of `class` and `object` on the Internet:

- Class (Class): defines the abstract characteristics of a thing. The definition of a class contains the form of the data and the operations on the data.
- Object (Object): is an instance of a class (Instance).

However, we also need to distinguish the relationship between `class` and `object`.
which is:

> The class defines the object, the object is produced by the class, and the objects produced by the same class are not the same.

Alternatively, you can also distinguish in an obvious way:

> Classes are not stored in memory space, and classes can only be stored in memory space as objects when they are instantiated as objects.

# 1.2 Abstraction process

We need to abstract so that the problem becomes a problem between classes, and then solve the problem through the class.

In the book "Thinking in Java", the object-oriented programming method summarized by Alan Kay is mentioned. At the same time, we might as well make an analogy, for example, we have a car now.

> **1. Everything is an object. **<br>
> The car is an object; you are certainly an object.
>
> **2. A program is a collection of objects that tell each other what to do by sending messages. **<br>
> The world the car shares with you is the program, and when you start the car, you send a message to the car to start.
>
> **3. Each object has its own storage composed of other objects. **<br>
> A car has an engine, a chassis...; you also have a digestive system, a respiratory system, a motor system.... They are all objects.
>
> **4. Every object has its type. **<br>
> And what type of car is it? It could be a machine, or it could be the car itself. We know that machines and cars here are both classes. Since this object can be an instance of two classes at the same time, what is the relationship between these two classes? Don't worry! You'll learn it shortly in the chapter 'Inheritance and Polymorphism' later.
>
> **5. All objects of a particular type can receive the same message. **<br>
> Do you feel a little incomprehensible when you see this sentence? Let's take a look at the previous one, it can be a machine, of course, it can also be the car itself. When we send a message to a class with the type 'Machine', our object of type 'Car' can also receive messages from other classes to the 'Machine' class. Such a feature, which we call `substitutability', is a powerful advantage of OOP languages.