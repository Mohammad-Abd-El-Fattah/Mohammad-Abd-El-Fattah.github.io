---
date: 2023-03-29
tags:
       - C++
       - OOP
---
# Adding Elements of a 2D Array in C++
- Here's the complete code for our program:
```cpp
#include <iostream>
using namespace std;

int main() {
    int sumA = 0; 
    int sumB = 0;
    int sumC = 0;
    int sumD = 0;

    int arr[3][3] = { {1, 2, 3}, {4, 5, 6}, {7, 8, 9} };

    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 3; j++) {
            cout << arr[i][j] << "\n";
        }
    }

    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 3; j++) {
            if (i == j)
                sumA += arr[i][j];
        }
    }
    cout << "sumA = " << sumA << " ";
    cout << endl;

    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 3; j++) {
            if (i + j == 2)
                sumB += arr[i][j];
        }
    }
    cout << "sumB = " << sumB << " \n ";

    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 3; j++) {
            if (i < j)
                sumC += arr[i][j];
        }
    }
    cout << "sumC = " << sumC << " \n ";

    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 3; j++) {
            if (i > j)
                sumD += arr[i][j];
        }
    }
    cout << "sumD = " << sumD << " \n ";

    return 0;
}
```
## Explanation
1. Include the iostream Library: This library is included to allow input and output operations.
```cpp
#include <iostream>
using namespace std;
```
2. Main Function: The main function is the entry point of the program. It initializes the sums to zero and defines a 3x3 array with predefined values.
```cpp
int main() {
    int sumA = 0; 
    int sumB = 0;
    int sumC = 0;
    int sumD = 0;

    int arr[3][3] = { {1, 2, 3}, {4, 5, 6}, {7, 8, 9} };
}
```
3. Print Array Elements: The program prints each element of the array.
```cpp
for (int i = 0; i < 3; i++) {
    for (int j = 0; j < 3; j++) {
        cout << arr[i][j] << "\n";
    }
}
```
4. Sum of Diagonal Elements: The program calculates the sum of the main diagonal elements (where the row index equals the column index).
```cpp
for (int i = 0; i < 3; i++) {
    for (int j = 0; j < 3; j++) {
        if (i == j)
            sumA += arr[i][j];
    }
}
cout << "sumA = " << sumA << " ";
cout << endl;
```
5. Sum of Anti-Diagonal Elements: The program calculates the sum of the anti-diagonal elements (where the sum of the row and column indices equals 2).
```cpp
for (int i = 0; i < 3; i++) {
    for (int j = 0; j < 3; j++) {
        if (i + j == 2)
            sumB += arr[i][j];
    }
}
cout << "sumB = " << sumB << " \n ";
```
6. Sum of Elements Above the Main Diagonal: The program calculates the sum of the elements above the main diagonal (where the row index is less than the column index).
```cpp
for (int i = 0; i < 3; i++) {
    for (int j = 0; j < 3; j++) {
        if (i < j)
            sumC += arr[i][j];
    }
}
cout << "sumC = " << sumC << " \n ";
```
7. Sum of Elements Below the Main Diagonal: The program calculates the sum of the elements below the main diagonal (where the row index is greater than the column index).
```cpp
for (int i = 0; i < 3; i++) {
    for (int j = 0; j < 3; j++) {
        if (i > j)
            sumD += arr[i][j];
    }
}
cout << "sumD = " << sumD << " \n ";
```