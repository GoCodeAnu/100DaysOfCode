//wap to find the transpose of 2d matrices of nth row and nth column
#include<stdio.h>
#define ROW 4
#define COLUMN 3
int main()
{
int mat[ROW][COLUMN],trans[COLUMN][ROW],i,j;
printf("enter the elements of matrices that you would like to transpose:");
for(i=0;i<ROW;i++)
{
for(j=0;j<COLUMN;j++)
{
printf("\nmat[%d][%d]=",i,j);
scanf("%d",&mat[i][j]);
}
}
printf("the matrices you would like to transpose is:\n");
for(i=0;i<ROW;i++)
{
for(j=0;j<COLUMN;j++)
{
printf("%d ",mat[i][j]);
}
printf("\n");
}
for(j=0;j<COLUMN;j++)
{
for(i=0;i<ROW;i++)
{
trans[j][i]=mat[i][j];
}
}
printf("the transpose of mat[%d][%d]is:\n",ROW,COLUMN);
for(i=0;i<COLUMN;i++)
{
for(j=0;j<ROW;j++)
{
printf("%d ",trans[i][j]);
}
printf("\n");
}
}
