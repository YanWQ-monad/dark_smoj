# 2703 颜色问题

## 题目描述

现在给出一个数组 $$a$$，$$a_i$$ 表示位置 $$i$$ 的颜色。有 $$n$$ 个询问，第 $$i$$ 个询问的颜色数限制是 $$i$$。

对于每一个询问，现在假设颜色数限制为 $$x$$，设 $$ans(x)$$ 为将原数组分成若干个连续的数组，使得每个数组内颜色种类数都不大于 $$x$$，的数组个数。

现在要求 $$ans(1),\,ans(2),\,\cdots,\,ans(n)$$。

## 输入格式

第一行一个整数 $$n$$。

接下来一行描述数组 $$a$$。

## 输出格式

输出 $$ans(1),\,ans(2),\,\cdots,\,ans(n)$$。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
8
1 5 7 8 1 7 6 1
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
8 4 3 2 1 1 1 1
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

| 测试点 | 范围 |
| :---: | :---: |
| 40% | $$1 \leq n \leq 10^3$$ |
| 100% | $$1 \leq n \leq 10^5,\ 1 \leq a_i \leq n$$ |



