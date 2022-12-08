https://leetcode.com/problems/two-sum/description/

## python 
```python
  class Solution:
    def twoSum(self, nums: List[int], target: int) -> List[int]: 
      seen = {}
      for i, v in enumerate(nums):
        reamining = target - v
        if reamining in seen : 
          return [seen[remaning] ,i]
         seen[v] = i 
      return []    
```

- Runtime: 58 ms 
- O(n) 

