---
date: 2023-03-29
tags:
       - C++
       - OOP
---
# Summing Elements of a Matrix in C++
- Here's the complete code for our program:
```cpp
#include<iostream>
using namespace std;

int main() {
    int arr[3][3] = { {100, 20, 50}, {80, 50, 70}, {50, 30, 40} };
    int sum = 0;
    int sumD = 0;

    // Calculate the sum of all elements in the matrix
    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 3; j++) {
            sum += arr[i][j];
        }
    }
    cout << "Total Matrix Values Is: " << sum << endl;

    // Calculate the sum of diagonal elements in the matrix
    for (int i = 0; i < 3; i++) {
        sumD += arr[i][i];
    }
    cout << "Total Matrix Diagonal Values Is: " << sumD << endl;

    return 0;
}
```
## Explanation
1. Include the iostream Library: This library is included to allow input and output operations.
```cpp
#include <iostream>
using namespace std;
```
2. Main Function: The main function is the entry point of the program. It initializes a 3x3 matrix with predefined values and variables to store the sums.
```cpp
int main() {
    int arr[3][3] = { {100, 20, 50}, {80, 50, 70}, {50, 30, 40} };
    int sum = 0;
    int sumD = 0;
}
```
3. Sum of All Elements: The program calculates the sum of all elements in the matrix using nested loops.
```cpp
for (int i = 0; i < 3; i++) {
    for (int j = 0; j < 3; j++) {
        sum += arr[i][j];
    }
}
cout << "Total Matrix Values Is: " << sum << endl;
```
4. Sum of Diagonal Elements: The program calculates the sum of the diagonal elements (where the row index equals the column index).
```cpp
for (int i = 0; i < 3; i++) {
    sumD += arr[i][i];
}
cout << "Total Matrix Diagonal Values Is: " << sumD << endl;
```