# 1. Two Sum

**Difficulty:** Easy  
**Language:** C++  

#### *Problem Link*: [1. Two Sum](https://leetcode.com/problems/two-sum//)

## Performance
- **Runtime:** N/A
- **Memory:** N/A

## Solution
```cpp
class Solution {public:    vector<int> twoSum(vector<int>& nums, int target) {       unordered_map<int, int> mp;        for (int i = 0; i < nums.size(); i++) {            if (mp.find(target - nums[i]) != mp.end()) {                return {mp[target - nums[i]], i};            }            mp[nums[i]] = i;        }        return {};    }};
```

## Complexity Analysis

Time Complexity: O(n)
Space Complexity: O(n)

>  _Complexity estimated using AI (gemini)._



---
*Solution automatically synced by [GitSync](https://github.com/pramay88/GitSync) 🚀*
