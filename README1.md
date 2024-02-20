#include <iostream>
using namespace std;
int main() {
	int a[] = { 0,1,2,3,4 };
	int* p[] = { a,a + 1,a + 2,a + 3,a + 4 };
	int** pp = p;
	cout << ("%d\t\n", a);
	cout << ("%d\t\n", *a);
	cout << ("%d\t\n", p);
	cout << ("%d\t\n", *p);
	cout << ("%d\t\n", **p);
	cout << ("%d\t", pp);
	cout << ("%d\t", *pp);
	cout << ("%d\t\n", **p);
	pp++;
	cout << ("%d\t", pp-p);
	cout << ("%d\t", *pp-a);
	cout << ("%d\t\n", **pp);
	*pp++;
	cout << ("%d\t", pp-p);
	cout << ("%d\t", *pp-a);
	cout << ("%d\t\n", **pp);
	*++pp;
	cout << ("%d\t", pp-p);
	cout << ("%d\t", *pp-a);
	cout << ("%d\t\n", **pp);
	++*pp;
	cout << ("%d\t", pp-p);
	cout << ("%d\t", *pp-a);
	cout << ("%d\t\n", **pp);
	pp = p;
	cout << ("%d\t", pp-p);
	cout << ("%d\t", *pp-a);
	cout << ("%d\t\n", **pp);
	**pp++;
	cout << ("%d\t", pp-p);
	cout << ("%d\t", *pp-a);
	cout << ("%d\t\n", **pp);
	*++ * pp;
	cout << ("%d\t", pp-p);
	cout << ("%d\t", *pp-a);
	cout << ("%d\t\n", **pp);
	++**pp;
	cout << ("%d\t", pp-p); 
	cout << ("%d\t", *pp-a);
	cout << ("%d\t\n", **pp);
	return 0;
}

C++