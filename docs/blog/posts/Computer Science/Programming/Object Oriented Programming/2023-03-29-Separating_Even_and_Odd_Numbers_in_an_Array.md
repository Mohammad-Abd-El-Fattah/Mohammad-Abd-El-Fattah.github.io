---
date: 2023-03-29
tags:
       - C++
       - OOP
---
# Separating Even and Odd Numbers in an Array Using C++

- Here's the complete code for our program:
```cpp
#include<iostream>
using namespace std;

int main() {
    int arr[5];
    int Total = 0;

    for (int i = 0; i < 5; i++) {
        cout << "Enter Value index of " << i << ": ";
        cin >> arr[i];
    }

    cout << "The Values Of Your Array are:\n";
    for (int i = 0; i < 5; i++) {
        cout << arr[i] << endl;
    }

    for (int i = 0; i < 5; i++) {
        Total += arr[i];
    }
    cout << "Total Value Of Array is " << Total << endl;

    cout << "Even Values In Your Array are:\n";
    for (int i = 0; i < 5; i++) {
        if (arr[i] % 2 == 0) {
            cout << arr[i] << " ";
        }
    }
    cout << endl;

    cout << "Odd Values In Your Array are:\n";
    for (int i = 0; i < 5; i++) {
        if (arr[i] % 2 != 0) {
            cout << arr[i] << " ";
        }
    }
    cout << endl;

    return 0;
}
```
## Explanation
1. Include the iostream Library: This library is included to allow input and output operations.
```cpp
#include <iostream>
using namespace std;
```
2. Main Function: The main function is the entry point of the program. It initializes an array of integers and a variable to store the total sum.
```cpp
int main() {
    int arr[5];
    int Total = 0;
}
```
3. Input Array Elements: The program prompts the user to enter values for each index of the array.
```cpp
for (int i = 0; i < 5; i++) {
    cout << "Enter Value index of " << i << ": ";
    cin >> arr[i];
}
```
4. Print Array Elements: The program prints each element of the array.
```cpp
cout << "The Values Of Your Array are:\n";
for (int i = 0; i < 5; i++) {
    cout << arr[i] << endl;
}
```
5. Calculate Total Sum: The program calculates the total sum of the array elements.
```cpp
for (int i = 0; i < 5; i++) {
    Total += arr[i];
}
cout << "Total Value Of Array is " << Total << endl;
```
6. Print Even Values: The program prints the even values in the array.
```cpp
cout << "Even Values In Your Array are:\n";
for (int i = 0; i < 5; i++) {
    if (arr[i] % 2 == 0) {
        cout << arr[i] << " ";
    }
}
cout << endl;
```
7. Print Odd Values: The program prints the odd values in the array.
```cpp
cout << "Odd Values In Your Array are:\n";
for (int i = 0; i < 5; i++) {
    if (arr[i] % 2 != 0) {
        cout << arr[i] << " ";
    }
}
cout << endl;
```