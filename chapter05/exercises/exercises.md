# 习题

## 1. 请画出例5.6中给出的3个程序段的流程图

    - 流程图1：

        ![img](https://s2.51cto.com/images/blog/202210/13111908_634783ac28d3858974.png)

    - 流程图2：

        ![img](https://s2.51cto.com/images/blog/202210/13111908_634783ac4681c68262.png)

    - 流程图3：

        ![img](https://s2.51cto.com/images/blog/202210/13111908_634783ac719f245090.png)

## 2. 请补充 $例5.7$ 程序,分别统计当 $“fabs(t)\geqslant 1e- 6”和“fabs(t)\geqslant 1e- 8”$ 时执行循环体的次数

`xt5-2.c`

## 3. 输人两个正整数 $m$ 和 $n$,求其最大公约数和最小公倍数

`xt5-3.c`

## 4. 输人一行字符,分别统计出其中英文字母、空格、数字和其他字符的个数

`xt5-4.c`

## 5. 求 $S_n=a+aa+aaa+\cdots+\overbrace{a\cdots aa}^{n个a}$的值，其中 $a$ 是一个数字，$n$ 表示 $a$ 的位数，例如：$2+22+222+2222+22222 (此时n=5)$ $n$ 由键盘键入

`xt5-5.c`

## 6. 求$\sum\limits_{n=1}^{20}n!$

`xt5-6.c`

## 7. 求$\sum\limits_{k=1}^{100}k+\sum\limits_{k=1}^{50}k^2+\sum\limits_{k=1}^{10}\frac1k$

`xt5-7.c`

## 8. 输出所有的“水仙花数”,所谓“水仙花数”是指一个 $3$ 位数,其各位数字立方和等于该数本身。例如 $153$ 是水仙花数,因为 $153=1^3+5^3+3^3$

## 9. 编程序找出 $1000$ 之内的所有完数,并按下面格式输出其因子

    6 its factors are 1,2,3

一个数如果恰好等于它的因子之和,这个数就称为“完数”。
例如,6的因子为1,2,3,而6=1+2+3,因此6是“完数”。

`xt5-9-1.c`

`xt5-9-2.c`

## 10. 有一个分数序列 $\frac21,\frac32,\frac53,\frac85,\frac{13}8,\frac{25}{13}\dots$求出这个数列的前20项之和

`xt5-10.c`

## 11. 一个球从 $100m$ 高度自由落下，每次落地后反弹回原高度的一半，再落下，再反弹。求它在第 $10$ 次落地时共经过多少米,第 $10$ 次反弹多高

`xt5-11.c`

## 12. 猴子吃桃问题

    猴子第1天摘下若干个桃子，当即吃了一半，还不过瘾，又多吃了一个。
    第2天早上又将剩下的桃子吃掉一半，又多吃了一个。
    以后每天早上都吃了前一天剩下的一半零一个。
    到第10天早上想再吃时，就只剩一个桃子了。求第1天共摘多少个桃子。

`xt5-12.c`

## 13. 用迭代法求 $x=\sqrt a$

求平方根的迭代公式为:
$$X_{n+1}=\frac12\times (X_n + \frac a{X_n})$$
要求前后两次求出的x的差的绝对值小于 $10^{-5}$。

- 算法1：

    1. 选一个方程的近似根，赋给变量 $x_0$；
    2. 将 $x_0$ 的值保存于变量 $x_1$ ，然后计算 $g(x_1)$ ，并将结果存于变量 $x_0$；
    3. 当 $x_0$ 与 $x_1$ 的差的绝对值还小于指定的精度要求时，重复步骤⑵的计算。
    若方程有根，并且用上述方法计算出来的近似根序列收敛，则按上述方法求得的 $x_0$ 就认为是方程的根。

    `xt5-13.c`
- 算法2：

    1. 先自定一个初值x0，作为a的平方根值，在我们的程序中取a/2作为x0的初值；
    利用迭代公式求出一个x1。此值与真正的a的平方根值相比，误差很大。
    2. 把新求得的x1代入x0中，准备用此新的x0再去求出一个新的x1。
    3. 利用迭代公式再求出一个新的x1的值，也就是用新的x0又求出一个新的平方根值x1，此值将更趋近于真正的平方根值。
    4. 比较前后两次求得的平方根值x0和x1，
    如果它们的差值小于我们指定的值，即达到我们要求的精度，
    则认为x1就是a的平方根值，去执行步骤5；
    否则执行步骤2，即循环进行迭代。

    `xt5-13-2.c`

## 14. 用牛顿迭代法求下面方程在 $1.5$ 附近的根：$2x^3-4x^2+3x-6=0$

- 基本公式：
    $$
    X_{n+1}=X_n-\frac{f(X_n)}{f'(X_n)}
    $$
  其中 $X_{n+1}$ 为第 $n+1$ 次迭代结果，$X_n$ 为第 $n$ 次迭代结果，$f'(X_n)$ 为 $f(X_n)$ 的导函数值。

- 算法：
    1. 把方程改写为多项式f(x)=2x^3-4x^2+3x-6，给定初值X0；
    2. 将Xn带入迭代公式Xn+1=Xn-f(Xn)/f (Xn)，求出Xn+1
    3. 判断精度fabs(Xn+1-Xn)是否达到要求，满足则输出，否则返回上一步

    `xt5-14-1.c`

    `xt5-14-2.c`

## 15. 用二分法求下面方程在$(-10,10)$ 之间的根:$2x^3-4x^2+3x-6=0$

- 定义：对于区间 $[a，b]$ 上连续不断且 $f(a)·f(b)<0$ 的函数 $y=f(x)$ ，通过不断地把函数 $f(x)$ 的零点所在的区间一分为二，使区间的两个端点逐步逼近零点，进而得到零点近似值的方法叫二分法。

    `xt5-15-1.c`

    `xt5-15-2.c`

    `xt5-15-3.c`

## 16. 输出以下图案

       *
      ***
     *****
    *******
     *****
      ***
       *

`xt5-16.c`

## 17. 两个乒乓球队进行比赛，各出3人。甲队为A，B，C 3人，乙队为X，Y，Z 3人。已抽签决定比赛名单。有人向队员打听比赛的名单，A说他不和X比，C说他不和X，Z比，请编程序找出3对赛手的名单

`xt5-17.c`