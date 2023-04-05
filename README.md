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








