# 4. Median of Two Sorted Arrays

**Difficulty:** 🟥 Hard  
**Language:** c++  

#### *Problem Link*: [4. Median of Two Sorted Arrays](https://leetcode.com/problems/median-of-two-sorted-arrays/)

## Performance
- **Runtime:** 31 ms (beats 5.56%)
- **Memory Usage:** 95.12 MB (beats 59.80%)

## Solution
```cpp
class Solution {
public:
    double findMedianSortedArrays(vector<int>& nums1, vector<int>& nums2) {
        vector<int> mergeV(nums1.size()+nums2.size());
        merge(nums1.begin(),nums1.end(),nums2.begin(),nums2.end(),mergeV.begin());
        int n=mergeV.size();
        double ans;
        if(n%2==0){
            ans= (double)(mergeV[(int)(n/2)-1]+mergeV[(int)(n/2)])/2;
        }
        else
            ans= mergeV[(n/2)];

        return ans;
        
    }
};
```

## Complexity Analysis (AI-Generated)  

Time Complexity: O(n log n)
Space Complexity: O(1)

> *Please analyze and update the complexity values above*



---
*Solution automatically synced by [GitSync](https://github.com/pramay88/GitSync) 🚀*
