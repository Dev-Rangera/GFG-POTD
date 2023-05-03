# GFG-POTD
Problem of The Day 

03-05-2023


You are given an array of strings arr of size n. You have to find out if it is possible to make a palindromic string by concatenating the strings in any order. Provided that all the strings given in the array are of equal length.


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
