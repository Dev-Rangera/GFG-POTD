class Solution {
  public:
    vector<int> leastPrimeFactor(int n) {
        // code here
        vector<int>ans;
        ans.push_back(0);
        
        
        for(int i=1;i<=n;i++){
            
            if(i==1 || i==2 ||i==3){
                ans.push_back(i);
            }
            
            else{
                int j=0;
                for(j=2;j<i;j++){
                    
                    if(i%j==0){
                        ans.push_back(j);
                        break;
                    
                    }
                }
                if(j==i){
                    ans.push_back(i);
                }
            }
        }
        return ans;
    }
};
