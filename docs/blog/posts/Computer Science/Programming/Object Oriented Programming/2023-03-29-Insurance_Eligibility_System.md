---
date: 2023-03-29
tags:
       - C++
       - OOP
---
# Insurance Eligibility System in C++

- Here's the complete code for our program:
```cpp
#include <iostream>
using namespace std;

int main() {
    int marital, gender;
    int age;
    cout << "Enter 1 For Single and 2 For Married \n";
    cin >> marital;
    if (marital != 2)
        goto step2;
    if (marital == 2)
        goto step1;

step1:
    if (marital == 2)
        cout << "You Are Insured";
    goto final;

step2:
    cout << "Enter 1 For Male and 2 For Female \n";
    cin >> gender;
    cout << "Enter Your Age\n";
    cin >> age;

    if ((marital == 1) && ((gender == 1 && age >= 30) || (gender == 2 && age >= 25))) 
        cout << "You Are Insured";
    else
        return 0;

final:
    return 0;
}
```
## Explanation
1. Include the iostream Library: This library is included to allow input and output operations.
```cpp
#include <iostream>
using namespace std;
```
2. Main Function: The main function is the entry point of the program. It initializes variables for marital status, gender, and age.
```cpp
int main() {
    int marital, gender;
    int age;
}
```
3. Input Marital Status: The program prompts the user to enter their marital status (1 for single, 2 for married).
```cpp
cout << "Enter 1 For Single and 2 For Married \n";
cin >> marital;
if (marital != 2)
    goto step2;
if (marital == 2)
    goto step1;
```
4. Married Case: If the user is married, they are automatically insured.
```cpp
step1:
if (marital == 2)
    cout << "You Are Insured";
goto final;
```
5. Single Case: If the user is single, the program prompts for gender and age, then checks if they meet the insurance criteria.
```cpp
step2:
cout << "Enter 1 For Male and 2 For Female \n";
cin >> gender;
cout << "Enter Your Age\n";
cin >> age;

if ((marital == 1) && ((gender == 1 && age >= 30) || (gender == 2 && age >= 25))) 
    cout << "You Are Insured";
else
    return 0;
```
6. Final Step: The program ends after displaying the insurance status.
```cpp
final:
return 0;
```