## 1st code
### 2024/3/9
![image](https://github.com/PhoenixCHW/My_leetcode/assets/39382795/2133d638-9133-45ab-9c7b-3d88965a85a9)
```python3
class Solution:
    def getCommon(self, nums1: List[int], nums2: List[int]) -> int:
        return (len(list(set(nums1) & set(nums2))) and min(list(set(nums1) & set(nums2)))) or -1
```
