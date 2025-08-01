# 第一章：绪论

## 1.1 数据结构的基本概念

![Alt text](image.png)

### 1.2_1 算法的基本概念

![Alt text](image-1.png)

### 1.2_2 算法的时间复杂度

![Alt text](image-2.png)

### 1.2_3 算法的空间复杂度

![Alt text](image-3.png)

# 第二章：线性表

## 2.1 线性表的定义和基本操作

![Alt text](image-4.png)

### 2.2_1 顺序表的定义

![Alt text](image-5.png)

#### 2.2_1_1 顺序表的插入删除

![Alt text](image-6.png)

#### 2.2_1_2 顺序表的查找

![Alt text](image-7.png)

### 2.3.1 单链表的定义

![Alt text](image-8.png)

### 2.3.2_1 单链表的插入删除

![Alt text](image-9.png)

### 2.3.2_2 单链表的查找

![Alt text](image-10.png)

### 2.3.2_3 单链表的建立

头插法、尾插法：核心就是初始化操作、指定结点的后插操作

### 2.3.3 双链表

![Alt text](image-11.png)

### 2.3.4 循环链表

![Alt text](image-12.png)

### 2.3.5 静态链表

![Alt text](image-13.png)

### 2.3.6 顺序表和链表的比较

![Alt text](image-14.png)

# 第三章：栈、队列和数组

### 3.1.1 栈的基本概念

![Alt text](image-15.png)

### 3.1.2 栈的顺序存储实现

![Alt text](image-16.png)

### 3.1.3 栈的链式存储实现

![Alt text](image-17.png)

### 3.2.1 队列的基本概念

![Alt text](image-18.png)

### 3.2.2 队列的顺序存储实现

![Alt text](image-19.png)

### 3.2.3 队列的链式存储实现

![Alt text](image-20.png)

### 3.2.4 双端队列

![Alt text](image-21.png)

### 3.3.1 栈在括号匹配中的应用

用栈实现括号匹配：
依次扫描所有字符，遇到左括号入栈，遇到右括号则弹出栈顶元素检
查是否匹配。
匹配失败情况：
① 左括号单身 ② 右括号单身 ③ 左右括号不匹配

### 3.3.2 栈在表达式求值中的应用

![Alt text](image-22.png)
![Alt text](image-23.png)

### 3.3.3 栈在递归中的应用

函数调用的特点：最后被调用的函数最先执行结束
函数调用时，需要用一个“函数调用栈” 存储：
① 调用返回地址
② 实参
③ 局部变量

### 3.3.4 队列的应用

树的层次遍历
图的广度优先搜索
多个进程争抢着使用有限的系统资源时，FCFS（First Come First Service，先来先服务）是一种常用策略

## 3.4 数组和特殊矩阵

![Alt text](image-24.png)

# 第四章：串

## 4.1 串的定义和实现

### 4.1.1 串的定义和基本操作

![Alt text](image-25.png)

### 4.1.2 串的存储结构

![Alt text](image-26.png)

## 4.2 串的模式匹配

### 4.2.1 朴素模式匹配算法

![Alt text](image-27.png)

#### 4.2.2.1 KMP 算法

#### 4.2.2.2 手算 next 数组

### 4.2.3 KMP 算法的进一步优化

# 第五章：树与二叉树

## 5.1 树的基本概念

### 5.1.1 树的定义和基本术语

![Alt text](image-28.png)

### 5.1.2 树的性质

![Alt text](image-29.png)

## 5.2 二叉树的概念

#### 5.2.1_1 二叉树的定义和基本术语

![Alt text](image-30.png)

#### 5.2.1_2 二叉树的性质

![Alt text](image-31.png)

### 5.2.2 二叉树的存储结构

![Alt text](image-32.png)
![Alt text](image-33.png)

## 5.3 二叉树的遍历和线索二叉树

### 5.3.1 二叉树的遍历

#### 5.3.1_1 二叉树的先序、中序、后序遍历

![Alt text](image-34.png)

#### 5.3.1_2 二叉树的层次遍历

树的层次遍历算法思想：
① 初始化一个辅助队列
② 根结点入队
③ 若队列非空，则队头结点出队，访问该结点，并将其左、右孩子插入队尾（如果有的话）
④ 重复 ③ 直至队列为空

#### 5.3.1_3 由遍历序列构造二叉树

![Alt text](image-35.png)

### 5.3.2 线索二叉树

#### 5.3.2_1 线索二叉树的概念

![Alt text](image-36.png)

#### 5.3.2_2 二叉树的线索化

![Alt text](image-37.png)

#### 5.3.2_3 在线索二叉树中找前驱后继

![Alt text](image-38.png)

## 5.4 树、森林

### 5.4.1 树的存储结构

![Alt text](image-40.png)

### 5.4.2 树、森林与二叉树的转换

![Alt text](image-41.png)

### 5.4.3 树和森林的遍历

![Alt text](image-42.png)

## 5.5 树和二叉树的应用

### 5.5.1 哈夫曼树

![Alt text](image-45.png)

#### 5.5.2_1 并查集

![Alt text](image-46.png)

#### 5.5.2_2 并查集的进一步优化

![Alt text](image-47.png)

# 第六章：图

## 6.1 图的基本概念

![Alt text](image-48.png)

## 6.2 图的存储

### 6.2.1 图的邻接矩阵

![Alt text](image-49.png)

### 6.2.2 图的邻接表

![Alt text](image-50.png)

### 6.2.3 十字链表、邻接多重表

![Alt text](image-51.png)

### 6.2.4 图的基本操作

![Alt text](image-52.png)

## 6.3 图的遍历

### 6.3.1 图的广度优先搜索

![Alt text](image-53.png)

### 6.3.2 图的深度优先搜索

![Alt text](image-54.png)

## 6.4 图的应用

### 6.4.1 最小生成树

![Alt text](image-55.png)

### 6.4.2 最短路径问题

#### 6.4.2_1 最短路径问题——BFS 算法

![Alt text](image-56.png)

#### 6.4.2_2 最短路径问题——Dijkstra 算法

#### 6.4.2_3 最短路径问题——Floyd 算法

![Alt text](image-57.png)

### 6.4.3 有向无环图描述表达式

### 6.4.4 拓扑排序

![Alt text](image-58.png)

### 6.4.5 关键路径

![Alt text](image-59.png)
