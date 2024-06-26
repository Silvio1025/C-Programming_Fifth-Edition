# 例题

## 4.1 在例3.5的基础上对程序进行改进

题目要求:

* 解得 $ax^2+bx+c=0$ 方程的根。  
* 由键盘输入 a , b , c 。
* 假设 a , b , c 的值任意，并不保证 $b^2-4ac\geqslant 0$ 。
* 需要在程序中进行判别:
  * 如果 $b^2-4ac\geqslant 0$ ，就计算并输出方程的两个实根;
  * 如果 $b^2-4ac<0$ ，就输出“此方程无实根”的信息。

[4-1.c](c4-1.c)

## 4.2 输入两个实数，按由小到大的顺序输出这两个数

[4-2.c](c4-2.c)

## 4.3 输入3个数a，b，c，要求按由小到大的顺序输出

[4-3.c](c4-3.c)

## 4.4 输入一个字符，判别它是否为大写字母，如果是，将它转换成小写字母；如果不是，不转换。然后输出最后得到的字符

[4-4.c](c4-4.c)

## 4.5 有一阶跃函数

$$
y=\begin{cases}
-1&(x < 0)\\
0&(x = 0)\\
1&(x > 0)
\end{cases}
$$

编一程序,输入一个 $x$ 值，要求输出相应的 $y$ 值。

[4-5.c](c4-5.c)

## 4.6 要求按照考试成绩的等级输出百分制分数段

* A等为85分以上，
* B等为70～84分，
* C等为60～69分，
* D等为 60分以下。

成绩的等级由键盘输入。

[4-6.c](c4-6.c)

## 4.7 用switch语句处理菜单命令

在许多应用程序中，用菜单对流程进行控制。

* 例如从键盘输入一个′A′或′a′字符，就会执行A操作，
* 输入一个′B′或′b′字符，就会执行B操作。

[4-7.c](c4-7.c)

## 4.8 写一程序，判断某一年是否为闰年

[4-8-3.c](c4-8-3.c)

## 4.9 求 $ax^2+bx+c=0$ 方程的解

[4-9.c](c4-9.c)

## 4.10 运输公司对用户计算运输费用。路程越远，运费越低

标准如下:

```text
s < 250         没有折扣  
250≤s<500       2％折扣  
500≤s<1000      5％折扣  
1000≤s<2000     8％折扣  
2000≤s<3000     10％折扣  
3000≤s          15％折扣
```

[4-10.c](c4-10.c)
