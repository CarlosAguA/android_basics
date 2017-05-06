# Object Oriented Programming

## What are objects?

Objects are instances from a class.  An object will contain the state information depending on the class which was instantiated from. For that reason, an object holds specific information about the class.

For example, the floor plan of a house would be the class and the house would be the instance.

## What is a java class?

A java class is the definition of how an object behaves and the possible states it could have.

## What is a constructor?

A constructor is defined within the class and is used to create object instances. It can or not receive parameters and multiple constructors within a class are allowed.

## What is inheritance?

Different kinds of objects often have a certain amount in common with each other. Object-oriented programming allows classes to inherit. So inheritance is one feature that lets extend the  commonly used states and behaviosr from other classes.  It can be applied by extending the class \(commonly called superclass\) to a subclass.

### Inheritance in Android / extending a class in Android.

Extending a class within an activity lets you use the methods and states within the activity \( i.e. `AppCompatActivity` is a class and the `setContentView` and `findViewById` are methods of that class\).

One can **Override **the methods from the extended class, so that you can change the behavior depending on your need.  One example of that is the `OnCreate()` method used to inflate the **View** from an xml file.

Other examples are the classes a TextView, ImageView and Button \(.java\). They all can have similar attributes like width, height, and visibility, among others. Instead of having all the states in each class one general class is definied called **View.java**. The previous classes are extended from the View class and the specific behaviors and states that those classes must have, are defined independently on each one.

![](/assets/inheritance.jpg)

#### Sources

[Oracle](https://docs.oracle.com/javase/tutorial/java/concepts/object.html)

\(Object Oriented Programming Part 1, Udacity ABND\)

