# Idead Programming Language (Statically Typed)
A lot of programming languages have been designed but the key point is missing in manay areas in their designs. 
Lanaguages should be easy for everyone to understand and implement their ideas.

This design is meant to be the kind that is easy to pick-up by beginners and easy to 
code and understand the code in the next time your come back to it without much thinking. 
It just reads  natural. My intension is not to create a new language but use the 
ideas available to create something better.

```d
//import whole package
import std;

import just module from packages
import std.io;

//import function from module 
import std.json: toString;

//import more than one functions from module 
import std.string, std.math: (cos, sin, ...);



//Entry Point
void main() {

    //Integers should read natural
    int8 number1 = 10;
    int16 number2 = 10;
    int32 number3 = 10;
    int64 number4 = 10;
    
    string name = "John";
    
    float8 amount = 10.00;
}

//auto is where compiler determines the type during compilation
auto foo(string = "hello") {}

//universal function call syntax (UFCS)
string name = "John";
foo(name);

name.foo(); //compiler translates as foo(name);

void foo(string name, int8 age=10, id=2 /* type is determined by compiler */) {}
string name = "John";
auto age = 3;
auto id = 0;

foo(name, age, id);
name.foo(age, id); // i.e. UFCS, where compiler interpretes as foo(name, age, id);
name.foo(age); //third argument is the default parameter




//cal wihout parenthesis
name.foo 


class Student {}
Student s = new Student() // or new Student




```
