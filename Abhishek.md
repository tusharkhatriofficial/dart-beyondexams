#  All About    Dart

**Flutter** is a single code base framework **means** we need not to learn other language for forntend and backend.

**Dart** provides you all the features to develop both frontend and backend(Logistics)

**Dart** is a programming which is used in flutter.

## why we are learning dart?

**Dart** is focused in both UI/UX.
**UI** : it refers to front-end.
**UX** : it refers to back-end(Logistics)

**Dart** language is a object-oriented and strongly typed.
**Dart** is a mixture of **javascript**, **java**, **Cscript** or **C#**.

## Benefits of Dart
- Use of **async** and **await** for asynchronous programming.
- Uses two compliers **AOT**(Ahead-of-time) and **JIT**(Just-in-time).
             **.** With those Compilers, We can perform hot reload and hot-restart function.
             **.** JIT gives you hot reload function which saves alot of time.
             **.** With the help of AOT, We can install our flutter apps in different platforms and run.

- **JIT** compilation is used during development, using a complier that is especially fast. Then, When app is ready for realease, it is complied **AOT**.
- Dart can be compiled into **Java scripts** so it can be executed in browsers.
- Flutter does not split layout between your program and add additional templating or layout like jsx or xml.
---
# Simple program in Dart
```dart
import 'dart:io'
void main (){
    print('Welcome to Dart')
    stdout.write("Enter Your Name"); // it is an alternative of print.
    var name = stdin. readLinesync(); // it is for taking user input.
    print ("Welcome, $name");//printing satement and doing concatenation. 
}
```
---
# Dart class & objects
- class is a blue print or design for the repetitive code.
- object is an isntance.
- By making class, code redundancy will be minimized.
- When we wnat to use that repetitive code or  blue print then, We make object and use it.

**example**
```dart
void main(){
    var dog = new animal(); // creating object in older version of dart.
    animal(); // creating object in new version of dart.
}
class Animal {
    Animal(); // it is a default constructor.
}
```
**new** is a run time allocatiom

---
# Variables & DataTypes in Dart
- **variable** is memory location having name which stores some data. it stores the value in runtime.
- **DataType** refers which type of data will be stored by the variable.
## common datatype
**Integer**: it stores integer value like, 3,4,5,4564...
**double**: it stores float value like: 3.4,5.55555...
**big Int**: it stores big integer value like:123456789098...
**String**: it stores alpha numeric values.
**collection**:it stores multiple value together.
**bool**:it stores either true or false.

In one variable, if we want to store same value or multiple values then we use **collection**.

**Example**
```dart
//Declaration of variable
int? a;
//?: it says value can be nullable
a = 5;// 5 is assign to a
//when you dont assign the value to variable then it will be showing null.
print (a);
a = 7;// Updating the value 
print (a);
//inline declaration
String name = "Abhi";

BigInt longValue = BigInt.parse('234567890123476');
print(longValue);
double percentage = 99.65;
num percentage = 99.65;// Num can be used for both integer and double values.
bool isLogin = false;
isLogin = true; 
```

---
#Var & Dynamic
```dart
var subject = "maths";
subject = "English";
// Here We did not say explictly that the value assigned is String.
//so, VAR identifies with the frist letter which type of data is stored and accordingly it will assign the datatypes.

var rollno = 11;
rollno = 56;
// same goes for integer value too.

var subject;
// Here we did not assign any values so, it becomes dynamic datatype.
// That means in Run time as per our choice, We can assign datatype to that variable.

section = "D";

section = "7";

section = "false";

// So, With help of dynamic datatypes, we can store multiple type datatypes in a single variable
```
---
