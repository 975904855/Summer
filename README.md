# Summer
zuoye
#include<stdio.h>
void main()
{
	int n,i,k,temp,max;
	int a[10];
	printf("n=");
	scanf("%d",&n);
	for(i=0;i<n;i++)
	   scanf("%d",&a[i]);
	for(k=0;k<n-1;k++)
	{
		max=k;
		for(i=k+1;i<n;i++)
			if(a[i]>a[k])
				max=i;
			temp=a[max];
			a[max]=a[k];
			a[k]=temp;
	}
	for(i=1;i<n;i++)
		printf("%d ",a[i]);
	printf("\n");

	

}
