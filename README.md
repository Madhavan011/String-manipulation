#include <iostream.h>        
#include <string.h>
#include <conio.h>
void reverseString(char *str) {
int start = 0;
int end = strlen(str) - 1;
char temp;
while (start < end) {
temp = str[start];
str[start] = str[end];
str[end] = temp;
start++;
end--;
}
}
int stringLength(const char*str)
{
int length=0;
While(*str!='\0'){
length++;
str++;
}
return length;
}
void main()
{
char str[100];
char str1[100]="Hello";
clrscr();
cout<<"Enter a string:";
cin.getline(str,100);
int length=stringLength(str);
cout<<"Length of the string:" << length << endl;
reverseString(str);
cout<<"Reverse string:"<<str<<endl;
getch();
}
