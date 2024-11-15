---
date: 2023-03-29
tags:
       - C++
       - OOP
---
# Study Estimates System in C++
- Here's the complete code for our program:
```cpp
#include<iostream>
using namespace std;

int main() {
    int degree;
    cout << "Please Enter Degree \n";
    cin >> degree;
    if (degree >= 85)
        cout << "Excellent \n";
    else if (degree >= 75)
        cout << "Very Good \n";
    else if (degree >= 65)
        cout << "Good \n";
    else if (degree >= 50)
        cout << "Passed \n";
    else
        cout << "Failed \n";
}
```
## Explanation
1. Include the iostream Library: This library is included to allow input and output operations.
```cpp
#include <iostream>
using namespace std;
```
2. Main Function: The main function is the entry point of the program. It prompts the user to enter their degree score and evaluates it.
```cpp
int main() {
    int degree;
    cout << "Please Enter Degree \n";
    cin >> degree;
}
```
3. Conditional Checks: The program uses conditional statements to categorize the degree score into different performance levels.
```cpp
if (degree >= 85)
    cout << "Excellent \n";
else if (degree >= 75)
    cout << "Very Good \n";
else if (degree >= 65)
    cout << "Good \n";
else if (degree >= 50)
    cout << "Passed \n";
else
    cout << "Failed \n";
```