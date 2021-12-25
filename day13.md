//wap to return more than one value from a function using pointers
#include<stdio.h>
void anu(int a,int b,int *sum,int *prod,int *sub);
int main()
{
int x=8,y=4,sum,prod,sub;
anu(x,y,&sum,&prod,&sub);
printf("the sum of %d and %d is = %d\n the product of %d and %d is = %d\n the subtraction of %d and %d = %d\n",x,y,sum,x,y,prod,x,y,sub);
}
void anu(int a,int b,int *sum,int *prod,int *sub)
{
*sum=a+b;
*prod=a*b;
*sub=a-b;
}
