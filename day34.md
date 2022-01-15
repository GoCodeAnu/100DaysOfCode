#include<stdio.h>
int main()
{
	char ch[100];
FILE *p;
p=fopen("myline.txt","r");
if(p==NULL)
{
printf("file doesnt exist");
return-1;
}
else
{
printf("opened sucessfully\n");
fgets(ch,100,p);
puts(ch);
fgets(ch,100,p);
puts(ch);
}
fclose(p);
return 0;
}
