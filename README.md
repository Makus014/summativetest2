# summativetest2

#include <iostream>
#include <string>
#include <math.h>
using namespace std;

void name();
void factorial();
void table();
void exponent();


int main() {

	name();
	cout << endl;

	factorial();
	cout << endl;

	table();
	cout << endl;

	exponent();
	cout << endl;

	return 0;
}

void name() {
	string name;
	cout << "Type your full name" << endl;
	getline(cin, name);
	cout << "Hello " << name << endl;
}

void factorial() {
	double factorial = 1.0;
	int number=0;
	int i = 0;
	cout << "Enter a number!" << endl;
	cin >> number;
	for (i = 1; i <= number; i++) {
		factorial *= i;
	}
	cout << "The factorial of " << number << " is " << factorial;
}

void table() {

	int number;
	int i;
	cout << "Type number (1-10)" << endl;
	cin >> number;
	///////////////////////////
	//Error reader!
	while (number > 10) {
		cout << "Error! Type again!" << endl;
		cin >> number;
	}
	while (number < 0) {
		cout << "Error! Type again!" << endl;
		cin >> number;
	}
	///////////////////////////
	for (i = 1; i <= 10; i++) {
		cout << number << " * " << i << " = " << number * i << endl;
	}
}

void exponent() {

	float Number = 0;
	int i;


	cout << "Type a number " << endl;
	cin >> Number;
	for (i = 5; i <= 10; i++) {
		cout << "The exponent of this number " << Number << "^" << i << endl;
	  }
}
