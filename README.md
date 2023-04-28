# Process Writeup

## Name: Gabriel Gradzki
## Course: APCSA
## Period: 6
## Concept: Unit 9/10, Inheratince& Recursion

### Context
I have successfully completed the 9th and 10th units of the AP CSA course, which are entitled "Inheratince" and "Recursion". I have learned how to make a child class and how to utilize parent classes in order to not have to repeat steps many times between multiple classes. As well as how to utilize overriding in the best situations. Some of the methods are super and different ways and attributes to use in a constructor or class which will impact what can happen with the classes and code. Although learning these skills was not easy, I had to push myself to reach my goals.

### Success 
Although the course was hard and confusing, there was a lot of things that I have learned that include how to make constructors for classes which were really confusing at first.

### Setting up a Child Class
By using inheritance, ``Java`` (A certian coding language) allows you to set up a child class which will take the public varibles and constructors from the parent class, to add more functionality specific to the class.

```
public class catContest extends cat
{
  Private String name;
  private String pattern;

  [to be continued]
}
```

By utlizing the `extends` keyword we are making the two classes linked together as a parent and child class (or superclass and subclass). This makes the child class have access to all the features of the parent that are public.

### Accessing the Parent Class
Now we run inot a different kind of problem, how do we access the parent class? More spefically the functionality, the methods, and constructors that reside inside of the parent class? In the parent and child class relationship some things are automatic, and some require a little specification: 

```
public class cat
{
  Private String toys;
  Private int weight;
  Private String color;
  Public String pattern;
  
  Public cat(String t, int w, String c)
  {
  toys = t;
  weight = w;
  color = c;
  }
}
```

In order to user certian varibles or constructors that are private tehy need to be connected to a public constructor that will make access inot it to get a answer from the input that was gotten. Otherwise there would be no access to those varibles and only the ones that are public.

### Challanges

One of the common challanges that I have faced when working with inheritance in Java is to ensure that the subclasses correctly inherit methods and properties of the parent class. In some cases, subclasses may unintentionally override or hide methods or properties of their parent classes, this leads to some unexpected behavior. For example, consider the following class hierarchy:

```
public class Vehicle {
    public void start() {
        System.out.println("The vehicle is starting.");
    }
}
public class Car extends Vehicle {
    public void start() {
        System.out.println("The car is starting.");
    }
}
```

In the example above we can see that car starts its methods from the parent class, called Vehicle. However, the Car class overrides the start() method with its own implementation. This would be very problomatic as in the code elsewhere the program expects the Car class to behave like a Vehicle, but the overridden `start()` method bahaves a bit differently. To fix this you want to include `@Override` methods in the subclass.

```
public class Vehicle {
    public void start() {
        System.out.println("The vehicle is starting.");
    }
}
public class Car extends Vehicle {
    @Override
    public void start() {
        System.out.println("The car is starting.");
    }
}
```

In this modified version of the previous code, the Car class uses the `@Override` annotation/method to indicate that it is intentionally overriding the `start()` method from its parent class. This ensures that the method is properly overridden, and prevents unintentional method hiding or overriding. In conclusion the `@Overriding` method ensures that the subclasses correctly inherit methods and properties from their parent classes when needed and overrides when it is which is a very important aspect of Java.

### Next Steps

Now that I know how parent classes and subclasses work later on I would want to utilize them correctly and whenever possible in order to make things better and more efficient as well as not have any errors that would cause the entire code to collapse.




