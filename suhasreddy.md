# All about Dart

Dart is an open-source object-oriented programming language with c-style syntax which was developed by **Google in 2011**

It is Focused on **frontend**(mobile,web apps) **user interface**(UI) development. 

void main(){
    for(int i=0; i<5; i++){
        print('hellow ${i + 1}');
    }
}

# Benefits of Dart

* Use of async and awit for asynchronous programming.

* Dart is one of very few languages(and perhaps the only "mainstream" language) that is well suited to being complied both **AOT(ahead-of-time)** and **JIT(just-in-time)**. Supporting both kinds of compliation provides significant advantages to Dart and (especialy) Flutter (**Hot Reload Feature**)

* JIT compilation is used during development, using a complier that is especially fast

* Extremely fast development cycles, and fast execution and startup times

* Flutter doesnt split layout between your program and an additional templating or layout language like JSM or XML, nor does it require separate visual layout tools



# Creating First Program In dart

As we have discussed earlier, Dart is easy to learn if you know any of Java, C++, JavaScript, etc. The simplest "Hello World" program gives the idea of the basic syntax of the programming language. It is the way of testing the system and working environment. In this tutorial, we will give the basic idea of Dart's syntax. There are several ways to run the first program, which is given below:

**Using Command Line**
**Running on Browser**
**Using IDE**

Before running the first program, it must ensure that we have installed the Dart SDK properly

void main(){
    print('Welcome to Dart');

    stdout.write('Enter your Name:');

    var name = stdin.readLineSync();

    print("Welcome, $name");
}

this program first take input and give output

output: 
Welcome to Dart
Enter your Name: suhas 
Welcone, suhas


# Dart Class and Object

# Classes

* Dart classes are the blueprint of the object, or it can be called object constructors. A class can contain fields, functions, constructors, etc.

* We can assume a class as a sketch (prototype) or a car. It contains all the details about model name, year, features, price, etc.

* Dart provides class keyword followed by a class name is used to define a class; all fields and functions are enclosed by the pair of curly braces ({})

**Syntax**

class ClassName {  
   <fields>  
   <getters/setters>  
  <constructor>  
 <functions>  
}  

# Objects

* Dart is object-oriented programming, and everything is treated as an object in Dart. An object is a variable or instance of the class used to access the class's properties.Object have two features - state and behavior.

* Suppose a man is an object with a state (name, age, health) and behavior (walking, running, and sleeping).

* After creating the class, we can create an instance or object of that class which we want to access its fields and functions. The new keyword is used to declare class followed by the class name. 

# Syntax

var object_name = new class_nsme(<constructor_arguments>);





