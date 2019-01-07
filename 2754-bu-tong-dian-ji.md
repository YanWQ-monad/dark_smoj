# 2754 不同点集

## 题目描述

二维坐标系里有 $$n$$ 个点，第 $$i$$ 个点坐标是 $$(x_i,\,y_i)$$。你用一个边长是 $$l$$（$$l$$ 可以是实数）的正方形去选取坐标系的点，正方形内部的点称为“点集”。一个点在正方形的边上也认为是在正方形的内部。$$l$$ 的范围必须在区间 $$[low,\,hi]$$ 内。问可以选取到多少种不同的“点集”。正方行的四条边必须要平行于坐标轴。

## 输入格式

多组测试数据。

第一行，一个整数 $$g$$。表示有 $$g$$ 组测试数据。

每组测试数据格式如下：

第一行，三个整数:  $$low,\,hi,\,n$$。

接下来有 $$n$$ 行，第 $$i$$ 行有两个整数：$$x_i,\,y_i$$。

数据保证：没有相同的点。

## 输出格式

共 $$g$$ 行，每行一个整数。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
5
5 5 3
-5 0
0 0
5 0

10 10 3
-5 0
0 0
5 0

1 100 3
-5 0
0 0
5 0

3 100000000 7
-1 -1
-1 0
-1 1
0 1
1 -1
1 0
1 1

64 108 11
-56 6
-234 34
12 2
324 235
-12 234
53 234
0 342
1 234
12 234
72 234
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
5
5
6
21
26
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

$$1 \leq g < 5$$，$$1 \leq low,\,hi \leq 10^8$$，$$1 \leq n \leq 40$$。$$-10^8 \leq x_i,\,y_i \leq 10^8$$。

## 来源

[Single Round Match 521 Round 1 Division I RangeSquaredSubsets](https://community.topcoder.com/stat?c=problem_statement&pm=11577)

