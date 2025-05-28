## NAME : SUBITHRA R
## REGISTER NO : 212224110050
# EX-01-Datatypes-Operators
## AIM:
Write a C program to read 3 characters one by one and print the characters in a reverse order.

## ALGORITHM:
1.	Declare three character variables to store the input characters.
2.	Use the scanf function to read the characters one by one from the user.
3.	Print the characters in reverse order using the printf function.
4.	End the program.

## PROGRAM:
```
#include <stdio.h>
int main()
{
    char ch1, ch2, ch3;
    scanf(" %c", &ch1);
    scanf(" %c", &ch2);
    scanf(" %c", &ch3);
    printf("Characters in reverse order: %c %c %c\n", ch3, ch2, ch1);
    return 0;
}
```
## OUTPUT:

![image](https://github.com/user-attachments/assets/e0d950d9-a337-4ed6-9e13-37334a990500)

## RESULT:
Thus the program to read 3 characters one by one and print the characters in a reverse order has been executed successfully.


# EX-02- Conditional-Statements
## AIM:
Write a C program to read A values and check whether A is positive number or not.

# ALGORITHM:
1.	Declare a variable to store the input value A.
2.	Use the scanf function to read the value of A from the user.
3.	Check if the value of A is greater than zero.
4.	If A is greater than zero, print a message indicating that it's a positive number. 
5.	Otherwise, print a message indicating that it's not a positive number.
6.End the program.

# PROGRAM:
```
#include<stdio.h>
int main()
{
    float a;
    scanf("%f",&a);
    if(a>=0)
    {
        printf("Number is positive.");
    }
       
    else
    {
      printf("Number is negative.");
    }
       
}
```

# OUTPUT:


![image](https://github.com/user-attachments/assets/87b4faa4-e3ce-45a8-a0aa-469d00e2ac8e)


# RESULT:
Thus the program to read A values and check whether A is positive number or not has been executed successfully.
 
 
 


# EX-03- Operators-Expressions
## AIM:
Write a program to find minimum between two fraction numbers using conditional operator or ternary operator.

## ALGORITHM:
1.	Declare variables to store the two fraction numbers and the result.
2.	Use the printf function to prompt the user to enter the first fraction number (numerator and denominator separately).
3.	Use the scanf function to read the numerator and denominator of the first fraction.
4.	Repeat steps 2 and 3 to get the second fraction from the user.
5.	Calculate the decimal values of both fractions by dividing the numerators by the denominators.
6.	Use the conditional (ternary) operator to compare the decimal values and store the minimum value in the result variable.
7.	Print the minimum value.

## PROGRAM:
```
#include <stdio.h>
int main() {
    int n1, d1, n2, d2;
    float f1, f2, minValue;

    printf("Enter numerator of first fraction: ");
    scanf("%d", &n1);
    printf("Enter denominator of first fraction: ");
    scanf("%d", &d1);

    printf("Enter numerator of second fraction: ");
    scanf("%d", &n2);
    printf("Enter denominator of second fraction: ");
    scanf("%d", &d2);

    f1 = (float)n1 / d1;
    f2 = (float)n2 / d2;

    minValue = (f1 < f2) ? f1 : f2;

    printf("Minimum of the two fractions: %.4f\n", minValue);

    return 0;
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/56a85ef3-5bfa-4da0-8836-ff4053d1243e)



## RESULT:
Thus the program to find minimum between two fraction numbers using conditional operator or ternary operator has been executed successfully.




# EX-04- Using Conditional Statements

## AIM:
Write a C program to check whether the input value is equal to 1 using simple if statement

## ALGORITHM:
1.	Declare a variable to store the input value.
2.	Use the scanf function to read the input value from the user.
3.	Use an if statement to check if the input value is equal to 1.
4.	If the condition in the if statement is true, print a message indicating that the input value is equal to 1.
5.	Otherwise, print a message indicating that it's not equal to 1.
6.	End the program.

## PROGRAM:
```
#include <stdio.h>
int main()
{

    int num;
    printf("Enter a number:");
    scanf("%d", &num);
    if (num == 1) 
    {
    
        printf("The number is equal to 1.\n");
	
    } else {
    
        printf("The number is not equal to 1.\n");
	
    }
    
    return 0;
} 
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/73c62ddc-a5dc-46dd-b2f4-85a045ab4668)


## RESULT:
Thus the program to check whether the input value is equal to 1 using simple if statement has been executed successfully



# EX-05- Calculating Total, Percentage, And Division Using Conditional Statements 
## AIM:
To write a C program that reads marks of three subjects, calculates the total and percentage, and then determines the division (First, Second, Pass, or Fail) based on the percentage and minimum marks criteria.
## ALGORITHM:
1.	Start
2.	Declare integer variables m1, m2, m3 for marks, and float variables tot, per.
3.	Input the marks for three subjects.
4.	Calculate total marks: tot = m1 + m2 + m3
5.	Calculate percentage: per = tot / 3
6.	Display total and percentage.
7.	Check if all marks are greater than or equal to 40:
8.	If yes:
a.	If percentage >= 60: Print “Division = First”
b.	Else if percentage >= 48: Print “Division = Second”
c.	Else if percentage >= 36: Print “Division = Pass”
9.	Else: Print “Division = Fail”
10.	End

## PROGRAM:
```
#include <stdio.h>
#include <string.h>

int main()
{
    int phy,che,ca,total;
    float per;
    char div[10];

   
    scanf("%d%d%d",&phy,&che,&ca);
    total = phy+che+ca;
    per = total/3.0;
    if (per>=60)
	 strcpy(div,"First");
    else if (per<60&&per>=48)
	    strcpy(div,"Second");
	else
	    if (per<48&&per>=36)
		strcpy(div,"Pass");
	     else
		strcpy(div,"Fail");

      
       printf("Total Marks = %d\nPercentage = %5.2f\nDivision = %s\n",total,per,div);
       return 0;
}


```
## OUTPUT:
![image](https://github.com/user-attachments/assets/8d57687e-d3df-4599-be00-cab5c76bb716)


## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.

