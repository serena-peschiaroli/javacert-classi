- 1.  x

Given the code fragment:


class Ball {

 double weight;

}

public class App {

 public static void main(String[] args) {

  // line n1

  System.out.println(b.weight);

 }

}


Which code fragment can be inserted at line n1 to enable the code to print 0.0?

The are 1 correct answers

Ball b = null;
b.weight = 0.0;
Ball.weight = 0.0;
Ball b = new Ball(0.0);
-[x] Ball b = new Ball();


_______________________________________________________________

- 2.  x

What is a Parameterized Constructor?
The are 1 correct answers

None of these
It is a constructor which can be called only once
It is a constructor which cannot be called
It is a constructor that takes a single parameters
-[x] It is a constructor that takes n number of parameters
It is a constructor that takes no parameters



_________________________________________________________--

- 3. x

Given the code:

public class Student {

 String sName;

 char grade;

 public static void main(String[] args) {

  	Student s = new Student();

  	System.out.println("[" + s.sName + ":" + s.grade + "]");

}

}

What is the result?

The are 1 correct answers

- -[x] [null: ]
- [ : ]
- [null:null]
- [:null]



________________________________________________________

- 4.  x


Which two Java reserved words are used to implement encapsulation?

The are 2 correct answers

final
static
-[x] public
extends
-[x] private



__________________________________________________________

- 5.  x


Under what situations does a class get a default constructor?

The are 1 correct answers
You have to define at least one constructor to get the default constructor
All classes in Java get a default constructor
All classes get default constructor from Object class
-[x] If the class does not define any constructors explicitly
None of the above


____________________________________________________________-

- 6. x

Which of the following classes have a default constructor?


class A {}

class B {

  B() {}

}

class C {

  C(String s) {}

}
The are 1 correct answers
-[x] A
A and B
B
B and C
C

_________________________________________________________

- 7. 

What are the properties of a constructor? Select all that apply.
The are 1 correct answers

1. A constructor has the same name as the class name.
2. A class can contain multiple constructors.
3. The constructors cannot be used for initializing values while object creation.
4. A class can contain only a single constructor.
5. A constructor is also known as a member method.
6. The constructor tells how much space to allocate to an object in memory.


All of these
2,3,5
1,2,3,5
-[x] 1,2,5,6
3,4
1,2,6


_____________________________________________________--


- 8. x

Given the contents of the Test.java file:


class MyClass {

 private int var1 = 100;

 public int var2 = 200;

 public void doCalc() {

  var1 = 100 * 2; //line n1

  var2 = 200 * 2;

 }

}

public class Test {

 public static void main(String[] args) {

  MyClass t = new MyClass();

  t.doCalc();

  System.out.println(t.var1 + “ : “ + t.var2); //line n2

 }

}


What is the result?

The are 1 correct answers

200 : 400
A compilation error occurs at line n1
-[x] A compilation error occurs at line n2
100 : 400


_____________________________________________________________


- 9.  

What will be the output of the following code?


package com.company;

class Const{

 int a, b;

 public Const(int a){

  this.a = a;

 }

 public Const(int a, int b){

  this.b = a;

  this.a = b;

 }
}

public class Main {

 public static void main(String[] args) {

  Const constructor_1 = new Const(5);

  Const constructor_2 = new Const(2,3);
  System.out.print(constructor_1.a + constructor_2.b);
 }
}

The are 1 correct answers

1
-[x] 7
8
2
-1


____________________________________________________________


- 10.  

Given the code in a file Application.java:


public class Helper {

 public static String dummy(String text) {

  return text;

 }

}

class Application {

 public static void main(String[] args) {

  System.out.print(“Hello World! “ + Helper.dummy(args[1]));

 }

}


And the commands:

javac Application.java

java Application Java Duke

What is the result?

The are 1 correct answers

Hello World! Duke
An exception is thrown at runtime
-[x] The code does not compile
Hello World! Java
The program fails to execute due to a runtime error



_________________________________________________________


- 11.  x

Given the classes:


Apple.java:

package fruits;

class Apple {

 public void getApple() {}

}

Salad.java:

package food;

// line n1
class Salad {

 Apple apple = new Apple();

