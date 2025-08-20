# 4. Median of Two Sorted Arrays

**Difficulty:** Hard  
**Language:** C++  

#### *Problem Link*: [4. Median of Two Sorted Arrays](https://leetcode.com/problems/median-of-two-sorted-arrays/description//)

## Performance
- **Runtime:** N/A
- **Memory:** N/A

## Solution
```cpp
class Solution {public:    double findMedianSortedArrays(vector<int>& nums1, vector<int>& nums2) {        std::vector<int> nums;        for(auto n: nums1)            nums.push_back(n);        for(auto n: nums2)            nums.push_back(n);        std::sort(nums.begin(), nums.end());        double m{0};        if(!nums.empty())        {            if(nums.size() % 2 == 0) {                double d1 = nums[nums.size() / 2 - 1];                 double d2 = nums[nums.size() / 2];                m = (d1 + d2)/2;                   } else                 m = nums[nums.size() / 2];        }        return m;
```

## Complexity Analysis

Time Complexity: O(n log n)
Space Complexity: O(n)

>  _Complexity estimated using AI (gemini)._



---
*Solution automatically synced by [GitSync](https://github.com/pramay88/GitSync) 🚀*
