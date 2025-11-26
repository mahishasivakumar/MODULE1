# Ex.No:4
# Ex.Name:Write a C++ program to find the maximum of two numbers between 95, 64 and maximum of three numbers between 22,28,21 using constructor overloading.
## Date:
## Aim:
To write a C++ program using constructor overloading to find the maximum of two numbers (95, 64) and three numbers (22, 28, 21).

## Algorithm:
STEP 1: Start the program.

STEP 2: Create a class Maximum to perform maximum operations.

STEP 3: Declare private data members to store numbers.

STEP 4: Create a constructor with two parameters to find the maximum of two numbers.

STEP 5: Create another constructor with three parameters to find the maximum of three numbers.

STEP 6: Inside each constructor, compare the numbers using conditional statements.

STEP 7: Store the maximum value in a variable.

STEP 8: Define a public method display() to print the maximum result.

STEP 9: In main(), create an object with two arguments and another with three arguments.

STEP 10: Call the display() method for each object to show results.




## Program:
```
#include <iostream>
using namespace std;

class Max {
public:
    Max(int a, int b) {
        if(a > b)
            cout << a << " is greater\n";
        else
            cout << b << " is greater\n";
    }

    Max(int a, int b, int c) {
        if(a >= b && a >= c)
            cout << a << " is greater\n";
        else if(b >= a && b >= c)
            cout << b << " is greater\n";
        else
            cout << c << " is greater\n";
    }
};

int main() {
    Max m1(95, 64);
    Max m2(22, 28, 21);
}

```


## Output:
<img width="652" height="180" alt="{5E774F0D-4B64-4029-9195-491925353C2A}" src="https://github.com/user-attachments/assets/6c1893d4-03b6-4625-84aa-930f82dbd654" />



## Result:
Thus, the C++ program using constructor overloading successfully finds:

The maximum of 95 and 64 → 95

The maximum of 22, 28, 21 → 28
