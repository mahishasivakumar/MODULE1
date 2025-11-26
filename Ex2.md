# Ex.No2
# Ex.Name:Write a program in C++ to convert temperature in Fahrenheit to Celsius using class methods(define member as private & define methods within class)
## Date:

## Aim:
To write a C++ program using a class to convert temperature from Fahrenheit to Celsius by defining data members as private and methods within the class.

## Algorithm:
STEP 1: Start the program.
STEP 2: Create a class named Temperature.
STEP 3: Declare a private data member fahrenheit.
STEP 4: Inside the class, define a public method getData() to read Fahrenheit value from the user.
STEP 5: Define another public method convert() to convert Fahrenheit to Celsius using the formula:
  Celsius = (Fahrenheit − 32) × 5 / 9
STEP 6: Define a method display() to print the Celsius value.
STEP 7: In the main() function, create an object of the Temperature class.
STEP 8: Call the method getData() to input Fahrenheit.
STEP 9: Call convert() and then display() to show the Celsius value.
STEP 10: End the program.


## Program:
```
#include <iostream>
using namespace std;
class conversion
{
    private:
    float f;
    public:
    void set(float x){
        f=x;
    }
    void temp()
    {
        cout<<"The temperature in Fahrenheit:"<<f<<endl;
        cout<<"The temperature in Celsius:"<<(f-32)*5/9;
    }
};
int main(){
    float fah;
    cin>>fah;
    conversion C;
    C.set(fah);
    C.temp();
}
```



## Output:
<img width="885" height="304" alt="{7AD94CC5-0155-4B70-9779-627152A57C74}" src="https://github.com/user-attachments/assets/fb263acf-c697-4e75-ac3d-6952100bdda8" />


## Result:
Thus, the C++ program is successfully executed to convert the temperature from Fahrenheit to Celsius using class methods with private data members.
