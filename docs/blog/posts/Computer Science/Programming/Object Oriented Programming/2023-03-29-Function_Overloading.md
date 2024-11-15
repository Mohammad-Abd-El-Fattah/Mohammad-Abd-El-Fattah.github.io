---
date: 2023-03-29
tags:
       - C++
       - OOP
---
# Function Overloading
- Here's the complete code for our program:
```cpp
#include<iostream>
using namespace std;

int x(int n, int m) {
    return n * m;
}

double x(double n, int m) {
    return n - m;
}

int main() {
    cout << "Value = " << x(5, 2) << endl;
    cout << "Value = " << x(2.5, 8) << endl;
    return 0;
}
```
## Explanation
1. Include the iostream Library: This library is included to allow input and output operations.
```cpp
#include <iostream>
using namespace std;
```
2. Function Overloading: We define two functions with the same name x but different parameter types.
```cpp
int x(int n, int m) {
    return n * m;
}

double x(double n, int m) {
    return n - m;
}
```
3. Main Function: The main function calls the overloaded functions with different arguments.
```cpp
int main() {
    cout << "Value = " << x(5, 2) << endl;
    cout << "Value = " << x(2.5, 8) << endl;
    return 0;
}
```