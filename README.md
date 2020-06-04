## Welcome to KKEL for Java

# LESSON: Abstract Class & Interface
   
  - Inheritance in Java OOPs with examples
  - Polymorphism in Java OOPs with Example 
  - Abstract Class Method
  - Interface
  - Interface vs Abstract Class in Java: What's the Difference?
  
### Types of Inheritance
There are Various types of inheritance in Java:
  - Single Inheritance
  - Multiple Inheritance
  - Multilevel Inheritance
  - Hierarchical Inheritance
  - Hybrid Inheritance

### Inheritance In Java
JAVA INHERITANCE is a mechanism in which one class acquires the property of another class. In Java, when an "Is-A" relationship exists between two classes, we use Inheritance. The parent class is called a super class and the inherited class is called a subclass. The keyword extends is used by the sub class to inherit the features of super class.

### Java Inheritance syntax
```markdown
class subClass extends superClass  
{  
   //methods and fields  
}  
```

### Java Inheritance Example
```markdown
class Doctor {
 void Doctor_Details() {
  System.out.println("Doctor Details...");
 }
}

class Surgeon extends Doctor {
 void Surgeon_Details() {
  System.out.println("Surgen Detail...");
 }
}

public class Hospital {
 public static void main(String args[]) {
  Surgeon s = new Surgeon();
  s.Doctor_Details();
  s.Surgeon_Details();
 }
}
```

### Super Keyword

The super keyword is similar to "this" keyword.

The keyword super can be used to access any data member or methods of the parent class.

Super keyword can be used at variable, method and constructor level. 

### Polymorphism in Java OOPs with Example

What is Polymorphism?

Polymorphism is a OOPs concept where one name can have many forms.

For example, you have a smartphone for communication. The communication mode you choose could be anything. It can be a call, a text message, a picture message, mail, etc. So, the goal is common that is communication, but their approach is different. This is called Polymorphism. 

### Java Polymorphism in OOP’s with Example

We have one parent class, ‘Account’ with function of deposit and withdraw. Account has 2 child classes

The operation of deposit and withdraw is same for Saving and Checking accounts. So the inherited methods from Account class will work.

### What is Abstract Class?

Abstract Classes are classes in Java, that declare one or more abstract methods. 

#### Abstract Class in Java: Important Points

  - An abstract class may also have concrete (complete) methods
  - For design purpose, a class can be declared abstract even if it does not contain any abstract methods
  - Reference of an abstract class can point to objects of its sub-classes thereby achieving run-time polymorphism Ex: Shape obj = new Rectangle();
  - A class must be compulsorily labeled abstract, if it has one or more abstract methods.
  
  #### Final Keyword in Java
  
  The final modifier applies to classes, methods, and variables. The meaning of final varies from context to context, but the essential idea is the same. 
  - A final class can not be inherited
  - A final variable becomes a constant and its value can not be changed
  - A final method can not be overridden. This is done for security reasons, and these methods are used for optimization.
  
  #### Abstract & final keywords example
  
  ```markdown
  abstract class Shape{
   final int b = 20;
   public void display(){
     System.out.println("This is display method");
   }
   abstract public void calculateArea();
}

public class Rectangle extends Shape{
   public static void main(String args[]){
      Rectangle obj = new Rectangle();
      obj.display();
      obj.b=200;
  }
  
}
```
1) Copy the following code into an Editor (jgrasp)
2) Save , Compile & Run the code.
3) Error =? The abstract method is not implemented int the class Rectangle. 
 - To fix the issue implement method calculateArea() in class Rectangle
5) Error = ? variable b is final 
 - To fix this comment out or remove/delete he statement ```obj.b=200;```

### Interface

#### What is an Interface?
An interface is just like Java Class, but it only has static constants and abstract method. Java uses Interface to implement multiple inheritance. A Java class can implement multiple Java Interfaces. All methods in an interface are implicitly public and abstract

#### Example for Implementing Interface
```class Dog implements Pet```

```interface RidableAnimal extends Animal, Vehicle```

#### Why is an Interface required?
Suppose you have a requirement where class "dog" inheriting class "animal" and "Pet". But you cannot extend two classes in Java. So what would you do? The solution is Interface.

#### Syntax for Declaring Interface
```markdown
interface {
//methods
}
```

#### Java Interface Example:
```markdown
interface Pet{
  public void test();
}
class Dog implements Pet{
   public void test(){
     System.out.println("Interface Method Implemented");
  }
   public static void main(String args[]){
     Pet p = new Dog();
     p.test();
  }
}
```

#### Interface Vs. Abstract Class
An abstract class permits you to make functionality that subclasses can implement or override whereas an interface only permits you to state functionality but not to implement it. A class can extend only one abstract class while a class can implement multiple interfaces

#### Sample code for Interface and Abstract Class in Java

Following is sample code to create an interface and abstract class in Java 

##### Interface Syntax
```
interface name{
//methods
}
```
##### Java Interface Example:
```
interface Pet {
    public void test();
}
class Dog implements Pet {
    public void test() {
        System.out.println("Interface Method Implemented");
    }
    public static void main(String args[]) {
        Pet p = new Dog();
        p.test();
    }
}
```

##### Abstract Class Syntax
```
abstract class name{
    // code
}
```
##### Abstract class example:
```
abstract class Shape {
    int b = 20;
    abstract public void calculateArea();
}

public class Rectangle extends Shape {
    public static void main(String args[]) {
        Rectangle obj = new Rectangle();
        obj.b = 200;
        obj.calculateArea();
    }
    public void calculateArea() {
        System.out.println("Area is " + (obj.b * obj.b));
    }
}
```

#### Constructor in Java with EXAMPLE
##### What is a constructor in Java?
