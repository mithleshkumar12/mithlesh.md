PROGRAMMING FOR PROGRAM SOLVING ESC-18105
NAME-Mithlesh Kumar
ROLL NO-2017103
BRANCH-ELECTRONICS AND COMMUNICATION

1.Programs to disply a welcome message using puts
#include<stdio.h>
int main()
{
puts("\nHELLO TO BUDDING ENGINEERS\n");
return 0;
}
Output of program

HELLO TO BUDDING ENGINEERS
2. programs to disply addres using puts
#include<stdio.h>
int main()
{
puts("Mithlesh Kumar \n ECE A2\n 2017103\n\VPO Dharampur,Nalanda,803110"};
return 0;
output of programs

Mithlesh Kumar
ECE A2
2017103
VPO Dharampur,Nalanda,803110
3.programs to find the sum of two number .
#include <stdio.h>
int main()
{
    int firstNumber, secondNumber, sumOfTwoNumbers;
    
    printf("enter the two integer ");
    scanf("%d %d", &firstNumber, &secondNumber);
    sumOfTwoNumbers = firstNumber + secondNumber;      
    printf("%d + %d = %d", firstNumber, secondNumber, sumOfTwoNumbers);
    return 0;
}
Output of programs

Enter two integers: 12
11
12 + 11 = 23
4.prorams to convert Centigrate to farhnhiet .
#include<stdio.h>
int main()
{
	
	float cen, fah;
	printf("Enter temperature in Celsius : ");
	scanf("%f",&cen);
	fah=(1.8 * cen) + 32;
	printf("\nTemperature in Fahrenheit = %f",fah);
	return 0;
}
output of programs

Enter the temerature in Celsious : 37
Temperatur in fahrenheit : 98.599998
5.programs to find the area and perimeter of circle .
#include<stdio.h>
int  main()
{

	float r, area, circum;
	printf("Enter the radius of the circle :");
	scanf("%f",&r);
	area=3.14*r*r;
	circum=2*3.14*r;
	printf("Area of the circle = %f\nCircumference of the circle = %f\n",area,circum);
	return 0;
}
output of programs :

Enetr the radius of the circle :5
Area of the circle =78.500000
Circumference of the circle = 31.400000
6. programs to swap the two number without using third variable .
#include<stdio.h>  
 int main()    
{    
int a=10, b=20;      
printf("Before swap a=%d b=%d",a,b);      
a=a+b;//a=30 (10+20)    
b=a-b;//b=10 (30-20)    
a=a-b;//a=20 (30-10)    
printf("\nAfter swap a=%d b=%d",a,b);    
return 0;  
}   
Output:

Before swap a=10 b=20
After swap a=20 b=10
7. programs to check whether even or odd number .
#include<stdio.h>
int main()
{
    int num;
    printf("Enter any number: ");
    scanf("%d", &num);
    if(num%2 == 0)
        printf("\nIt's an even number.");
    else
        printf("\nIt's an odd number.");
	
    return 0;
}
Output of programs

Enter any number:4
It's an even number.
8.program to find the factorial of the number .
#include<stdio.h>
int main()
{
    int num, i, fact=1;
    printf("Enter any number: ");
    scanf("%d", &num);
    for(i=num; i>0; i--)
        fact = fact*i;
    printf("\nFactorial of %d = %d", num, fact);
    
    return 0;
}
Output the programs

Enter any number:5
factorial of 5 = 120
9. programs to fizz buzz
#include <stdio.h>

int main(void)
{
    int i;
    for(i=1; i<=100; i++)
    {
        if(((i%3)||(i%5))== 0)
            printf("number= %d FizzBuzz\n", i);
        else if((i%3)==0)
            printf("number= %d Fizz\n", i);
        else if((i%5)==0)
            printf("number= %d Buzz\n", i);
        else
            printf("number= %d\n",i);

    }

    return 0;
}
Output the programs

1
2
fizz
4
buzz
..........
10.programs to print week of days using switch case
#include <stdio.h>

int main()
{
    int week;
   
    printf("Enter week number(1-7): ");
    scanf("%d", &week);
    
    switch(week)
    {
        case 1: 
            printf("Monday");
            break;
        case 2: 
            printf("Tuesday");
            break;
        case 3: 
            printf("Wednesday");
            break;
        case 4: 
            printf("Thursday");
            break;
        case 5: 
            printf("Friday");
            break;
        case 6: 
            printf("Saturday");
            break;
        case 7: 
            printf("Sunday");
            break;
        default: 
            printf("Invalid input! Please enter week number between 1-7.");
    }

    return 0;
}
Output of programsg

Input week number(1-7): 2
Tuesday
11. programe to make a calculator using switch case
#include<stdio.h>
int main() {
    char operator;
    double firstNumber,secondNumber;
    printf("Enter an operator (+, -, *,): ");
    scanf("%c", &operator);
    printf("Enter two operands: ");
    scanf("%lf %lf",&firstNumber, &secondNumber);
    switch(operator)
    {
        case '+':
            printf("%.1lf + %.1lf = %.1lf",firstNumber, secondNumber, firstNumber + secondNumber);
            break;
        case '-':
            printf("%.1lf - %.1lf = %.1lf",firstNumber, secondNumber, firstNumber - secondNumber);
            break;
        case '*':
            printf("%.1lf * %.1lf = %.1lf",firstNumber, secondNumber, firstNumber * secondNumber);
            break;
        case '/':
            printf("%.1lf / %.1lf = %.1lf",firstNumber, secondNumber, firstNumber / secondNumber);
            break;
        
        default:
            printf("Error! operator is not correct");
    }
    
    return 0;
}
Output

Enter an operator (+, -, *,): *
Enter two operands: 1.5
4.5
1.5 * 4.5 = 6.8
12. programs to cheak leap of year
#include <stdio.h>
int main()
{
    int year;
    printf("Enter a year: ");
    scanf("%d",&year);
    if(year%4 == 0)
    {
        if( year%100 == 0)
        {
            
            if ( year%400 == 0)
                printf("%d is a leap year.", year);
            else
                printf("%d is not a leap year.", year);
        }
        else
            printf("%d is a leap year.", year );
    }
    else
        printf("%d is not a leap year.", year);
    
    return 0;
}
Output 1

Enter a year: 1900
1900 is not a leap year.
13. programs to cheak prime number or not
#include <stdio.h>
int main()
{
    int n, i, flag = 0;
    printf("Enter a positive integer: ");
    scanf("%d", &n);
    for(i = 2; i <= n/2; ++i)
    {
       
        if(n%i == 0)
        {
            flag = 1;
            break;
        }
    }
    if (n == 1) 
    {
      printf("1 is neither a prime nor a composite number.");
    }
    else 
    {
        if (flag == 0)
          printf("%d is a prime number.", n);
        else
          printf("%d is not a prime number.", n);
    }
    
    return 0;
}
Output

Enter a positive integer: 29
29 is a prime number.
14. programs to find number pallindrome or not
#include <stdio.h>
int main()
{
    int n, reversedInteger = 0, remainder, originalInteger;
    printf("Enter an integer: ");
    scanf("%d", &n);
    originalInteger = n;
    
    while( n!=0 )
    {
        remainder = n%10;
        reversedInteger = reversedInteger*10 + remainder;
        n /= 10;
    }
    
    if (originalInteger == reversedInteger)
        printf("%d is a palindrome.", originalInteger);
    else
        printf("%d is not a palindrome.", originalInteger);
    
    return 0;
}
output

Enter an integer: 1001
1001 is a palindrome.
15.programs to fybonic series
#include <stdio.h>
int main()
{
    int i, n, t1 = 0, t2 = 1, nextTerm;
    printf("Enter the number of terms: ");
    scanf("%d", &n);
    printf("Fibonacci Series: ");
    for (i = 1; i <= n; ++i)
    {
        printf("%d, ", t1);
        nextTerm = t1 + t2;
        t1 = t2;
        t2 = nextTerm;
    }
    return 0;
}
Output

Enter the number of terms: 10
Fibonacci Series: 0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 
16 programs to print simple matrix in array
int main() {
  int values[5];
  printf("Enter 5 integers: ");
  
  for(int i = 0; i < 5; ++i) {
     scanf("%d", &values[i]);
  }
  printf("Displaying integer");
  for(int i = 0; i < 5; ++i) {
     printf("%d\n", values[i]);
  }
  return 0;
}
Output

Enter 5 integers: 1
-3
34
0
3
Displaying integers: 1
-3
34
0
3
programs to print 2D array
#include <stdio.h>    
void main ()    
{    
    int arr[3][3],i,j;     
    for (i=0;i<3;i++)    
    {    
        for (j=0;j<3;j++)    
        {    
            printf("Enter a[%d][%d]: ",i,j);                
            scanf("%d",&arr[i][j]);    
        }    
    }    
    printf("\n printing the elements ....\n");     
    for(i=0;i<3;i++)    
    {    
        printf("\n");    
        for (j=0;j<3;j++)    
        {    
            printf("%d\t",arr[i][j]);    
        }    
    }    
} 
Output

Enter a[0][0]: 56   
Enter a[0][1]: 10   
Enter a[0][2]: 30  
Enter a[1][0]: 34  
Enter a[1][1]: 21 
Enter a[1][2]: 34    

Enter a[2][0]: 45
Enter a[2][1]: 56
Enter a[2][2]: 78   

 printing the elements .... 
 
56      10      30  
34      21      34  
45      56      78
programs to addtion of matrics
#include <stdio.h>
int main(){
    int r, c, a[100][100], b[100][100], sum[100][100], i, j;
    printf("Enter number of rows (between 1 and 100): ");
    scanf("%d", &r);
    printf("Enter number of columns (between 1 and 100): ");
    scanf("%d", &c);
    printf("\nEnter elements of 1st matrix:\n");
    for(i=0; i<r; ++i)
        for(j=0; j<c; ++j)
        {
            printf("Enter element a%d%d: ",i+1,j+1);
            scanf("%d",&a[i][j]);
        }
    printf("Enter elements of 2nd matrix:\n");
    for(i=0; i<r; ++i)
        for(j=0; j<c; ++j)
        {
            printf("Enter element a%d%d: ",i+1, j+1);
            scanf("%d", &b[i][j]);
        }
    
    for(i=0;i<r;++i)
        for(j=0;j<c;++j)
        {
            sum[i][j]=a[i][j]+b[i][j];
        }
    
    printf("\nSum of two matrices: \n");
    for(i=0;i<r;++i)
        for(j=0;j<c;++j)
        {
            printf("%d   ",sum[i][j]);
            if(j==c-1)
            {
                printf("\n\n");
            }
        }
    
    return 0;
}
Output

Enter number of rows (between 1 and 100): 2
Enter number of columns (between 1 and 100): 3

Enter elements of 1st matrix:
Enter element a11: 2
Enter element a12: 3
Enter element a13: 4
Enter element a21: 5
Enter element a22: 2
Enter element a23: 3
Enter elements of 2nd matrix:
Enter element a11: -4
Enter element a12: 5
Enter element a13: 3
Enter element a21: 5
Enter element a22: 6
Enter element a23: 3

Sum of two matrices: 
-2   8   7   

10   8   6  
programs to substract the two matrix

int main()
{
    printf("\n\n\t\tStudytonight - Best place to learn\n\n\n");

    int n, m, c, d, first[10][10], second[10][10], sum[10][10], diff[10][10];
    printf("\nEnter the number of rows and columns of the first matrix \n\n");
    scanf("%d%d", &m, &n);

    printf("\nEnter the %d elements of the first matrix \n\n", m*n);
    for(c = 0; c < m; c++)   // to iterate the rows
        for(d = 0; d < n; d++)   // to iterate the columns
            scanf("%d", &first[c][d]);

    printf("\nEnter the %d elements of the second matrix \n\n", m*n);
    for(c = 0; c < m; c++)   // to iterate the rows
        for(d = 0; d < n; d++)   // to iterate the columns
            scanf("%d", &second[c][d]);

 
    printf("\n\nThe first matrix is: \n\n");
    for(c = 0; c < m; c++)   // to iterate the rows
    {
        for(d = 0; d < n; d++)   // to iterate the columns
        {
            printf("%d\t", first[c][d]);
        }
    printf("\n");
	    
    printf("\n\nThe second matrix is: \n\n");
    for(c = 0; c < m; c++)   // to iterate the rows
    {
        for(d = 0; d < n; d++)   // to iterate the columns
        {
            printf("%d\t", second[c][d]);
        }
    printf("\n");
    }

  
    for(c = 0; c < m; c++)
        for(d = 0; d < n; d++)
            sum[c][d] = first[c][d] + second[c][d];

    printf("\n\nThe sum of the two entered matrices is: \n\n");
    for(c = 0; c < m; c++)
    {
        for(d = 0; d < n; d++)
        {
            printf("%d\t", sum[c][d]);
        }
        printf("\n");
    }

    
    for(c = 0; c < m; c++)
        for(d = 0; d < n; d++)
            diff[c][d] = first[c][d] - second[c][d];

    
    printf("\n\nThe difference(subtraction) of the two entered matrices is: \n\n");
    for(c = 0; c < m; c++)
    {
        for(d = 0; d < n; d++)
        {
            printf("%d\t", diff[c][d]);
        }
        printf("\n");
    }

    printf("\n\n\t\t\tCoding is Fun !\n\n\n");
    return 0;
}
output

1 2 3
4 5 6
7 8 9

Input elements in 3x3 matrix2:
9 8 7
6 5 4
3 2 1
Output

Difference of both matrices =
-8 -6 -4
-2  0  2
4  6  8
programs to transpose the matrix
#include <stdio.h>
 
void main()
{
    static int array[10][10];
    int i, j, m, n;
 
    printf("Enter the order of the matrix \n");
    scanf("%d %d", &m, &n);
    printf("Enter the coefiicients of the matrix\n");
    for (i = 0; i < m; ++i)
    {
        for (j = 0; j < n; ++j)
        {
            scanf("%d", &array[i][j]);
        }
    }
    printf("The given matrix is \n");
    for (i = 0; i < m; ++i)
    {
        for (j = 0; j < n; ++j)
        {
            printf(" %d", array[i][j]);
        }
        printf("\n");
    }
    printf("Transpose of matrix is \n");
    for (j = 0; j < n; ++j)
    {
        for (i = 0; i < m; ++i)
        {
            printf(" %d", array[i][j]);
        }
        printf("\n");
    }
}
output :

Enter the order of the matrix
3 3
Enter the coefiicients of the matrix
3 7 9
2 7 5
6 3 4
The given matrix is
 3 7 9
 2 7 5
 6 3 4
Transpose of matrix is
 3 2 6
 7 7 3
 9 5 4
programs to find multiplication of matrix
#include <stdio.h>

int main()
{
 int m, n, p, q, c, d, k, sum = 0;
 int first[10][10], second[10][10], multiply[10][10];

 printf("Enter the number of rows and columns of first matrix\n");
 scanf("%d%d", &m, &n);
 printf("Enter the elements of first matrix\n");

 for (  c = 0 ; c < m ; c++ )
   for ( d = 0 ; d < n ; d++ )
     scanf("%d", &first[c][d]);

 printf("Enter the number of rows and columns of second matrix\n");
 scanf("%d%d", &p, &q);

 if ( n != p )
   printf("Matrices with entered orders can't be multiplied with each other.\n");
 else
 {
   printf("Enter the elements of second matrix\n");

   for ( c = 0 ; c < p ; c++ )
     for ( d = 0 ; d < q ; d++ )
       scanf("%d", &second[c][d]);

   for ( c = 0 ; c < m ; c++ )
   {
     for ( d = 0 ; d < q ; d++ )
     {
       for ( k = 0 ; k < p ; k++ )
       {
         sum = sum + first[c][k]*second[k][d];
       }

       multiply[c][d] = sum;
       sum = 0;
     }
   }

   printf("Product of entered matrices:-\n");

   for ( c = 0 ; c < m ; c++ )
   {
     for ( d = 0 ; d < q ; d++ )
       printf("%d\t", multiply[c][d]);

     printf("\n");
   }
 }

 return 0;
}
output

Enter the number of rows and columns of first matrix 3 3
Enter the elements of first matrix
1 2 0
0 1 1 
2 0 1 
Enter the number of rows and columns of second matrix 3 3
Enter the elements of second matrix
1 1 2
2 1 1 
1 2 1
Product of entered matrices:-
5	3	4	
3	3	2	
3	4	5
17 programs to find squre of number using function
#include<stdio.h>

int square(int); 

int main()
{
     int number, answer;
    
     printf("Enter your number:");
     scanf("%d", &number);
    
     answer = square(number);  
    
     printf("Square of %d is %d.", number, answer);
}

int square(int n)
{
     
     return(n*n); 
}
Output of the Program:

Enter your number:5
Square of 5 is 25.
18 programs to swape a number by call by value
#include <stdio.h>
 
 
void swap(int, int);
 
int main()
{
   int x, y;
 
   printf("Enter the value of x and y\n");
   scanf("%d%d",&x,&y);
 
   printf("Before Swapping\nx = %d\ny = %d\n", x, y);
 
   swap(x, y); 
 
   printf("After Swapping\nx = %d\ny = %d\n", x, y);
 
   return 0;
}
 
void swap(int a, int b)
{
   int temp;
 
   temp = b;
   b = a;
   a = temp;
    printf("Values of a and b is %d  %d\n",a,b);
}
Output:

Enter the value of x and y
Before Swapping
x = 10
y = 5
Values of a and b is 5 10
After Swapping
x = 10
y = 5
19 programs to swape two number by call by refernce
#include <stdio.h>
 
int main()
{
  int x, y, t;
 
  printf("Enter two integers\n");
  scanf("%d%d", &x, &y);
 
  printf("Before Swapping\nFirst integer = %d\nSecond integer = %d\n", x, y);
 
  t = x;
  x = y;
  y = t;
 
  printf("After Swapping\nFirst integer = %d\nSecond integer = %d\n", x, y);
 
  return 0;
}
The output of the program:

Enter two integers
23
45
Before Swapping
First integer = 23
Second integer = 45
After Swapping
First integer = 45
Second integer = 23
20 programs to find factorial of number using recursion
#include<stdio.h>
int find_factorial(int);
int main()
{
   int num, fact;
   
   printf("\nEnter any integer number:");
   scanf("%d",&num);
 
   
   fact =find_factorial(num);
 
   
   printf("\nfactorial of %d is: %d",num, fact);
   return 0;
}
int find_factorial(int n)
{
   
   if(n==0)
      return(1);
 
   
   return(n*find_factorial(n-1));
}
Output:

Enter any integer number: 4
programe to intialization or disply structure
#include <stdio.h>

struct employee{
	char name[30];
	int empId;
	float salary;
};

int main()
{
	struct employee emp={"Mike",1120,76909.00f};
	
	printf("\n Name: %s"	,emp.name);
	printf("\n Id: %d"		,emp.empId);
	printf("\n Salary: %f\n",emp.salary);
	return 0;
}
Output

 Name: Mike 
 Id: 1120 
 Salary: 76909.000000

factorial of 4 is: 24
