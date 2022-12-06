# odevv

//dizinin en büyük ve en küçük elamanını döndürren fonskiyon. dizi 5 elemanlı.

#include<stdio.h>

int maxBul(int dizi[]);
int minBul(int dizi[]);

int main(void)
{
	int sayilar[5];
	
	for(int i=0;i<5;i++)
	{
		printf("%d. sayiyi giriniz.\n" , i+1);
		scanf("%d" , &sayilar[i]);
	}
	
	printf("en buyuk sayi:%d\n" , maxBul(sayilar));
	printf("en kucuk sayi:%d\n" , minBul(sayilar));
	
	return 0;
}

int maxBul(int dizi[])
{
	int max;
	max=dizi[0];
	
	for(int i=0;i<5;i++)
	{
		if(max<dizi[i])
		{
			max=dizi[i];
		}
	}
	
	return max;
}

int minBul(int dizi[])
{
	int min;
	min=dizi[0];
	
	for(int i=0;i<5;i++)
	{
		if(min>dizi[i])
		{
			min=dizi[i];
		}
	}
	
	return min;
}
