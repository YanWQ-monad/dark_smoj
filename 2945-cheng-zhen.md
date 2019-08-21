# 2945 城镇

## 题目描述

L 国一共有 $$n$$ 座城镇，开始时它们两两不连通。L 国计划依次建造 $$n - 1$$ 条道路，把所有城镇连通起来。每建完一条道路，你需要回答这条道路所在连通块内距离最远的两座城镇之间的距离。两座城镇之间的距离定义为从一座走到另一座所需要经过的最少道路数。

## 输入格式

第一行一个整数 $$n$$，表示城镇的数量。

接下来 $$n - 1$$ 行，每行两个整数 $$a_i,\,b_i$$ 表示接下来建的道路连通的两座城镇。

保证 $$n - 1$$ 条道路能够使所有城镇连通。

## 输出格式

输出 $$n - 1$$ 行，每行一个整数表示建完第 $$i$$ 条道路后的答案。

## 输入样例

{% code-tabs %}
{% code-tabs-item title="sample.in" %}
```text
5
3 5
3 4
1 2
1 3
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 输出样例

{% code-tabs %}
{% code-tabs-item title="sample.out" %}
```text
1
2
1
3
```
{% endcode-tabs-item %}
{% endcode-tabs %}

## 数据范围

对于 20% 的数据，$$n \leq 300$$

对于 50% 的数据，$$n \leq 2 \times 10^3$$

对于另外 20% 的数据，保证 $$b_i = i + 1,\ a_i \leq i$$

对于 100% 的数据，$$n \leq 3 \times 10^5$$
