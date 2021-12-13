# 100DaysOfCode
//wap to find the factorial of any number
#include<stdio.h>
int fact(int a);
int main()
{
	int n;
	printf("enter two number if you are happy right now?\n");
	char repeat;
 repeat:
printf("enter any positive number");
scanf("%d",&n);
	if(n<0)
	{
		printf("negative number has no factorial\n");
	printf("	please try again\n");
		goto repeat;
	}
	else
	printf("the factorial of %d is %d\n",n,fact(n));
}
int fact(int a)
{
int factorial=1,i;
if (a==1)
{
return 1;
}
for(i=2;i<=a;i++)
{
factorial*=i;
}
return(factorial);
}
