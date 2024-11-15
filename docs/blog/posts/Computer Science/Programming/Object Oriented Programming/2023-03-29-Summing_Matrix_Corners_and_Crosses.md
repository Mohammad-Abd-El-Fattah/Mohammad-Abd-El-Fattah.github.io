---
date: 2023-03-29
tags:
       - C++
       - OOP
---
# Summing Matrix Corners and Crosses in C++
- Here's the complete code for our program:
```cpp
#include <iostream>
using namespace std;
int main() {
    int sumA = 0;
    int sumB = 0;
    int sumC = 0;
    int sumD = 0;
    int sumE = 0;
    int sumF = 0;
    int Array[3][3] = {
        {1, 2, 3},
        {4, 5, 6},
        {7, 8, 9}
    };
    int Array1[3][3] = {
        {10, 11, 12},
        {13, 14, 15},
        {16, 17, 18}
    };
    int sumArray[3][3];
    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 3; j++) {
            if (i == j)
                sumA += Array[i][j];
        }
    }
    cout << "sumA = " << sumA << " \n ";

    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 3; j++) {
            if (i + j == 2)
                sumB += Array[i][j];
        }
    }
    cout << "sumB = " << sumB << " \n ";

    
    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 3; j++) {
            if (i < j)
                sumC += Array[i][j];
        }
    }
    cout << "sumC = " << sumC << " \n ";


    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 3; j++) {
            if (i > j)
                sumD += Array[i][j];
        }
    }
    cout << "sumD = " << sumD << " \n ";
    
    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 3; j++) {
            if ((i > j) || (i < j))
                sumE += Array[i][j];
        }
    }
    cout << "sumE = " << sumE << " \n ";
    cout << endl;

    
    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 3; j++) {
            sumArray[i][j] = Array[i][j] + Array1[i][j];
        }
    }

    
    cout << "The Result of Adding Two Matrices is:\n";
    for (int i = 0; i < 3; i++) {
        for (int j = 0; j < 3; j++) {
            cout << sumArray[i][j] << " ";
        }
        cout << endl;
    }

    return 0;
}
```
## Explanation
1. Include the iostream Library: This library is included to allow input and output operations.
```cpp
#include <iostream>
using namespace std;
```
2. Main Function: The main function is the entry point of the program. It initializes two 3x3 matrices with predefined values and variables to store the sums.
```cpp
int main() {
    int sumA = 0;
    int sumB = 0;
    int sumC = 0;
    int sumD = 0;
    int sumE = 0;
    int sumF = 0;

    int Array[3][3] = {
        {1, 2, 3},
        {4, 5, 6},
        {7, 8, 9}
    };

    int Array1[3][3] = {
        {10, 11, 12},
        {13, 14, 15},
        {16, 17, 18}
    };

    int sumArray[3][3];
}
```
3. Sum of Right Diagonal: The program calculates the sum of the right diagonal elements (where the row index equals the column index).
```cpp
for (int i = 0; i < 3; i++) {
    for (int j = 0; j < 3; j++) {
        if (i == j)
            sumA += Array[i][j];
    }
}
cout << "sumA = " << sumA << " \n ";
```
4. Sum of Left Diagonal: The program calculates the sum of the left diagonal elements (where the sum of the row and column indices equals 2).
```cpp
for (int i = 0; i < 3; i++) {
    for (int j = 0; j < 3; j++) {
        if (i + j == 2)
            sumB += Array[i][j];
    }
}
cout << "sumB = " << sumB << " \n ";
```
5. Sum of Upper Right Triangle Values: The program calculates the sum of the elements above the main diagonal (where the row index is less than the column index).
```cpp
for (int i = 0; i < 3; i++) {
    for (int j = 0; j < 3; j++) {
        if (i < j)
            sumC += Array[i][j];
    }
}
cout << "sumC = " << sumC << " \n ";
```
6. Sum of Lower Left Triangle Values: The program calculates the sum of the elements below the main diagonal (where the row index is greater than the column index).
```cpp
for (int i = 0; i < 3; i++) {
    for (int j = 0; j < 3; j++) {
        if (i > j)
            sumD += Array[i][j];
    }
}
cout << "sumD = " << sumD << " \n ";
```
7. Sum of Upper Right and Lower Left Triangle Values: The program calculates the sum of the elements above and below the main diagonal (excluding the diagonal elements).
```cpp
for (int i = 0; i < 3; i++) {
    for (int j = 0; j < 3; j++) {
        if ((i > j) || (i < j))
            sumE += Array[i][j];
    }
}
cout << "sumE = " << sumE << " \n ";
```
8. Addition of Two Matrices: The program calculates the element-wise sum of the two matrices and stores the result in a third matrix.
```cpp
for (int i = 0; i < 3; i++) {
    for (int j = 0; j < 3; j++) {
        sumArray[i][j] = Array[i][j] + Array1[i][j];
    }
}
```
9. Print the Result of Adding Two Matrices: The program prints the result of the element-wise addition of the two matrices.
```cpp
cout << "The Result of Adding Two Matrices is:\n";
for (int i = 0; i < 3; i++) {
    for (int j = 0; j < 3; j++) {
        cout << sumArray[i][j] << " ";
    }
    cout << endl;
}
```