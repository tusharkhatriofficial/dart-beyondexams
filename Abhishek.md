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