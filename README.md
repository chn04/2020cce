# 2020cce
## 第一章
```c
#include <stdio.h>
int p1(int a,int b)
{
	int c;
	while(c=a%b)
	{
		a=b;
		b=c;
	}
	return b;
}
int main()
{
	int x,y;
	scanf("%d%d",&x,&y);
	int d;
	d=p1(x,y);
	int j,k;
	j=x/d;
	k=y/d;
	printf("%d %d\n",j,k);
}
```
## 第二章
```c
#include <stdio.h>
int a[10];
int main()
{
	int n;
	for(int i=1;i<=10;i++)
	{
		if(n==0)
		break;
		else scanf("%d",&a[i]);
	}
	for(int i=10;i>=1;i--)
	{
		if(a[i]!=0)printf("%d ",a[i]);
	}
	printf("\n");
}
```
## 第三章
```c
#include <stdio.h>
int MYPOWER(int x,int y)
{
	int ans=1;
	if(x>=1 && x<=9)
	{
		for(int i=1;i<=y;i++)
		{
			ans*=x;
		}
	}
	return ans;
}
int main(void)
{
	int a,b;
	scanf("%d%d",&a,&b);
	printf("[%d]",MYPOWER(a,b));
	return 0;
}
```
## 第四章
```c
#include <stdio.h>
int main()
{
	int a,n=0;
	scanf("%d",&a);
	for(int i=2;i<=a;i++)
	{
		int j,z;
		j=i-1;
		z=j*i;
		n=n+z;
	}
	printf("%d\n",n);
}
```
## 第五章
```c
#include <stdio.h>
int main()
{
	int a;
	scanf("%d",&a);
	printf("%d=%d*%d+%d*%d+%d*%d\n",a,50,a/50,5,a%50/5,1,a%50%5/1);
}
```
## 第六章
```c
#include <stdio.h>
int main()
{
	int a;
	scanf("%d",&a);
	int k=0;
	for(int i=1;i<=a;i++)
	{
		if(a%i==0)k++;
	}
	printf("%d\n",k);
}
```
## 第七章
```c
#include <stdio.h>
int main()
{
	int a,k=0;
	for(int i=1;i<=10;i++)
	{
		scanf("%d",&a);
		if(a%3==0)
		{
			k++;
		}
	}
	printf("%d\n",k);
}
```
## 第八章
```c
#include <stdio.h>
int main()
{
	int a;
	scanf("%d",&a);
	if(a>=90)printf("A\n");
	else if(a>=80)printf("B\n");
	else if(a>=60)printf("C\n");
	else printf("F\n");
}
```
## 第九章
```c
#include<stdio.h>
int main()
{
int n1=10,n2=20,n3=30;
printf(“n1:%d n2:%d n3:%d\n”,n1,n2,n3);
int *p=&n1;
*p=200;
printf(“n1:%d n2:%d n3:%d\n”,n1,n2,n3);
int *p2=&n3;
*p2=300;
printf(“n1:%d n2:%d n3:%d\n”,n1,n2,n3);
p2=p;
*p2=400;
printf(“n1:%d n2:%d n3:%d\n”,n1,n2,n3);
return 0;
}
```
