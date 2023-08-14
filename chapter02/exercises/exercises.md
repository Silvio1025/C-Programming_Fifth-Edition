# 习题

## 1. 什么是算法？试从日常生活中找3个例子，描述它们的算法

- 算法：总体来说，算法是解决问题的方法和步骤。  
- 生活中的例子：
  - 报大学：首先填报志愿表、交报名费、拿到准考证、按时参加考试、收到录取通知书、按照日期到指定学校报到。  
  - 去北京听演唱会：首先在网上购票、然后按时坐车到北京，坐车到演唱会会场。
  - 把大象放进冰箱：先打开冰箱门，然后将大象放进冰箱，关冰箱。

## 2. 什么叫结构化的算法？为什么要提倡结构化的算法

- 由人们规定的几种基本结构按一定规律组成的算法就是结构化算法；
- 结构化算法限制了传统流程图中箭头的滥用，即不允许无规律地是流程随意转向，只能顺序地进行，提高了算法的质量，使算法的设计和阅读方便。

## 3. 试述3种基本结构的特点，请另外设计两种基本结构(要符合基类结构的特点)

- 结构化程序设计方法主要由以下三种基本结构组成：
  - 顺序结构：顺序结构是一种线性、有序的结构，它依次执行各语句模块
  - 选择结构：选择结构是根据条件成立与否选择程序执行的通路。
  - 循环结构：循环结构是重复执行一个或几个模块，直到满足某一条件位置。
  - 重新设计基本结构要满足以下几点：
    1. 只有一个入口
    2. 只有一个出口
    3. 结构内的每一部分都有机会执行到
    4. 结构内不存在死循环

## 4. 编写程序，求解以下问题

1. 有两个瓶子$A$和$B$，分别存放醋和酱油，要求将它们互换（即$A$瓶原来盛醋，现在用来盛酱油，$B$瓶则相反）。  
`xt4-4-1.c`
2. 依次输入$10$个数，要求输出其中最大的数。  
`xt4-4-2.c`
3. 有三个数$a$，$b$，$c$，要求按大小顺序输出。  
`xt4-4-3.c`
4. 求 $1$+$2$+$3$+$\dots$+$100$。  
`xt4-4-4.c`
5. 判断一个数 $n$ 能否同时被 $3$ 和 $5$ 整除。  
`xt4-4-5.c`
6. 将$100$ $\sim$ $200$之间的素数输出。  
`xt4-4-6.c`
7. 求两个数的 $m$ 和 $n$ 的最大公约数。  
`xt4-4-7.c`
8. 求方程 $ax^2+bx+c=0 $ 的根。分别考虑：$①$有两个不等的实根；$②$有两个相等的实根。  
`xt4-4-8.c`

## 8. 编写以下程序

1. 输出1900~2000年中是闰年的年份  
符合下面两个条件之一的年份是闰年：  
$①$能被 $4$ 整除但不能被 $100$ 整除；  
$②$能被 $100$ 整除且能被 $400$ 整除。  
`xt4-8-1.c`
2. 求 $ax²+bx+c=0$ 的根。  
`xt4-8-2.c`