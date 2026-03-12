C++ code:
Method 1:
#include<iostream>
#include<vector>
using namespace std;
void sortArray(vector<int>& v,int n)
{
    int count0=0,count1=0,count2=0;
    for(int i=0;i<n;i++)
    {
        if(v[i]==0) count0++;
        if(v[i]==1) count1++;
        if(v[i]==2) count2++;
    }
    for(int i=0;i<count0;i++) v[i]=0;
    for(int i=count0;i<count0+count1;i++) v[i]=1;
    for(int i=count0+count1;i<n;i++) v[i]=2;
    for(int x:v)
    {
        cout<<x<<" ";
    }
}
int main()
{
    int n;
    cin>>n;
    vector<int>v(n);
    for(int i=0;i<n;i++)
    {
        cin>>v[i];
    }
    sortArray(v,n);
}

Method 2:
#include<iostream>
#include<algorithm>
#include<vector>
using namespace std;
void sortArray(vector<int>& v,int n)
{
    int low=0,mid=0,high=n-1;
    while(mid<=high)
    {
        if(v[mid]==0)
        {
            swap(v[low],v[mid]);
            low++;
            mid++;
        }
        else if(v[mid]==1)
        {
            mid++;
        }
        else
        {
            swap(v[mid],v[high]);
            high--;
        }
    }
    for(int i=0;i<n;i++)
    {
        cout<<v[i]<<" ";
    }
}
int main()
{
    int n;
    cin>>n;
    vector<int>v(n);
    for(int i=0;i<n;i++)
    {
        cin>>v[i];
    }
    sortArray(v,n);
}

Input:
6
2 0 2 1 1 0

Output:
0 0 1 1 2 2 
