Binary search to get lowest average within array

https://leetcode.com/problems/koko-eating-bananas/
https://leetcode.com/problems/capacity-to-ship-packages-within-d-days/


```python

hi = max(arr) or sum(array
lo = 1 or max(array)
boundary_idx = - 1
curr = 0 
while lo <= hi:
  mid = (lo + hi) // 2
  _sum = 0 
  iterate w/i over array
    _sum += array[i] 
  if _sum gets to target condition:
    #target increase or decrease
  if target <= hi:
    boundary_idx = mid
    hi = mid - 1
  else:
    lowest = mid + 1

```

Find peak element in rotated sorted

```

#find peak element
l, r = 0, len(nums) - 1
boundary_idx = r 
while l < r:
    m = (l + r) // 2
    if m != 0 and m != len(nums) - 1 and nums[m - 1] >= nums[m] <= nums[m + 1]:
        boundary_idx = m
        break
    if nums[m] >= nums[l] and nums[m] <= nums[r]:
        r = m - 1
        boundary_idx = r
    elif nums[l] >= nums[m] and nums[m] <= nums[r]:
        r = m - 1
        boundary_idx = r
    else:
        l = m + 1

```
