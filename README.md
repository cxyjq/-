# bubble_sort
The first time upload my code
'#include<stdio.h>
void bubble_sort(int* arr,int sz)
{
	int count = 0;
	for (int i = 0; i < sz-1; i++)
	{
		count = 0;
		for (int j = 0; j < sz - 1 - i; j++)
		{
			if (arr[j] > arr[j + 1])
			{
				int mid = arr[j];
				arr[j] = arr[j + 1];
				arr[j + 1] = mid;
				count = 1;
			}
		}
		if (count == 0)
			break;
	}
}
int main()
{
	int arr[100] = { 0 };
	int n;
	scanf("%d", &n);
	for (int i = 0; i < n; i++)
		scanf("%d", &arr[i]);
	bubble_sort(arr, n);
	for (int i = 0; i < n; i++)
		printf("%d", arr[i]);
}'
