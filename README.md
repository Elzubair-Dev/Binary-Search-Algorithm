# Binary-Search-Algorithm
Binary search algorithm is one of the advanced searching algorithms
        
## Code:
```
using namespace std;
#include<iostream>
int BSearch(int arr[], int l, int h, int num)
{
	int m = (l + h) / 2;
	if (arr[m] == num)
	{
		return m;
	}
	else if (arr[m] > num)
	{
		h = m - 1;
	}
	else if (arr[m] < num)
	{
		l = m + 1;
	}
	if (l > h)return -1;
	else
	BSearch(arr, l, h, num);
}
int main()
{
	int x = 0;
	int z[] = { 10,20,30,40 };
	int n = sizeof(z) / sizeof(z[0]);
	cout << "Original Array is [";
	for (int i = 0; i < n; i++) {
		cout << z[i] << " ";
	}
	cout << "]\n\n";
	cout << "Enter the Number\n";
	cin >> x;
	int r = BSearch(z, 0, n - 1, x);
	if (r == -1)cout << "Number is not exist\n";
	else cout << "Found in index no: " << r + 1 << "\n";
}
```
      
## Buy me a Coffee:
if you want to support me
(https://www.buymeacoffee.com/zu698air)
       
#### Don't forgit to give me a Star
      
## Done
