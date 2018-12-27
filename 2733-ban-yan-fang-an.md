# 2733 扮演方案

## 题目描述

FJ 有 $$n$$ 头奶牛，第 $$i$$ 头奶牛的体重是 $$w_i$$。现在 FJ 要把这 $$n$$ 头奶牛分成两堆，扮演警察和小偷的游戏。每头奶牛要么扮演警察要么扮演小偷。扮演警察的至少要有一头奶牛，扮演小偷的奶牛也至少要有一头。扮演警察的所有奶牛聚在一起，会产生一个“合作指数”，“合作指数”的值是所有扮演警察的奶牛的体重按照二进制数展开后，再进行二进制 $$\operatorname{and}$$ 操作的结果。同样，扮演小偷的奶牛们也有“合作指数”，也是同样的计算方法。为了使得游戏好玩，FJ 决定，扮演警察的奶牛的“合作指数”和扮演小偷的奶牛的“合作指数”要相等。

问题是：有多少种“不同的扮演方案”？

下面定义不同的“扮演方案”，假设 A、B 是两种扮演方案，如果至少存在一头奶牛（不妨假设是奶牛 X），奶牛 X 在方案 A 中扮演的角色和在方案 B 中扮演的角色不同，那么方案 A 和方案 B 就是不同的方案。

## 输入格式

多组测试数据。

一个行，一个整数 $$r$$。

每组测试数据格式如下：

第一行，一个整数 $$n$$。

第二行，$$n$$ 个整数，第 $$i$$ 个整数表示 $$w_i$$。

## 输出格式

一个整数。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
3
4
1 2 3 4
5
1 2 3 4 5
3
6 6 6
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
2
8
6
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 样例解释

第 1 组测试数据解释：

1. 奶牛 1 和奶牛 2 扮演警察，奶牛 3 和奶牛 4 扮演小偷。
2. 奶牛 1 和奶牛 2 扮演小偷，奶牛 3 和奶牛 4 扮演警察。

## 数据范围

$$1 \leq r \leq 5$$，$$1 \leq n \leq 50$$，$$0 \leq w_i \leq 2^{20}-1$$。
