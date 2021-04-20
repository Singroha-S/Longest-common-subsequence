#include<bits/stdc++.h>
using namespace std;

int LCSs(string x,string y,int m,int n)
{
    int t[m+1][n+1];
    int r=0;
    for(int i=0;i<m+1;i++)
    {
        for(int j=0;j<n+1;j++)
        {
            if(i==0||j==0)
            {
                t[i][j]=0;
            }
            else if(x[i-1]==y[j-1])
            {
                t[i][j]=1+t[i-1][j-1];
                r=max(r,t[i][j]);
            }
            else
            {
                t[i][j]=0;
            }
        }
    }
    return r;
}

int main()
{
    string x;
    string y;
    cin>>x;
    cin>>y;
    int m=x.length();
    int n=y.length();
    cout<<endl<<LCSs(x,y,m,n);
}
