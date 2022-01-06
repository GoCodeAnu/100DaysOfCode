//wap to know about structures within structure
#include<stdio.h>
int main()
{
struct marks{
int marks1;
int marks2;
};
struct students{
char name[20];
struct marks maks;
} st1,st2;
printf("enter name and marks for 1st sutdent");
scanf("%s %d %d",st1.name,&st1.maks.marks1,&st1.maks.marks2);
printf("enter name and marks for 2nd sutdent");
scanf("%s %d %d",st2.name,&st2.maks.marks1,&st2.maks.marks2);
printf("name=%s\t marks1=%d \tmarks2=%d\n",st1.name,st1.maks.marks1,st1.maks.marks2);
printf("name=%s\t marks1=%d \tmarks2=%d\n",st2.name,st2.maks.marks1,st2.maks.marks2);
}
