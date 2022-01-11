#include<stdio.h>
int main()
{
FILE *fptr;
int ch;
fptr=fopen("myfile.text","w");
if(fptr==NULL)
{
printf("file doesnt exist\n");
exit(1);
}
else
{
printf("enter text:");
while((ch=getchar())!=EOF)
fputc(ch,fptr);
}
fclose(fptr);
}
