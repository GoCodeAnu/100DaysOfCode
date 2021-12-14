//wap to find the factorial of a number using recursion
#include<stdio.h>
int fact(int a);
int main()
{
int n;
char label;
label:
printf("enter any positive number");
scanf("%d",&n);
if(n<1)	
{
printf("Please try again!\n");
goto label;
}
printf("the factorial of %d is %d\n",n,fact(n));
}
int fact(int a)
{
if(a==1)
{
	return 1;
}
else 
return (a*fact(a-1));
}
