# Introduction
* You need to build and run program to get an output
* ```
  #include <iostream>
  using namespace std
  ```
  - The configuration options for the cpp file
  - will talk abt later
* cout = console out
* endl = end line
# Variables
* you declare a string and int the same way in Java 
  - ```
    string myName = "Blake";
    ```
  - you can also declare a string or int without assigning it to a number or words 
  - ```
    int myAge;
    myAge = 21;
    ```
* Print out a variable with a line of text
  - ```
    cout << "My name is " << myName << endl;
    ```
  - output: My name is Blake
  - ```
    cout << "My name is " << myName << " and my age is " << myAge << endl;
    ```
  - output: My name is Blake and my age is 
  - ```
    string myName = "Blake";
    cout << "My name is " << myName << endl;
    myName = "James Blake";
    cout << "My new name is " << myName << endl;
    ```
  - output: My name is Blake [newline] My new name is James Blake
# Data Types
* Char is declared just as java
  - ```
    char grade = 'A'; 
    ```
* Float - floating point number. float can store less decimal points than double. 
  - talked abt later in the class, kinda the same as a double
* double is declared just as java
  - ```
    double gpa = 3.5
    ```
* Boolean is declared just as java but called "bool"
  - ```
    bool isMale = true;
    ```
* When printing out numbers, you don't have to use quotes
  - ```
    cout << 31 << endl;
    ```
# Working with Strings
* "endl" means that it prints a new line
  - ``` 
    cout << "Hello";
    cout << "Hi" << endl;
    ```
  - output: HelloHi 
* can use "\n" to make new line
  - ```
    cout << "Hello\n"
    cout << "Hi" << endl;
    ```
  - output: Hello [newline] Hi
* String functions: 
  - .legnth: gives length of string
  - ```
    string phrase = "Hello";
    cout << phrase.length();
    ```
  - output: 5
* []: gives specific character of string and can change letters of string
  - ```
    string phrase = "Hello";
    cout << phrase[1];
    ```
  - output: e
  - ```
    string phrase = "Hello";
    phrase[0] = 'B';
    cout << phrase;
    ```
  - output: Bello
* .find(string str, int index) : find the index of a character or string from a specific string by giving a keyword within that specific string and an index on where to start
  - ```
    string phrase = "Hello";
    cout << phrase.find("lo", 0);
    ```
  - output: 4
* .substr(int index, int length) : takes a substring of a specific string by giving it a starting index and a length of how long of a substring. 
  - ```
    string phrase = "Hello";
    cout << phrase.substr(1, 3);
    ```
  - output: ell
  - ```
    string phrase = "Hello";
    string phraseSub;
    phraseSub = phrase.substr(1, 3)
    cout << phraseSub
    ```
  - output: ell
# Working with Numbers
* You can print out integers and doubles without quotes
  - ```
    cout << -40;
    ```
  - output: -40
* You can also print addition, subtraction, division, multiplication, and module opertaion (%) 
  - ```
    cout << 5 + 6;
    ```
  - output: 11
  - ```
    cout << 5 + 4 * 2;
    ```
  - output: 13
* You can do the same (++) or (--) with integer variables
  - ```
    int wnum = 5;
    wnum++;
    ```
* it prints out decimal number with a int and double
  - ```
    int num1 = 5;
    double num2 = 1.5;
    cout << num1 + num2;
    ```
  - output: 6.5
* A function is a collection of code that will perform a specific task
* To use math functions you have to put "#include <cmath>" at the top of the code
* pow(int num1, int num2): num1 to the power of num2
  - ```
    cout << pow(3, 2);
    ```
  - output: 9
* sqrt(int num): gives square root of num
  - ```
    cout << sqrt(9);
    ```
  - output: 3
* round(int num): rounds the num
  - ```
    cout << round(4.6);
    ```
  - output: 5
* ceil(int num): rounds up no matter what
* floor(int num): round down no matter what
* fmax(int num1, int num2): returns the bigger number
  - ```
    cout << fmax(3, 10);
    ```
  - output: 10
* fmin(int num1, int num2): returns smaller number
# Getting User Input
* when given information, you need to store it in a variable
* 
* ```
  int age;
  cout << "Enter your age: ";
  cin >> age; // user input
  cout << "You are " << age << " years old";
  ```
* Output: Enter your age: ____ [enter] You are ___ years old
  - the ____ is the user input
* double, and char works the same
* Strings work differently
* ```
  string name;
  cout << "Enter your name: "
  getline(cin, name);  // gets a text from the user
  cout << "Hello " << name;
  ```
* Output: Enter your name: ____ [enter] Hello _____
# Building a calculator
* ```
  #include <iostream>
  #include <cmath>
  using namespace std;
  
  int main() {
  double num1, num2; // can stack variables if they are the same data type
  cout << "Enter first number: ";
  cin >> num1;
  cout << "Enter second number: ";
  cin << num2;
  cout << num1 + num2;
  return 0;
  }
  ```
* Output: Enter first number: ____ [enter] Enter second number: ____ [enter] -(numbers added together)-
# Building a Madlibs game
* ```
  #include <iostream>
  #include <cmath>
  using namespace std;
  
  int main() {
  string color, pluralNoun, celebrity;
  cout << "enter a color: "
  getline(cin, color):
  cout << "enter a plural noun: ";
  getline(cin, pluralNoun);
  cout << "enter a celebrity: ";
  getline(cin, celebrity); 
  cout << "Roses are " << color << endl;
  cout << pluralNoun << " are blue" << endl;
  cout << "I love " << celebrity << endl;
  return 0;
  }
  ```
* output: enter a color: _____ [enter] enter a plural noun: ____ [enter] enter a celebrity: _____ [enter] Roses are -color- [newline] -pluralNoun- are blue [newline] I love -celebrity-
# Arrays

  
  
