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

======================
Basic output: Text
======================

