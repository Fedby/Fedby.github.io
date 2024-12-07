#include <bits/stdc++.h>
using namespace std;
int  fb(int n){
    int a[1000001];
    a[1]=1;
    a[2]=1;
    for(int i=3;i<=n;i++){
        a[i]=a[i-1]+a[i-2];
        if(a[i]>=10007){
            a[i]-=10007;
        }
    }
    cout<<a[n];
}
int main() {
    int n;
    cin>>n;
    fb(n);
 return 0;
}