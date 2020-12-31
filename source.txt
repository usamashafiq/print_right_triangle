#include<iostream>
#include<conio.h>
using namespace std;
void print_right_triangle(int, char = '*');
void main() {
	int a;
	char c,q;
	cout << "Enter a size " << endl;
	cin >> a;
	
	cout << "you want to enter char   ans in (Y/N) " << endl;
	cin >> c;
	if (c == 'y'||c=='Y') {
		cout << "Enter a char '@,#,$,%' " << endl;
		cin >> q;
		print_right_triangle(a, q);
	}
	else {
		print_right_triangle(a);
	}
	
	_getch();
}
void print_right_triangle(int a, char b) {

	for (int i = a; i >= 1; i--)
	{
		for (int j = a; j>i; j--)
		{
			cout << b;
		}
		cout << "\n";
	}






}
