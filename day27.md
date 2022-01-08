//wap to know how a structure variable is returned to  the main function
#include<stdio.h>
struct student{
	char name[20];
	int marks;
	char grade;
};
void display(struct student );
struct student change (struct student stu);
int main ()
{
struct student stu1={"anu",670,'B'};
struct student stu2={"sashi",760,'A'};
stu1=change(stu1);
stu2=change(stu2);
display(stu1);
display(stu2);
}
struct student change (struct student stu)
{
stu.marks=stu.marks+10;
return stu;
}
void display(struct student stu)
{
	printf("name=%s\t marks=%d \t grade=%c\n",stu.name,stu.marks,stu.grade);
}


