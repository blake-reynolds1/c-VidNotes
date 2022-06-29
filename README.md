# C++ Introduction
* note: Possibly look up each section to see how it differs with java
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
* declared the same as java
  - ```
    int luckyNums[] = {1, 2, 3, 4};
    luckyNums[1] = 5;
    cout << luckyNums[1];
    ```
  - output: 5
  - ```
    int nums[10] = {1, 2, 3};
    nums[10] = 5;
    cout << nums[10];
    ```
# Functions
* function is a collection of code that preforms specific tasks, like a method
  - ```
    int main() {
    return 0;
    }
    ```
* void : function does not return anything (no return type)
  - ```
    void sayHi() {
      cout << "Hello";
    }
    int main() {
    cout << "Top";
    sayHi(); // call function
    cout << "bottom";
    return 0;
    }
    ```
  - output: TopHelloBottom
  - ```
    void sayHi(string name, int age) {
      cout << "Hello" << name << "you are " << age << endl;
    }
    int main() {
    sayHi("Bill", 5);
    sayHi("Mike", 10):
    return 0;
    }
    ```
    - output: Hello Bill you are 5 [newline] Hello Mike you are 10
* cannot put a function below the main if the main is calling
  - ```
    int main() {
    sayHi("Bill", 5);
    return 0;
    }
    void sayHi(string name, int age) {
    cout << "Hello" << name << "you are " << age << endl;
    }
    ```
  - output: ERROR
* Function stub to make the function work
  - ```
    void sayHi(string name, int age);
  
    int main() {
    sayHi("Bill", 5);
    return 0;
    }
    void sayHi(string name, int age) {
    cout << "Hello" << name << "you are " << age << endl;
    }
    ```
  - output: Hello Bill you are 5
# Return type
* return type works the same as java
  - ```
    double cube(double num) {
    double result = num * num * num; // could return num * num * num instead
    return result: 
    }
    int main() {
    double answer = cube(5.0);
    cout << answer;
    ```
    - output: 125
# If statements
* if statements work the same as java
  - ```
    bool isMale = true;
    if (isMale) {
    cout << "You are a male"; 
    }
    else {
    cout << "You are not male";
    }
    ```
  - output: You are a male
* && - both have to be true 
* || - one has to be true 
  - ```
    bool isTall = true;
    bool isMale = true;
    if(isMale && isTall) { //both have to be true
    cout << "You are a tall male";
    } else {
    cout << "You are not tall or not a man";
    }
    ```
  - output: You are a tall male
* else if
  - ```
    bool isTall = true;
    bool isMale = false;
    if(isMale && isTall) { 
    cout << "You are a tall male";
    } else if(isMale && !isTall) {
    cout << "You are a male but not tall";
    } else if(!isMale && isTall) {
    cout << "You are tall but not male";
    } else {
    cout << "You are not tall and not a man";
    }
    ```
  - output: You are tall but not male
# More If Statements
* Using comparisons in if statements
* Work the same as java
  - ```
    int getMax(int num, int num2, int num3) {
    int result;
    if (num >= num2 && num >= num3) {
    result = num;
    } else if (num2 >= num && num2 >= num3) {
    result = num2
    } else {
    result = num3;
    }
    return result;
    }
    int main() {
    int max = getMax(5, 4, 1)
    cout << max;
    return 0;
    }
    ```
  - output: 5 
# Building a better calculator
* ```
  int main() {
    int num1, num2;
    char op;
    cout << "Enter first number: ";
    cin >> num1;
    cout << "Enter operator: ";
    cin >> op;
    cout << "Enter second number: ";
    cin >> num2;
    int result;
    if(op == '+') {
      result = num1 + num2;
    }
   else if(op == '-') {
     result = num1 - num2;
    }
   else if(op == '/') {
      result = num1 / num2;
   }
   else if(op == '*') {
     result = num1 * num2;
   }
    else {
      cout << "Invalid operator";
    }
    cout << result;
  }
  ```
- output: Enter first number: -5- [newline] Enter operator: -+- [newline] Enter second number: -2- [newline] 7
# Switch statement
* Switch statements are special type of if statements
* ```
  string getDayOfWeek(int dayNum) {
    string dayName;
    // stopped at case 2 but can go farther
    switch(dayNum) {
      case 0: 
        dayName = "Sunday";
        break; // stops if case 0 is true
      case 1:
        dayName = "Monday";
        break;
      case 2:
        dayName = "Tuesday";
        break;
      default: // if no cases are true
        dayName = "Invalid day number";
    }
    return dayName;
  }
  int main() {
    cout << getDayOfWeek(2);
  }
  ```
  - output: Tuesday
