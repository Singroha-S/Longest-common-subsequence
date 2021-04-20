#include<bits/stdc++.h>
using namespace std;

string LCS(string x,string y,int m,int n)
{
    int t[m+1][n+1];
    int i=m;
    int j=n;
    string s=" ";
    while(i>0&&j>0)
    {
        if(x[i-1]==y[j-1])
        {
            s.push_back(x[i]);
            i--;
            j--;
        }
        else
        {
            if(t[i][j-1]>t[i-1][j])
            {
                s.push_back(y[j-1]);
                j--;
            }
            else if(t[i-1][j]>t[i][j-1])
            {
                 s.push_back(x[i-1]);
                i--;
            }
        }
    }
    while(i>0)
    {
         s.push_back(x[i-1]);
                i--;
    }
     while(j>0)
    {
         s.push_back(y[j-1]);
                j--;
    }
    return s;
}

int main()
{
    string x;            
    string y;            
    cin>>x;
    cin>>y;
    int m=x.length();
    int n=y.length();
    cout<<LCS(x,y,m,n);
}
