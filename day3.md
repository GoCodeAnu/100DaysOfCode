//wap to arrange elements in ascending and descending order in the array
#include<stdio.h>
#define N 10
int main()
{
	int i,j,temp;
int a[N]={24,43,13,32,54,46,56,76,89,76};
for(i=0;i<N;i++)
{
for(j=i+1;j<N;j++)
{
if(a[i]>a[j])
{
temp=a[i];
a[i]=a[j];
a[j]=temp;
}
}
}
printf("the ascending order is:\n");
for(i=0;i<N;i++)
{
printf("  %d",a[i]);
}
for(i=0;i<N;i++)
{
for(j=i+1;j<N;j++)
{
if(a[i]<a[j])
{
temp=a[i];
a[i]=a[j];
a[j]=temp;
}
}
}
printf("\nthe descending order is:\n");
for(i=0;i<N;i++)
{
printf("  %d",a[i]);
}
}