# While loops
* Works the same as java
  - ```
    int index = 1;
    while(index <= 5) {
      cout << index;
      index++;
    }
    ```
  - output: 12345
* do while loop - like a while reversed. do first then check condititon
  - ```
    int index = 6;
    do {
      cout << index << endl;
      index++;
    } while (index <=5);
    ```
  - output: 6
# Building Guessing game
* ```
  int main() {
   int secretNum = 6;
   int guess;
   int guessCount = 0;
   bool outOfGuesses = false;
   while (secretNum != guess && !outOfGuesses) {
    if (guessCount <= 3) {
     cout << "Enter guess: ";
     cin >> guess;
     guessCount++;
    }
    else {
      outOfGuesses = true;
    }
   }
   if (outOfGuesses) {
    cout << "You lose!"
   }
   else {
   cout << "You Win!";
   }
  }
  ```
output: Enter guess: -2- [newline] Enter guess: -4- [newline] Enter guess: -6- [newline] You win!
# For loops
* Same as java
  - ```
    for (int i = 1; i <= 5; i++) {
      cout << index;
    }
    ```
  - output: 12345
  - ```
    int nums[] = {1, 2, 3, 4, 5}
    for (int i = 0; i < 5; i++) {
      cout << nums[i];
    }
    ```
  - output: 12345
# Building an Exponent function
* ```
  int power(int base, int pow) {
    int result = 1;
    for (int i = 0; i < pow; i++) {
      result = result * base;
    }
    return result;
  }
  int main() {
    cout << power(4, 3);
  }
  ```
  - output: 64
# 2d Arrays and nested loops
* 2d array
  - ```
    int numGrid[3][2] = {         // 2 columns, 3 rows
                          {1, 2}, // 1st element
                          {3, 4}, // 2nd element
                          {5, 6}  // 3rd element
                      };
    cout << numGrid[0][1] << endl;
    cout << numGrid[2][0];
    ```
  - output: 1 [newline] 5
* nested for loop
  - ```
    int numGrid[3][2] = {         
                          {1, 2}, 
                          {3, 4}, 
                          {5, 6}  
                      };
    for(int i = 0; i < 3; i++) {
      for (int x = 0; x < 2; x++) {
        cout << numGrid[i][x];
      }
      cout << endl;
    }
    ```
  - output: 12 [newline] 34 [newline] 56 [newline]
# Pointers
* pointer is a type of information that we can work with, basically memory addresses
* RAM - random access memory
* pointer uses RAM
  - ```
    int age = 19;
    double gpa = 3.2;
    string name = "Mike";
    cout << &age << endl; // print the memory address where age is stored
    cout << &gpa; << endl;
    cout << &name;
    ```
  - output: 0x6afee0 [newline] 0x6afee0 [newline] 0x6afedc
  - ```
    int age = 19;
    int *ptrAge = &age;  // container where we can store a ptr
    double gpa = 3.2;
    double *ptrGpa = &gpa // ptr has to have the same variable
    string name = "Mike";
    string *ptrName = &name; 
    cout << ptrAge;
    ```
  - output: 0x6afedc
* Dereferencing a pointer - grab the value that's inside of the memory address
  - ```
    int age = 19;
    int *ptrAge = &age;
    cout << *ptrAge; // dereference ptr
    ```
  - output: 19
  - ```
    double gpa = 3.2;
    double *ptrGpa = &gpa;
    cout << *&gpa; // dereference
    ```
  - output: 3.2
# Classes and Object
* class - blueprint for a new data type 
* Object - instance of the class
* ```
  class Book {  //blueprint
    public:
      string title;
      string author;
      int pages;
  };
  int main() {
    Book book1; // object
    book1.title = "Harry Potter"; // attributes
    book1.author = "J.K. Rowling";
    book1.pages = 500;
    Book book2; // object
    book2.title = "Lord of the Rings"; // attributes
    book2.author = "Tolkein";
    book2.pages = 700;
    cout << book1.title << endl;
    cout << book2.pages << endl;
  }
  ```  
  - output: Harry Potter [newline] 700
