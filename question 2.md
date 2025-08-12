#include<iostream>
using namespace std;

int U(int A[],int n)
{ 
for(int i=0;i<n;i++)
{
int x=0;
for (int j=i;j<n;j++)
{
if(A[i]==A[j])
{
x++;
}
}
if(x==2)
{
cout<<"duplicate number is = "<<A[i]<<endl;
}
}
return 0;
}

int main()
{
int A[6]={7,1,2,1,2,1};
cout<<U(A,6);
return 0;
}

/*output - 
chetanyabhargav@MacBook-Air-13 DSA LAB Assignnment 1 % cd "/Users/chetanyabhargav/Desktop/chetan
ya_coding/DSA LAB Assignnment 1/" && g++ question2.cpp -o question2 && "/Users/chetanyabhargav/D
esktop/chetanya_coding/DSA LAB Assignnment 1/"question2
duplicate number is = 2
duplicate number is = 1
0%                                                                                              
chetanyabhargav@MacBook-Air-13 DSA LAB Assignnment 1 % 
*/
