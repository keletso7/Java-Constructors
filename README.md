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

**Syntax**
```markdown
super.<method-name>();
   ```

You can use the [editor on GitHub](https://github.com/keletso7/Keletso7/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/keletso7/Keletso7/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