 //line n2

 public void prepareSalad () {

  apple.getApple();

 }

}


Which two modifications, independently, enable the Salad.java file to compile?

The are 1 correct answers

The code will not compile
Replace line n1 with import fruits.Apple.getApple();
-[x] Replace line n1 with import fruits.Apple;
 Replace line n1 with import fruits;
Replace line n2 with fruits.Apple apple = new Apple ();
-[x] Replace line n2 with fruits.Apple apple = new fruits.Apple ();

_______________________________________________________-


- 12.   x 

Given the code fragment:

1. public class App {
2
3. }


Which code fragments are valid at line 2?

The are 2 correct answers
for (int count = 0; count < 5; count++) { System.out.print(count); }
package p1; import java.util.*;public void display() { List nums = new ArrayList();}
-[x] {int num;}private String name = “John”;
-[x] public void display() { System.out.print(name); }



__________________________________________________________


- 13.  

Which of the following types of classes are available in java?
1. Static Class.

2. Abstract Class.

3. Concrete Class.

4. Singleton Class.

5. POJO Class.

The are 1 correct answers

1,4
2,4
1,2,5
2,4,5
-[x] All of these
1,2,3,4



________________________________________________________


- 14.  x

Fill in the blanks: The ___________________ access modifier allows

access to everything the ___________________ access modifier does and

more.

The are 1 correct answers
private, protected
protected, package
private, protected
private, public
-[x] public, private
None of the above

_______________________________________________________-

- 15.  x

Given:


class Product {

 String color = null;

 Product (Product p) {

 this.color = p.color;

 }

}


And the code fragment:


Product p1 = new Product(); //line n1

p1.color = “White“;

Product p2 = new Product(p1);

System.out.println(p1.color + “ : “ + p2.color);


What is the result?

The are 1 correct answers

-[x] A compilation error occurs at line n1
White : null
null: null
White : White



____________________________________________________

- 16.  

Private access modifier is applicable only within a same class?

The are 1 correct answers

-[x] TRUE
FALSE



_____________________________________________-


- 17. x

Given:


class Bus {

 String type = “default“;

 //line n1

 Bus (String type) {

  // line n2

  this.type = type;

 }

}

public class App {

 public static void main(String[] args) {

  Bus b1 = new Bus();

  System.out.println(b1.type);

  Bus b2 = new Bus(“luxury“);

  System.out.println(b2.type);

 }

}


What is the result?

The are 1 correct answers

The code fails to compile. To make it compile, at line n1 insert: this () { }
The code fails to compile. To make it compile, at line n2 insert: this ();
-[x] The code fails to compile. To make it compile, at line n1 insert: Bus () { }
The code compiles and prints: default luxury




________________________________________________________________

- 18.  x

Given the following code:

public class Boot {
  static String s;

  static {
    s = "";
  }

  {
    System.out.print("shinier ");
  }

  static {
    System.out.print( s.concat("better "));
  }

  Boot() {
    System.out.print( s.concat("bigger "));
  }

  public static void main(String[] args) {
    new Boot();
    System.out.println("boot");
  }

}
What is the result?

The are 1 correct answers
 

better bigger boot
bigger shinier better boot
-[x] better shinier bigger boot
An ExceptionInInitializationError is thrown at runtime
shinier better bigger boot
better bigger shinier boot




__________________________________________________________________


- 19.   x

Given the classes in different files:

 

package xcom;

public class Useful {
  int increment (int x) {
    return ++x;
  }
}


import xcom.*; //line 1
public class Needy3 {
  public static void main(String[] args) {
    xcom.Useful u = new xcom.Useful(); //line 2
    System.out.println(u.increment(5));
  }
}
 

Which statements are true? (Choose all that apply)

The are 1 correct answers
The output is 0
The code compiles if line 2 is changed to read
Useful u = new Useful();
The output is 6
-[x] Compilation fails
The code compiles if line 1 is removed



__________________________________________________________________

- 20. 

Which of the following keywords is used to allocate memory to an object in Java?
The are 1 correct answers

void
-[x] new
this
allocate
return
thread

__________________________________________________________-_____

- 21. 

