## Problem Record

**1. Problem Name & Number**

- 49. Group Anagrams
    

**2. Simple Illustration (Problem in Plain Words)**

- Group words that are anagrams into lists.
    
- Example: `["eat","tea","tan","ate","nat","bat"]` → `[["eat","tea","ate"],["tan","nat"],["bat"]]`
    

**3. Crude / First Solution (Optional)**

- Sort each string, use sorted version as key in hashmap.
    
- Time: `O(m * n log n)` where `m = number of words`, `n = avg length`.
    
- Space: `O(m * n)`.
    

**4. Optimal Solution**

- Count letters in each word using array of size 26. Use tuple(count) as key in hashmap.
    
- Time: `O(m * n)`
    
- Space: `O(m * n)`
    

**5. Code (Optimal)**

```python
from collections import defaultdict

class Solution:
    def groupAnagrams(self, strs: List[str]) -> List[List[str]]:
        res = defaultdict(list)
        for s in strs:
            count = [0] * 26
            for c in s:
                count[ord(c) - ord('a')] += 1
            res[tuple(count)].append(s)
        return list(res.values())
```

**6. Edge Cases / Variants**

- Empty input → `[]`
    
- Single word → `[[word]]`
    
- Repeated words → grouped together
    

**7. Patterns & Concepts Used**

- Hashing
    
- Arrays as fixed-size keys
    

**8. Self-Check / Review Notes**

- Understood tradeoff: sorting vs fixed-length key.
    
- Remember to wrap `res.values()` in `list()`.
    
- Next time: re-derive frequency count idea without hints.