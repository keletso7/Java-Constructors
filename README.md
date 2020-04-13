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

### Java Inheritance systax
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

