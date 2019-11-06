----
# **PROGRAMMING FOR PROBLEM SOLVING ESC-18105**
----
![](https://nptel.ac.in/content/college_assets/college_logo/1078_logo.jpg)
----
## **NAME** - *INDRAJEET SINHA*
## **ROLL NO.** - *1915097*
## **BRANCH** - *COMPUTER SCIENCE*
----
# PROGRAMS
----
## 1. Add two numbers
```C
#include <stdio.h>
int main()
{
	int a,b,c;
	printf("enter the numbers");
	scanf("%d %d",&a,&b);
	c=a+b;
	printf("sum of numbers is %d",c);
	return 0;
}
```
---
## 2. Average of number
```C
#include <stdio.h>
int main()
{
    int n, i;
    float num[100], sum = 0.0, average;
    printf("Enter the numbers of elements: ");
    scanf("%d", &n);
    while (n > 100 || n <= 0)
    {
        printf("Error! number should in range of (1 to 100).\n");
        printf("Enter the number again: ");
        scanf("%d", &n);
    }
    for(i = 0; i < n; ++i)
    {
        printf("%d. Enter number: ", i+1);
        scanf("%f", &num[i]);
        sum += num[i];
    }
    average = sum / n;
    printf("Average = %.2f", average);
    return 0;
}
```
---
## 3. Weekdays
``` C
#include <stdio.h>
void main()
{
	char ch;
	printf("enter s for sunday\n m for monday\n t for tuesday\n w for wednesday\n h for thursday\n f for friday\n a for saturday\n");
	scanf(" %s",&ch);
	switch (ch)
	{
		case 's':
		printf("sunday");
		break;
		case 'm':
		printf("monday");
		break;
		case 't':
		printf("tuesday");
		break;
		case 'w':
		printf("wednesday");
		break;
		case 'h':
		printf("thrusday");
		break;
		case 'f':
		printf("friday");
		break;
		case 'a':
		printf("saturday");
		break;
		default :
		printf("wrong input");
		break;
	}
}
```
---
## 4. Odd Even
``` C
#include <stdio.h>
void main()
{
int i;
printf("enter number ");
scanf("%d",&i);
if (i%2==0)
printf("number is even");
else
printf("number is odd");
}

```
---
## 5. Table of a number
```C
#include<stdio.h>
int main(){
	int i,n,c;
        scanf("%d",&n);
	for(i=1;i<=10;i++){
		if(i<5){
   
               c=n*i;
		printf(" %d * %d = %d    %d * %d = %d\n",n,i,c,n,10+i,n*(10+i));
		}
		else if(i>=5) 
		{c=n*i;
                  printf(" %d * %d = %d    %d * %d = %d\n",n,i,c,n,10+i,n*(10+i));
		}
	/*	else 

                    printf(" %d * %d = %d    %d * %d = %d\n",n,i,c,n,10+i,n*())
*/


  }
  
	return 0;
}
```
---
## 6. Armstrong Number
``` C
#include<stdio.h>
int main(){
	int n,temp,rem,s=0;
	scanf("%d",&n);
	temp=n;
	while(temp!=0){
		rem=temp%10;
		s=s+rem*rem*rem;
		temp/=10;
	}
	if(s==n){
		printf("Armstrong number\n");
	}
	else
		printf("Not an Armstrong number\n");
	return 0;
}
```
---
## 7. Calculator
``` C
#include <stdio.h>
int main()
{
	int a,b,c;
	char cal;
	printf("enter a and b and operator");
	scanf("%d %d %c",&a,&b,&cal);
	switch (cal)
	{
		case '+':
		c=a+b;
		printf("%d",c);
		break;
		case '-':
		c=a-b;
		printf("%d",c);
		break;
		case '*':
		c=a*b;
		printf("%d",c);
		break;
		case '/':
		c=a/b;
		printf("%d",c);
	}
	printf("\n");
}
```
---
## 8. Bubble sort
``` C
#include<stdio.h>
int main(){
	int a[30];
	int n,i,j,k,temp;
	scanf("%d",&n);
	for(i=0;i<n;i++){
		scanf("%d",&a[i]);
	}
	for(j=0;j<n-1;j++){
		for(k=0;k<n-j-1;k++)
		{
			if(a[k]>a[k+1]){
				temp=a[k];
				a[k]=a[k+1];
				a[k+1]=temp;
			}
		}
	}
	for(i=0;i<n;i++){
		printf("%d",a[i]);
		printf("\n");
	}
return 0;
}
```
---
## 9. Binary search
``` C
#include <stdio.h>
 
int main()
{
   int c, first, last, middle, n, search, array[100];
 
   printf("Enter number of elements\n");
   scanf("%d",&n);
 
   printf("Enter %d integers\n", n);
 
   for (c = 0; c < n; c++)
      scanf("%d",&array[c]);
 
   printf("Enter value to find\n");
   scanf("%d", &search);
 
   first = 0;
   last = n - 1;
   middle = (first+last)/2;
 
   while (first <= last) {
      if (array[middle] < search)
         first = middle + 1;    
      else if (array[middle] == search) {
         printf("%d found at location %d.\n", search, middle+1);
         break;
      }
      else
         last = middle - 1;
 
      middle = (first + last)/2;
   }
   if (first > last)
      printf("Not found! %d isn't present in the list.\n", search);
 
   return 0;  
}
```
---
## 10. Factorial of a number
``` C
#include <stdio.h>
void main()
{
	int a,n=1,i;
	printf("enter i");
	scanf("%d",&i);
	for(a=1;a<=i;a++)
	n=n*a;
	printf("factorial of a is %d \n",n);
}

```
---
## 11. Fizz Buzz
``` C
#include <stdio.h>
int main()
{
	int a,i;
	printf("enter number ");
	scanf("%d",&a);
	for(i=1;i<=a;i++)
	{
		if(i%15==0)
		printf("fizzbuzz\n");
		else if(i%5==0)
		printf("buzz\n");
		else if(i%3==0)
		printf("fizz\n");
		else
		printf("%d\n",i);
	}
	return 0;
}
```
---
## 12. Sum of first 100 numbers
``` C
#include <stdio.h>
 
int main()
{
  int n, sum = 0, c, value;
 
  printf("How many numbers you want to add?\n");
  scanf("%d", &n);
 
  printf("Enter %d integers\n", n);
 
  for (c = 1; c <= n; c++)
  {
    scanf("%d", &value);
    sum = sum + value;
  }
 
  printf("Sum of the integers = %d\n", sum);
 
  return 0;
}
```
---
## 13. Greater of two number
``` C
#include<stdio.h>
int main(){
	int a,b;
	scanf("%d %d",&a,&b);
	if(a>b)
		printf("a is Greater\n");
	else
		printf("b is greater\n");
	return 0;
}
```
---
## 14. Greater of three number
``` C
#include <stdio.h>
int main()
{
    double n1, n2, n3;
    printf("Enter three different numbers: ");
    scanf("%lf %lf %lf", &n1, &n2, &n3);
    if( n1>=n2 && n1>=n3 )
        printf("%.2f is the largest number.", n1);
    if( n2>=n1 && n2>=n3 )
        printf("%.2f is the largest number.", n2);
    if( n3>=n1 && n3>=n2 )
        printf("%.2f is the largest number.", n3);
    return 0;
}
```
---
## 15. GCD
``` C
#include<stdio.h>
int main(){
	int a,b,i,skv;
	scanf("%d %d",&a,&b);
		for(i=1;i<=a && i<=b;i++){
			if(a%i==0 && b%i==0){
                            skv=i;
			}
		}
		printf("%d\n",skv);
		return 0;
}
```
## 16. Leap Year
``` c
#include <stdio.h>
int main()
{
	int year;
	printf("enter year ");
	scanf("%d",&year);
	if (year%4==0)
	printf("%d is a leap year\n",year);
	else
	printf("%d is not a leap year\n",year);
	return 0;
}
```
---
## 17. Linear Search
``` C
#include<stdio.h>
int main(){
	int n,i,search,arr[100];
	printf("Enter thesize of array\n");
	scanf("%d",&n);
	for(i=0;i<n;i++){
		scanf("%d",&arr[i]);
	}
	scanf("%d",&search);
	for(i=0;i<n;i++){
		if(arr[i]==search){
			printf("%d is the required element present at %d\n",search,i+1);
			break;
		}
		else
		{	printf("No element\n");
		break;}
}

	return 0;
}
```
---
## 18. Matrix Addition
``` C
#include <stdio.h>
int main()
{
int a[3][3],b[3][3],c[3][3],i,j;
printf("enter matrix a\n");
for(i=0;i<=2;i++)
{
for(j=0;j<=2;j++)
scanf("%d",&a[i][j]);
}
printf("enter matrix b\n");
for (i=0;i<=2;i++)
{
for(j=0;j<=2;j++)
scanf("%d",&b[i][j]);
}
for(i=0;i<=2;i++)
{
for(j=0;j<=2;j++)
c[i][j]=a[i][j]+b[i][j];
}
printf("\n");
printf("sum of matrix\n");
for(i=0;i<=2;i++)
{
for(j=0;j<=2;j++)
printf("%d ",c[i][j]);
printf("\n");
}
printf("\n");
}
```
---
## 19. Transpose of Matrix
``` C
#include <stdio.h>
int main()
{
int a[3][3],b[3][3],c[3][3],i,j;
printf("enter matrix a\n");
for(i=0;i<=2;i++)
{
for(j=0;j<=2;j++)
scanf("%d",&a[i][j]);
}
printf("matrix a\n");
for(i=0;i<=2;i++)
{
for(j=0;j<=2;j++)
printf("%d ",a[i][j]);
printf("\n");
}
for (i=0;i<=2;i++)
{
for(j=0;j<=2;j++)
b[j][i]=a[i][j];
}
printf("\n");
printf("transpose of matrix\n");
for(i=0;i<=2;i++)
{
for(j=0;j<=2;j++)
printf("%d ",b[i][j]);
printf("\n");
}
printf("\n");
return 0;
}
```
---
## 20. Sum of Digits
``` C
#include <stdio.h>
 
int main()
{
   int n, t, sum = 0, remainder;
 
   printf("Enter an integer\n");
   scanf("%d", &n);
 
   t = n;
 
   while (t != 0)
   {
      remainder = t % 10;
      sum       = sum + remainder;
      t         = t / 10;
   }
 
   printf("Sum of digits of %d = %d\n", n, sum);
 
   return 0;
}
```
---
## 21. Palindrome
``` C
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
```
---
## 22. Swap two numbers using call by value
``` C
#include <stdio.h>
int swap(int num1,int num2);
void main()
{
	int a,b,c;
	printf("enter the numbers a and b ");
	scanf("%d %d",&a,&b);
	printf("numbers before swap are %d and %d\n",a,b);
	c=swap(a,b);
	printf(" numbers after swap are %d and %d\n",a,b);
}
int swap(int num1,int num2)
{
	int c;
	c=num1;
	num1=num2;
	num2=c;
}
```
---
## 23. Swap two numbers using call by reference
``` C
#include <stdio.h>
int swap(int *num1,int *num2);
void main()
{      
        int a,b,c;
        printf("enter the numbers a and b ");
        scanf("%d %d",&a,&b);
        printf("numbers before swap are %d and %d\n",a,b);
        c=swap(&a,&b);
        printf(" numbers after swap are %d and %d\n",a,b);
}
int swap(int *num1,int *num2)
{
        int c;
        c=*num1;
        *num1=*num2;
        *num2=c;
}
```
---
## 24.Enter the details of employee using structures
``` C
#include<stdio.h>
#include<string.h>
struct employee
{
int code;
char name[25];
char department[25];
float salary;
};
void main()
{
struct employee aemployee;
printf("Enter Employee's code:");
scanf("%d",&aemployee.code);
printf("Enter Employee's name:");
scanf("%s",aemployee.name);
scanf("%s",aemployee.name);
printf("Enter Employee's department:");
scanf("%s",aemployee.department);
printf("Enter employee's salary:");
scanf("%f",&aemployee.salary);
printf("\n\n Particulars of employee are:");
printf("\n Employee's code:%d",aemployee.code);
printf("\n Employee's name:%s",aemployee.name);
printf("\n Employee's department:%s",aemployee.department);
printf("\n Employee's salary:%f\n",aemployee.salary);
}
```
---
## 25. Fraction Product
```C
#include<stdio.h>
struct fraction
{
        int num;             
        int den;
};
int main()
{
        int rnum,rden;
        struct fraction f1,f2;
        printf("Enter numerator and denominator of first fraction\n");
        scanf("%d%d",&f1.num,&f1.den);
        printf("Enter numerator and denominator of second fraction\n"$
        scanf("%d%d",&f2.num,&f2.den);
        rnum=f1.num*f2.num;
        rden=f1.den*f2.den;
         printf("\n Product is :%d/%d\n",rnum,rden);
return 0;
}      
```
----
