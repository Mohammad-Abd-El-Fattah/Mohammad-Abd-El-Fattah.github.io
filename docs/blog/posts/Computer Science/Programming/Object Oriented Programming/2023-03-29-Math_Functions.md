---
date: 2023-03-29
tags:
       - C++
       - OOP
---
# Math Functions in C++
- Here's the complete code for our program:
```cpp
#include <iostream>
#include <cmath> 
using namespace std;

int main() {
    int x = 4;
    int y = 2;
    int z = -3;
    
    cout << "Square root = " << sqrt(x) << endl;
    cout << "Power = " << pow(x, y) << endl; 
    cout << "Abs = " << abs(z) << endl; 
    
    return 0;
}
```
## Explanation
1. Include the cmath Library: This library is included to provide access to common mathematical functions.
```cpp
#include <cmath>
```
2. Main Function: The main function is the entry point of the program. It initializes three integers and uses built-in functions to calculate the square root, power, and absolute value.
```cpp
int main() {
    int x = 4;
    int y = 2;
    int z = -3;
    
    cout << "Square root = " << sqrt(x) << endl;
    cout << "Power = " << pow(x, y) << endl;
    cout << "Abs = " << abs(z) << endl;
    
    return 0;
}
```
3. Square Root Calculation: The sqrt function calculates the square root of x.
```cpp
cout << "Square root = " << sqrt(x) << endl;
```
4. Power Calculation: The pow function calculates x raised to the power of y.
```cpp
cout << "Power = " << pow(x, y) << endl;
```
5. Absolute Value Calculation: The abs function calculates the absolute value of z.
```cpp
cout << "Abs = " << abs(z) << endl;
```