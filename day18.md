//wap to print 2d string element
#include<stdio.h>
#define N 5
#define LEN 10
int main()
{
	int i;
char str[N][LEN]={"yellow","orange","green","blue","red"};
for(i=0;i<N;i++)
{
printf("the value is =%s\n",str[i]);
printf("the address is =%u\n",str[i]);
}
}
