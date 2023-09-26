// User function template for C++

class Solution{
    public:
    // arr[] : int input array of integers
    // k : the quadruple sum required
    vector<vector<int> > fourSum(vector<int> &arr, int k) {
        // Your code goes here
        vector<vector<int>> ans;
        int n=arr.size();
        int p,q;
        sort(arr.begin(),arr.end());
        for(int i=0;i<n-3;i++)
        {
            for(int j=i+1;j<n-2;j++)
            {
                p=j+1;
                q=n-1;
                while(p<q)
                {
                    if(arr[i]+arr[j]+arr[p]+arr[q]==k)
                    {
                    vector<int>nums;
                    nums={arr[i],arr[j],arr[p],arr[q]};
                    ans.push_back(nums);
                   
                    }
                    if(arr[i]+arr[j]+arr[p]+arr[q]<k)
                    p++;
                    else
                    q--;
                }
            }
        }
         sort(ans.begin(), ans.end());

    // Use the unique algorithm to remove duplicates
    ans.erase(unique(ans.begin(), ans.end()), ans.end());
        return ans;
    }
};
