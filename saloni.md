# Video-1
# Learn Dart For Flutter

Dart is a programming language.
frontend : It helps to build UI.
backend : It helps to build logics.

# Why are we learning Dart?
 It has two frontends : UI & UX
 logic build means : UX is being build.
 frontend build means : UI is being build.

  Dart 
  * Object oriented and strongly typed.
  * Developed by Google in 2011.
  * A mixture of JavaScript, Java.

  **Benefits**:
 **Asynchronous programming** : It means parallel programming.
 * There is a problem of _Time not defined_ in dart so we use async & await for asynchronous programming.
 * **AOT** & **JIIT** are compilers which are used for hotreload and hotrestart.
  **AOT**(Ahead Of Time) & **JIIT**(Just In Time)
 * AOT: compile all files to run on a particular platform.
   JIIT: changes can be seen instantly i.e. hot restart & hot reload.
 * Development becomes faster with AOT & JIIT.

 
 |  Flutter|API    |
 |   ---   |   ---   |
 | Utility | Widgets |
 |     Dart Code     |

 * If we are installing complete application in this case with the help of AOT on that platform we deploy specific native code with the help of flutter sdk.
***

# Video-2

**Basic ideas regarding function, input, output, variable**
```
void main() {                 // main function from where the execution starts of dart program.
  print("Welcome to AMC");    // if something is to be printed on console or to show the o/p.
  stdout.write("Enter your name"); //can use stdout too instead of print statement.
  var name = stdin.readLineSync(); //The lines we will write on console that whole line will come under this variable.
  print("Welcome, $name");

}
```
Note : Dart is a mixture of JavaScript, Java & CScript

# Video-3
**Class? Object?** in Dart.
**For class**
 Basically, class in dart is a blueprint or template that defines the structure and behavior of objects.

 **Syntax:**
 ```
 class Doll {    //class is a keyword & Doll is a identifier.

  Doll();       //Constructor
 }
 ```
 These can be included in class :
 |**Constructor** |
 |**Function**    |
 |**Fields**      |
 |**Members**     |
***
 **For object**
 Objects are basic building blocks of dart programming.
 **To create object**
 ```
 var Saloni = new Doll();
 ```
 **Note:**
 * **New version** says without new keyword we can make object of class.
 * **new** : It is a runtime allocation.
 
 Example:
```
  void main() {                
    print("Welcome to AMC");    
    stdout.write("Enter your name"); 
    var name = stdin.readLineSync(); 
    print("Welcome, $name");

    Doll();             //Creating an class object.
}
class Doll {
  Doll(); 
}
```
  











 





