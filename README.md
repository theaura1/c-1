# c-1
1st program
 #include<fstream.h>
#include<conio.h>

void main()
{
ifstream fin;
fin.open("sample.txt");
char ch;
int i,a=0,s=0,d=0;

while(fin)
{
fin.get(ch);
i=ch;
if(i>63&&i<91||i>96&&i<123)
a++;
else
if(ch==' ')
s++;
else
if(i>47&&i<58)
d++;
}
cout<<"No. OF Alphabates:"<<a;
cout<<"nNo. Of Digits:"<<d;
cout<<"nNo. Of Spaces:"<<s;
getch();
}
