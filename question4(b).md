//input 2 matrices and find their product//
#include<stdio.h>
int main(void)
{
int m,n,p,q;
printf("Enter the value of p,q,m,n");
scanf("%d%d%d%d",&p,&q,&m,&n);
int r,c,e,a[p][q],b[m][n],l[p][n];
if (q==m)
{
{
r=0;
do{
c=0;
do{
printf("Enter element in a");
scanf("%d ",&a[r][c]);
c++;
}while(c<n);
r=r+1;
}while(r<m);
}
{
r=0;
do{
c=0;
do{
printf("Enter element in b");
scanf("%d ",&b[r][c]);
c++;
}while(c<n);
r=r+1;
}while(r<m);
}
printf("Resultant mateix\n");
for(r=0;r<m;r++)
{
for(c=0;c<n;c++)
{
l[r][c]=0;
for(e=0;e<n;e++)
{
l[r][c]+=a[r][e]*b[e][c];
}
printf("%d",l[r][c]);
}
printf("\n");
}
}
else
printf("Multiplication not possible");
}

/*output = 
Enter the value of p,q,m,n2
2
2
2
Enter element in a2
Enter element in a3
Enter element in a4
Enter element in a5
Enter element in b5
Enter element in b4
Enter element in b3
Enter element in b2
Resultant mateix
1311
3127
*/
