#include <iostream>
#include <cstring>
#include <cstdio>
using namespace std;
int rank[22];
int a[22];
int n,themax;
int dp[22];


void search(){	
		for(int i=1;i<=n;i++){
			dp[i]=1;
			for(int j=1;j<i;j++){
				
				if(rank[a[i-1]]>rank[a[j-1]]){
				dp[i]=max(dp[i],dp[j]+1);			
			}
			}
			themax=max(dp[i],themax);
			}

}

int main(){	freopen("in.txt","r",stdin);
		cin >> n;
		for(int i=1;i<=n;i++){
				cin >> rank[i];
		}
		int t;
		while(cin >> t){
			a[t-1]=1;
			for(int i=2;i<=n;i++){
				int t; cin >> t; a[t-1]=i;
				
				}
			themax=0;
			memset(dp,0,sizeof(dp));
			search();
			cout << themax << endl;
			}		
		
	
	
	
	return 0;}
