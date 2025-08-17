# 第一章：计算机系统概述

## 1.1 操作系统的基本概念

![Alt text](image.png)
![Alt text](image-1.png)

## 1.2 操作系统的发展与分类

![Alt text](image-2.png)

## 1.3 操作系统运行环境

### 1.3.1 操作系统的运行机制

![Alt text](image-3.png)

### 1.3.2 中断与异常

![Alt text](image-4.png)

### 1.3.3 系统调用

![Alt text](image-5.png)

## 1.4 操作系统结构

![Alt text](image-6.png)
![Alt text](image-7.png)

## 1.5 操作系统引导

![Alt text](image-8.png)

## 1.6 虚拟机

![Alt text](image-9.png)

# 第二章：进程与线程

## 2.1 进程与线程

### 2.1.1 2.1.2 进程的概念、组成与特征

![Alt text](image-10.png)

### 2.1.3 线程的状态与转换

![Alt text](image-12.png)

### 2.1.4 进程控制

![Alt text](image-13.png)
![Alt text](image-14.png)
![Alt text](image-15.png)
![Alt text](image-16.png)
![Alt text](image-17.png)

### 2.1.5 进程通信

![Alt text](image-18.png)
![Alt text](image-19.png)

### 2.1.6 线程的概念与特点

![Alt text](image-20.png)
![Alt text](image-21.png)
![Alt text](image-22.png)
![Alt text](image-23.png)
![Alt text](image-24.png)

## 2.2 CPU 调度

### 2.2.1 调度的概念、层次

![Alt text](image-25.png)
![Alt text](image-26.png)

### 2.2.4 进程调度的时机、切换与过程、方式

![Alt text](image-27.png)

### 2.2.3 调度算法的评价指标

![Alt text](image-28.png)

### 2.2.5 进程调度算法

#### 先来先服务算法

![Alt text](image-30.png)

#### 短作业优先算法

![Alt text](image-31.png)

#### 高响应比优先算法

![Alt text](image-32.png)

#### 时间片轮转算法

![Alt text](image-33.png)

#### 优先级调度算法

![Alt text](image-34.png)

#### 多级反馈队列算法

![Alt text](image-35.png)

#### 多级队列调度算法

![Alt text](image-36.png)

### 2.2.6 多处理机调度

![Alt text](image-37.png)

## 2.3 同步与互斥

### 2.3.1 同步和互斥的基本概念

![Alt text](image-38.png)

### 2.3.2 进程控制的实现方法

![Alt text](image-39.png)
![Alt text](image-40.png)

### 2.3.3 互斥锁

### 2.3.4 信号量

![Alt text](image-41.png)
![Alt text](image-42.png)

### 2.3.5 信号量的典型问题

### 2.3.6 管程

![Alt text](image-43.png)

## 2.4 死锁

### 2.4.1 死锁的概念

![Alt text](image-44.png)

### 2.4.2 死锁的预防

![Alt text](image-45.png)

### 2.4.3 死锁的避免

数据结构：
长度为 m 的一维数组 Available 表示还有多少可用资源
n _ m 矩阵 Max 表示各进程对资源的最大需求数
n _ m 矩阵 Allocation 表示已经给各进程分配了多少资源
Max – Allocation = Need 矩阵表示各进程最多还需要多少资源
用长度为 m 的一位数组 Request 表示进程此次申请的各种资源数
银行家算法步骤：
① 检查此次申请是否超过了之前声明的最大需求数
② 检查此时系统剩余的可用资源是否还能满足这次请求
③ 试探着分配，更改各数据结构
④ 用安全性算法检查此次分配是否会导致系统进入不安全状态
安全性算法步骤：
检查当前的剩余可用资源是否能满足某个进程的最大需求，如果可以，就把该进程加入安全序列，
并把该进程持有的资源全部回收。
不断重复上述过程，看最终是否能让所有进程都加入安全序列。
系统处于不安全状态未必死锁，但死锁时一定处于不安全状态。系统处于安全状态一定不会死锁。

### 2.4.4 死锁的检测与恢复

![Alt text](image-46.png)

# 第三章：内存管理

## 3.1 内存管理概念

### 3.1.1 内存管理的基础知识

![Alt text](image-47.png)
![Alt text](image-48.png)
![Alt text](image-49.png)
![Alt text](image-50.png)

### 3.1.2 连续分配管理方式

![Alt text](image-51.png)
![Alt text](image-52.png)

### 3.1.3 分页管理方式

![Alt text](image-53.png)
![Alt text](image-54.png)
![Alt text](image-55.png)
![Alt text](image-56.png)

### 3.1.4 分段管理方式

![Alt text](image-57.png)

### 3.1.5 段页式管理方式

![Alt text](image-58.png)

## 3.2 虚拟内存管理

### 3.2.1 虚拟内存的基本概念

![Alt text](image-59.png)

### 3.2.2 请求分页管理方式

![Alt text](image-60.png)

### 3.2.4 页面置换算法

![Alt text](image-61.png)

### 3.2.5 页面分配策略

![Alt text](image-62.png)

### 3.2.6 内存映射文件

![Alt text](image-63.png)

# 第四章：文件管理

## 4.1 文件系统基础

### 4.1.1 初识文件系统

![Alt text](image-64.png)

### 4.1.2 文件的逻辑结构

![Alt text](image-65.png)

### 4.1.3 文件目录

![Alt text](image-66.png)

### 4.1.4 文件的物理结构

![Alt text](image-67.png)

### 4.1.5 逻辑结构 VS 物理结构

![Alt text](image-68.png)

### 4.1.6 文件存储空间管理

![Alt text](image-69.png)

### 4.1.7 文件的基本操作

![Alt text](image-70.png)

### 4.1.8 文件共享

![Alt text](image-71.png)

### 4.1.9 文件保护

![Alt text](image-72.png)

## 4.3 文件系统

### 4.3.1 文件系统的层次结构

![Alt text](image-73.png)

### 4.3.2 文件系统布局

![Alt text](image-74.png)

### 4.3.3 虚拟文件系统

![Alt text](image-75.png)
![Alt text](image-76.png)
