# 2861 无向图

## 题目描述

给你一张 $$n$$ 个点 $$m$$ 条边的无向图，走过每条边都需要花费 1 秒。

给你一个整数 $$k$$，请你选择至多 $$k$$ 个点，令经过这些点也需要花费 1 秒，使得从点 0 走到点 $$n - 1$$ 的最短时间最大。

输出这个最大值。

注意：不能选择点 0 或点 $$n - 1$$。

## 输入格式

第一行三个正整数 $$n,\,m,\,k$$，意义见题面描述。

接下来 $$m$$ 行，每行两个数 $$x,\,y$$，表示 $$x$$ 和 $$y$$ 之间存在一条边，保证 $$0 \leq x,\,y < n$$，不存在重边和自环，且点 0 和点 $$n - 1$$ 连通。

## 输出格式

一行一个数表示答案。

## 输入样例 1

{% code-tabs %}
{% code-tabs-item title="sample1.in" %}
```text
3 2 0
0 1
1 2
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例 1

{% code-tabs %}
{% code-tabs-item title="sample1.out" %}
```text
2
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输入样例 2

{% code-tabs %}
{% code-tabs-item title="sample2.in" %}
```text
3 2 1
0 1
1 2
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例 2

{% code-tabs %}
{% code-tabs-item title="sample2.out" %}
```text
3
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输入样例 3

{% code-tabs %}
{% code-tabs-item title="sample3.in" %}
```text
3 2 3
0 1
1 2
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例 3

{% code-tabs %}
{% code-tabs-item title="sample3.out" %}
```text
3
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

对于全部数据，$$2 \leq n \leq 100$$，$$1 \leq m \leq \frac{n(n - 1)}{2}$$，$$0 \leq k \leq n$$。

对于 $$30\%$$ 的数据，保证答案不超过 $$k = 0$$ 时的答案 $$+1$$。

## 来源

[FJWC 2019 Day 5, Problem 1, 最短路](http://218.5.5.242:9021/problem/190)

