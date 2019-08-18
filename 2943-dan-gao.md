# 2943 蛋糕

## 题目描述

你有一块大小为 $$n \times m$$ 的蛋糕，你想把它切成 $$1 \times 1$$ 的小块。每次你可以选择横着或者竖着切一刀，把蛋糕切成两部分，这两部分再分别进行切割，直到全都变成 $$1 \times 1$$ 的小块。你想知道有多少种不同的切法（交换任意两块蛋糕的切割顺序算同一种方案），对 `1000000007` 取模。

## 输入格式

一行两个整数 $$n,\,m$$，表示开始时蛋糕的大小。

## 输出格式

输出一行一个整数，表示切蛋糕的方案数对 `1000000007` 取模的结果。

## 输入样例 1

{% code-tabs %}
{% code-tabs-item title="sample1.in" %}
```text
2 3
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例 1

{% code-tabs %}
{% code-tabs-item title="sample1.out" %}
```text
8
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输入样例 2

{% code-tabs %}
{% code-tabs-item title="sample2.in" %}
```text
3 5
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例 2

{% code-tabs %}
{% code-tabs-item title="sample2.out" %}
```text
13008
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

对于 30% 的数据，$$1 \leq n,\,m \leq 8$$

对于另外 20% 的数据，$$n = 1$$

对于另外 20% 的数据，$$n = 2$$

对于 100% 的数据，$$1 \leq n,\,m \leq 300$$。

