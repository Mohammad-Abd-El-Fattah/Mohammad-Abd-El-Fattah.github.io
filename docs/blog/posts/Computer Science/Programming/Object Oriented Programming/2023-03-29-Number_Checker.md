---
date: 2023-03-29
tags:
       - C++
       - OOP
---
# Odd/Even and Positive/Negative Check
- Here's the complete code for our program:
```cpp
#include <iostream>
using namespace std;

int main() {
    int x;
    cout << "Enter Any Number \n";
    cin >> x;
    if ((x >= 0) && (x % 2 == 0))
        cout << "Number Is Positive Even \n";
    else if ((x <= 0) && (x % 2 == 0))
        cout << "Number Is Negative Even \n";
    else if ((x >= 0) && (x % 2 != 0))
        cout << "Number Is Positive Odd \n";
    else if ((x <= 0) && (x % 2 != 0))
        cout << "Number Is Negative Odd \n";
    else
        cout << "Enter Valid Number \n";
    return 0;
}
```
## Explanation
1. Include the iostream Library: This library is included to allow input and output operations.
```cpp
#include <iostream>
using namespace std;
```
2. Main Function: The main function is the entry point of the program. It prompts the user to enter a number and checks its properties.
```cpp
int main() {
    int x;
    cout << "Enter Any Number \n";
    cin >> x;
}
```
3. Conditional Checks: The program uses conditional statements to determine if the number is positive/negative and odd/even.
```cpp
if ((x >= 0) && (x % 2 == 0))
    cout << "Number Is Positive Even \n";
else if ((x <= 0) && (x % 2 == 0))
    cout << "Number Is Negative Even \n";
else if ((x >= 0) && (x % 2 != 0))
    cout << "Number Is Positive Odd \n";
else if ((x <= 0) && (x % 2 != 0))
    cout << "Number Is Negative Odd \n";
else
    cout << "Enter Valid Number \n";
return 0;
```