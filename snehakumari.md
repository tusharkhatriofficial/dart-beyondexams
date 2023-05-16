## _**WHAT IS A DART?**_


- Dart is a language that focused on **frontened** (mobile,web apps) **User Interface(UI)**
- Dart is developed by **Google** in 2011 and is a mixture of JavaScript,Java,C#
- Dart is an **Object Oriented & Strongly Typed**


___
### _**BENEFITS OF DART**_

 - Easy to learn
 - Comes with good documentation
 - Dart syntax is clean
 - Can compile to self-contained snapshots
 - It is portable
 - It is the only language that is well suited to being compiled both **AOT** (ahead-of-time) and **JIT** (just-in-time)
 - Extremely fast development cycles & fast execution & startup times


___


#### _**FIRST DART PROGRAM**_

```dart

void main() {

    print('Welcome to Dart!'); //used to show the output

    stdout.write('Enter your name:'); //used to show the output

    var name = stdin.readLineSync(); //can also use stdout 

    print("Welcome, $name");

}
```
___


### _**DART CLASS**_

- Class is the blueprint of objects and class is the collection of data member and data function means which include this fields, getter and setter and constructor and functions.


Syntax:  
```dart
class class_name {

    //Body of class
}
```
where- 
- Class is the keyword use to initialize the class.
- class_name is the name of the class.
- Body of class consists of fields, constructors, getter and setter methods, etc.

Example:
```dart
class fruit {

   fruit();

}
```

### _**DART OBJECT**_

- Objects are the instance of the class and they are declared by using new keyword followed by the class name.

Syntax:  
```dart
var object_name = new class_name([ arguments ]);
```

- new is the keyword use to declare the instance of the class
- object_name is the name of the object and its naming is similar to the variable name in dart.
- class_name is the name of the class whose instance variable is been created.
- arguments are the input which are needed to be pass if we are willing to call a constructor.


After the object is created, there will be the need to access the fields which we will create. We use the dot(.) operator for that purpose.

Syntax:  
```
 // For accessing the property
object_name.property_name;

// For accessing the method
object_name.method_name();
```

___