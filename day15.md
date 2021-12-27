//wap to dereference a void pointers
#include<stdio.h>
int main()
{
int a=5;
float b=3.4567, *fb=&b;
char ch='A', *chh=&ch;
void *vpp;
vpp=&a;
printf("%u \n",vpp);
printf("%d\n",*(int *)vpp);
vpp=fb;
printf("%u \n",vpp);
printf("%f\n",*(float *)vpp);
vpp=chh;
printf("%u \n",vpp);
printf("%c\n",*(char *)vpp);
}
