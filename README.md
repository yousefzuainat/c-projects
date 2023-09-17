
#include <iostream>
using namespace std;
int main()
{
    while (true)
    {

        cout << "\n**********~simple calculator~**********\n";
        char op;
        double num1, num2;
        cout << "Enter first number : \n";
        cin >> num1;
        cout << "Enter second number : \n";
        cin >> num2;
        cout << "Enter operator(+,-,*,/)\n: ";
        cin >> op;
        switch (op)
        {
        case '+':
            cout << num1 << " + " << num2 << " = " << num1 + num2 << endl;
            break;
        case '-':
            cout << num1 << " - " << num2 << " = " << num1 - num2 << endl;
            break;
        case '*':
            cout << num1 << " * " << num2 << " = " << num1 * num2 << endl;
            break;
        case '/':
            if (num2 == 0)
            {
                cout << "Error" << endl;
            }
            else
            {
                cout << num1 << " / " << num2 << " = " << num1 / num2 << endl;
                break;
            }
        default:
            cout << "Error ! ";
        }
        cout << "\n**********~Thank you for use~**********\n";
    }
}
