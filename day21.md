//wap to encript the given text and decript it again
#include<stdio.h>
int main()
{
char word[20];
puts("enter your message:\n");
gets(word);
int i=0;
while (word[i]!='\0')
{
word[i]=word[i]-33;
i++;
}
puts("the encrypted string is:\n");
puts(word);
i=0;
while (word[i]!='\0')
{
word[i]=word[i]+33;
i++;
}
puts("the decrypted string or the original string is:\n");
puts(word);
}
