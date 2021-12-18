//wap to multiply two matrices
#include<stdio.h>
int main()
{
	int R1,R2,C1,C2;
	char level;
	level :
	printf("enter the order of first matrix  and second matrix in the order m*n and m*n");
	scanf("%d %d %d %d",&R1,&C1,&R2,&C2);
int A[R1][C1],B[R2][C2],C[R1][C2],i,j,k;
if(C1!=R2)
{
printf("!!!!!the column of first matrix must match the row of second matrix.Please update the row and column!!!!!\n");
goto level;
}
printf("enter the elements for first matrix:\n ");
for(i=0;i<R1;i++)
{
for(j=0;j<C1;j++)
{
printf("A[%d][%d]=",i,j);
scanf("%d",&A[i][j]);
}
}
printf("enter the elements for second matrix:\n ");
for(i=0;i<R2;i++)
{
for(j=0;j<C2;j++)
{
printf("B[%d][%d]=",i,j);
scanf("%d",&B[i][j]);
}
}
printf("the matrix A is:\n");
for(i=0;i<R1;i++)
{
for(j=0;j<C1;j++)
{
printf("%d  ",A[i][j]);
}
printf("\n");
}
printf("the matrix B is:\n");
for(i=0;i<R2;i++)
{
for(j=0;j<C2;j++)
{
printf("%d  ",B[i][j]);
}
printf("\n");
}
for(i=0;i<R1;i++)
{
for(j=0;j<C2;j++)
{
	C[i][j]=0;
for(k=0;k<C1;k++)
{
C[i][j]+=A[i][k]*B[k][j];
}
}
}
printf("the resultant matrix after multiplication  is:\n");
for(i=0;i<R1;i++)
{
for(j=0;j<C2;j++)
{
printf("%d  ",C[i][j]);
}
printf("\n");
}
}
