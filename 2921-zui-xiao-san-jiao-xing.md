# 2921 最小三角形

## 题目描述

给出 $$n$$ 个整点，要你选择三个点，使得这三个点组成的三角形面积最小。

## 输入格式

第一行一个 $$n$$，表示整点数目。

接下来 $$n$$ 行，每行两个整数 $$x,\,y$$，表示一个点。

保证不会三点共线。

## 输出格式

一行一个整数，即最小的三角形面积的 2 倍。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
4
0 0
0 1
1 0
1 1
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

## 样例解释

选 $$(0,\,0),\,(0,\,1),\,(1,\,0)$$，面积为 0.5，即输出 1。

## 数据范围

40% 的数据：$$2 \leq n \leq 200$$

100% 的数据：$$2 \leq n \leq 2 \times 10^3$$，$$x \leq x,\,y \leq 10^5$$

保证没有三点共线。

