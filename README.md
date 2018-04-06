# averageOf5Numbers
Finds the average of any 5 numbers

#include "stdafx.h"
#include<iostream>;
using namespace std;

float findAverage(float, float, float, float, float);

int main()
{
	float num1, num2, num3, num4, num5, output;
	cout << "Enter 5 numbers seperated by spaces: ";
	cin >> num1 >> num2 >> num3 >> num4 >>num5;
	output = findAverage(num1, num2, num3, num4, num5);
	cout << "\nThe average of the 5 numbers is: " << output << "\n";
	system("pause");
    return 0;
}

float findAverage(float number1, float number2, float number3, float number4, float number5)
{
	float average = (number1 + number2 + number3 + number4 + number5) / 5;
	return average;
}
