## 1st code
### 2024/2/11
![image](https://github.com/PhoenixCHW/My_leetcode/assets/39382795/dfd7300e-1ceb-41f0-b64a-c0dc220e1239)

```python3
class Solution:
    def constructRectangle(self, area: int) -> List[int]:
        import math
        MM = int(math.sqrt(area))
        ansList = []
        for i in range(1,MM+1):
            if area / i == area // i:
                ansList.append([(i + area / i),[area //i , i]])
        return ansList[-1][1]


```