# Constuctor functions
* constructor - special function that gets called whenever we create a object of class
  - ```
    class Book {  
     public:
       string title;
       string author;
       int pages;
       Book() { //constructor
          cout << "Creating object" << endl;
       }
    };
    int main() {
      Book book1; // object
     Book book2; // object
    }
    ```
  - output: Creating object [newline] Creating object
  - ```
    class Book {  
     public:
        string title;
        string author;
        int pages;
        Book(string name) {
          cout << name << endl;
        }
    };
    int main() {
     Book book1("Harry Potter");
     Book book2("Lord of the Rings");
    }
    ```
  - output: Harry Potter [newline] Lord of the Rings
  - ```
    class Book {  
     public:
        string title;
        string author;
        int pages;
        Book() {
          title = "no title";
          author = 'no author"
          pages = 0;
        Book(string aTitle, string aAuthor, int aPages) {
          title = aTitle;
          author = aAuthor;
          pages = aPages;
        }
    };
    int main() {
     Book book1("Harry Potter", "JK Rowling", 5000);
     Book book2("Lord of the Rings", "Tolkein", 700);
     Book book3()
     cout << book1.title << endl;
     cout << book3.title;
    }
    ```
  - output: Harry Potter [newline] no title
# Object Functions
* Object functions - function that we can put in our classes
  - ```
    class Student {
      public:
        string name;
        string major;
        Student(string aName, string aMajor, double aGpa) {
          name = aName;
          major = aMajor;
          gpa = aGpa;
        }
        bool hasHonors() {
          if (gpa > 3.5) {
            return true;
          }
          else {
            return false;
          }
        }
    };
    int main() {
      Student student1("Jim", "Business", 2,4);
      Student student2("Pam", "art", 3.6);
      cout << student1.hasHonors(); // 0 output means false
      cout << student2.hasHonors(); // 1 output means true
    }
  - output: 01
# Getters and Setters
* getters and setters - allow you to control the access to the different attributes and elements in classes
  - ```
    class Movie {
      private: // main can't access these variables
        string rating;
      public: 
        string title;
        string director;
        Movie(string aTitle, string aDirector, string aRating) {
          title = aTitle;
          director = aDirector;
          setRating(aRating);
        }
        void setRating(string aRating) {
          if (aRating == "G" || aRating == "PG" || aRating == "PG-13" || aRating = "R") {
            rating = aRating;
          }
          else {
            rating = "NR";
          }
        }
        string getRating() {
          return rating;          
    };
    int main() {
      Movie avengers("The Avengers", "Joss Whedon", "PG-13");
      avengers.setRating("Dog"); // if commented out - the output would be PG-13
      cout << avengers.getRating();
    }
    ```
  - output: NR
# Inheritance
* Inheritance - define a class and define other classes and those classes can extend the functionality or inherit all the functionality all the attributes of that original class
  - ```
    class Chef {
      public:
        void makeChicken() {
          cout << "The chef makes chicken" << endl;
        }
        void makeSalad() {
          cout << "The chef makes salad" << endl;
        }
        void makeSpecialDish() {
          cout << "The chef makes BBQ ribs" << endl;
        }
    };
    class ItalianChef : public Chef { // the ItalianChef has access to all the functionality of Chef
    };
      
    int main() {
      Chef chef;
      chef.makeChicken();
      ItalianChef italianChef;
      italianChef.makeChicken();
    }
    ```
  - output: The chef makes chicken [newline] The chef makes chicken
  - ```
    class Chef { // super class
      public:
        void makeChicken() {
          cout << "The chef makes chicken" << endl;
        }
        void makeSalad() {
          cout << "The chef makes salad" << endl;
        }
        void makeSpecialDish() {
          cout << "The chef makes BBQ ribs" << endl;
        }
    };
    class ItalianChef : public Chef { // subclass
      public: 
       void makePasta() {
          cout << "The chef makes pasta" << endl;
       }
       void makeSpecialDish() { // override 
          cout << "The chef makes chiken parm" << endl;
        }
    };
      
    int main() {
      Chef chef;
      chef.makesSpecialDish();
      ItalianChef italianChef;
      italianChef.makePasta();
      italianChef.makesSpecialDish();
    }
    ```
  - output: The chef makes BBQ ribs [newline] the chef makes pasta  [newline] the chef makes chicken parm

  
  
