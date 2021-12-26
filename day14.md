//wap to pass 2d array elements using function
#include<stdio.h>
int main()
{
int arr[3][4]={{1,2,3,4},{11,22,33,44},{55,66,77,88}};
int i,j;
printf("Before callin function :\n");
printf("the size of arr is %d\n",sizeof(arr));
printf("the array elements are:\n");
func(arr);
for(i=0;i<3;i++)
{
for(j=0;j<4;j++)
{
printf("%d\t",arr[i][j]);
}
printf("\n");
}
}
func(int a[][4])
{
int i,j;
printf("After calling the size of arr is %d\n",sizeof(a));
for(i=0;i<3;i++)
{
for(j=0;j<4;j++)
{
a[i][j]=a[i][j]+2;
}
printf("\n");
}
}
