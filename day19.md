//wap to use sprintf() 
#include<stdio.h>
#include<string.h>
int main()
{
	char name[20]="Anu Ale Magar";
int m1=85,m2=90,m3=89,m4=98,m5=97;
float per=(m1+m2+m3+m4+m5)/5;
char str1[50];
sprintf(str1,"name- %s %d %d %d %d %d \n percentage-%.3f",name,m1,m2,m3,m4,m5,per);
printf("%s",str1);
}
