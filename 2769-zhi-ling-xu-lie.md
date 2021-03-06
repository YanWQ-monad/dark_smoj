# 2769 指令序列

## 题目描述

有 $$n$$ 头奶牛，编号 0 至 $$n-1$$。有 $$n$$ 个房间从左往右排成一行，编号 0 至 $$n-1$$。

每个房间都住一头牛。一开始，$$i$$ 号奶牛住在第 $$i$$ 个房间。

农夫 FJ **依次**执行 $$n-1$$ 个指令，第 $$i$$ 个指令是一个整数 $$c_i$$，表示的意义是把住在第 $$c_i$$ 个房间的奶牛和住在第 $$c_i+1$$ 房间的奶牛交换。**所有的** $$c_i$$ **都不能相同。**

执行完这 $$n-1$$ 个指令后，FJ 从第 0 个房间开始检查到第 $$n-1$$ 个房间，检查每一个房间最终的住的是哪头奶牛，FJ 用 $$r_i$$ 表示最终第 $$i$$ 个房间住的奶牛的编号。

FJ 把指令序列（$$c_1,\,c_2,\,c_3,\, \cdots ,\,c_{n-1}$$）称为一种“排序方案”。

例如 $$n = 3$$，那一开始是：

```text
房间号：		0 1 2
奶牛编号：	0 1 2
```

执行指令序列 $$(0,\,1)$$ 的流程如下：

第一步：执行指令 0，变成：

```text
房间号：		0 1 2
奶牛编号：	1 0 2
```

第一步：执行指令 1，变成：

```text
房间号：		0 1 2
奶牛编号：	1 2 0
```

所以，执行完指令序列 $$(0,\,1)$$ 后，$$r_0 = 1,\,r_1 = 2,\,r_2 = 0$$。

现在给出 $$n$$，给出最终的 $$r$$，问有多少种不同的“排序方案”，答案模 `1000000007`。

## 输入格式

多组测试数据。

第一行，一个整数 $$g$$，表示有 $$g$$ 组测试数据。

每组测试数据格式：

第一行，一个整数 $$n$$。

第二行，$$n$$ 个整数，第 $$i$$ 个整数是 $$r_i$$。

## 输出格式

共 $$g$$ 行，每行一个整数。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
5
3
1 2 0

2
0 1

4
2 0 3 1

4
1 0 3 2

20
1 3 0 5 2 7 4 8 10 6 12 9 14 11 16 13 18 15 19 17
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
1
0
2
0
716743312
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

$$1 \leq g \leq 10$$，$$1 \leq  n \leq 50$$，$$0 \leq r_i < n$$，所有的 $$r_i$$ 都不相同。

## 来源

[Single Round Match 517 Round 1 Division I AdjacentSwaps](https://community.topcoder.com/stat?c=problem_statement&pm=11537)

