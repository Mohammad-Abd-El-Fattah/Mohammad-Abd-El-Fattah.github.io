---
date: 2023-03-29
tags:
       - C++
       - OOP
---
# Calculating the Factorial of a Number in C++
- Here's the complete code for our program:
```cpp
#include <iostream>
using namespace std;

unsigned long Factorial(int n) {
    if (n > 1)
        return n * Factorial(n - 1);
    else
        return 1;
}

int main() {
    int n;
    cout << "Enter Number :";
    cin >> n;
    cout << "Factorial=" << endl << Factorial(n);
    return 0;
}
```
## Explanation
1. Include the iostream Library: This library is included to allow input and output operations.
```cpp
#include <iostream>
using namespace std;
```
2. Recursive Function Definition: We define a function Factorial that takes an integer parameter n and returns the factorial of n. The function calls itself recursively until n is 1.
```cpp
unsigned long Factorial(int n) {
    if (n > 1)
        return n * Factorial(n - 1);
    else
        return 1;
}
```
3. Main Function: The main function is the entry point of the program. It prompts the user to enter a number, calls the Factorial function, and prints the result.
```cpp
int main() {
    int n;
    cout << "Enter Number :";
    cin >> n;
    cout << "Factorial=" << endl << Factorial(n);
    return 0;
}
```