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
# Functions in Dart
- **Function** linked with a well- defined task.
#####problem facing without function
- code is becoming bulky.
- we can not reuse the code.
- Buggyness(Error in one place, it will show everywhere)
- No Readability.

**Function** solve all these problems.

**example**
```dart
void main(){
    var myC = myclass();// it is a constructor
    myC.printName(Abhishek);
    //set of codes
    //set of codes
    myC.printName(flutter);
    //set of code
    //set of code
    myC.printName(Mern Stack)
}
class myclass(){
    void printName(String name){// Function Declaration
        print(name);// Function Definition
    }
}
```
**Another example**
```dart
int main(){
    var myC = myclass();
    print(myC.Add(10,20));
    //set of codes
    print(myC.Add(100,200));
}
class myclass(){
    myclass(){
        print("My class object is created!");
    }
    int Add(int num1, int num2){
        int sum= num1+num2;
        return sum;
        //below return statement code will not execute.
    }
    
}
```
---
#List In Dart
**Dart List** is similar to an array, which is the ordered collection of the objects.

- The array is the most popular and commonly used collection in any other programming languages.
- The syntax of declaring the list is given below:
var list1= [10,20,30,40,50];
- The dart list is defined by storing all elements inside the same bracket [] and seprated by commas.
### add & add All
```dart
main(){
    var listNames = [10,20,30,40];
    listNames.add(50);
    //add: At runtime, it will add in list, it will add element at the end of list.
    //Normal or blanklist
    var names = [];
    names.add All (listnames);
    add All: A function which add the all item of list and print after giving print statement.
    //IN list we can store different type of datatypes
    names.add("Ramesh");
    names.add("Suresh");
    names.add("Abhishek");
    print ("$names");
 
}
```
### insert & insert All
```dart
var listno = [10,20,30,40];
var names =[];
names.insert(2,100);
//insert: Here in 3rd position of list 100 will be add.
//Bascially, wiht the help of isert we can add the value in whatever position in list.
names.insert All(3, list no);
//values will be inserted and then further or below things will be added.
names.add ("Ramesh");
names.add ("gamesh");
names.add ("Aamesh");
print("$names");
```

### update
```dart
main(){
    var names = [];
    names.add ("Abhi");
    names.add ("Ramanujan");
    names.add ("Aahan");
    names.add ("Rakesh");
    print("$names");
    names[3]= "Suresh";
    //In 4th position of list name Rakesh will be updated to suresh.
    print("$names");
}
```
### Replace
```dart
main(){
    var listno = [10,20,30,40];
    listno.add(50);
    print("$listno");
    listno.replace Range (0,3,[1,2,3,4]);
    // it means the value will be replace in list at index(0-3)
    print ("$listno");
}
```
### Remove
```dart
var listno = [10,20,30,40];

listno.remove last();
//it will remove at index of list
listno.remove(40);
// value 40 will be removed from list 
// value must be present in list.
listno.remove At(1);
// it will remove the value between this range
```
### Some important operation 
```dart
print ("Length: ${listno.length}");
print ("Reversed: ${listno.reversed}");
print ("First: ${listno.length}");
print ("last: ${listno.length}");
print ("Is Empty: ${listno.length}");
print ("It Not Empty : ${listNo. is not Empty}");
print ("2nd index element: ${listno.elementA(2)}");
```
---
