// User function Template for C++

class Solution {
  public:
    int shortestDistance(int N, int M, vector<vector<int>> A, int X, int Y) {
        // code here
        if(!A[0][0]) return -1;
        int ans = 0;
        vector<vector<bool>> visit(N,vector<bool>(M,false));
        queue<pair<int,int>> que;
        
        que.push({0,0});
        visit[0][0] = true;
        
        while(!que.empty()){
            int n = que.size();
            for(int k=0;k<n;k++){
                auto node = que.front();
                que.pop();
                int i = node.first;
                int j = node.second;
                
                if(i==X and j==Y) return ans;
                
                if(i+1<N and !visit[i+1][j] and A[i+1][j]==1){
                    que.push({i+1,j});
                    visit[i+1][j] = true;
                }
                if(i-1>=0 and !visit[i-1][j] and A[i-1][j]==1){
                    que.push({i-1,j});
                    visit[i-1][j] = true;
                }
                if(j+1<M and !visit[i][j+1] and A[i][j+1]==1){
                    que.push({i,j+1});
                    visit[i][j+1] = true;
                }
                if(j-1>=0 and !visit[i][j-1] and A[i][j-1]==1){
                    que.push({i,j-1});
                    visit[i][j-1] = true;
                }
            }
            ans++;
        }
      return -1;   
    }
};
