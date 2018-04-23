#include <iostream>
#include <cstring>
#include <cstdlib>
using namespace std;
double a, b;
char *a1, *b1;
int main(int argc, char* argv[])
{
	if (argc != 4)
	{
		cout << "Number of parameters must be 3" << endl;
		return 1;
	}
	if (strlen(argv[2]) != 1)
	{
		cout << "The second parameter must contain only 1 character" << endl;
		return 2;
	}
	a = strtod(argv[1], &a1);
	b = strtod(argv[3], &b1);
	if (strlen(a1) != 0 || strlen(b1) != 0)
	{
		cout << "An operand should be a number" << endl;
		return 3;
	}
	if (argv[2][0] == '+')
		cout << a + b << endl;
	else if (argv[2][0] == '-')
		cout << a - b << endl;
	else if (argv[2][0] == '*')
		cout << a * b << endl;
	else if (argv[2][0] == '/')
		cout << a / b << endl;
	else
	{
		cout << "The second parameter must be +,-,* or /" << endl;
		return 4;
	}
	return 0;
}
