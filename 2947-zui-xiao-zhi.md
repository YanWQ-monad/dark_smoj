# 2947 最小值

## 题目描述

Maxtir 又有一个长度为 $$n$$ 的整数序列 $$a$$。

定义区间 $$[l,\,r]$$ 的价值为 $$f(\min_{i=l}^r a_i)$$，其中 $$f(x) = Ax^3 + Bx^2 + Cx + D$$。

特殊地，规定 $$\min_{l=x}^x a_i = a_x$$。

现在 Maxtir 希望将序列分割成若干个区间，使得所有区间的价值之和最大。

## 输入格式

第一行输入一个正整数 $$n$$ 个四个整数 $$A,\,B,\,C,\,D$$。

第二行输入 $$n$$ 个整数，第 $$i$$ 个数表示 $$a_i$$。

## 输出格式

输出一行一个整数 $$ans$$ 表示答案。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
5 0 0 1 10
9 9 5 2 6
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
81
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

对于 10% 的数据，满足 $$n \leq 100$$

对于 30% 的数据，满足 $$n \leq 10^3$$

对于另外 20% 的数据，满足 $$A = B = 0,\,C \leq 0$$

对于 100% 的数据，满足 $$1 \leq n \leq 2 \times 10^5$$，$$\forall | f(a_i) | \leq 10^{13}$$，输入数据均在整数 `int` 范围内。

