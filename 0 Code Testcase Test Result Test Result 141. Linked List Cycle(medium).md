## 1st code
### 2024/3/6

```python
# Definition for singly-linked list.
# class ListNode:
#     def __init__(self, x):
#         self.val = x
#         self.next = None

class Solution:
    def hasCycle(self, head: Optional[ListNode]) -> bool:
        if not head or not head.next:
            return False
        
        fastmove = head
        slowmove = head
        
        while fastmove.next and fastmove.next.next:
            fastmove = fastmove.next.next
            slowmove = slowmove.next

            if slowmove == fastmove:
                return True
        
        return False
```
