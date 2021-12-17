# Function-exponent-value
#using functions to find exp value from 1-10
#include<iostream>
#include<math.h>
#include<string>
using namespace std;
void number(int exponent)  //function definition
{
	cout << "\n\t\t\t\t\tExponent value from 1 till 10: " << endl;
	for (int i = 1; i <= 10; i++)
	{
		cout<< "\t\t\t\t\t" << i << "^" << exponent << " is: " << pow(exponent, i) << endl;
	}
	 cout<< "\n\t\t\t\t\tYOU HAVE REACHED THE END OF THE CODE\n\n";
}
int main()  //main function
{
	int value;   //declaring variable 'value' with datatype integer
	cout << "\n\t\t\t\t\tEnter a number: ";
	cin >> value;
	while (cin.fail() != 0)   //error handling
	{
		cout << "\t\t\t\t\t\aInvalid Data.\n\t\t\t\t\tEnter a number: ";
		cin.clear();
		cin.ignore();
		cin >> value;
	}
	number(value); //function call
	return 0;
}
