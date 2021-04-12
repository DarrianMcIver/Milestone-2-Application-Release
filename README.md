# Milestone-2-Application-Release
#include <stdio.h>

int main()
{
	char operator;
	float num1, num2, result = 0;

	//Gives the user the option to what operation they would like to use
	

	printf("n\ Enter a operator (+, -, *, /) : ");
	scanf_s("%c", &operator);

	//This enter the value of number 1 and number 2 for the user to input. 
	

	printf("\n Enter two numbers for calculations: ");
	scanf_s("%f%f", &num1, &num2);

	//This line of code will execute the operator (+,-,*,/)
	 
	switch (operator)
	{
	//if user enters +
	case'+':
			result = num1 + num2;
			break;
	// if user enters -
	case'-':
			result = num1 - num2;
			break;
	//if user enters *
	case'*':
			result = num1 * num2;
			break;
	// if user enters /
	case'/':
			result = num1 / num2;
			break;
	// if the user does not enter +,-,*,/ then the following error will occur below
		default:
			printf("\n Invalid Operator");
	}
	printf("The Result of %.2f %c %.2f = %.2f", num1, operator, num2, result);
	return 0;



#include<stdio.h>

int main()
{
    int num1, num2, sum;
    int* ptr1, * ptr2;

    printf("Enter any two Number: ");
    scanf("%d%d", &num1, &num2);

    printf("\nAddress of %d is %p", num1, &num1);
    printf("\nAddress of %d is %p", num2, &num2);

    ptr1 = &num1;
    ptr2 = &num2;

    printf("\n\nptr1 = %p", ptr1);
    printf("\nptr2 = %p", ptr2);

    printf("\n\nValue at %p is %d", ptr1, *ptr1);
    printf("\nValue at %p is %d", ptr2, *ptr2);

    sum = *ptr1 + *ptr2;
    printf("\n\nSum of %d and %d is %d", *ptr1, *ptr2, sum);
    getch();
    return 0;
}
