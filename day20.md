//wap to check palindrome without using string function
#include<stdio.h>
int main()
{
char str[20];
int flag;
int i=0;
puts("please enter the word you would like to check the palindromicity");
gets(str);
int count=0;
while(str[count]!='\0')
{
count++;
}
int len=count-1;
while(i<=len)
{
if(str[i]==str[len])
{
flag=1;
}
else
{
	flag=0;
	break;
}
i++;
len--;
}
if(flag==1)
printf("palindrome");
else
printf("not palindrome");
}
