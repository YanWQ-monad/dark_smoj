# 2687 最大公约数

## 题目描述

给出一个长度为 $$n$$ 的数组 $$a$$，现在问 $$\gcd(a_i,a_{i+1},\cdots,a_j) \cdot (j-i+1)$$ 的最大值。其中 $$\gcd$$ 为其中的所有数的最大公约数，其中 $$i \leq j$$。

## 输入格式

第一行一个 $$t$$ 表示数据组数。

每组数据第一行一个 $$n$$，

接下来一行有 $$n$$ 个数，表示数组 $$a$$。

## 输出格式

对于每组测试数据，输出相应的答案。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
1
5
30 60 20 20 20
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
80
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

| 测试点 | 范围 |
| :---: | :---: |
| 30% | $$1 \leq n \leq 200$$  |
| 50% | $$1 \leq n \leq 10^3$$  |
| 100% | $$1 \leq n \leq 10^5$$  |

$$1 \leq t \leq 5,\ 1 \leq a_i \leq 10^9$$ 

