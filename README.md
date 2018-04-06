# averageOf5Numbers
Finds the average of any 5 numbers
//The user enters 5 numbers and then their average is displayed on the screen

#include "stdafx.h"
#include<iostream>;
  using namespace std;
  
  int main()
  {
    int num1,num2,num3,num4,num5,average;
    cout<<"Enter 5 numbers seperated by spaces: ";
    cin >> num1 >> num2 >> num3 >> num4 >> num5;
    average = (num1+num2+num3+num4+num5)/5;
    cout << "The average of the 5 numbers is: " << average <<endl;
    system("pause");
    return 0;
   }
