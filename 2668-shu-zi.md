# 2668 数字

## 题目描述

有 1~$$n$$ 这 $$n$$ 个数字，问有多少个非空集合 $$S$$ 满足里面所有数都在 $$[1,n]$$ 范围内，并且没有任何一个数位 0~9 同时出现在不同的两个数的十进制表示下。

例如，$$n = 12$$，$$\{1, 2, 3\}$$, $$\{2, 11\}$$, $$\{3, 4, 5, 6, 7, 8, 9, 12\}$$ 合法，但是 $$\{1, 2, 10\}$$, $$\{2, 5, 12\}$$ 非法。

## 输入格式

第一行一个正整数 $$t$$ 表示数据组数。

每组测试数据第一行以个整数 $$n$$。

## 输出格式

对于每组数据，输出相应的答案模 `1000000007`。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
2
3
12
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
Case 1: 7
Case 2: 1151
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

| 数据点 | 范围 |
| :---: | :---: |
| 30% | $$1 \leq n \leq 15$$ |
| 60% | $$1 \leq n \leq 10^3 $$ |
| 100% | $$1 \leq n \leq 10^9,\ 1 \leq t \leq 5$$ |

## 来源

[UVA 1734](https://uva.onlinejudge.org/external/17/1734.pdf)，[UVALive 7344](https://icpcarchive.ecs.baylor.edu/external/73/7344.pdf)

