# Algorithms & Data-Structures

## CORE CONTENT

### Resource

- [The Algorithms](https://the-algorithms.com/)
- [VisuAlgo](https://visualgo.net/zh)
- [Leetcode](https://leetcode.cn/)
- [MIT OpenSourceWare](https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-fall-2011/)

### Books

- [LeetCode 101 - A Grinding Guide.pdf](http://files.evmix.top/computer-science/algorithms-data-structures/LeetCode%20101%20-%20A%20Grinding%20Guide.pdf)
- [大话数据结构.pdf](http://files.evmix.top/computer-science/algorithms-data-structures/%E5%A4%A7%E8%AF%9D%E6%95%B0%E6%8D%AE%E7%BB%93%E6%9E%84.pdf)
- [真实世界的算法.pdf](http://files.evmix.top/computer-science/algorithms-data-structures/%E7%9C%9F%E5%AE%9E%E4%B8%96%E7%95%8C%E7%9A%84%E7%AE%97%E6%B3%95.pdf)
- [算法 4th.pdf](http://files.evmix.top/computer-science/algorithms-data-structures/%E7%AE%97%E6%B3%95%204th.pdf)
- [算法图解.pdf](http://files.evmix.top/computer-science/algorithms-data-structures/%E7%AE%97%E6%B3%95%E5%9B%BE%E8%A7%A3.pdf)
- [算法导论 2nd.pdf](http://files.evmix.top/computer-science/algorithms-data-structures/%E7%AE%97%E6%B3%95%E5%AF%BC%E8%AE%BA%202nd.pdf)
- [算法笔记.pdf](http://files.evmix.top/computer-science/algorithms-data-structures/%E7%AE%97%E6%B3%95%E7%AC%94%E8%AE%B0.pdf)
- [算法设计与分析.pdf](http://files.evmix.top/computer-science/algorithms-data-structures/%E7%AE%97%E6%B3%95%E8%AE%BE%E8%AE%A1%E4%B8%8E%E5%88%86%E6%9E%90.pdf)
- [编程珠玑 2nd.pdf](http://files.evmix.top/computer-science/algorithms-data-structures/%E7%BC%96%E7%A8%8B%E7%8F%A0%E7%8E%91%202nd.pdf)

### Data Structures Basic Concepts

#### Abstract Data Type

$\text{DataType = (D, O)}$

$\text{Example ADT: Stack}$
$D = \langle e_1, e_2, ..., e_n \rangle$
$O = \{\text{CreateStack, Push, Pop, Top, IsEmpty}\}$

#### Logical Structure

- Set structure
- Linear structure
- Tree structure
- Graph structure

#### Physical Storage Structure

- Sequential storage structure
- Linked storage structure
- Indexed storage structure
- Hash storage structure

### Algorithms Basic Concepts

#### Basic Characteristics

- 输入/输出
- 有穷性
- 确定性
- 可行性

#### Design Constraints

- 正确性
- 可读性
- 健壮性
- 时间效率高
- 空间占用低

#### Algorithm efficiency measurement

- 统计法
- 分析估算法

#### Time and space complexity / Big O

|Complexity |Name |Explain|Example|
|:-:|:-:|:-:|:-:|
|O(1) |常数|算法的执行时间不随输入规模的变化而变化|访问数组的特定元素|
|O(log n)|对数|算法的执行时间随着输入规模的对数增长|二分查找|
|O(n)|线性|算法的执行时间与输入规模成正比|遍历数组|
|O(n log n)|线性对数|通常出现在高效的排序算法中（如归并排序和快速排序的平均情况）|归并排序|
|O(n²)|平方|算法的执行时间与输入规模的平方成正比|冒泡排序、选择排序|
|O(n³)|立方|算法的执行时间与输入规模的立方成正比|三重嵌套循环的算法（如简单的矩乘法）|
|O(2^n)|指数|算法的执行时间随着输入规模以指数级增长|斐波那契数列的递归计算|
|O(n!)|阶乘|算法的执行时间随着输入规模的阶乘增长，通常出现在组合问题中|生成所有可能的排列|

## Practice

### Foundation

#### Basic Structures

| **数据结构**    | **关键操作**              | **应用场景**             | **推荐练习**         |
| --------------- | ------------------------- | ------------------------ | -------------------- |
| Array           | 访问、插入、删除、遍历    | 基础操作，排序、滑动窗口 | LeetCode 1, 27       |
| Linked List     | 单链表/双链表             | 插入/删除灵活            | LeetCode 206, 141    |
| Stack           | Push/Pop/Top/IsEmpty      | DFS、括号匹配、递归模拟  | LeetCode 20, 155     |
| Queue           | Enqueue/Dequeue           | BFS、任务调度            | LeetCode 225, 207    |
| Deque           | 双端操作                  | 滑动窗口、缓存           | LeetCode 239         |
| String          | KMP, Rabin-Karp, Manacher | 模式匹配、最长回文       | LeetCode 28, 5       |
| Hash-Structures | 插入、查找、删除          | 高效集合表示             | LeetCode 1, 349, 380 |

#### Sorting Algorithms

- O(n log n)
    - Quick-Sort
    - Merge-Sort
    - Heap-Sort
- O(n)
    - Radix-Sort
    - Counting-Sort
    - Bucket-Sort
- O(n²)
    - Shell-Sort
    - Selection-Sort
    - Insertion-Sort
    - Bubble-Sort
- Practical
    - Tim Sort
    - Intro Sort

#### Search Algorithms

- Linear Search
- Binary Search

### Problem-Solving Techniques

| Iteration           | 循环遍历     | 基础数组/链表操作            |
| ------------------- | ------------ | ---------------------------- |
| Recursion           | 自身调用     | DFS, 递归问题                |
| Brute-Force         | 枚举所有可能 | 全排列、子集                 |
| Divide & Conquer    | 分而治之     | MergeSort, QuickSort         |
| Sliding Window      | 可变窗口     | 最小覆盖子串、最长无重复子串 |
| Two-Pointer         | 双指针       | 有序数组双指针, 快慢指针     |
| Greedy              | 贪心选择     | 区间调度、最小硬币找零       |
| Dynamic Programming | 状态转移     | 背包、最长上升子序列         |
| Backtracking        | 回溯搜索     | N皇后、解数独                |
| Branch & Bound      | 剪枝搜索     | 旅行商、分支限界             |
| Randomized          | 随机化算法   | QuickSelect, 随机哈希        |

> ⚡提示：学习顺序可以先掌握迭代/递归和简单暴力，再学分治与滑动窗口，再到贪心、DP和回溯。

### Intermediate

| **数据结构**      | **关键操作/特性** | **应用场景**         | **推荐练习**      |
| ----------------- | ----------------- | -------------------- | ----------------- |
| Binary Tree / BST | 插入/删除/查找    | DFS/BFS, 排序        | LeetCode 94, 98   |
| Heap (Min/Max)    | Insert, Extract   | 优先队列、Top-K问题  | LeetCode 215, 703 |
| Graph             | 邻接表/邻接矩阵   | DFS/BFS、最短路、MST | LeetCode 207, 743 |
| Union-Find        | 并查集操作        | 连通性、Kruskal MST  | LeetCode 200, 547 |

### Advanced

| **结构**                          | **特性/用途**        | **典型应用**       |
| --------------------------------- | -------------------- | ------------------ |
| Segment Tree / Fenwick Tree       | 区间查询/更新        | 区间和、区间最大值 |
| Trie / Suffix Tree / Suffix Array | 字符串索引           | 字典匹配、子串搜索 |
| Balanced Tree (AVL, Splay, 2-3)   | 平衡查询             | 高效查找/索引      |
| ISAM / B+ Tree                    | 索引顺序存储         | 数据库、文件系统   |
| Bloom Filter                      | 空间效率高、允许误判 | 缓存判重、网络爬虫 |
| LRU Cache / Skip List             | 高效缓存 / 排序      | 缓存系统、快速查找 |

## Specialize

| **应用**      | **算法/结构**        | **场景**               |
| ------------- | -------------------- | ---------------------- |
| AI / ML       | Tensor运算、多维数组 | 神经网络、图神经网络   |
| Cryptography  | RSA, AES, ECC        | 信息安全、加密通信     |
| 高维/概率结构 | Bitmap, Bloom Filter | 数据库、集合判重、缓存 |
