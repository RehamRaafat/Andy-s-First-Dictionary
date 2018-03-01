#include <bits/stdc++.h>

using namespace std;

int main()
{
    set<string>s;
    string v,x="";
    while(cin>>v)
    {
        for(int i=0; i<v.size(); i++)
        {
            v[i]=tolower(v[i]);
        }
        for(int j=0; j<v.size(); j++)
        {
            if(v[j]>=32||v[j]<=64&&v[j])
                continue;
            else
                x+=v[j];

        }
        s.insert(x);
         for(set<string>::iterator itr=s.begin(); itr!=s.end(); itr++)
        {
            cout<<*itr<<endl;
        }
    }

    return 0;
}
