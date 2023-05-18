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
 # Video-4
***
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
# Video-5
# Dart var Vs Dynamic - Differences
**Main difference**
String value multiple times we can assign in variable 
but
In dynamic, as many time we want we can store multiple types of datatypes in that variable or also can override it multiple times in that particular runtime.

**Let's go in deep for more clarification.**
Let's take an example:
```
void main () {
  print("Welcome to NewWorld!");

  //var
  var subject = "English"; //we maynot even mention var here. "English" identify the 1st value it got is string.

  subject = 7; //This will show error as with the 1st value i.e. "English" it will assign that what is the datatype of this particular var.
}
```
**Variable means we can vary, if we want we can overrise values in it. Short form of it is var.**

---
Another example:
```void main() {
  print("Welcome to NewWorld!");

  //var
  var section;      //when we declared this var we couldn't initialize any value at that time so by default datatype becomes dynamic.
                    //We can write dynamic too in place of var. 
                    //It will work same as var.

  section = "A";

  section = 2;     //we can only assign integer value as 2 is an integer so cannot store another datatype.
  

  section = true;

  var rollno = 82;

  rollno = 16;
}
```
In the above program, we wrote var to know the difference, when we are not giving any datatype through var, then we take only var   & with var creating a variable initially not giving it any value. Just declared it so, the variable type becomes dynamic.

**For more information,**
When the values are coming from server or through API we don't know the datatype but we still need to store it.
So, the type of data will be assigned in it for the first time at that time only if any value we are assigning together then that var becomes as the same type as the data is.

***
# Video-6
# Functions? and their use in Dart.
-> We can call it method or function.
**Roles:**
* We use it to reduce the redundancy of class.
* To increase the reusability we use class.
* Anything can be executed 10 times or more by writing the function only once.
Any code which is reusable in that particular class, we can define it in a function & where that set of instruction is needed then there we can call function.

Things to be known,
-**Functions made are function declaration.**
-**Set of instruction written in it is function definition.**
-**In main program when the function is called is    called function calling.**

Showing how to make function,
```
void main() {
  print("Welcome to myworld");

}

void myFunc() {  //function name must be unique to be uniquely identified.

}
```
Example for **Declaration & Definition**
```
void main() {
  print("Welcome to myworld!");

  var myW = myWorld()
  myW.printName();      //Creating object of the class.
                        //Function inside the class.
                        //It is function calling.
}
class myWorld {
  void printName() {     //Declaration
                         //It doesn't return anything as we had kept void there.
                         //The code inside this function will come into execution.
    print("Web Tech");    //Definition
                          //Called as definition where we define logic of that function.
  }
}
```
**We have given only one line definition here but where 4 lines or 6 lines are in use then in that case we have to use function.**
**Functions with different values**
```
void main() {
  print("Welcome to myworld!");

  var myW = myWorld()
  myW.printName("web dev");     //fun with diff values.
  //
  //                          //set of codes.
  //
  myW.printName("Flutter");    //fun with diff values.
  //
  //
  //
  myW.printName("Saloni");     //fun with diff values.
}

class myWorld {
  void printName(String name) {
    print(name);
  }
}
```
**When we call printName it takes us to 
void printName(String name) <-- this String
the name gets printed where inside name we have "web dev".So, it will print that & similarly others.**

-Adding two integers.
-print statement displayed.
-myWorld class created whose constructor has been called & then the value was been printed which was 
Welcome to myWorld!
```
void main() {
  print("Welcome to myworld!");

  var myW = myWorld()
  
  print(myW.Add(4,5));

}
class myWorld {
  myWorld() {                //Default Constructor
    print("myWorld object created!");
  }
  void printName(String name) {   //Declaration
    print(name);                  //Definition
  }
  int Add(int no1, int no2) {
    int sum = mo1+no2;
    return sum;
  }
}
```
Output:
Welcome to myWorld!
myWorld object created!
9
***
# Video-7
# List In Dart.
We manage list in dart similar to array where we store similar order of elements, data, object, etc.

**List:** Collection of multiple data where multiple data can be similar type data or different type of data, collection of data.

**The syntax of declaring the list as given below:**

var[list] = [10, 20, 30, 40, 50]

The dart list is defined by storing all elements inside the bracket([]) & separated by commas (,).

**List in Dart**
                               
0_____1____2____3____4________Index
| 10 | 20 | 30 | 40 | 50 |         
|--- |--- |--- |--- |--- |
__________________________Elements

**Example:**
```
import'package:flutter/Cupertino.dart';
main() {
  var ListNo = [10,20,30,40];       //We can take similar data but there's no such conditions so we can take multiple data too.
  ListNames.add(50);

  print("$ListNames");
}
```
Output:
[10,20,30,40,50]

To Insert:
names.insert(2, 100);

Add, Insert role:
names.insert(2, 100);
names.insertAll(3, ListNo);

O/p:
[Ram, Sita, 100, 10, 20, 30, 40, 50, Gita, Rosy]

To update any index:
names[2] = "Geetu"

Replace:
```
import'package:flutter/Cupertino.dart';
main() {
  var ListNo = [10,20,30,40];       //We can take similar data but there's no such conditions so we can take multiple data too.
  ListNames.add(50);

  print("$ListNames");
}
print("$ListNo");
ListNo.replaceRange(0, 3,[1, 2, 3, 4,]);

print("$ListNo");
```
O/p:
[10, 20, 30, 40, 50]
[1, 2, 3, 4, 40, 50]

Remove:
```
ListNo.removeLast();  //will remove last no.
ListNo.remove(20);    //will remove only 20.
ListNo.removeAt(1);    //will remove 1st index no. 20.
ListNo.removeRange(0, 4);  //It will delete upto [10, 20, 30, 40]. It will not delete upto 4th element, it will just delete elements before 4.
```
***













  






  











 





