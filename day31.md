#include<stdio.h>
int main()
{
FILE *p;
char ch;
if((p=fopen("myfile.txt","r"))==NULL)
printf("this file doesnt exist\n");
else
{
while ((ch=fgetc(p))!=EOF)
printf("%c",ch);
}
fclose(p);
}
