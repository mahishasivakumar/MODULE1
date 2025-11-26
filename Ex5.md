# Ex.No:5
# Ex.Name:Write a C++ program using friend function to find the minimum integer value  among the member of both the classes.
## Date:
## Aim:
To write a C++ program using a friend function to find the minimum integer value among the members of two different classes.

## Algorithm:
STEP 1: Start the program.

STEP 2: Create Class A with one private integer data member.

STEP 3: Create Class B with one private integer data member.

STEP 4: Declare a common friend function findMin() in both classes.

STEP 5: Define a public method in each class to input the integer value.

STEP 6: Define the friend function findMin() outside both classes.

STEP 7: In the friend function, access the private members of both classes.

STEP 8: Compare the integer values using if–else.

STEP 9: Display the smallest value.

STEP 10: End the program.




## Program:
```
#include <iostream>
using namespace std;

class A;
class B;

int findMin(A x, B y);

class A {
    int n;
public:
    A(int a) { n = a; }
    friend int findMin(A x, B y);
};

class B {
    int m;
public:
    B(int b) { m = b; }
    friend int findMin(A x, B y);
};

int findMin(A x, B y) {
    return (x.n < y.m) ? x.n : y.m;
}

int main() {
    A a(10);
    B b(7);
    cout << "Minimum value is " << findMin(a, b);
}

```


## Output:
<img width="712" height="325" alt="{1F59D5BA-7AA6-4482-91CB-47E4F1A0C291}" src="https://github.com/user-attachments/assets/14806ff0-aa36-462f-9cdc-29e9af4a459b" />




## Result:
Thus, the C++ program using a friend function successfully finds the minimum integer value among members of two different classes.


