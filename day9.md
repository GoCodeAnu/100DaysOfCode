//wap to print value of array element and address using pointer notations
#include<stdio.h>
int main()
{
int arr[5]={1,2,3,4,5};
int i;
for(i=0;i<=4;i++)
{
printf("the value of arr[%d]=%d\n",i,*(arr+i));
printf("the address of arr[%d]=%d\n",i,arr+i);
}
}
