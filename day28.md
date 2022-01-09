//wap to pass whole array to the function
#include<stdio.h>
struct student{
char name[20];
int rollno;
int marks;
};
void display(struct student);
void dec_marks(struct student stuarr[]);
int main()
{
int i;
struct student stuarr[3]={
{"anu",1,45},
{"anup",2,55},
{"anuja",3,15}
};
dec_marks(stuarr);
for(i=0;i<3;i++)
display(stuarr[i]);
}
void dec_marks(struct student stuarr[])
{
int i;
for(i=0;i<3;i++)
{
stuarr[i].marks=stuarr[i].marks-5;
}
}
void display(struct student stu)
{
printf("name=%s\t roll no=%d\t marks=%d\n",stu.name,stu.rollno,stu.marks);
}
