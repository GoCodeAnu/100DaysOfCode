//wap to print the array element using pointer subscript
#include<stdio.h>
int main()
{
int a[5]={1,2,3,4,5};
int *p=a;
int i;
for(i=0;i<5;i++)
{
printf("the value of a[%d]=%d\n",i,p[i]);
printf("the address of a[%d]=%u\n",i,p+i);
}
}
