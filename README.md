# Program_a_mathematical_expression
/*Запрограммировать следующее выражение: (а + b — f / а) + f * a * a — (a + b) Числа а, b, f вводятся с клавиатуры. 
Организовать пользовательский интерфейс, таким образом, чтобы было понятно, в каком порядке должны вводиться числа.*/
#include <iostream>
using namespace std;
int main()
{
	setlocale(LC_ALL, "RUSSIAN");
	int a, b, f;
	float x;
	link:
	cout << endl;
	cout << "Введите значение переменной a\n" << "Примечание! переменная a не может быть равна 0: " << endl;
	cin >> a;
	cout << "Введите значение переменной b: " << endl;
	cin >> b;
	cout << "Введите значение переменной f: " << endl;
	cin >> f;
	if (a != 0)
	{
		cout << "x = " << (a + b - f / a) + f * a * a - (a + b);
	}
	else
	{
		cout << "Ошибка!!! Переменная a = 0" << endl;
		goto link;
	}
}

