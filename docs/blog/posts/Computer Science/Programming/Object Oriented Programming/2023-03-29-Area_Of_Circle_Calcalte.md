---
date: 2023-03-29
tags:
       - C++
       - OOP
---
# Calculating the Area of a Circle in C++
- Here's the complete code for our program:
```cpp
#include <iostream>
using namespace std;

float area(float r);

int main() {
    float rad;
    cout << "Enter Half Radius" << endl;
    cin >> rad;
    cout << "area = " << area(rad) << endl;
    return 0;
}

float area(float r) {
    const float Pi = 3.14;
    return Pi * r * r;
}
```
## Explanation
1. Include the iostream Library: This library is included to allow input and output operations.
```cpp
#include <iostream>
using namespace std;
```
2. Function Declaration: We declare a function area that takes a float parameter r (the radius) and returns the area of the circle.
```cpp
float area(float r);
```
3. Main Function: The main function is the entry point of the program. It prompts the user to enter the radius, calls the area function, and prints the result.
```cpp
int main() {
    float rad;
    cout << "Enter Half Radius" << endl;
    cin >> rad;
    cout << "area = " << area(rad) << endl;
    return 0;
}
```
4. Area Calculation: The area function calculates the area using the formula ( \pi \times r^2 ). We use a constant value for Pi (3.14).
```cpp
float area(float r) {
    const float Pi = 3.14;
    return Pi * r * r;
}
```