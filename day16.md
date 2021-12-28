just did thebasic string today
//wap to print the address of the string literal and print them
#include<stdio.h>
#include<string.h>
int main()
{
	char str[]="beautiful";
	int i;
for(i=0;str[i]!='\0';i++)
{
printf("the address =%d\t",&str[i]);
printf("the value=%c\t",str[i]);
printf("\n");
}
}
