//Random Numbers
#include <iostream>
#include <array>
#include <random>
using namespace std;


int main()
{
	array <int, 1000> randNumbers;
	int numCount = 0;

	for (int i = 0; i < randNumbers.size(); i++) {
		randNumbers[i] = rand() % 100 + 1;
	}

	for (int i = 0; i < randNumbers.size(); i++) {
		if (randNumbers[i] == 6) numCount++;
	}

	cout << "6 has appeared " << numCount << " times.";
	return 0;
}
//Largest Number
#include <iostream>
#include <array>
#include <string>
#include <math.h>
using namespace std;


int main()
{
	int Numbers[10];
	int Largest = 0;

	for (int i = 0; i < 10; i++) {
		cout << "Enter number " << i + 1 << ": ";
		cin >> Numbers[i];
		while (cin.fail()) {
			cin.clear();
			cin.ignore(1000, '\n');
			cout << "Invalid Input! Try again \nEnter number " << i + 1 << ": ";
			cin >> Numbers[i];
		}
	}

	cout << endl;

	for (int i = 0; i < 10; i++) {
		if (Numbers[i] > Largest)
		{
			Largest = Numbers[i];
		}
	}
	cout << "Largest number is: " << Largest;
	return 0;
}	
//Smallest Number
#include <iostream>
#include <array>
#include <string>
#include <math.h>
using namespace std;


int main()
{
	int Numbers[10];
	int Smallest;


	for (int i = 0; i < 10; i++) {
		cout << "Enter number " << i + 1 << ": ";
		cin >> Numbers[i];
		while (cin.fail()) {
			cin.clear();
			cin.ignore(1000, '\n');
			cout << "Invalid Input! Try again \nEnter number " << i + 1 << ": ";
			cin >> Numbers[i];
		}
	}
	Smallest = Numbers[0];
	cout << endl;
	for (int i = 0; i < 10; i++) {
		if (Numbers[i] < Smallest) {
			Smallest = Numbers[i];
		}
	}
	cout << "Smallest number is : " << Smallest;
	return 0;
}	
