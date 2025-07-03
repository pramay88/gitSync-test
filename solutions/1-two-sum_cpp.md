# 1. Two Sum

**Difficulty:** [object Object]  
**Language:** c++  
**Date Solved:** July 4, 2025

## Problem Link
[1. Two Sum](https://leetcode.com/problems/two-sum/submissions/1685407888/)

## Performance
- **Runtime:** 0 ms (beats 100.00%)
- **Memory Usage:** 14.96 MB (beats 21.56%)

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
