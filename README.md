# GFG-POTD
Problem of The Day 

03-05-2023

class Solution{
public:
    bool makePalindrome(int n,vector<string> &arr){
  
   bool makePalindrome(int n, vector<string> &arr){
        unordered_map<string, int> mp;
        if(n == 1) return false;
        
        for(auto s: arr) {
            mp[s]++;
            reverse(s.begin(), s.end());
            mp[s]++;
        }
        
        return mp.size() == n;
    }
  }   
 }; 
