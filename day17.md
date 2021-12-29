//wap to use string function(strcmp)
#include<stdio.h>
#include<string.h>
int main()
{
char name1[20],name2[20];
puts("name1:");
gets(name1);
puts("name2");
gets(name2);
if((strcmp(name1,name2))==0)
printf("name1 and name 2 are same:");
else
printf("name1 and name2 are not same:");
}