Should we make a variable public inside a class to achieve encapsulation?
The are 1 correct answers

-[x] Incorrect
Correct



__________________________________________________________________
- 22. 

The below program will be executed successfully or not? Select either Correct or Incorrect.
The are 1 correct answers

package com.company;

class MyClass{
String name;
private MyClass(String name){
this.name = name;
}

}

public class Main {

public static void main(String[] args) {

MyClass myClass = new MyClass("Adam");
}
}

-[x] Incorrect
Correct



__________________________________________________________________
- 23. 

Which of the following are not a valid access modifiers in Java?
The are 3 correct answers

default
-[x] static
-[x] void
private
protected
-[x] main



__________________________________________________________________
- 24. 

What is the use of getter and setter methods?
The are 1 correct answers

To send data to the server
To achieve polymorphism
-[x] To achieve encapsulation
To achieve abstraction
To achieve multithreading
To get the data from the server



__________________________________________________________________
- 25. 

Which of the following keyword is used to create an object?
The are 1 correct answers

extend
append
static
allocate
public
-[x] new




__________________________________________________________________
- 26. 

What modifiers can be used with a top-level class?
The are 3 correct answers

private
protected
-[x] abstract
default
-[x] final
-[x] public




__________________________________________________________________

- 27. 

Private access modifier is accessible only within a same class?
The are 1 correct answers

Incorrect
-[x] Correct

__________________________________________________________________

- 28. 

What will be the output of the following code?
The are 1 correct answers

class Const{

int a, b, c;

Const(int a){
this(1, 2);
}

Const(int a, int b){
this(1,2,3);
}

Const(int a, int b, int c){
System.out.print(a+b+c);

}

}



public class Main {

public static void main(String[] args) {
new Const(5);

}

}

3
4
5
-[x] 6
2
zero

__________________________________________________________________

- 29. 

What is a singleton class in Java?
The are 1 correct answers

No object can be created inside this class.
The class which can have many objects at a time.
A class that don’t have any methods.
The class which can have only one object at a time.
-[x] A class in which all the methods are made protected.
A class that contains an inner class.

__________________________________________________________________

- 30. 

What will happen if we don’t provide an access modifier while declaring a class in Java?
The are 1 correct answers

It will be considered as having a private access modifier
It will throw an error
It will be considered as having a protected access modifier
All of these options are correct
-[x] It will be considered as having a default access modifier
None of these

__________________________________________________________________

- 31. 


Which keyword is used for constructor chaining in Java?
The are 1 correct answers

class
constructor
public
none of these
-[x] this
new

__________________________________________________________________

- 32. 

Propose the expected result of this code.
The are 1 correct answers


package com.company;

class Parent{
int value1;
int value2;

public int getValue1() {
return value2;
}

public void setValue1(int value1) {
this.value1 = value1;
}

public int getValue2() {
return value1;
}

public void setValue2(int value2) {
this.value2 = value2;
}
}

public class Main {

public static void main(String[] args) {
Parent parent = new Parent();
parent.setValue1(5);
System.out.print(parent.getValue1());
}
}

5
1
compile time error
50
-[x] Zero
runtime error


__________________________________________________________________

- 33. 

Which of the following are valid access modifiers in Java?
The are 3 correct answers

main
-[x] default
-[x] private
-[x] protected
static
void


__________________________________________________________________

- 34. 

What will happen if a variable is made private?
The are 1 correct answers

It can be accessible outside the package.
-[x] It can only be accessible within a class where it is defined.
It can be accessed by all the classes.
It cannot be accessed by interfaces and abstract classes.
It can be accessed by anywhere within the Java project.
It will not be accessible outside the package.

__________________________________________________________________

- 35. 

The below code will be executed successfully?
The are 1 correct answers

package com.company;

class ArrayClass{
int arr[];

public ArrayClass(int arr[]){
this.arr = arr;
}
}

public class Main {

public static void main(String[] args) {

new ArrayClass(new int[]{});
}
}

Incorrect
-[x] Correct

__________________________________________________________________

- 36. 

Is it possible to call a constructor inside another in Java?
The are 1 correct answers

Incorrect
-[x] Correct

__________________________________________________________________

