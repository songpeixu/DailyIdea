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

注意到`list(zip(*matrix))[::-1]`的用法，`zip`获取tuple，`*`有转置功能，再配合`[::-1]`，对矩阵进行了逆时针旋转90°的操作


###### 新威电池实验
- 如何将SOC作为充放电阶段结束的判定条件
- 如何使用恒温箱
- 对所有通道执行相同的启动操作
- 如何更合理的使用保存下来的数据
- 了解数据的存储位置
