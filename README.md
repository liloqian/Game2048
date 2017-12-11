# Game2048

---

> 大学期间这个游戏每个人都应该玩过一段时间，简单但是好玩
> 《Android群英传》一书最后就是这个例子，看了下源码简单做个总结

---

作者源码： [https://github.com/xuyisheng/AndroidHeroes/tree/master/13.%E5%AE%9E%E4%BE%8B%E6%8F%90%E9%AB%98/Game2048](https://github.com/xuyisheng/AndroidHeroes/tree/master/13.%E5%AE%9E%E4%BE%8B%E6%8F%90%E9%AB%98/Game2048)

![](https://i.imgur.com/KwsDEnh.png)

![](https://i.imgur.com/BJy4Vai.png)

## 基本流程

![](https://i.imgur.com/QLhooQP.png)

### 第一步： 每次开始刷新出来2个随机位置的数字，2或者4
### 第二步： 玩家可以上下左右滑动，玩家滑动后需要做处理
####	2.1判断上下左右那个方向做相应的处理，下面会举一个向右滑动的情况来介绍，因为不同方向的滑动算法不一样
####    2.2每次滑动后要增加一个新的数字
####    2.3判断游戏是否结束（达到目标或者失败），还是继续


![](https://i.imgur.com/Jl30758.png)

> 如果左右滑动就一行一行进行处理，上下滑动就一列一列处理
向那边滑动从那边开始遍历

