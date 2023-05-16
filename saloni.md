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
#Video-4
_**Variables and  Datatypes**_
---
**Let's know about what is variable? & why do we need variable?**

**Suppose**, if we have an value then we need to remember but we do not want it to be remembered instead we want to store it somewhere so that whenever we have its requirement then from that particular memory address we take that value.

We make those value get stored in the **memory blocks.**
 * When we store it, it has particular address location.
 * Address will be in integer format (long no.).
 * It will be difficult for us to remember it. That's why we make it store with a name is called **variable.**

**From this we get to know that,**
In the whole program is we have to store a value that will be needed throughout the program multiple times then create a variable, make the value store & can give that variable a name.
Whenever we call it with that name it will provide the value.

**The type of value we store in variable is datatype.**

**_Datatypes_** => 0 - 9 -> Integer
                => values in point -> Double
                => when the value exceeds its limit -> Big Int
                => Alphabets, characters -> String(it is array of characters)
                => Conditional programs(True or False) -> Boolean Type
**For now let's only concentrate on how do we declare variable, what kind of data is to be stored and lastly how do we initialize it.**

_In the program._
```
//Declaration of variable
int a;
print(a); //error: The non-nullable local variable 'a' must be assigned before it can be used.
```
**To remove the error show in the above program we initialize ? before int which shows the value can be nullable.**
```
int? a;  //it can be nullable.
print(a);  //error is gone.
```
---


  






  











 





