# 2950 异或

## 题目描述

有一个长度为 $$n$$ 的自然数序列 $$a$$，要求将这个序列恰好分成至少 $$m$$ 个连续子段。每个子段的价值为该子段的所有数的按位异或。要使所有子段的价值按位与的结果最大，输出这个最大值。

## 输入格式

第一行一个正整数 $$q$$，表示询问组数。

接下来 $$q$$ 组输入，每组输入两行：

第一行两个正整数 $$n,\,m$$。

第二行 $$n$$ 个正整数，描述序列 $$a$$。

## 输出格式

一行一个正整数，表示答案。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
1
5 3
1 2 3 4 5
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
1
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

对于所有数据，满足 $$1 \leq q \leq 12$$，$$1 \leq m \leq n$$，$$0 \leq a_i < 2^{30}$$。

| 测试点 | 范围 |
| :---: | :---: |
| 20% | $$1 \leq n \leq 20$$ |
| 40% | $$1 \leq n \leq 100,\ a_i < 256$$ |
| 60% | $$1 \leq n \leq 100$$ |
| 100% | $$1 \leq n \leq 1000$$ |

