# Lecture-14
//Largest Number
#include <iostream>
#include <string>
#include <iomanip>
#include <array>

using namespace std;
int main()
{
	int inputs[10];
	int largest = -2147483647;
	for (int i = 0; i < 10; i++) {
		cout << "enter integer " << i + 1 << ": ";
		cin >> inputs[i];

		if (cin.fail()) {
			cout << "Invalid input\n";
			cin.clear();
			cin.ignore(3);
		}

		if (largest < inputs[i]) largest = inputs[i];
	}

	cout << "Largest Integer inputted: " << largest;

	return 0;
}
//Smallest Number
#include <iostream>
#include <string>
#include <iomanip>
#include <array>

using namespace std;
int main()
{
	int inputs[10];
	int largest = 2147483647;
	for (int i = 0; i < 10; i++) {
		cout << "enter integer " << i + 1 << ": ";
		cin >> inputs[i];

		if (cin.fail()) {
			cout << "Invalid input\n";
			cin.clear();
			cin.ignore(3);
		}

		if (largest > inputs[i]) largest = inputs[i];
	}

	cout << "Smallest Integer inputted: " << largest;

	return 0;
}
                                                 
