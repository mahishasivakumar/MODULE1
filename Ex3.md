# Ex.No:3
# Ex.Name:Write a C++ program to calculate the mean of two integers using friend function, read the values from user through a member function of a class.

## Date:

## Aim:
To write a C++ program to calculate the mean of two integers using a friend function, where the values are read through a member function of a class.


## Algorithm:

STEP 1: Start the program.

STEP 2: Create a class MeanCalc to store two integers.

STEP 3: Declare two private integer data members.

STEP 4: Declare a public member function to read the two integers from the user.

STEP 5: Declare a friend function findMean() inside the class.

STEP 6: Define the friend function outside the class.

STEP 7: Inside the friend function, access the private data members of the object.

STEP 8: Compute the mean using the formula:
  mean = (a + b) / 2

STEP 9: Display the calculated mean value.

STEP 10: End the program.




## Program:
```
#include <iostream>
using namespace std;

class A {
    int x, y;
public:
    void read() {
        cin >> x >> y;
    }
    friend void mean(A o);
};

void mean(A o) {
    int m = (o.x + o.y) / 2;
    cout << "Mean value:" << m;
}

int main() {
    A a;
    a.read();
    mean(a);
}

```



## Output:
<img width="575" height="306" alt="{DF3ECEBA-6240-4204-8849-67DAA4BE2BA9}" src="https://github.com/user-attachments/assets/54fffec2-0e05-4cff-a23e-9073a0a56439" />



## Result
Thus, the program successfully reads two integers from the user using a member function and calculates the mean using a friend function.

