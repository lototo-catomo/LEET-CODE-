//PROBLEM NAME : Longest substring without repeating characters
//PROBLEM LINK : https://leetcode.com/problems/longest-substring-without-repeating-characters/


class Solution {
public:
    int lengthOfLongestSubstring(string s) {
        
        int l=0,r=0;
        int n=s.length();
        map<char,int> m;
        
        for(int i=0;i<n;i++)
            m[s[i]]=-1;
        int mx=INT_MIN;
        
        for(;r<n;)
        {
            if(m[s[r]]==-1)
            {   m[s[r]]=r;
                r++;   }
            else
            {   mx=max(mx,r-l);
             cout<<s[r]<<m[s[r]]<<" "<<l<<" "<<r<<endl;  
             for(int i=l;i<m[s[r]];i++)
                    m[s[i]]=-1;
                l=m[s[r]]+1;
                m[s[r]]=r;
                r++;
             
            }
        }   
        
        
        mx=max(mx,r-l);
            
            return mx;
        
        
        
        
    }
};


