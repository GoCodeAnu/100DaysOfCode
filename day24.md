//wap to take input of data of student using structures of array
#include<stdio.h>
int main()
{
struct student{
char name[20];
int rollno;
};
int i;
struct student styearsgirls[5];
printf("enter name and roll no of respective students:\n");
for(i=0;i<5;i++)
{
scanf("%s %d",styearsgirls[i].name,&styearsgirls[i].rollno);
}
printf("name and roll no of respective students are:");
for(i=0;i<5;i++)
{
printf("\n%s\t%d\n",styearsgirls[i].name,styearsgirls[i].rollno);
}
}
