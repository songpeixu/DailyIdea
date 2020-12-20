# DailyIdea

record daily idea

```
class Solution:
    def spiralOrder(self, matrix: List[List[int]]) -> List[int]:
        res = []
        while matrix:
            res += matrix.pop(0)
            matrix = list(zip(*matrix))[::-1]
        return res
```

注意到`list(zip(*matrix))[::-1]`的用法，`zip`获取tuple，\*\有转置功能，再配合`[::-1]`，对矩阵进行了逆时针旋转90°的操作
