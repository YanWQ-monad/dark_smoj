# 2706 覆盖植物

## 题目描述

有一个 $$n$$ 行 $$m$$ 列的二维矩阵，`#` 是障碍物，`.` 是植物。下面定义“灯照”：

1. 灯照是二维矩阵的子矩阵；
2. 灯照内部不能有障碍物格子。

设 $$light_{i,j}$$ 为能照到第 $$i$$ 行第 $$j$$ 列格子的所有不同灯照的数量（即该格子能被多少个不同的灯照覆盖）。

你的任务是输出：$$light_{i,j}$$ 的总和，其中 $$1 \leq i \leq n,\,1 \leq j \leq m$$。

## 输入格式

第一行，$$n$$ 和 $$m$$。

 接下来是 $$n$$ 行 $$m$$ 列的二维矩阵。

## 输出格式

一个整数。

## 输入样例 1

{% code-tabs %}
{% code-tabs-item title="sample1.in" %}
```text
3 3
...
...
...
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例 1

{% code-tabs %}
{% code-tabs-item title="sample1.out" %}
```text
100
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输入样例 2

{% code-tabs %}
{% code-tabs-item title="sample2.in" %}
```text
3 4
..#.
#...
...#
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例 2

{% code-tabs %}
{% code-tabs-item title="sample2.out" %}
```text
40
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

| 测试点 | 范围 |
| :---: | :---: |
| 100% | $$1 \leq n, m \leq 2 \times 10^3$$ |

