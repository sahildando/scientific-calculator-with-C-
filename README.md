# scientific-calculator-with-C-
#include <iostream>
#include <math.h>

using namespace std;

int main() {
  double num1, num2, result;
  char op;

  cout << "Enter the first number: ";
  cin >> num1;

  cout << "Enter the second number: ";
  cin >> num2;

  cout << "Enter the operation (+, -, *, /, ^, sqrt, sin, cos, tan): ";
  cin >> op;

  switch (op) {
    case '+':
      result = num1 + num2;
      break;
    case '-':
      result = num1 - num2;
      break;
    case '*':
      result = num1 * num2;
      break;
    case '/':
      result = num1 / num2;
      break;
    case '^':
      result = pow(num1, num2);
      break;
    case 'sqrt':
      result = sqrt(num1);
      break;
    case 'sin':
      result = sin(num1);
      break;
    case 'cos':
      result = cos(num1);
      break;
    case 'tan':
      result = tan(num1);
      break;
    default:
      cout << "Invalid operation!";
      return 0;
  }

  cout << "The result is: " << result << endl;

  return 0;
}
