# 2949 质数乘积

## 题目描述

对于给定的一个正整数 $$n$$，判断 $$n$$ 是否能分成若干个正整数之和（可以重复），其中每个正整数都能表示成两个质数乘积。

## 输入格式

第一行一个正整数 $$q$$，表示询问组数。

接下来 $$q$$ 行，每行一个正整数 $$n$$，表示询问。

## 输出格式

共 $$q$$ 行，每行一个正整数，为 `0` 或 `1`。`0` 表示不能，`1` 表示能。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
5
1
4
5
21
25
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
0
1
0
1
1
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 样例解释

$$4 = 2 \times 2$$

$$21 = 6 + 15 = 2 \times 3 + 3 \times 5$$

$$25 = 6 + 9 + 10 = 2 \times 3 + 3 \times 3 + 2 \times 5$$

## 数据范围

| 测试点 | 范围 |
| :---: | :---: |
| 30% | $$1 \leq q,\,n \leq 20$$ |
| 60% | $$1 \leq q \leq 10^4,\ 1 \leq n \leq 5 \times 10^3$$ |
| 100% | $$1 \leq q \leq 10^5,\ 1 \leq n \leq 10^{18}$$ |

