###### Modified by Josh Beto

## Introduction to Streams / Problem Solving


### Streams Intro: cout & cin

* ```cout``` and ```cin``` are *variables* provided by ```iostream```
* ```cout``` is of type ```ostream```
* ```cin``` is of type ```istream```

* When we use ```cout <<```, we write to a source ```stdout```, your console
* When we use ```cin >>```, we read from a source ```stdin```, your keyboard

* Sources for ```istream``` and ```ostream``` type variables can be different depending on where you want to read or write from.
* Some examples of sources include: files, other programs, networks, etc.

### Buffer
* Future lecture

### Operators

* You can think of operators as a special kind of *function*
* Operators take in a set of arguments and may return a value
* Take the ```+``` operator as an example:
```cpp
int main() {
    int x = 3 + 2; // '+' operator takes in arguments '3' and '2', adds them, and returns '5'
    return 0;
}
```

* Like functions, operators can also be *overloaded*
```cpp
/*  In this example, the '<<' operator takes in multiple types. This is how
    you are able to use cout << *type* with many different types from 'int' to 'double'! 
*/
ostream& operator<< (bool val);
ostream& operator<< (int val);
ostream& operator<< (double val);
```

* *Challenge*: Why are you able to chain together multiple ```<<``` or ```>>``` respectively? 
* *Hint*: Look back on what ```<<``` and ```>>``` return and the ```cin``` and ```cout``` types


### Problem Solving Tips
* If you get stuck on a part, skip to the parts you know and *abstract* the parts you do not know. *Abstract* means to understand what something does, but not think about how it is done. 
* Example: You have a function ```bool isAcceptable(int x)``` and need to remove elements within a ```vector<int>``` *v* that are considered not acceptable. You can simply call ```isAcceptable(int x)``` to check for which elements to remove even if you do not know how to write ```bool isAcceptable(int x)```

### Mini Quiz
* Part 1: Write a function to calculate the digital root of a number. The definition of a digital root can be found here: https://en.wikipedia.org/wiki/Digital_root
* Part 2: Implement the following function: ```highestRoot(const vector<int> &v)```. This function returns the number within *v* with the highest digital root. Assume *v* is nonempty.
* Part 3: Write a main that generates 10 random integers from range 10-999 and prints the integer with the highest digital root among them.
