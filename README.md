- š Hi, Iām @princekumarb
- š Iām interested in ...
- š± Iām currently learning ...
- šļø Iām looking to collaborate on ...
- š« How to reach me ...

<!---
princekumarb/princekumarb is a āØ special āØ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
* C program to count frequency of each element of array
 */

@@ -0,0 +1,33 @@
#include<iostream>
using namespace std;
int main()
{
	int n;
	cin>>n;
	int arr[n];
	for(int i=0;i<n;i++)
	{
		cin>>arr[i];

	}
	int counter =1;
	while(counter<n)
	{
	for(int i=0;i<n-counter;i++)
	{
			if(arr[i]>arr[i+1])
			{
		int temp = arr[i];
		arr[i]=arr[i+1];
		arr[i+1]=temp;		
			}
		}
		counter++;
	}
	for(int i=0;i<n;i++)
	{
		cout<<arr[i]<<" ";
	}
	cout<<endl;
}
