# averageOf5Numbers
Finds the average of any 5 numbers

// 5NumberAverage.cpp : Defines the entry point for the console application.
//

#include "stdafx.h"
#include<iostream>
#include<string>
using namespace std;

float findAverage(float, float, float, float, float);

int main()
{
	string response;
	float num1, num2, num3, num4, num5, output;
	do{
		cout << "Enter 5 numbers seperated by spaces: ";
		cin >> num1 >> num2 >> num3 >> num4 >> num5;
		output = findAverage(num1, num2, num3, num4, num5);
		cout << "\nThe average of the 5 numbers is: " << output << "\n";
		cout<<"Do you want to find the average of 5 other numbers? ";
		cin >> response;
	} while ((response == "Yes")||(response =="yes")||(response=="yea")||(response=="Yea"));
	system("pause");
    	return 0;
}

float findAverage(float number1, float number2, float number3, float number4, float number5)
{
	float average = (number1 + number2 + number3 + number4 + number5) / 5;
	return average;
}
