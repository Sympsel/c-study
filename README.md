# c-study
每日进步一点点

12.30
//菱形打印

```c
#include<stdio.h>
int main()
{
	char ch;
	int n;
	printf("请输入组成菱形的字符\n");
	scanf("%c", &ch);
	printf("请输入菱形的边长（字符个数）\n");
	scanf("%d", &n);

	for (int i = 1; i <= n; i++)
	{
		for (int j = 1; j <= n-i; j++)
			printf(" ");
		for (int j = 1; j <= (2 * i - 1); j++)
			printf("%c", ch);
		printf("\n");
	}
	for (int i = 1; i < n; i++)
	{
		for (int j = 1; j <= i; j++)
			printf(" ");
		for (int j = 1; j <= 2 * n - 2 * i - 1; j++)
			printf("%c", ch);
		printf("\n");
	}



	return 0;
}
