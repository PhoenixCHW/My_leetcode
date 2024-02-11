## 1st code
### 2024/2/11
![image](https://github.com/PhoenixCHW/My_leetcode/assets/39382795/b875cf9e-f5ca-4ae9-98cb-9c9f1dca1afe)


```python3
class Solution:
    def alternateDigitSum(self, n: int) -> int:
        ans = 0
        nStr = str(n)
        for i in range(len(nStr)):
            if i % 2 == 0:
                ans += int(nStr[i])
            else:
                ans -= int(nStr[i])
        return ans
```
