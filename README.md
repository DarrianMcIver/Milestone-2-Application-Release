# Milestone-2-Application-Release
#include <stdio.h> 


// implementing struct in the program
struct calculator
{
	int num1;
	int num2;

};

//implementing union in the program

union Data 
{
	int i;
	float f;
	char str[20];
};

int main()
{
	struct calculator = { 5, 10 };
	char operator;
	float num1, num2, result = 0;
	union Data data;
	printf("memory size : %d\n", sizeof(data))

	//Gives the user the option to what operation they would like to use
	

	printf("\n Enter a operator (+, -, *, /) : ");
	scanf_s ("%c", &operator, 1);

	//This enter the value of number 1 and number 2 for the user to input. 
	
	
	
	printf("\n Enter two numbers for calculations: ");
	scanf_s("%f", &num1, sizeof (float));
	scanf_s("%f", &num2, sizeof (float));
	auto sum = num1 + num2;

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

}
