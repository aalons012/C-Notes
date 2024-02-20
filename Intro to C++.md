A Simple C++ Program appears BELOW:

``` 
#include <iostream>
using namespace Std;

int main(){
};
```

A *PROGRAM* Always start with 
```
main()
```
Executing the statements within the main's braces "{}". 
One. 
At. 
A. 
Time.
As Shown Below (With an Example):
```
int main(){

  std::cout << " Hello, My Name is Andy";
  std::cout << endl;

return 0;
};
```
Noticed how every row for the code ended with a ";", or Semicolon. 
Each Statement typically appears on a line and ends with semicolon, as english would end sentences with a period.

The "cout" statements output various values.
The "return 0" statement ends the program
  - the 0 tells the operating system that the program ended without error

======================
Basic input
======================
Programs commonly get input values, perform some processing on that input, and put output values to a screen or elsewhere. Input is commonly gotten from a keyboard, a file, fields on a web form or app, etc.

The Following statement gets an input value and puts that value into variable
```
cin >> ...
```
"cin" is short for characters in.

Example below
```
#include <iostream>
include namespace std;

int main() {
  int wage;

  cin >> wage;

  cout << "Salary is ";
  cout << wage * 40 * 52
  cout << endl;

  return 0;
}
```
The cin >> wage statement gets an input value from the keyboard (or file, etc.) and puts that value into the wage variable. 
  - If you type the number 20, since theres an "int" on wage. The Input would be 20, so the wage = 20, since the "cin >> ..." code tells you to put number on the input.
  - input:
    - ```
      20
      ```
wage's value can then be used in subsequent processing and outputs.
  - Because of adding 20 for the cin >> wage it will then use the other statements that you've added. It will then multiply the wage times 40 times 52, and because of having the "cout" it will output the total number of the wage.
  - Output:
      - ```
        Salary is 41600
        ```

Basic output: Text
======================

The cout construct supports output; cout is short for characters out. Outputting text is achieved via: 

cout << "desired text";

Text in double quotes " " is known as a string literal. 
Multiple cout statements continue printing on the same output line. 
The statement cout << endl; starts a new output line, called a newline. 
  - Note endl is short for "end line".
  - A common error is to type the number "1" or a capital I as in "in", instead of a lower case l as in "end line".

Example(s):
1:
```
#include <iostream>
using namespace std;

int main() {

   cout << "Keep calm";
   cout << "and";
   cout << "carry on";

   return 0;
}
```
Output: 
```
Keep calmandcarry on
```
2:
```
#include <iostream>
using namespace std;

int main() {

   cout << "Keep calm";
   cout << endl; 
   cout << "and";
   cout << endl; 
   cout << "carry on";
   cout << endl; 

   return 0;
}
```
Output: 
```
Keep calm 
and 
carry 
on
```
The notation  cout << ...  gives the appearance of the item on the right being "streamed" to cout (like items flowing along a stream into a lake), where cout represents the computer's screen.


Outputting a variable's value
============================

Outputting a variable's value is achieved via: cout << x;. Note that no quotes surround x.

Example
```
#include <iostream>
using namespace std;

int main() {
   int wage;
   
   wage = 20;

   cout << "Wage is: ";
   cout << wage; 
   cout << endl;
   cout << "Goodbye.";
   cout << endl;

   return 0;
}

Note that the programmer intentionally did not start a new output line after outputting "Wage is: " so that the wage variable's value would appear on that same line
```
Output
```
Wage is: 20
Goodbye.
```

Outputting multiple items with one statement
=============================================

Programmers commonly use a single output statement for each line of output by combining the outputting of text, variable values, and a new line. The programmer simply separates the items with << symbols. Such combining can improve program readability because the program's code corresponds more closely to the program's output.

Example:
```
#include <iostream>
using namespace std;

int main() {
   int wage;

   wage = 20;

   cout << "Wage is: " << wage << endl; 
   cout << "Goodbye." << endl;

   return 0;
}
```

Newline character
====================
A new output line can also be produced by inserting \n, known as a newline character, within a string literal. Ex: Outputting "1\n2\n3" outputs each number on its own output line. \n use is rare but appears in some existing code, so it is mentioned here. \n consists of two characters, \ and n, but together are considered as one newline character. Good practice is to use endl to output a newline, as endl has some technical advantages not mentioned here.


Comments
========
A comment is text a programmer adds to code, to be read by humans to better understand the code but ignored by the compiler. Two common kinds of comments exist:

  -  A single-line comment starts with // and includes all the following text on that line. Single-line comments commonly appear after a statement on the same line.
  -  A multi-line comment starts with /* and ends with */, where all text between /* and */ is part of the comment. A multi-line comment is also known as a block comment.


Whitespace
==========
Whitespace refers to blank spaces (space and tab characters) between items within a statement and blank lines between statements (called newlines). A compiler ignores most whitespace.

Good practice is to deliberately and consistently use whitespace to make a program more readable. Programmers usually follow conventions defined by their company, team, instructor, etc., such as:

  -  Use blank lines to separate conceptually distinct statements.
  -  Indent lines the same amount.
  -  Align items to reduce visual clutter.
  -  Use a single space before and after any operators like =, +, *, or <<
  -  to make statements more readable.

Example of using whitespace correctly:
```
#include <iostream>
using namespace std;

int main() {
   int myFirstVar;    // Aligned comments yield less
   int yetAnotherVar; // visual clutter 
   int thirdVar; 
  
   // Above blank line separates variable declarations from the rest
   cout << "Enter a number: ";
   cin  >> myFirstVar;
  
   // Above blank line separates user input statements from the rest   
   yetAnotherVar = myFirstVar;        // Aligned = operators
   thirdVar      = yetAnotherVar + 1; 
   // Also notice the single-space on left and right of + and =
   // (except when aligning the second = with the first =)

   cout << "Final value is " << thirdVar << endl; // Single-space on each side of <<
  
   return 0; // The above blank line separates the return from the rest
}
```

Example of using whitespace incorrectly:
```
#include <iostream>
using namespace std;
int main() {
int numPeople; int      totalOuncesPasta;     
cout<<"Enter number of people: ";cin>>numPeople;
totalOuncesPasta = numPeople * 3;  cout << "Cook " << totalOuncesPasta << " ounces of pasta." << endl;      return 0;}
```

