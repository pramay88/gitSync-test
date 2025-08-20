# 4. Median of Two Sorted Arrays

**Difficulty:** Hard  
**Language:** Unknown  

#### *Problem Link*: [4. Median of Two Sorted Arrays](https://leetcode.com/problems/median-of-two-sorted-arrays/description//)

## Performance
- **Runtime:** N/A
- **Memory:** N/A

## Solution
```unknown
# If k is in the right half of A + B, remove the larger right half.             if a_index + b_index < k:                 if a_value > b_value:                     return solve(k, a_start, a_end, b_index + 1, b_end)                 else:                     return solve(k, a_index + 1, a_end, b_start, b_end)
```

## Complexity Analysis

Time Complexity: O(log(m+n))
Space Complexity: O(log(m+n))

>  _Complexity estimated using AI (gemini)._



---
*Solution automatically synced by [GitSync](https://github.com/pramay88/GitSync) 🚀*
