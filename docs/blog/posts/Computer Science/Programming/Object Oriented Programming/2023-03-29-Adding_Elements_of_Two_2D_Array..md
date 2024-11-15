---
date: 2023-03-29
tags:
       - C++
       - OOP
---
# Finding the Biggest Number Between Two Values in C++
- Here's the complete code for our program:
```cpp
#include<iostream>
using namespace std;

int bignum(int num1, int num2) {
    if (num1 > num2)
        return num1;
    else
        return num2;
}

int main() {
    int x, y;
    
    cout << "Enter Two Values" << endl;
    cin >> x >> y;
    
    cout << "Biggest number = " << bignum(x, y) << endl;
    return 0;
}
```
## Explanation
1. Include the iostream Library: This library is included to allow input and output operations.
```cpp
#include <iostream>
using namespace std;
```
2. Function Definition: We define a function bignum that takes two integer parameters and returns the larger of the two.
```cpp
int bignum(int num1, int num2) {
    if (num1 > num2)
        return num1;
    else
        return num2;
}
```
3. Main Function: The main function is the entry point of the program. It prompts the user to enter two values, calls the bignum function, and prints the result.
```cpp
int main() {
    int x, y;
    
    cout << "Enter Two Values" << endl;
    cin >> x >> y;
    
    cout << "Biggest number = " << bignum(x, y) << endl;
    return 0;
}
```