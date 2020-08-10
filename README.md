# Count-pairs-codevita-zone-1-
#include <bits/stdc++.h>
using namespace std;
int main() {
   int n,k,p,q,count=0;
   cin>>n>>k;
   int a[n];
   for(int i=0;i<n;i++){
       cin>>a[i];
   }
   for(int i=0;i<n;i++){
         p=(a[i]-k);
         q=(a[i]+k);
        for(int j=0;j<=n;j++){
        if(i!=j){
        if(a[j]<=q && a[j]>=p ){
            count++;
            break;
        }
      }
   }
 }
    cout<<count;
   return 0;
}
