Testing Code below 
- RAM
=======
#include <iostream>
#include <fstream>
#include <string>

using namespace std;
int main()
{
int num;
int count=1;
int fib1=0;
int fib2=1;
int fib0;
int tem;
char comma=',';

cout << "How many Fibonacci #'s do you want to display? ";
cin>>num;

while (num<1 || num>70)
{
cout << "Please enter a number in the range of 1-70.";
cin>>num;
}
while (count<=num)
{
if (count==1)
{
cout<<fib1;
}
else if (count==2)
{
cout<<comma<<fib2;
}
else
{
fib0=fib1+fib2;
cout<<comma<<fib0;
fib1=fib2;
fib2=fib0;





}
count++;
}
}
