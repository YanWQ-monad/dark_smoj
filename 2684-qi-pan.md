# 2684 棋盘

## 题目描述

给出 $$n$$ 和 $$m$$，表明给出一个 $$n \times m$$ 的棋盘。

每次你可以在棋盘的某两个空位 $$(x_a, y_b)$$ 和 $$(x_b, y_b)$$ 放置两个棋子，当且仅当满足 $$|x_a-x_b| + |y_a-y_b|=3$$。

问最多能放几个棋子。

## 输入格式

第一行两个正整数 $$n$$ 和 $$m$$。

## 输出格式

对于每组测试数据，按照格式输出相应的答案。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
3 3
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
8
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

| 测试点 | 范围 |
| :---: | :---: |
| 20% | $$1 \leq n, m \leq 10$$ |
| 40% | $$1 \leq n, m \leq 10^3$$ |
| 100% | $$1 \leq n, m \leq 10^9$$ |

