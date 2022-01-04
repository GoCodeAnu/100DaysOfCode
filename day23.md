//program to display sructure variable
#include<stdio.h>
struct student{
char name[20];
int roll;
float marks;
};
int main()
{
struct student stu1={"Anu",8,495.687};
struct student stu2={"bishal",002,567.45};
struct student stu3;
printf("please enter the name of third student,his or her roll number and marks obtained");
scanf("%s %d %f",stu3.name,&stu3.roll,&stu3.marks);
printf("name=%s- roll=%d marks=%f\n",stu1.name,stu1.roll,stu1.marks);
printf("name=%s- roll=%d marks=%f\n",stu2.name,stu2.roll,stu2.marks);
printf("name=%s- roll=%d marks=%f\n",stu3.name,stu3.roll,stu3.marks);
}
