#include <stdio.h>
int main() {
    float num1;
    float num2;
    char op;
    float result;
    printf("Enter the first number: ");
    scanf("%f", &num1);
    printf("Enter the operation (+, -, *, /): ");
    scanf(" %c", &op);
    printf("Enter the second number: ");
    scanf("%f", &num2);
    switch (op) {
        case '-':
            result = num1 - num2;
            printf("Result: %f\n", result);
            break;
        case '+':
            result = num1 + num2;
            printf("Result: %f\n", result);
            break;
        case '*':
            result = num1 * num2;
            printf("Result: %f\n", result);
            break;
        case '/':
            if (num2 != 0) {
                result = num1 / num2;
                printf("Result: %f\n", result);
            } else {
                printf("Error: Division by zero.\n");
            }
            break;
        default:
            printf("Error: Invalid operator.\n");
    }

    return 0;
}
