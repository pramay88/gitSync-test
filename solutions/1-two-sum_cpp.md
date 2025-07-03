# 1. Two Sum

**Difficulty:** [object Object]  
**Language:** c++  
**Date Solved:** July 4, 2025

## Problem Link
[1. Two Sum](https://leetcode.com/problems/two-sum/submissions/1685379670/)

## Performance
- **Runtime:** 3 ms (beats 71.03%)
- **Memory Usage:** 14.87 MB (beats 37.11%)

## Solution
```cpp
class Solution {
public:
    vector<int> twoSum(vector<int>& nums, int target) {
       unordered_map<int, int> mp;
        for (int i = 0; i < nums.size(); i++) {
            if (mp.find(target - nums[i]) != mp.end()) {
                return {mp[target - nums[i]], i};
            }
            mp[nums[i]] = i;
        }
        return {};
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
