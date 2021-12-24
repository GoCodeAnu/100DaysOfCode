//wap to print the elements of 2D array using pointer notation 
#include<stdio.h>
int main()
{
int a[3][4]={{1,2,3,4},{5,6,7,8},{11,22,33,44}};
int i,j;
int (*p)[4];
p=a;
for(i=0;i<3;i++)
{
	printf("the address of %dth 1D array is=%u %u\n",i,p+i,*(p+i));
for(j=0;j<4;j++)
{
printf("the value is=%d %d \t",p[i][j],*(*(p+i)+j));
}
printf("\n");          
}
}
