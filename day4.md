//wap to pass whole array to a function and see how the changes made in formal arguments affect the actual arguements
#include<stdio.h>
int main()
{
int arr[10]={1,2,3,4,5,6,7,8,9,10},i;
arrrfunc(arr);
printf("the new array is:\n");
for(i=0;i<10;i++)
{
	printf("  %d",arr[i]);
}
}
arrrfunc(int aarr[10])
{
 int i,sum=0;
	for(i=0;i<10;i++)
	{
aarr[i]=aarr[i]*aarr[i];
sum+=aarr[i];
}
printf("the sum of array is:%d\n",sum);
}
