# 2965 小Y的序列

## 题目描述

小 Y 有一个长度为 $$n$$ 的序列 $$a$$，现在有两种操作：

1. 输入两个整数 $$l,\,r$$，将序列 $$a$$ 的第 $$l$$ 位到第 $$r$$ 位循环右移一位。
2. 输入三个整数 $$l,\,r,\,x$$，询问区间 $$l$$ 到 $$r$$ 中有多少个数等于 $$x$$。

## 输入格式

第一行两个整数 $$n,\,q$$。

第二行 $$n$$ 个整数，表示序列 $$a$$。

接下来 $$q$$ 行每行一个操作。

若为第一种操作，则格式为 `1 p q`，其中 `l = 1 + (lastans + p - 1) mod n`，`r = 1 + (lastans + q - 1) mod n`。

若为第二种操作，则格式为 `2 p q y`，其中 `l = 1 + (lastans + p - 1) mod n`，`r = 1 + (lastans + q - 1) mod n`，`x = 1 + (lastans + y - 1) mod n`。

其中 `lastans` 表示上一次操作 2 的答案，初始时 `lastans = 0`。

**若** $$l>r$$**，则交换** $$l$$ **和** $$r$$**。**

## **输出格式**

每个操作 2 输出一行一个数表示答案。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
8 6
8 4 2 2 7 7 8 8
1 1 6
1 8 3
2 2 5 8
2 1 3 7
1 4 5
2 2 8 8
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
2
0
3
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

对于前 20% 的测试数据，满足 $$1 \leq n,\,q \leq 1000$$。

对于另外 40% 的测试数据，$$n,\,q \leq 1.4 \times 10^5$$。

对于另外 30% 的测试数据，所有第一种操作在第二种操作之前。

对于 100% 的测试数据，满足 $$1 \leq n,\,q \leq 2 \times 10^5$$，$$1 \leq a_i,\,p,\,q,\,y \leq n$$。

数据有一定梯度。

