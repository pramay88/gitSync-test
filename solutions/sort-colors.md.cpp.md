# Sort Colors

**Difficulty:** Medium  
**Language:** c++  
**Date Solved:** July 2, 2025

## Problem Link
[Sort Colors](https://leetcode.com/problems/sort-colors/submissions/1683171127/)

## Performance
- **Runtime:** 3 ms (beats 2.94%)
- **Memory Usage:** 11.66 MB (beats 49.04%)

## Solution
```cpp
class Solution {
public:
    void sortColors(vector<int>& nums) {
        int j = 0, i = 0, k = nums.size() - 1;
        while(i <= k){
            if(nums[i] == 0)
                swap(nums[i++], nums[j++]);
            else if(nums[i] == 2)
                swap(nums[i], nums[k--]);
            else i++;
        }
    }
};
```

## Complexity Analysis
- **Time Complexity:** O(?)
- **Space Complexity:** O(?)

> *Please analyze and update the complexity values above*

## Approach
<!-- Describe your approach here -->

## Key Insights
<!-- Add key insights or lessons learned -->

---
*Solution automatically synced by [LeetCode Git Pusher](https://github.com) 🚀*
