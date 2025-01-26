# Codeforces-Solutions
#codeforces#competitive-programming#cpp-solutions
## Solved Problems:
https://codeforces.com/problemset/problem/2056/C
https://ide.usaco.guide/OHYrAdcJWStJ2MDbUYc


#include <bits/stdc++.h>
#include <cstdint>
#define int long long
#define pb push_back
using namespace std;
void solve(){
    int n; cin >> n;
    if(n==6){
        cout<<1<<" "<<1<<" "<<2<<" "<<3<<" "<<1<<" "<<2<<endl;
    }
    else if(n==7){
        cout<<1<<" "<<1<<" "<<2<<" "<<3<<" "<<1<<" "<<2<<" "<<3<<endl;
    }
    else{
        if(n%2==0){
            for(int i=1; i<=n/2; i++){
                cout<<i<<" ";
            }
             for(int i=1; i<=n/2; i++){
                cout<<i<<" ";
            }
            cout<<endl;
        }
        else{
            for(int i=1;i<=n/2 ; i++){
                cout<<i<<" ";
            }
            for(int i=1;i<=n/2 ; i++){
                cout<<i<<" ";
            }
            cout<<(n/2)+1<<endl;
        }
    }
}
int32_t main() {
	int t; cin >> t;
    while(t--){
        solve();
    }
}
