//wap to  know about pointers to structure
#include<stdio.h>
int main()
{
	struct employee{
	char name[20];
	int age;
	float salary;
	};
	struct employee emp1={"susmita",20,4000},*ptr;
	ptr=&emp1;
	printf("name=%s\t age=%d\t salary=%f",ptr->name,ptr->age,ptr->salary);
}
