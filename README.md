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
