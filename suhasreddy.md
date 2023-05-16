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

