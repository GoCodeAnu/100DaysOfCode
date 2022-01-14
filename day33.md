//wap to know about character input output
#include<stdio.h>
int main()
{
FILE *P;
char nam;
P=fopen("character_io.txt","r");
if(P==NULL)
{
printf("file doesnt exist\n");
return -1;
}
else
{
printf("opened sucessfully\n");
nam=fgetc(P);
while(nam !=-1)
{
printf("%c",nam);
nam=fgetc(P);
}
fclose(P);
return 0;
}
}
