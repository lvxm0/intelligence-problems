# <center>Intelligence Problems</center>

intelligence problems for interviews.

### 水壶倒水

1. 无穷多的水
2. 5L 容器和 6L 容器

<details> <summary> 如何得到 3L 水？ </summary>

1. 倒满 6L 容器，然后全部倒到 5L 容器，6L 容器剩余 1L，5L 容器的水全部倒掉，将 6L 容器的 1L 倒到 5L 容器
    - 6L 容器: 0L
    - 5L 容器: 2L
2. 倒满 6L 容器，然后全部倒到 5L 容器，6L 容器剩余 2L（因为 5L 容器已经有 1L 了），5L 容器的水全部倒掉，将 6L 容器的 2L 倒到 5L 容器
    - 6L 容器: 0L
    - 5L 容器: 2L
3. 重复上述步骤，可得到 3L 的水

</details>

### 不足量的箱子

1. 10 箱黄金，每箱 100 块，每块一两。
2. 有贪官，把某一箱的每块都磨去一钱。

<details> <summary> 称一次找到不足量的那个箱子 </summary>

第一个箱子拿一块，第二个箱子拿两块，第 n 个箱子拿 n 块，最后缺了 n 钱就是第 n 个箱子

</details>

### 拿乒乓球

1. 排列着100个乒乓球
2. 两个人轮流拿球装入口袋
3. 能拿到第100个乒乓球的人为胜利者
4. 每次拿球者至少要拿1个，但最多不能超过5个

<details> <summary> 如果你是最先拿球的人，你该拿几个？以后怎么拿就能保证你能得到第100个乒乓球？ </summary>

1. 首先拿 4 个
2. 之后每次别人拿 n 个，你就拿 6 - n 个

</details>

### 时钟时针，分针，秒针重合

<details> <summary> 在一天的24小时之中，时钟的时针、分针和秒针完全重合在一起的时候有几次？ </summary>

2 次。一次 0 点，一次 12 点。

首先秒针是跳着走的，也就是一秒是 6 度，所以最后角度也要是 6 的倍数。

然后，时针角速度 w，则分针角速度 12w，秒针 720w。计算时针和分针重合时，秒针是否也重合就可以了。

时针和分针重合 12wt - wt = 2π，解得 t = 12/11 小时，同时可以得到，每 12 小时只会重合 11 次，此时时针的角度为 30x12/11xn, n=[0, 11]，秒针的角度为 360x60x12/11xn。计算可得只有当 n 为 0 或者 11 时，才会和秒针重合，因为秒针的。

</details>